---
layout: default
title: Notes
lang: en
permalink: /en/notes/
translation: /notes/
---

# Notes

<p class="page-intro">Short notes about things that reduce guesswork, make problems easier to find and keep useful working context close at hand.</p>

<article class="note-card"><p class="case-kicker">HPC · PoliTech</p><h2>On a cluster, look first and change second</h2><p>Before touching the network, queue or storage, capture the current state and make sure important calculations are not affected. A clear checklist is safer than a set of commands remembered by heart.</p></article>

<article class="note-card"><p class="case-kicker">VOSK · FastAPI</p><h2>A voice service is better when it accepts the file you have</h2><p>People send mp3, ogg, m4a and many other formats. The service can prepare the audio itself, while the caller chooses the language, model size and whether punctuation is needed.</p></article>

<article class="note-card"><p class="case-kicker">Chatbots · MCP/skills</p><h2>A good chatbot also helps find an old decision</h2><p>Save messages, add search, show a few replies around a matching phrase — and a chat becomes a useful knowledge base. Codex can retrieve that fragment through a connected tool and answer with a source.</p></article>

<article class="note-card"><p class="case-kicker">MikroTik · proxy-home</p><h2>Not all home traffic needs to go through a proxy</h2><p>Selected destinations can go to a separate gateway while everything else works as usual. Keep the rules narrow, check their counters and save a router backup before a change.</p></article>

<article class="note-card"><p class="case-kicker">Telegram · ISPmanager</p><h2>Build settings instead of copying them by hand</h2><p>One set of source data can become profiles for different apps, be checked and published through ISPmanager. Short Telegram messages then show whether the router and gateway are doing well.</p></article>

<article class="note-card"><p class="case-kicker">Messenger · proxy-home</p><h2>A new service beside the gateway should not control the gateway</h2><p>Give the messenger its own address and Docker environment. Chats and authentication can then live next to proxy-home without access to its routes, TUN interface or firewall rules.</p></article>

<article class="note-card"><p class="case-kicker">Checks in CI</p><h2>A security check should not get in the way of a release</h2><p>It is better to run a check only where it is needed and get a separate, readable report. Then it helps developers instead of becoming another mysterious red build.</p></article>

<article class="note-card"><p class="case-kicker">Deployment</p><h2>A deployment should be able to run twice</h2><p>If a configuration setting is missing, the script can create it. There is no need to fill a template with dozens of empty defaults, and a repeat run is no longer a gamble.</p></article>

<article class="note-card"><p class="case-kicker">Database · CI</p><h2>Tests are not trustworthy without a known database state</h2><p>Before testing, the database needs to be in a clear state. The build checks the backup, restores the data, then deploys the app and runs the tests.</p></article>

<article class="note-card"><p class="case-kicker">Releases</p><h2>Sometimes a new file matters more than a green build</h2><p>Comparing a new archive with the previous one quickly reveals accidental libraries, debug files and packaging changes. It is a simple safety net before a release is handed over.</p></article>

<article class="note-card"><p class="case-kicker">Clusters</p><h2>Compare settings instead of debating them</h2><p>There is a trusted template and a running cluster. A script shows the difference between them without complaining about comments or addresses that change from environment to environment.</p></article>
