**Test Question:**

**Lab Start Command:** `[student@workstation ~]$ lab start persisting-mounting`

**Problem 1:**

1. Examine the `~/DO188/labs/persisting-mounting/podman-python-server/Containerfile` file. This image uses the `/server` directory as the web root directory for the Python HTTP server. The `registry.ocp4.example.com:8443/redhattraining/podman-python-server` container image is based on this Containerfile.

   Provide the contents of the `Containerfile`.

**Problem 2:**

2. Copy the `index.html` file to the `~/www` directory. The `~/www` directory serves as a bind mount that contains the HTML for the container.

   Provide the command used to copy the `index.html` file.

**Problem 3:**

3. Test the `podman-python-server` container with the `~/www` directory mounted as a bind mount.

   a) Provide the command used to start the container with the given parameters.

   b) In a web browser, navigate to `localhost:8000`. You are presented with an error.

   c) Provide the command used to check the container logs.

**Problem 4:**

4. Correct the permission for the `~/www` directory.

   a) Provide the command used to verify the directory permissions in a new user namespace.

   b) Provide the command used to verify the group ID inside of the `podman-server` container.

   c) Provide the command used to change the group of the `~/www` directory and its content to the `python-server` group ID.

   d) Provide the command used to verify the directory permissions in a new user namespace after making the changes.

**Problem 5:**

5. Retest the `podman-server` container with the `~/www` directory mounted as a bind mount.

   a) In a web browser, access `localhost:8000`. You are presented with the `index.html` page.

   b) Provide the command used to stop the container.

**Problem 6:**

6. Create a named volume with the `index.html` page.

   a) Provide the command used to create a volume called `html-vol`.

   b) Provide the command used to change into the `persisting-mounting` lab directory.

   c) Provide the command used to import the `index.tar.gz` archive file into the `html-vol` volume.

**Problem 7:**

7. Start a new container that uses the `podman-server` image. Use a volume mount instead of the bind mount.

   a) Provide the command used to start the `podman-server` container with the given parameters.

   b) In a web browser, access `localhost:8000`. You are presented with the `index.html` page.

   c) Provide the command used to stop the container.

**Lab Finish Command:** `[student@workstation ~]$ lab finish persisting-mounting`

**Note:** Follow each step carefully and provide the required information or commands as instructed.
