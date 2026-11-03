







-----------------------
         
        # e.g. "linux"
      ult branch you need
XXXXXXXXXXXXXXXXXXX"


-------------------------
e re
----------------------------
rl = ://i.s/{owner}/{po}/bll/{branch}"
ads)


#  te zip ito a localolder
zip_bytes = io.ByteO(resp.ntent)
e(zip_bytes) as z:
    # The zip contains a top‑level folde like "owner-repo-<hash>"
    # Extract everything into a folder named after the repo
    extract_path = f"./{repo}"
    os.makedirs(extract_path, exist_ok=True)
    z.extractall(path=extract_path)

print(f"✅  Repository '{owner}/{repo}' extracted to ./{repo}")



