# SkinCare AI

Plataforma web de apoyo al tamizaje temprano de lesiones cutáneas (proyecto académico, Universidad del Norte).

- **Página:** https://marchenayamit-cyber.github.io/skincare/
- Compara dos modelos entrenados con ISIC 2019: **CNN pura** (ResNet50 con *fine-tuning*) y **CNN + KNN** (k = 21, distancia coseno sobre los embeddings de la CNN).
- Muestra la probabilidad de malignidad calibrada (temperature scaling, T = 2.630), la decisión según el umbral ajustado en validación y el mapa **Grad-CAM**.
- El modelo corre en el navegador con ONNX Runtime Web: las imágenes no salen del equipo del usuario.
- Inicio de sesión básico: contraseñas guardadas como hash PBKDF2-SHA256 en el navegador.

Ver `LEEME.txt` para la descripción de cada archivo.

> Herramienta de apoyo al tamizaje con fines académicos. No es un diagnóstico médico ni reemplaza a un dermatólogo.
