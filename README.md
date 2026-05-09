
# 🎓 ASUS Suceava - Website Oficial & Platformă de Management

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)]()
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)]()
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)]()
[![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)]()

> Platforma web oficială a Asociației Studenților din Universitatea „Ștefan cel Mare” din Suceava (ASUS), construită de la zero folosind tehnologii web native (Vanilla) și integrată cu un backend serverless.

🔗 **[Live Demo](https://iustin-timu.github.io/Site-ASUS/)**

## 💡 Despre Proiect

Acest proiect a fost dezvoltat pentru a oferi asociației studențești o prezență online modernă, rapidă și ușor de administrat. Am ales să nu folosesc framework-uri complexe (precum React sau Vue), ci să demonstrez o înțelegere solidă a bazelor: **DOM Manipulation, CSS Modern (Grid/Flexbox, Variables) și JavaScript Asincron.**

Proiectul este împărțit în două componente majore:
1. **Interfața Publică (Frontend):** O aplicație web responsivă, cu design modern, suport pentru Dark/Light Mode și conținut generat dinamic.
2. **Panoul de Administrare (Backend/Auth):** Un dashboard securizat creat pentru echipa de conducere, care permite adăugarea, ștergerea și editarea proiectelor și știrilor în timp real, direct în baza de date.

## ✨ Funcționalități Cheie (Technical Highlights)

* 🌗 **Dark / Light Mode Toggle:** Implementat nativ folosind variabile CSS (`--color-surface`, `--color-text`) și atributul `data-theme` controlat prin JavaScript.
* ⚡ **Conținut Dinamic (Fetch API & Async/Await):** Secțiunile de Știri, Proiecte și "Eveniment Curent" sunt extrase asincron din baza de date și redate (rendered) în DOM la încărcarea paginii.
* 🛡️ **Autentificare & Securitate:** Panoul de admin este protejat prin Supabase Auth. Accesul este permis doar utilizatorilor cu credențiale valide, sesiunile fiind gestionate via JWT.
* 📱 **Mobile-First & Fully Responsive:** Design adaptabil pe orice rezoluție folosind Media Queries, Flexbox și CSS Grid. Meniu de navigație de tip "Off-canvas Drawer" pentru mobil.
* 🎬 **Animații pe Scroll (Intersection Observer API):** Performanță optimizată prin utilizarea `IntersectionObserver` pentru a declanșa animații (fade-in, slide-up) și numărătoare dinamice doar atunci când elementele intră în viewport.
* 🚀 **Zero Dependencies (pe UI):** Interfața este 100% Vanilla HTML/CSS/JS. Singura librărie externă este SDK-ul de la Supabase și librăria de iconițe vectoriale (Lucide Icons).

## 🛠️ Stack Tehnologic

* **Frontend:** HTML5 (Semantic), CSS3 (Custom Properties, BEM-like naming), Vanilla JavaScript (ES6+).
* **BaaS (Backend as a Service):** [Supabase](https://supabase.com/) (PostgreSQL REST API).
* **Autentificare:** Supabase Auth (Email & Password).
* **Iconițe:** [Lucide Icons](https://lucide.dev/).

## ⚙️ Structura Proiectului

```text
📁 asus-website/
├── 📄 index.html          # Pagina principală (Landing Page dinamic)
├── 📄 admin.html          # Panoul de control securizat (CMS)
├── 📄 stiri.html          # Arhiva completă de știri
├── 📄 stiri-detaliu.html  # Template pentru citirea unui singur articol
├── 📄 reprezentanti.html  # Pagina cu structura studenților reprezentanți
├── 📄 conducere.html      # Pagina cu echipa de conducere
└── 📁 logouri/            # Resurse statice (imagini parteneri, logo-uri)
