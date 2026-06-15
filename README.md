# TP Integrador - Computación Aplicada
## Equipo Rojo

### Integrantes
- Luciano Helguero
- Rodrigo Stepaniuk
- Mayra Melina Rossi

### Descripción
Repositorio de entrega del Trabajo Práctico Integrador.
Contiene los backups comprimidos de los directorios del servidor Debian configurado.

### Contenido
- `root.tar.gz` — Backup del directorio /root
- `etc.tar.gz` — Backup del directorio /etc
- `opt.tar.gz` — Backup del directorio /opt
- `www_dir.tar.gz` — Backup del directorio /www_dir
- `backup_dir.tar.gz` — Backup del directorio /backup_dir
- `var.tar.gz.part_*` — Backup del directorio /var, spliteado en partes de 50MB

### Cómo recomponer /var
Las partes de /var se vuelven a unir y descomprimir con:
\`\`\`bash
cat var.tar.gz.part_* > var.tar.gz
tar -xzf var.tar.gz
\`\`\`
