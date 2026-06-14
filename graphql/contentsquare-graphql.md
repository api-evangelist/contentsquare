# ContentSquare GraphQL Schema

## Overview

This conceptual GraphQL schema models the ContentSquare digital experience analytics (DXA) platform. ContentSquare captures every user interaction on web and mobile properties to surface friction points, conversion blockers, and behavioral insights via session replay, heatmaps, journey analysis, and zone-based analytics.

The schema is derived from the ContentSquare REST APIs documented at https://developers.contentsquare.com/ and reflects the platform's core data model including sessions, page views, zones, heatmaps, funnels, journeys, and campaign attribution.

## Schema Source

- **Provider**: ContentSquare
- **API Docs**: https://developers.contentsquare.com/
- **REST API Reference**: https://docs.contentsquare.com/en/api/export/
- **Schema Type**: Conceptual GraphQL (derived from REST API documentation)

## Types Summary

| Category | Types |
|---|---|
| Session & Visit | Session, Visit, VisitPage, PageView |
| Device & Environment | Device, Browser, Platform, Network |
| Geography | Country, City |
| Identity & Segmentation | User, Segment, AudienceSegment, Filter |
| Zone Analytics | Zone, ZoneStats, ZoneHover, ZoneClick, ZoneExposure, CSZoneMapping, ZoneRecap |
| Heatmap & Maps | Heatmap, ClickMap, ScrollMap, ClickMapData, ScrollMapData |
| Conversion & Events | ConversionRate, EventTrigger, Event, CustomVariable |
| Targeting | PageTarget |
| Analysis | Analysis, FunnelAnalysis, FunnelStep, JourneyAnalysis, ImpactAnalysis, RevenueImpact |
| UX & Errors | UX360, ErrorReport, FrictionScore |
| Performance | SpeedAnalysis, LoadTime |
| Campaign Attribution | Campaign, CampaignSource, Source, Medium, Term, Content |
| Tagging & Auth | ExperienceTag, APIKey, Token |

## Key Relationships

- A **Session** contains multiple **Visit** records, each Visit has multiple **VisitPage** entries.
- Each **VisitPage** is associated with a **PageView** that links to **Zone** analytics including **ZoneStats**, **ZoneHover**, **ZoneClick**, and **ZoneExposure**.
- **Heatmap**, **ClickMap**, and **ScrollMap** aggregate zone-level interaction data across page views.
- **FunnelAnalysis** chains **FunnelStep** nodes to model conversion paths.
- **JourneyAnalysis** traces multi-page navigation paths across sessions.
- **ImpactAnalysis** and **RevenueImpact** connect behavioral friction to business outcomes.
- **Campaign** attribution links sessions to marketing **Source**, **Medium**, **Term**, and **Content** dimensions.
- **AudienceSegment** and **Filter** enable behavioral cohort analysis across all analytics types.

## Authentication

ContentSquare APIs use OAuth 2.0 client_credentials flow. The token endpoint returns both a JWT access token and a dynamic regional base URL. All queries should be executed against the regional endpoint returned at authentication time.

## Usage Notes

This schema is conceptual and intended for integration planning, API documentation, and schema-driven development. It maps ContentSquare's REST API data model into a GraphQL-idiomatic structure to support tooling, federation, and unified data graph use cases.
