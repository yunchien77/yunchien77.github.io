---
title: Setting Up Your Own Blog with Jekyll on Windows
date: 2025-08-19 14:00:00 +0800
author: Chien
categories: [ Jekyll ]
tags: [ Website, Jekyll, GitHub Page ]
summary: Let's build a personal website.
---

A step-by-step guide to installing and using Jekyll (with the Chirpy theme) to build your personal website:

[Tutorial for Windows](https://jekyllrb.com/docs/installation/windows/)

[Quickstart](https://jekyllrb.com/docs/)

[Themes](https://jekyllrb.com/docs/themes/)

## 1. Install Ruby (with Devkit version)

- Download the Windows 64-bit Ruby installer with Devkit from the official page:  
  [Ruby Installer](https://rubyinstaller.org/downloads/)

- After installation, the command prompt will open automatically to install the necessary MSYS2 software. During installation, either press Enter to accept the default options or select the `MSYS2 and MINGW development toolchain` option. Close the command prompt when finished.

---

## 2. Install Jekyll and Bundler

- Open the "Start Command Prompt with Ruby" terminal.  
- Update the RubyGems system:

  ```
  gem update --system
  ```
- Install Jekyll and Bundler:

  ```
  gem install jekyll bundler
  ```
- Verify the installation:

  ```
  jekyll -v
  ```

---

## 3. Choose a Jekyll Theme

- You can browse popular themes here to find one you like:  
  [Themes Page](http://jekyllthemes.org/)  
- For this guide, we use the Chirpy theme from GitHub:  
  [jekyll-theme-chirpy Github](https://github.com/cotes2020/jekyll-theme-chirpy/)

---

## 4. Download and Set Up the Chirpy Project

- Run the following commands in your terminal:

  ```
  git clone https://github.com/cotes2020/jekyll-theme-chirpy.git
  cd jekyll-theme-chirpy
  ```
- Install the project dependencies:

  ```
  bundle install
  ```

---

## 5. Start the Local Server for Preview

- From the project directory, run:

  ```
  bundle exec jekyll serve --watch
  ```
- The preview URL is usually:  
  [http://127.0.0.1:4000](http://127.0.0.1:4000)

---

## 6. Further Configuration

- Check out the official Chirpy theme Wiki for in-depth customization and usage tips:  
  [jekyll-theme-chirpy/wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)  
- You can also refer to the Chirpy Starter template for a quick start:  
  [chirpy-starter](https://github.com/cotes2020/chirpy-starter)