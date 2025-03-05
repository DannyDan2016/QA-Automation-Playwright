Portafolio de Automatización de Pruebas 🚀

📌 Sobre Mí

Soy Danny, Ingeniero de Calidad de Software con más de 6 años de experiencia en pruebas funcionales, no funcionales y automatización de pruebas y metodologías ágiles. Me especializo en la implementación de Page Object Model (POM) con Playwright, Cypress y Selenium, asegurando que las pruebas sean mantenibles, reutilizables y escalables.

Actualmente, estoy en búsqueda de oportunidades donde pueda aportar mis conocimientos en automatización, mejorar la capacidad de prueba del software y promover estrategias para la prevención de errores y calidad del producto.

Este repositorio contiene proyectos de automatización de pruebas utilizando Playwright, Cypress y Selenium, aplicando el patrón de diseño Page Object Model (POM) para garantizar la mantenibilidad y escalabilidad de los tests.

El objetivo es demostrar habilidades en la automatización de pruebas funcionales y de regresión, aplicando buenas prácticas y estrategias de prueba en entornos ágiles.

Tecnologías y Herramientas

Lenguajes de Programación: JavaScript, TypeScript y Python

Frameworks de Automatización:

Playwright

Cypress

Selenium

Gestión de dependencias: npm

Reportes: Allure Report

Patrón de Diseño: Page Object Model (POM)

Control de Versiones: Git & GitHub

Requisitos Previos

Antes de ejecutar los proyectos, asegúrate de tener instalado:

Node.js (v16 o superior)

npm

Playwright y sus dependencias: npx playwright install

📂 Estructura del Portafolio
🔹 Proyecto 1: SauceDemo Automation - Automatización de pruebas en el sitio SauceDemo, utilizando el patrón Page Object Model (POM).

🔹 Proyecto 2: demoqa.com - Automatización de pruebas en el sitio demoqa.com, utilizando el patrón Page Object Model (POM).

🔹 Configuración y ejecución - Guía paso a paso para correr los tests en tu máquina.

🚀 Proyecto 1: SauceDemo Automation

Descripción: En este proyecto se automatizan los flujos críticos de la aplicación SauceDemo, incluyendo:

✅ Login exitoso y fallido
✅ Añadir y eliminar productos del carrito
✅ Finalizar una compra (checkout)
✅ Validaciones de UI y performance

Tecnologías utilizadas:

Playwright con JavaScript

Page Object Model (POM)

GitHub Actions (para futuras integraciones CI/CD)

Reportes automáticos (configuración en proceso)

Estructura Proyecto SauceDemo Automation

📂 tu-repositorio
 ┣ 📂 tests
 ┃ ┣ 📜 login.spec.js   # Pruebas de inicio de sesión
 ┃ ┣ 📜 cart.spec.js    # Pruebas del carrito de compras
 ┃ ┗ 📜 checkout.spec.js # Pruebas de checkout
 ┣ 📂 page_objects
 ┃ ┣ 📜 LoginPage.js    # Definición de la página de login
 ┃ ┗ 📜 InventoryPage.js # Definición de la página de inventario
 ┣ 📜 playwright.config.js # Configuración de Playwright
 ┣ 📜 package.json # Dependencias del proyecto
 ┗ 📜 README.md  # Documentación del repositorio

SauceDemo

A continuación, se presenta un ejemplo de prueba automatizada para el inicio de sesión en SauceDemo:

const { test, expect } = require('@playwright/test');

test('Inicio de sesión exitoso en SauceDemo', async ({ page }) => {
    await page.goto('https://www.saucedemo.com/');
    await page.fill('[data-test="username"]', 'standard_user');
    await page.fill('[data-test="password"]', 'secret_sauce');
    await page.click('[data-test="login-button"]');
    await expect(page).toHaveURL('https://www.saucedemo.com/inventory.html');
});

🔧 Configuración y Ejecución

1️⃣ Requisitos previos

Tener Node.js instalado (versión 16 o superior)

Tener Visual Studio Code

Tener Playwright instalado globalmente con:

npx playwright install


2️⃣ Clonar el repositorio

git clone https://github.com/tu-usuario/qa-automation-portfolio.git
cd qa-automation-portfolio

3️⃣ Ejecutar pruebas

Para correr todas las pruebas:

npx playwright test

Para correr un test específico:

npx playwright test tests/login.spec.ts

Recursos Adicionales

Documentación Oficial de Playwright

Documentación Oficial de Cypress

Documentación Oficial de Selenium

📬 Contacto

Si deseas ponerte en contacto conmigo:

📧 Correo: parradodanny@outlook.com

💼 LinkedIn: https://www.linkedin.com/in/danny-parrado-qa-engineer 

🌍 Portafolio:

¡Gracias por visitar mi portafolio! 😊
