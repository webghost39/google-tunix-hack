# Setup Instructions

## How to run the gemma2-2b demo

### 1. Weights & Biases (W&B) Setup

1. Go to [https://wandb.ai/](https://wandb.ai/) to sign up for an account
2. Get your API key
3. In your Kaggle notebook:
   - Go to **Add-ons** in the menu
   - Click **Secrets**
   - Add a new secret with:
     - Label: `WANDB_API_KEY`
     - Value: Your W&B API key

### 2. Kaggle API Setup

1. Go to your Kaggle settings and get your username
2. Create an API key in Kaggle settings
3. In your Kaggle notebook, create two secrets:
   - Secret 1:
     - Label: `KAGGLE_USERNAME`
     - Value: Your Kaggle username
   - Secret 2:
     - Label: `KAGGLE_KEY`
     - Value: Your Kaggle API key

### 3. Running the Notebook

1. Import the notebook (`grpo-demo-gemma2-2b-207651-11232025.ipynb`) to your Kaggle account
2. Click **Run All** to execute all cells

**Important Notes:**
- The full run takes approximately **1 hour 20 minutes** to complete
- Session timeout may cause failures - it's recommended to **run in background**
- To run in background:
  1. Click the **Save Version** button
  2. Change version type to **Save & Run All (Commit)**
  3. In Advanced Settings, enable **Save Output**

The notebook I shared would failed after training finished since I commented out the `wandb.init(project='tunix')`, you can uncomment it to check if it works.
