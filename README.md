import streamlit as st

# Título de la aplicación
st.title("Fútbol: Noticias y Estadísticas")

# Descripción introductoria
st.write("Bienvenido a la aplicación de fútbol. Aquí puedes encontrar información sobre equipos, jugadores y estadísticas recientes.")

# Sección de Noticias
st.header("Últimas Noticias de Fútbol")
st.text("1. El Real Madrid vence en el clásico contra el Barcelona.")
st.text("2. Lionel Messi se lleva el Balón de Oro 2024.")
st.text("3. La Premier League alcanza cifras récord de audiencia.")

# Tabla de Estadísticas
st.header("Estadísticas de Jugadores")
data = {
    "Jugador": ["Lionel Messi", "Cristiano Ronaldo", "Erling Haaland", "Kylian Mbappé"],
    "Goles": [30, 28, 25, 27],
    "Asistencias": [12, 10, 8, 14]
}
st.table(data)

# Entrada interactiva
st.header("Busca información sobre tu equipo favorito")
equipo = st.text_input("Escribe el nombre del equipo")
if equipo:
    st.write(f"Estás buscando información sobre el equipo: {equipo}")
    st.write("Por favor, permanece atento mientras ampliamos esta sección.")

# Imagen representativa
st.image(
    "https://upload.wikimedia.org/wikipedia/commons/6/66/Soccer_ball.svg",
    caption="Fútbol: El deporte más popular del mundo",
    use_column_width=True
)

# Footer
st.write("---")
st.write("Creado con Streamlit. Mantente al día con lo último del mundo del fútbol.")
