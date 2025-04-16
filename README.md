# 🕵️ i_see_ip.py & i_forgot_i_made_i_see_ip.py

> "It's like that, but nothing like that at all."

These two scripts are your go-to tools when you've got a list of IP addresses and want to see them dancing across a map like suspects in a crime doc. Originally whipped up for a very specific, chaotic purpose (you know who you are), they still might be useful if your OSINT game involves rogue CSVs and internet crumbs.

---

## 📌 What They Do

### `i_see_ip.py`
- Accepts a `.txt` file of IP addresses.
- Looks up geolocation data for each.
- Saves data to `IPs_INFO.csv`.
- Creates a heatmap-style interactive HTML map (`MAP_output.html`) of those IPs.

### `i_forgot_i_made_i_see_ip.py`
- Similar in theory, different in execution.
- Takes an existing CSV (`assets.csv`) and appends lat/lon columns.
- Designed for... reasons. It just is. Trust the chaos.

---

## 🧰 Requirements
```bash
pip install ip2geotools geocoder folium pandas
```

---

## 📁 File Format Examples

### For `i_see_ip.py`
**ip-list.txt**:
```
8.8.8.8
1.1.1.1
...
```

### For `i_forgot_i_made_i_see_ip.py`
**assets.csv**:
```
IP_ADDRESS
8.8.8.8
1.1.1.1
...
```

---

## 🗺️ Output
- `IPs_INFO.csv` – with location, lat, long, and count of IPs
- `MAP_output.html` – open in your browser and bask in the glow of digital travel

---

## 🛠️ Usage
### Run `i_see_ip.py`
```bash
python i_see_ip.py
```

### Run `i_forgot_i_made_i_see_ip.py`
```bash
python i_forgot_i_made_i_see_ip.py
```

---

## ⚠️ Disclaimer
- Rate limits may apply from geo APIs.
- It’s best not to unleash this on massive datasets unless you're prepared to sit.
- Works best with a VPN and a coffee.

---

## 💬 Author's Note
Sometimes you make something useful. Other times you make `i_forgot_i_made_i_see_ip.py` because caffeine told you it was a good idea. Either way… enjoy the chaos. 🧠📍
