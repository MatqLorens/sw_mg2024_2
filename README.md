# **Projekt: CI/CD z Docker i GitHub Actions**

## **Opis projektu**

Niniejszy projekt przedstawia konfigurację **łańcucha CI/CD** do budowania, skanowania i publikowania obrazów Docker przy użyciu **GitHub Actions**. Głównym celem jest zapewnienie, że obrazy nie zawierają podatności sklasyfikowanych jako **krytyczne** lub **wysokie**, zanim zostaną przesłane do **GitHub Container Registry (GHCR)**.  
Workflow korzysta z narzędzia **Docker Scout** do analizy obrazów pod kątem podatności.

---

## **Weryfikacja Działania Workflow**

### **Uruchomienie Workflow**
Workflow można uruchomić na dwa sposoby:
- Ręcznie za pomocą **workflow_dispatch**.
- Automatycznie po utworzeniu tagu (`v1.0.0`).

### **Wynik w GHCR**
Po zakończeniu działania workflow obraz jest dostępny w GitHub Container Registry:
