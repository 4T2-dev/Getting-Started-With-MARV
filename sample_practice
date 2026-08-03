# ==========================================
# MARV Student Tutorial - Practice Script
# ==========================================
# Welcome! You opened this file using an interactive MARV project button.

def calculate_progress(completed_tasks, total_tasks):
    """Calculate student completion percentage."""
    if total_tasks <= 0:
        return 0.0
    percentage = (completed_tasks / total_tasks) * 100
    return round(percentage, 1)

def display_welcome_banner():
    """Print an encouraging welcome banner."""
    title = "Welcome to your MARV Interactive Workspace!"
    divider = "=" * len(title)
    print(divider)
    print(title)
    print(divider)

if __name__ == "__main__":
    display_welcome_banner()
    total = 5
    done = 5
    progress = calculate_progress(done, total)
    print(f"\nCourse Progress: {done}/{total} steps complete ({progress}%).")
    print("Great job navigating your code workspace!")
