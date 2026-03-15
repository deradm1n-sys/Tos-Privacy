# Tos-Privacy
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

<header>
<h1>[BOTNAME]</h1>
<p>Moderation • Levelsystem • Automatisierung • Discord Server Management</p>
<a class="btn" href="#invite">Bot einladen</a>
</header>

<nav>
<a href="#features">Features</a>
<a href="#dashboard">Dashboard</a>
<a href="#tos">Terms</a>
<a href="#privacy">Privacy</a>
<a href="#dev">Developer</a>
</nav>

<section id="features">
<h2>Bot Features</h2>
<div class="cards">
<div class="card">
<h3>Moderation</h3>
<p>Automatische Moderation, Warnsystem, Timeout, Kick & Ban Befehle.</p>
</div>

<div class="card">
<h3>Levelsystem</h3>
<p>XP sammeln, Ranglisten, Rollenbelohnungen und Aktivitätsstatistiken.</p>
</div>

<div class="card">
<h3>Automatisierung</h3>
<p>Auto-Role, Welcome Messages, Reaction Roles und Logs.</p>
</div>

<div class="card">
<h3>Custom Commands</h3>
<p>Eigene Commands erstellen und automatisieren.</p>
</div>
</div>
</section>

<section id="dashboard">
<h2>Dashboard Konzept</h2>
<div class="card">
<p>Ein Web-Dashboard erlaubt Serveradministratoren:</p>
<ul>
<li>Moderationseinstellungen ändern</li>
<li>Levelsystem konfigurieren</li>
<li>Auto-Moderation aktivieren</li>
<li>Custom Commands erstellen</li>
<li>Logs und Statistiken anzeigen</li>
</ul>

<p>Typischer Stack für ein Dashboard:</p>
<div class="code">
Frontend: React / Next.js
Backend: Node.js
Discord Auth: OAuth2
Database: MongoDB oder PostgreSQL
Hosting: Vercel / Railway / VPS
</div>
</div>
</section>

<section id="tos">
<h2>Terms of Service</h2>
<div class="card">
<p><strong>Letzte Aktualisierung:</strong> 15. März 2026</p>

<p>Diese Nutzungsbedingungen regeln die Nutzung des Discord-Bots <b>[BOTNAME]</b>.</p>

<h3>Nutzung</h3>
<ul>
<li>Keine illegalen Aktivitäten</li>
<li>Kein Missbrauch des Bots</li>
<li>Discord Terms müssen eingehalten werden</li>
</ul>

<h3>Haftung</h3>
<p>Der Bot wird "wie verfügbar" bereitgestellt. Der Betreiber haftet nicht für Datenverlust oder Schäden.</p>

<h3>Beendigung</h3>
<p>Server können bei Missbrauch vom Bot ausgeschlossen werden.</p>
</div>
</section>

<section id="privacy">
<h2>Datenschutzerklärung (DSGVO)</h2>
<div class="card">
<p>Der Bot kann folgende Daten speichern:</p>
<ul>
<li>Discord Benutzer-ID</li>
<li>Server-ID</li>
<li>Channel-ID</li>
<li>Server Einstellungen</li>
</ul>

<h3>Zweck</h3>
<p>Diese Daten werden ausschließlich verwendet um Funktionen des Bots bereitzustellen.</p>

<h3>Rechte der Nutzer</h3>
<ul>
<li>Auskunft über gespeicherte Daten</li>
<li>Löschung der Daten</li>
<li>Korrektur falscher Daten</li>
</ul>

<p>Anfragen: support@deine-domain.de</p>
</div>
</section>

<section id="dev">
<h2>Developer – Slash Command Beispiele</h2>
<div class="card">
<p>Beispiel für <b>/tos</b> und <b>/privacy</b> Slash Commands mit Node.js und discord.js:</p>

<div class="code">
const { SlashCommandBuilder } = require('discord.js');

module.exports = {
 data: new SlashCommandBuilder()
  .setName('tos')
  .setDescription('Zeigt die Nutzungsbedingungen'),
 async execute(interaction) {
  await interaction.reply('Terms of Service: https://deinedomain.de/#tos');
 }
};
</div>

<br>

<div class="code">
const { SlashCommandBuilder } = require('discord.js');

module.exports = {
 data: new SlashCommandBuilder()
  .setName('privacy')
  .setDescription('Zeigt die Datenschutzerklärung'),
 async execute(interaction) {
  await interaction.reply('Privacy Policy: https://deinedomain.de/#privacy');
 }
};
</div>
</div>
</section>

<section id="invite">
<h2>Bot Einladen</h2>
<div class="card">
<p>Füge den Bot zu deinem Server hinzu:</p>

<div class="code">
https://discord.com/api/oauth2/authorize?client_id=BOTID&permissions=8&scope=bot%20applications.commands
</div>
</div>
</section>

<footer>
<p>© 2026 [BOTNAME] – Discord Bot</p>
</footer>

</body>
</html>
