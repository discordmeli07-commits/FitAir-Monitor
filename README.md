# 🏋️‍♂️ FitAir Monitor

![FitAir Monitor Banner](https://dummyimage.com/1200x300/0f172a/ffffff\&text=FitAir+Monitor)

**Sistema intel·ligent de monitorització de qualitat de l’aire i ocupació en espais esportius**

---

## 📌 Descripció

FitAir Monitor és un projecte basat en **ESP32** que permet controlar en temps real les condicions ambientals d’un espai esportiu.

Mesura:

* 🌬️ CO₂
* 🌡️ Temperatura
* 💧 Humitat
* 👥 Ocupació

👉 L’objectiu és millorar el **confort**, la **seguretat** i la **qualitat de l’aire**.

---

## 🎯 Objectius

* Evitar aire carregat en gimnasos
* Detectar sobreocupació
* Informar en temps real
* Ajudar a prendre decisions (ventilar, reduir aforament…)

---

## 🧠 Funcionament del sistema

![Diagrama sistema](https://dummyimage.com/900x400/1e293b/ffffff\&text=ESP32+-+Sensors+-+Web)

1. L’ESP32 llegeix els sensors
2. Envia les dades via WiFi
3. La web les mostra en temps real
4. Es calcula l’estat de l’aire

---

## 🧰 Tecnologies utilitzades

* 🔌 ESP32
* 🌐 HTML, CSS, JavaScript
* 📡 WiFi (HTTP / MQTT)

### Sensors:

* MH-Z19 → CO₂
* DHT22 → temperatura i humitat
* PIR → ocupació

---

## 🖥️ Interfície web

![Dashboard](https://dummyimage.com/900x400/0f172a/ffffff\&text=Dashboard+FitAir+Monitor)

La web mostra:

* Dades en temps real
* Estat de la qualitat de l’aire
* Disseny minimalista i clar

---

## 🚀 Instal·lació

### 1. Clonar el repositori

```bash
git clone https://github.com/el-teu-usuari/fitair-monitor.git
```

### 2. Obrir la web

Obre `index.html` al navegador.

### 3. Configurar ESP32

* Connectar sensors
* Configurar WiFi
* Enviar dades a la web

---

## 🔌 Exemple de dades

```json
{
  "co2": 920,
  "temperatura": 23.1,
  "humitat": 52,
  "ocupacio": 28
}
```

---

## ⚠️ Nivells de qualitat de l’aire

| CO₂ (ppm) | Estat     | Acció           |
| --------- | --------- | --------------- |
| < 800     | 🟢 Òptim  | Correcte        |
| 800-1200  | 🟡 Avís   | Ventilar        |
| > 1200    | 🔴 Perill | Acció immediata |

---

## 📈 Millores futures

* 📊 Gràfiques en temps real
* 🔔 Alertes automàtiques
* 📱 App mòbil
* 🌬️ Control automàtic de ventilació

---

## 👨‍💻 Autor

Projecte educatiu – FitAir Monitor

---

## 📄 Llicència

Ús educatiu.
