#docker pull nginx
FROM nginx
# Install dependencies
RUN apt update && \ 
    # utilse  '\'  pour retourne  a la ligne 
    apt install nano -y
# Copy the rest of the application code to the container
COPY index.html /usr/share/nginx/html/    
# Expose port 80 for the application
ENV port=80
EXPOSE ${port}
# # Add a volume mount point
# VOLUME ["/usr/share/nginx/html/"]
# # Set the working directory
# WORKDIR /usr/share/nginx/html/