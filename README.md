# DE
https://gist.github.com/anonymous/0f28f13f6485c7fc187b474f7f2f276b
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DemAgency - Kişisel Web Sayfanız</title>
    <style>
        /* Stil tanımlamaları burada bulunabilir. */
    </style>
</head>
<body>
    <header>
        <h1>DemAgency</h1>
    </header>
    <nav>
        <a href="#about">Hakkımda</a>
        <a href="#contact">İletişim</a>
        <a href="#portfolio">Portföy</a>
        <a href="#blog">Blog</a>
        <div id="language-selector">
            <select onchange="changeLanguage()">
                <option value="tr">Türkçe</option>
                <option value="nl">Felemenkçe</option>
                <option value="en">İngilizce</option>
                <option value="de">Almanca</option>
                <option value="fr">Fransızca</option>
            </select>
        </div>
    </nav>
    <div class="content">
        <section id="about">
            <h2 id="about-heading">Hakkımda</h2>
            <p id="about-content">Merhaba, ben [Adınız]. Bir day trader'ım ve hobilerim arasında basketbol bulunuyor. Kendi web sayfamı oluşturdum ve burada deneyimlerimi, analizlerimi ve diğer ilgi alanlarımla ilgili içerikleri paylaşıyorum.</p>
        </section>
        <section id="contact">
            <h2 id="contact-heading">İletişim</h2>
            <p id="contact-content">Benimle iletişime geçmek için aşağıdaki bilgileri kullanabilirsiniz:</p>
            <p>Email: [Email Adresiniz]</p>
            <p>Sosyal Medya: [Sosyal Medya Linkleri]</p>
        </section>
        <section id="portfolio">
            <h2 id="portfolio-heading">Portföy</h2>
            <p id="portfolio-content">Burada işlerinizi ve projelerinizi sergileyebilirsiniz.</p>
        </section>
        <section id="blog">
            <h2 id="blog-heading">Blog</h2>
            <p id="blog-content">Son yazılarınızı ve analizlerinizi burada paylaşabilirsiniz.</p>
        </section>
    </div>
    <footer class="footer">
        &copy; 2023 DemAgency | Tüm Hakları Saklıdır
    </footer>

    <script>
        function changeLanguage() {
            var language = document.getElementById("language-selector").querySelector("select").value;
            var translations = {
                "tr": {
                    "about-heading": "Hakkımda",
                    "about-content": "Merhaba, ben [Adınız]. Bir day trader'ım ve hobilerim arasında basketbol bulunuyor. Kendi web sayfamı oluşturdum ve burada deneyimlerimi, analizlerimi ve diğer ilgi alanlarımla ilgili içerikleri paylaşıyorum.",
                    "contact-heading": "İletişim",
                    "contact-content": "Benimle iletişime geçmek için aşağıdaki bilgileri kullanabilirsiniz:",
                    "portfolio-heading": "Portföy",
                    "portfolio-content": "Burada işlerinizi ve projelerinizi sergileyebilirsiniz.",
                    "blog-heading": "Blog",
                    "blog-content": "Son yazılarınızı ve analizlerinizi burada paylaşabilirsiniz."
                },
                "nl": {
                    "about-heading": "Over Mij",
                    "about-content": "Hallo, ik ben [Uw Naam]. Ik ben een daytrader en mijn hobby is basketbal. Ik heb mijn eigen website gemaakt waar ik mijn ervaringen, analyses en andere interesses deel.",
                    "contact-heading": "Contact",
                    "contact-content": "U kunt contact met mij opnemen via de volgende gegevens:",
                    "portfolio-heading": "Portfolio",
                    "portfolio-content": "Hier kunt u uw werk en projecten presenteren.",
                    "blog-heading": "Blog",
                    "blog-content": "Hier kunt u uw recente artikelen en analyses delen."
                },
                "en": {
                    "about-heading": "About Me",
                    "about-content": "Hello, I'm [Your Name]. I'm a day trader, and my hobby is basketball. I've created my own website where I share my experiences, analyses, and other interests.",
                    "contact-heading": "Contact",
                    "contact-content": "You can reach me using the following information:",
                    "portfolio-heading": "Portfolio",
                    "portfolio-content": "Here you can showcase your work and projects.",
                    "blog-heading": "Blog",
                    "blog-content": "You can share your latest articles and analyses here."
                },
                "de": {
                    "about-heading": "Über Mich",
                    "about-content": "Hallo, ich bin [Ihr Name]. Ich bin ein Daytrader, und mein Hobby ist Basketball. Ich habe meine eigene Website erstellt, auf der ich meine Erfahrungen, Analysen und andere Interessen teile.",
                    "contact-heading": "Kontakt",
                    "contact-content": "Sie können mich über die folgenden Informationen erreichen:",
                    "portfolio-heading": "Portfolio",
                    "portfolio-content": "Hier können Sie Ihre Arbeit und Projekte präsentieren.",
                    "blog-heading": "Blog",
                    "blog-content": "Hier können Sie Ihre neuesten Artikel und Analysen teilen."
                },
                "fr": {
                    "about-heading": "À Propos de Moi",
                    "about-content": "Bonjour, je suis [Votre Nom]. Je suis day trader et mon hobby est le basketball. J'ai créé mon propre site web où je partage mes expériences, analyses et autres centres d'intérêt.",
                    "contact-heading": "Contact",
                    "contact-content": "Vous pouvez me joindre en utilisant les informations suivantes :",
                    "portfolio-heading": "Portfolio",
                    "portfolio-content": "Vous pouvez présenter ici votre travail et vos projets.",
                    "blog-heading": "Blog",
                    "blog-content": "Vous pouvez partager ici vos derniers articles et analyses."
                }
            };
            var keys = Object.keys(translations[language]);
            for (var i = 0; i < keys.length; i++) {
                var element = document.getElementById(keys[i]);
                if (element) {
                    element.textContent = translations[language][keys[i]];
                }
            }
        }
    </script>
</body>
</html>
