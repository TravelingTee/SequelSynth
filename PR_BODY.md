Sequel branding: rebrand NotebookLlama to Sequel

Summary

- Rebranded the UI and docs to “Sequel,” using centralized branding constants.
- Preserved package name and functionality; only user-facing strings and docs changed.

What’s included

- Centralized branding in src/notebookllama/branding.py
  - PRODUCT_NAME = "Sequel"
  - TAGLINE, PRIMARY_COLOR, ACCENT_COLOR
- Streamlit pages updated:
  - Home.py
  - pages/1_Document_Management_UI.py
  - pages/2_Document_Chat.py
  - pages/3_Interactive_Table_and_Plot_Visualization.py
  - pages/4_Observability_Dashboard.py
- README updated with Sequel name, tagline, and attribution to NotebookLlama (MIT)
- pyproject.toml description updated
- Added assets/sequel-logo.svg
- Import fix so files run under Streamlit’s script execution (fallback absolute import)

Screenshots
Home (branding visible):
![Home](/home/ubuntu/screenshots/localhost_8501_050923.png)

Document Management (branding visible; expected DB connection error until Postgres/docker compose is up):
![Document Management](/home/ubuntu/screenshots/localhost_8501_050907.png)

Notes

- Some features require environment keys and/or Docker (Postgres, Jaeger) per upstream:
  - OpenAI, ElevenLabs, and LlamaCloud
  - docker compose up for analytics/observability
- Package/module name remains notebookllama to avoid breaking imports; only UI/docs branding changed.

License and Attribution

- Derived from run-llama/notebookllama (MIT)
- LICENSE remains MIT; attribution added in README

Link to Devin run
https://app.devin.ai/sessions/7b1a2c4ae9b3454bbb6c96727e880b58

Requested by

- User: TravelingTee
- GitHub: @TravelingTee
