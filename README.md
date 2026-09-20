# averis
Averis Hackathon 2026

## Setup instruction: Running in localhost
Ensure that Node.js and npm are installed in the device.
Run the following commands in the terminal to ensure they are installed correctly.

```bash
node -v
```
```bash
npm -v
```
The terminal should give the version of Node.js and npm, for example 11.6.2 and v24.13.0


### Step 1: Clone the Repository
```bash
git clone
https://github.com/WanQi-01/averis.git
```

### Step 2: Navigate into project folder
```bash
cd averis
```

### Step 3: Install Dependencies
Navigate into the app folder and install dependencies:
```bash
cd averisapp
npm install
```

### Step 4: Create .env.local file
Create a new file named `.env.local` inside the `averisapp/` folder and add the following variables:

```env
NEXT_PUBLIC_SUPABASE_URL=<replace this with the project URL>
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=<replace this with the project API anon key>
SUPABASE_SERVICE_ROLE_KEY=<replace this with the service role key>
```

To find the Supabase values, go to your [Supabase project dashboard](https://supabase.com/dashboard) → select the project → **Settings** → **API**. You will find the Project URL, the anon/public key (`NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY`), and the service role key (`SUPABASE_SERVICE_ROLE_KEY`) there.

### Step 5: Run the Deployment Server
Run the following command in the terminal:
```bash
cd averisapp
npm run dev
```

### Step 6: Open the project in your browser
Open [http://localhost:3000] in your browser to view the project.


## Additional Notes & COmmon Issues

### Error 1: Module Not Found: Can't Resolve 'react-icons'
- Open the terminal and run `npm install react-icons` in the terminal.

### Error 2: Port in use
- If the project fails to start with `Error: port 3000 is already in use`
- Stop the process manually or change the port in `package.json`

### Error 3: Supabase Connection issues
- Check if the Supabase URL and API keys are correct
    - NEXT_PUBLIC_SUPABASE_URL
    - NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY
    - SUPABASE_SERVICE_ROLE_KEY
- Do not put a space between the variables and values, e.g. `SUPABASE_SERVICE_ROLE_KEY =`
- Restart the development server after changing .env.local



### After checking, restart the development server
```bash
cd averisapp
npm install
```



