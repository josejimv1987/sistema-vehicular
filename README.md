# 🚗 Sistema de Gestión Vehicular

![Badge](https://img.shields.io/badge/Status-Desarrollo%20Activo-brightgreen)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![MySQL](https://img.shields.io/badge/MySQL-8.0-orange)
![React](https://img.shields.io/badge/React-18+-61DAFB)

Sistema completo para gestión de vehículos, usuarios y reservas con arquitectura moderna.

## 🌟 Características Principales
- **Gestión de Flota**: Registro detallado de vehículos (marca, modelo, año, etc.)
- **Reservas Inteligentes**: Sistema de reservas con verificación de disponibilidad en tiempo real
- **Dashboard Administrativo**: Visualización de métricas clave y reportes
- **Autenticación Segura**: Roles de usuario (admin/cliente) con JWT
- **API RESTful**: Documentación Swagger incluida

## 🛠 Stack Tecnológico
| Capa         | Tecnologías                                                                 |
|--------------|-----------------------------------------------------------------------------|
| **Frontend** | React 18, Vite, Tailwind CSS, Axios, React Query                            |
| **Backend**  | Python Flask, SQLAlchemy, Flask-RESTful, Flask-Migrate, JWT                 |
| **Base de Datos** | MySQL 8.0 (Dockerizado) con relaciones avanzadas                          |
| **DevOps**   | Docker, GitHub Actions, ESLint + Prettier                                  |

## 🚀 Instalación Rápida

### Requisitos Previos
- Docker 20.10+
- Node.js 18+
- Python 3.10+

```bash
# 1. Clonar repositorio
git clone https://github.com/tu-usuario/sistema-vehicular.git
cd sistema-vehicular

# 2. Iniciar contenedores
docker-compose up -d

# 3. Instalar frontend
cd frontend && npm install && npm run dev

# 4. Configurar backend
cd ../backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
flask db upgrade
flask run
