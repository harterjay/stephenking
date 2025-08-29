# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML application that creates an interactive Stephen King bibliography with Excel export functionality. The project is entirely self-contained and runs in the browser without any build process or external dependencies.

## Architecture

The application is a standalone HTML file (`stephen_king_excel_generator.html`) that combines:

- **Frontend**: HTML5 with CSS3 styling featuring glassmorphism design
- **Data**: Hardcoded JavaScript array containing Stephen King's complete bibliography (80+ books)
- **Functionality**: Vanilla JavaScript for filtering, searching, tooltips, and Excel generation
- **External Dependencies**: SheetJS XLSX library loaded from CDN for Excel export

Key features:
- Interactive book cards with hover tooltips showing plot summaries and publication facts
- Filtering by book type (novels, collections, novellas, non-fiction, Bachman books)
- Search functionality by title
- Statistics dashboard
- Excel export with customizable data selection

## Development Commands

This project requires no build process or package management:

- **Run locally**: Open `stephen_king_excel_generator.html` directly in any modern web browser
- **No installation needed**: All dependencies loaded via CDN
- **No server required**: Runs entirely client-side

## Code Structure

The single HTML file contains:
- Embedded CSS with custom styling and responsive design
- Comprehensive book data array with metadata for each Stephen King publication
- JavaScript modules for:
  - Book filtering and search
  - Statistics calculation
  - Tooltip management
  - Excel file generation
  - DOM manipulation

## Data Schema

Each book entry contains:
- Title, Type, Date, Category, Year
- Plot summary
- Publication facts and trivia
- Categorization for filtering (novel, collection, novella, nonfiction, bachman)

## Browser Compatibility

Requires modern browser with support for:
- ES6 JavaScript features
- CSS Grid and Flexbox
- HTML5 semantic elements