
## 🍴 **What is a Fork in GitHub?**

A **fork** is your **own copy** of someone else's repository.

### 🔹 Why Fork?
- You **don’t have write access** to the original repo.
- You want to **experiment** or **contribute** without affecting the original project.
- Ideal for **open-source contributions**.

---

## 🔄 **What is a Pull Request (PR)?**

After you’ve made changes in your forked repo, a **Pull Request** is a request to **"pull" your changes** back into the original repo.

### 🔹 Why PR?
- It lets project maintainers **review** your changes.
- They can **discuss**, **request changes**, or **merge** it into the original.

---

## 🧪 **Fork + PR Workflow:**

Let’s say you want to contribute to an open-source repo called `test-project`.

### 👣 Step-by-Step:

1. **Fork the repository**  
   - Click `Fork` on the GitHub repo page.

2. **Clone your fork to local**  
   ```bash
   git clone https://github.com/your-username/test-project.git
   ```

3. **Create a new branch**  
   ```bash
   git checkout -b feature/my-enhancement  # feature/my-enhancement is the name of the new branch
   ```

4. **Make changes and commit**  
   ```bash
   git add .
   git commit -m "Added new feature"
   ```

5. **Push to your forked repo**  
   ```bash
   git push origin feature/my-enhancement
   ```

6. **Create a Pull Request**  
   - Go to the original repo on GitHub.
   - Click `Compare & pull request`.
   - Add a title, description, and submit it!

---

The owner of the original repo sees your PR.
They can review, comment, request changes, or merge it into their main branch.

---

## ☝️ 3 things to remember while making a pull request

1. **Write small pull request**
   - Easier to review and merge
   - Less room for bugs
   - Clear history of changes

2. **Review your own pull request first**
   - Review + build + test your PRs

3. **Provide context and Guidance**
   - Help your reviewer by writing clear titles and descriptions and add links!
