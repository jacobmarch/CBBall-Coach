# Project Design: College Basketball Coach Simulator - Gameplay Flow

## 1. Overview

This document outlines the gameplay flow for a browser-based college basketball coach simulator game, focusing on a quick and streamlined experience. The player manages recruiting, roster, and strategies, then simulates games to progress through seasons.

### Tech Stack

- Frontend: Vue with Vite
- Backend: Flask
- Database: SQLite

## 2. Core Gameplay Loop

The game revolves around a seasonal loop: Offseason -> Preseason -> Regular Season -> Postseason. The focus is on strategic decision-making and efficient simulation.

## 3. Detailed Gameplay Flow

### 3.1. Offseason

The offseason is dedicated to recruiting and roster management. It consists of five stages:

1.  **Transfer Portal - Stage 1 (Initial Scouting):** Evaluate available players in the transfer portal.  Identify potential targets based on needs and available scholarships.
2.  **Transfer Portal - Stage 2 (Recruiting):**  Make offers and attempt to sign transfer players. Players have attributes and desired roles that influence their decision.
3.  **High School Recruiting - Stage 1 (Scouting):** Scout high school prospects.  Limited scouting resources require strategic allocation.
4.  **High School Recruiting - Stage 2 (Offers & Visits):** Offer scholarships and schedule visits for top recruits. Manage recruiting budget and prioritize targets.
5.  **High School Recruiting - Stage 3 (Commitments):** Recruits make their commitment decisions.  Success depends on scouting, offers, and program prestige.

**Roster Requirement:** The user must have at least 10 players on their roster to begin the season. If they do not, they will be assigned random players with low ratings to fill out the remainder of the roster.

### 3.2. Preseason

The preseason involves setting up the team for the upcoming season.

1.  **Roster Configuration:** Choose starting lineup and bench players.  Consider player attributes, morale, and chemistry.
2.  **Strategy Selection:** Select offensive and defensive strategies.  Choose from a variety of pre-set strategies or customize existing ones. This is the primary strategic input before games.

### 3.3. Regular Season

The regular season consists of simulated games.

1.  **Game Simulation:** Games are simulated based on team attributes, selected strategies, and a degree of randomness.
2.  **Score Display:** The user views the final score and basic game statistics. No in-game intervention is possible; the focus is on pre-game strategy.

### 3.4. Postseason

The postseason consists of the conference tournament and, if qualified, the national tournament.

1.  **Conference Tournament:** Participate in the conference tournament.  Games are simulated as in the regular season.
2.  **National Tournament (NCAA):** If the team qualifies, participate in the national tournament. Games are simulated as in the regular season.
3.  **Season End:** After the tournaments conclude, the game returns to the offseason, restarting the gameplay loop.

## 4. Key Considerations

*   **Streamlined Simulation:** The focus is on quick game simulations with minimal user intervention during games.
*   **Strategic Depth:** The depth of the game comes from recruiting, roster management, and pre-game strategy selection.
*   **Progression:** The player progresses by improving their team through recruiting and strategic decisions, leading to better performance in simulated games and tournaments.

