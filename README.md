# 🏋️‍♂️ AirSport Guardian

![banner](https://via.placeholder.com/1000x300?text=AirSport+Guardian)

**Sistema intel·ligent de control de qualitat de l’aire i ocupació en espais esportius**

---

## 📌 Descripció

AirSport Guardian és un projecte basat en **ESP32** que permet monitoritzar en temps real:

* 🌬️ Nivells de CO₂
* 🌡️ Temperatura
* 💧 Humitat
* 👥 Ocupació de l’espai

L’objectiu és **millorar el confort i la seguretat** en instal·lacions esportives, evitant ambients carregats i situacions de risc.

---

## 🎯 Objectius

* Controlar la qualitat de l’aire en interiors
* Detectar sobreocupació
* Informar en temps real als usuaris
* Facilitar la presa de decisions (ventilar, reduir aforament, etc.)

---

## 🧠 Funcionament

![diagrama](https://via.placeholder.com/800x400?text=Diagrama+del+sistema)

1. L’ESP32 llegeix dades dels sensors
2. Les dades s’envien via WiFi
3. La web mostra la informació en temps real
4. Es genera un estat (Òptim / Avís / Perill)

---

## 🧰 Tecnologies utilitzades

* 🔌 **ESP32**
* 🌐 HTML, CSS, JavaScript
* 📡 WiFi (HTTP / MQTT)
* 📊 Sensors:

  * CO₂ (MH-Z19 o similar)
  * Temperatura i humitat (DHT22)
  * Sensor d’ocupació (PIR o comptador)

---

## 🖥️ Interfície web

![web](https://via.placeholder.com/800x400?text=Interficie+web)

La web mostra:

* Dades en temps real
* Estat de la qualitat de l’aire
* Interfície clara i minimalista

---

## 🚀 Instal·lació

### 1. Clonar el repositori

```bash
git clone https://github.com/el-teu-usuari/airsport-guardian.git
```

### 2. Obrir la web

Obre `index.html` al navegador.

### 3. Configurar ESP32

* Connectar sensors
* Configurar WiFi
* Enviar dades a la web

---

## 🔌 Exemple de dades (JSON)

```json
{
  "co2": 850,
  "temperatura": 22.5,
  "humitat": 55,
  "ocupacio": 30
}
```

---

## ⚠️ Nivells de qualitat de l’aire

| CO₂ (ppm) | Estat     | Acció              |
| --------- | --------- | ------------------ |
| < 800     | 🟢 Òptim  | Cap acció          |
| 800-1200  | 🟡 Avís   | Ventilar           |
| > 1200    | 🔴 Perill | Evacuar / Ventilar |

---

## 📈 Millores futures

* 📊 Gràfiques en temps real
* 🔔 Sistema d’alertes
* 📱 Versió mòbil
* 🤖 Automatització de ventilació

---

## 👨‍💻 Autor

Projecte desenvolupat per a finalitat educativa.

---

## 📄 Llicència

Aquest projecte és d’ús educatiu.

---

⭐ Si t’ha servit, pots donar-li una estrella al repositori!
