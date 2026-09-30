<div align="center">

<img src="/header.svg" alt="Gael Alejo - Fullstack Developer | .NET & C#" width="100%"/>

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=15&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=620&lines=Fullstack+Developer+%C2%B7+.NET+%2F+C%23;APIs+REST+%C2%B7+SQL+Server;Primero+que+funcione.+Despu%C3%A9s%2C+que+sea+mantenible." alt="Typing SVG" /></a>

</div>

---

## `new Developer()`

```csharp
public record Developer
{
    public string   Name           => "Gael Alejo";
    public string   Role           => "Fullstack Developer Jr · .NET / C#";
    public string   Location       => "Querétaro, México 🇲🇽";
    public string[] Focus          => ["APIs REST", "Desktop", "SQL Server / EF Core", "Web Apps"];
    public string   CurrentProject => "ConsensoClima — clima multi-fuente con señal de confianza";
    public string[] Learning       => ["async/await y concurrencia", "Inyección de dependencias", "xUnit", "EF Core"];
    public string   Mindset        => "Primero que funcione. Después, que sea mantenible.";
}
```

Egresado de Ingeniería en Sistemas Computacionales (UPQ). He desarrollado aplicaciones de escritorio en **.NET** con **WPF** y **Windows Forms** bajo el patrón **MVVM**, APIs REST, App Webs y bases de datos relacionales con **SQL Server**. Usando **Dapper** y **EF Core** como capa de acceso a datos, y para la experiencia UI **Angular**. Antes de programar de tiempo completo configuré redes con equipos Cisco y Huawei, así que me gusta entender el sistema completo: desde la red hasta la consulta SQL.

Hoy estoy profundizando en la programacion con C# y Python creando proyectos que resuelven problemas reales, no solo CRUDs: concurrencia, inyección de dependencias, diseño por interfaces, pruebas, y patrones de diseño. Ademas en la IA, no solo como herramienta de trabajo, sino en el Deep Learnig, IA Agentica y Redes Generativas. 

---

## 🧱 Stack

**Backend**

![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-5C2D91?style=for-the-badge&logo=dotnet&logoColor=white)

**Datos**

![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Entity Framework](https://img.shields.io/badge/Entity_Framework-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![Dapper](https://img.shields.io/badge/Dapper-2D2D2D?style=for-the-badge&logoColor=white)

**Frontend**

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-1e99f7?style=for-the-badge&logo=typescript&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-e51530?style=for-the-badge&logo=angular&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

**Herramientas & Nube**

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-158be5?style=for-the-badge&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-e7860c?style=for-the-badge&logoColor=white)

**Aprendiendo ahora**

![Python](https://img.shields.io/badge/Python-512BD4?style=flat-square)
![IA Agentica/Redes GAN](https://img.shields.io/badge/IA%20Agentica%20&%20Redes%20GAN-512BD4?style=flat-square)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-512BD4?style=flat-square)

---

## 🌦️ Proyecto destacado: ConsensoClima `🚧 en construcción`

> El clima de una sola API es un punto único de falla. **ConsensoClima** consulta varias fuentes al mismo tiempo, consolida cada ciudad en una lectura única y entrega una **señal de confianza** (qué tanto coinciden las fuentes). Si una fuente se cae o tarda, la corrida sigue y el reporte lo indica.

<img src="https://github.com/Gael-AH444/Gael-AH444/raw/main/consensoclima-diagram.svg" alt="Flujo de ConsensoClima" width="100%"/>

**Qué pongo en práctica:**

- **Concurrencia de I/O** con `async/await` y `Task.WhenAll`: consultar 10 ciudades debe tardar casi lo mismo que consultar 1.
- **Diseño por interfaces** (`IProveedorClima`): las fuentes son intercambiables y el agregador recibe las que existan vía DI.
- **Agregación con LINQ** en dos niveles: promedio, rango entre fuentes y nivel de acuerdo por ciudad.
- **Resiliencia**: timeout con `CancellationToken` y manejo de fallos por fuente, sin tumbar la corrida.
- **Generic Host** (DI + configuración + logging + `IHttpClientFactory`) y **tests** con fuentes falsas (xUnit + Moq).

📂 **[Ver el repositorio →](https://github.com/Gael-AH444/ConsensoClima)**

---

## 📂 Proyectos

| Proyecto | Descripción | Stack |
| --- | --- | --- |
| 🌦️ **[ConsensoClima](https://github.com/Gael-AH444/ConsensoClima)** | Clima multi-fuente con consolidación y señal de confianza; tolera fuentes caídas | `csharp` `dotnet` `async` `linq` `xunit` |
| 🛒 **[API de Productos](http://www.apiproductogael.somee.com/swagger/index.html)** | API REST para gestión de productos, documentada con Swagger | `csharp` `aspnet` `mysql` `swagger` |
| 🛍️ **[Carrito de compras](https://shoppingcartprojet.netlify.app/)** | Carrito funcional con manejo de estado en el cliente | `javascript` `html` `css` |
| ✉️ **[Simulador de envío de emails](https://simuladorcorreos.netlify.app/)** | Formulario con validación en tiempo real y flujo de envío simulado | `javascript` `html` `css` |
| 🌐 **[Portafolio](https://miportafoliogaelah.netlify.app/)** | Mi sitio personal: experiencia, stack y proyectos | `javascript` `html` `css` |

---

## 🧭 Trayectoria

| | Rol / Formación | Periodo | Enfoque |
| --- | --- | --- | --- |
| 💼 | **Desarrollador de sofware** | 2025 — Actualidad | Web apps con .NET + Angular · APIs con JS y TS · Desarrollo y personalizacion de modulos en ERPs (Netsuite & Dynamics F&O 365)|
| 💼 | **Programador Jr** | 2023 — 2024 | Apps de escritorio .NET (WPF, WinForms) con MVVM · Dapper y EF · diseño de BD con T-SQL · documentación técnica (UML, casos de uso) |
| 🌐 | **IP Intern** | 2022 — 2023 | Configuración de routers y switches Cisco/Huawei · protocolos capa 2 · migración de equipos y soporte remoto |
| 🎓 | **Ing. en Sistemas Computacionales** | 2019 — 2023 | Universidad Politécnica de Querétaro |

---


## 📊 Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=Gael-AH444&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=a78bfa&icon_color=a78bfa&text_color=e6edf3" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Gael-AH444&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=a78bfa&text_color=e6edf3" />

<a href="https://git.io/streak-stats"><img src="https://streak-stats.demolab.com?user=Gael-AH444&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=a78bfa&ring=a78bfa&fire=f78166&currStreakLabel=a78bfa" alt="GitHub Streak" /></a>

</div>

---

## 🌐 Contacto

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gael_Alejo-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jesus-gael-alejo-hernandez-6372063b1)
[![Portafolio](https://img.shields.io/badge/Portafolio-Ver_sitio-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://miportafoliogaelah.netlify.app/)
[![Email](https://img.shields.io/badge/Email-Escr%C3%ADbeme-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:gaelalejo.444@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Gael--AH444-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Gael-AH444)

</div>

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:512BD4,50:2b1a5e,100:0d1117&height=100&section=footer" width="100%"/>

<div align="center">

*"Make it work, make it right, make it fast."* — Kent Beck

</div>
