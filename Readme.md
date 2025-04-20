# 📄 CV en LaTeX + Docker

Este repositorio contiene mi currículum vitae escrito en **LaTeX**, con la ventaja de que puede compilarse fácilmente utilizando **Docker**. De esta forma, no necesitas instalar LaTeX localmente en tu máquina.

---

## 🚀 Cómo compilar el CV con Docker

### 🐳 Requisitos

- Tener [Docker](https://www.docker.com/products/docker-desktop/) instalado.

### 📦 Comando de compilación

Desde la raíz del proyecto (donde está `cv.tex`), ejecutá:

```bash
docker run --rm -v $(pwd):/data -w /data texlive/texlive pdflatex cv.tex
