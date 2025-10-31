---
layout: default
title: Blog de Analítica Avanzada
---

<div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); padding: 3rem 2rem; border-radius: 15px; color: white; margin-bottom: 3rem; box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);">
  <h1 style="margin: 0; font-size: 2.5rem;">Hey, bienvenido 👋</h1>
  <p style="font-size: 1.2rem; margin-top: 1rem; opacity: 0.95;">
    Este es mi rincón digital donde transformo datos caóticos en insights (casi siempre). 
    Aquí documento mis experimentos con <strong>Spark</strong>, mis batallas contra datasets enormes, 
    y esos momentos mágicos cuando el código finalmente corre sin errores.
  </p>
</div>

## 🛠️ Mi stack de batalla

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 1.2rem; margin: 2.5rem 0;">
  <div style="background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%); padding: 1.8rem; border-radius: 12px; border: 2px solid #667eea30; transition: transform 0.3s;">
    <div style="font-size: 2rem; margin-bottom: 0.5rem;">⚡</div>
    <strong style="color: #667eea; font-size: 1.1rem;">Apache Spark</strong><br>
    <span style="color: #666; font-size: 0.9rem;">Cuando tu laptop dice "no puedo más"</span>
  </div>
  
  <div style="background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%); padding: 1.8rem; border-radius: 12px; border: 2px solid #764ba230; transition: transform 0.3s;">
    <div style="font-size: 2rem; margin-bottom: 0.5rem;">🐍</div>
    <strong style="color: #764ba2; font-size: 1.1rem;">Python & PySpark</strong><br>
    <span style="color: #666; font-size: 0.9rem;">Mi lenguaje de confort (y desesperación)</span>
  </div>
  
  <div style="background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%); padding: 1.8rem; border-radius: 12px; border: 2px solid #667eea30; transition: transform 0.3s;">
    <div style="font-size: 2rem; margin-bottom: 0.5rem;">🌊</div>
    <strong style="color: #667eea; font-size: 1.1rem;">Data Streaming</strong><br>
    <span style="color: #666; font-size: 0.9rem;">Datos que nunca duermen</span>
  </div>
  
  <div style="background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%); padding: 1.8rem; border-radius: 12px; border: 2px solid #764ba230; transition: transform 0.3s;">
    <div style="font-size: 2rem; margin-bottom: 0.5rem;">📊</div>
    <strong style="color: #764ba2; font-size: 1.1rem;">Visualización</strong><br>
    <span style="color: #666; font-size: 0.9rem;">Porque los ejecutivos no leen tablas</span>
  </div>
</div>

---

## 📖 Lo último del blog

{% for post in site.posts %}
<article style="background: white; border-radius: 12px; padding: 2rem; margin-bottom: 2rem; box-shadow: 0 4px 20px rgba(0,0,0,0.08); border-left: 5px solid #667eea; transition: transform 0.3s, box-shadow 0.3s;">
  
  <h3 style="margin-top: 0; font-size: 1.6rem;">
    <a href="{{ post.url | relative_url }}" style="color: #2d3748; text-decoration: none; background: linear-gradient(to right, #667eea, #764ba2); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">
      {{ post.title }}
    </a>
  </h3>
  
  <div style="color: #718096; font-size: 0.9rem; margin-bottom: 1.2rem; display: flex; align-items: center; gap: 1rem; flex-wrap: wrap;">
    <span>📅 {{ post.date | date: "%d de %B, %Y" }}</span>
    {% if post.author %}
    <span>✍️ {{ post.author }}</span>
    {% endif %}
    <span style="color: #cbd5e0;">•</span>
    <span>⏱️ 5 min de lectura</span>
  </div>
  
  <p style="color: #4a5568; line-height: 1.7; margin-bottom: 1.5rem;">
    {{ post.excerpt | strip_html | truncatewords: 45 }}
  </p>
  
  {% if post.categories %}
  <div style="margin-bottom: 1.5rem; display: flex; flex-wrap: wrap; gap: 0.5rem;">
    {% for category in post.categories %}
    <span style="background: linear-gradient(135deg, #e7f3ff 0%, #f0e7ff 100%); color: #667eea; padding: 0.4rem 1rem; border-radius: 20px; font-size: 0.85rem; font-weight: 500; border: 1px solid #667eea20;">
      #{{ category }}
    </span>
    {% endfor %}
  </div>
  {% endif %}
  
  <a href="{{ post.url | relative_url }}" style="display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.7rem 1.8rem; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; text-decoration: none; border-radius: 25px; font-weight: 500; transition: transform 0.3s, box-shadow 0.3s; box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);">
    Leer completo
    <span style="transition: transform 0.3s;">→</span>
  </a>
  
</article>
{% endfor %}

---

