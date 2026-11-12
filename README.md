# UAM KPI/KPA Dashboard — rodada fora da condição nominal: vento

Site estático (GitHub Pages) com os resultados da rodada **vento** de
06/11/2026 do projeto SIGMASky: 36 cenários (C1.x a C8.x) × 50 réplicas.

- RUN do orquestrador: `20261109_044748_77e95d0c` (`/dados/orbolato/runs/sim_off_nominal_20261106/wind` no Lessonia).
- Gerado com [projetosigmasky/uam_metrics](https://github.com/projetosigmasky/uam_metrics) `0fcf2af`
  (`generate_reports.py --run-id 20261109_044748_77e95d0c --scenario-codes <36 códigos>`).
- Inclui a análise separada eVTOL × tráfego aeroportuário (FR24, dia de pico de SBSP,
  01/12/2022) na aba Segurança e em `assets/data/airport_traffic/`.
- Helicópteros que pararam a ~1 m do último waypoint e nunca foram removidos pelo BlueSky
  (19.152 voos) foram cortados na chegada; ver o README do uam_metrics.
- A rodada nominal correspondente está em https://projetosigmasky.github.io/uam_metrics/.
- Sem os arquivos de auditoria locais (`passage_events.jsonl`, `waypoints_by_replica.csv`,
  `assets/data/runs/`) e sem a calibração dos baselines, que pertence à rodada nominal.
