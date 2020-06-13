# podman-save-commit

      #podman pull docker.io/httpd : First we pull the image , in these case we are pulling the httpd image
  
      #podman images : using this command we see image is get pulled or not
      #podman run -it cc bash :using this command we run the command and do changes in the file and exit from it
      #podman ps : using this command we can se the runnig containers
      #podman ps -a :uysing this command we can see all the containers which are running and not running 
      #podman commit 0438d587c367 sagar : using this command we can commit the exited container to a new image (syntax is podman commit <container_id> new_image_name)
      #podman images : using this command we can see the newly created image
      #podman save -o sagar.tar localhost/sagar : now we have to convert the image into tar file so we can share to to other and they we also used it so using this comman dwe can save it to tar file (syntax podman save -o <tar_file_name> <image_name_or_image_id>)
      #ls : this will show the tar file
      #podman rmi 9b : now we remove the image.
      #podman images : check whether the image is present or not
      #podman load -i sagar.tar : Now load the tar file to image and we can use that file
      #podman images :  Now we  can see the image 
      #podman run -d -p 18080:80 localhost/sagar : run that image
      #podman ps : ee the container is running or not
