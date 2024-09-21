# Artifact-deployment

**Artifact deployment** ka matlab hai kisi software project ke final build output (jo ki **artifact** hota hai) ko production ya kisi specific environment me deploy karna ya place karna, taaki wo project wahan kaam kare sake. 

Yeh artifact ho sakta hai:
- **JAR file** (Java application ke liye)
- **WAR file** (Web application ke liye)
- **Docker image** (containerized application ke liye)
- **Executable files** (compiled code)
- **Static files** (HTML, CSS, JS for web apps)

### Artifact Deployment ka Process:

1. **Build**: Jab aap apni application ka code likhte hain, to usse build karte waqt ek executable ya deployable file banti hai. Isko hum artifact kehte hain.
   - Example: Maven project se `.jar` ya `.war` file banana.

2. **Storage**: Build hone ke baad artifact ko kisi artifact repository me store kiya jaata hai, jaise:
   - **Jenkins** ke through build karke **Nexus** ya **Artifactory** me store karna.
   - **Docker images** ko **DockerHub** ya private registry me store karna.

3. **Deployment**: Ab ye artifact ready hota hai deploy hone ke liye. Isko kisi environment (Dev, QA, Staging, Production) me deploy kiya jaata hai.
   - **Cloud servers** (AWS EC2, GCP, etc.) par deploy karna.
   - **Kubernetes clusters** me deploy karna.
   - **On-premise servers** par deploy karna.

### Real-Life Example:

1. **JAR Deployment**: 
   - Aapne ek Java project build kiya. Usse `.jar` file bani. Is jar file ko aap production server par deploy karenge taaki application run kare.

2. **Docker Deployment**: 
   - Aapne Docker image banayi aur usse `DockerHub` me push kiya. Us Docker image ko aap production server par pull karke run karenge.

3. **Web App Deployment**:
   - Aapne React/Angular app banaya aur usse static HTML, CSS, aur JS files me convert kiya (artifact). Ab in files ko aap kisi web server (jaise Nginx, Apache) par deploy karenge taaki users unhe access kar sakein.

### Conclusion:
Artifact deployment ka matlab hai, apni application ke final output ko (artifact) production ya kisi environment me deploy karke usse use karna.
