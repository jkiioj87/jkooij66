







-----------------------
         
        # e.g. "linux"
      ult branch you need
XXXXXXXXXXXXXXXXXXXXXXXX"


-------------------------
hole repo)
----------------------------
ip_url = f"https://api.github.com/repos/{owner}/{repo}/zipball/{branch}"
resp = requests.get(zip_url, headers=headers)
se_for_status()

#  the zip into a local folder
zip_bytes = io.BytesIO(resp.content)
with zipfile.ZipFile(zip_bytes) as z:
    # The zip contains a top‑level folde like "owner-repo-<hash>"
    # Extract everything into a folder named after the repo
    extract_path = f"./{repo}"
    os.makedirs(extract_path, exist_ok=True)
    z.extractall(path=extract_path)

print(f"✅  Repository '{owner}/{repo}' extracted to ./{repo}")



