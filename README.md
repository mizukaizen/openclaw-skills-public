# OpenClaw Skills — melisarchimedes

Public SKILL.md-format skills for AI agents.

## Skills

### astro-transits

Astrological transit calculator with natal chart support. Daily transits, weekly forecasts, void-of-course Moon, aspects, stations, and ingresses. Uses Swiss Ephemeris.

**Install:**

```bash
# ClawHub
npx clawhub@latest install astro-transits

# Skills.sh
npx skills add melisarchimedes/openclaw-skills-public/astro-transits

# Direct
git clone https://github.com/melisarchimedes/openclaw-skills-public.git
```

**Quick start:**

```bash
pip install pyswisseph

# Generate your natal chart
python3 scripts/natal_chart.py --date "1990-06-15" --time "14:30" --tz "America/New_York" --lat 40.7128 --lon -74.0060 --save natal.json

# Daily transits
python3 scripts/transits.py --chart natal.json

# Weekly forecast
python3 scripts/transits.py --chart natal.json --week

# Void-of-course Moon
python3 scripts/voc_check.py
```

## Licence

MIT