## 🎯 ¿Qué encontrarás en este blog?

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.5rem; margin: 3rem 0;">
  
  <div style="background: linear-gradient(135deg, #e7f3ff 0%, #f0e7ff 100%); padding: 2rem; border-radius: 15px; border: 2px solid #667eea20;">
    <div style="font-size: 2.5rem; margin-bottom: 1rem;">🔍</div>
    <h4 style="color: #2d3748; margin: 0 0 1rem 0; font-size: 1.2rem;">Análisis del mundo real</h4>
    <p style="color: #4a5568; margin: 0; line-height: 1.6;">
      Nada de datasets de juguete. Aquí trabajamos con datos que encuentras en empresas reales, 
      con todos sus problemas y peculiaridades incluidos.
    </p>
  </div>
  
  <div style="background: linear-gradient(135deg, #fff9e6 0%, #ffe6f0 100%); padding: 2rem; border-radius: 15px; border: 2px solid #ffc10720;">
    <div style="font-size: 2.5rem; margin-bottom: 1rem;">💻</div>
    <h4 style="color: #2d3748; margin: 0 0 1rem 0; font-size: 1.2rem;">Código que funciona</h4>
    <p style="color: #4a5568; margin: 0; line-height: 1.6;">
      Implementaciones completas que puedes copiar, ajustar y usar. Con explicaciones de por qué 
      las cosas funcionan (o no) de cierta manera.
    </p>
  </div>
  
  <div style="background: linear-gradient(135deg, #e6fff9 0%, #e6f0ff 100%); padding: 2rem; border-radius: 15px; border: 2px solid #28a74520;">
    <div style="font-size: 2.5rem; margin-bottom: 1rem;">📊</div>
    <h4 style="color: #2d3748; margin: 0 0 1rem 0; font-size: 1.2rem;">Visualizaciones útiles</h4>
    <p style="color: #4a5568; margin: 0; line-height: 1.6;">
      Gráficas que realmente cuentan una historia. No solo bonitas, sino que te ayudan 
      a tomar decisiones basadas en datos.
    </p>
  </div>
  
  <div style="background: linear-gradient(135deg, #ffe6e6 0%, #fff0e6 100%); padding: 2rem; border-radius: 15px; border: 2px solid #dc354520;">
    <div style="font-size: 2.5rem; margin-bottom: 1rem;">🚀</div>
    <h4 style="color: #2d3748; margin: 0 0 1rem 0; font-size: 1.2rem;">Best practices (aprendidas a golpes)</h4>
    <p style="color: #4a5568; margin: 0; line-height: 1.6;">
      Patrones y técnicas que he ido descubriendo en el camino. Algunos por lectura, 
      otros por romper cosas hasta que funcionaron.
    </p>
  </div>
  
</div>

---

## 👩‍💻 Sobre mí

<div style="background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%); padding: 2.5rem; border-radius: 15px; border-left: 5px solid #667eea;">
  
  <p style="font-size: 1.1rem; color: #2d3748; line-height: 1.8; margin-bottom: 1.5rem;">
    Soy <strong style="color: #667eea;">Maria Fernanda Herazo Escobar</strong>, estudiante de Analítica Avanzada 
    y entusiasta del Big Data. Mi día a día incluye pelear con clusters de Spark, entrenar modelos de ML 
    que a veces funcionan, y tratar de convencer a los datos de que me cuenten sus secretos.
  </p>
  
  <p style="color: #4a5568; line-height: 1.8; margin-bottom: 1.5rem;">
    Este blog nació como mi cuaderno de apuntes públicos. Un lugar donde documento lo que aprendo, 
    los errores que cometo (y cómo los soluciono), y esos momentos "aha!" que hacen que todo valga la pena.
  </p>
  
  <p style="color: #4a5568; line-height: 1.8; margin: 0;">
    <strong>Mi filosofía:</strong> Si algo me tomó horas entenderlo, tal vez pueda ayudar a que alguien 
    más lo entienda en minutos. Y si encuentro mejores formas de hacer las cosas, aprendo de la comunidad.
  </p>
  
</div>

---

## 💬 Hablemos

<div style="background: white; padding: 2rem; border-radius: 12px; border: 2px solid #667eea20; text-align: center;">
  <p style="color: #4a5568; font-size: 1.1rem; margin-bottom: 1rem;">
    ¿Tienes preguntas, sugerencias o encontraste un bug en mi código?
  </p>
  <p style="color: #718096; margin: 0;">
    Déjame un comentario en cualquier artículo. Me encanta cuando la gente me señala formas 
    de mejorar o me cuenta cómo usó algo que compartí.
  </p>
</div>

---

<div style="text-align: center; padding: 2.5rem; background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%); border-radius: 12px; margin-top: 4rem; border: 1px solid #dee2e6;">
  <p style="color: #6c757d; margin: 0; font-size: 0.95rem;">
    <strong style="color: #495057;">Construido con:</strong> Jekyll • GitHub Pages • Apache Spark • Python • Mucho café ☕
  </p>
  <p style="color: #adb5bd; font-size: 0.85rem; margin-top: 0.8rem;">
    Última actualización: {{ site.time | date: "%d de %B de %Y" }}
  </p>
</div>