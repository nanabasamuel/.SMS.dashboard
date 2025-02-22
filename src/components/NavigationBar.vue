<template>
  <div class="header-container">
    <!-- Original nav section -->
    <nav class="nav-wrapper">
      <div class="left-section">
        <!-- Logo with Font Awesome -->
        <div class="logo">
          <i class="fas fa-bolt logo-icon"></i>
          <span class="logo-text">sMs</span>
        </div>
        
        <!-- Menu Toggle -->
        <button class="menu-toggle">
          <i class="fas fa-bars"></i>
        </button>

        <!-- Search Section -->
        <div class="search-section">
          <input 
            type="text" 
            placeholder="Search projects..."
            class="search-input"
          >
        </div>
      </div>

      <!-- Icons Section -->
      <div class="icons-section">
        <button class="icon-btn">
          <i class="fas fa-envelope"></i>
        </button>
        <button class="icon-btn">
          <i class="fas fa-bell"></i>
        </button>
        <button class="icon-btn">
          <i class="fas fa-cog"></i>
        </button>
      </div>
    </nav>
    
    <!-- Extended background section -->
    <div class="extended-section"></div>
  </div>
</template>

<script>
export default {
  name: 'NavigationBar'
}
</script>

<style scoped>
.header-container {
  background-color: var(--primary-color);
}

.nav-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.75rem 1.5rem;
  color: var(--icon-hover);
}

.extended-section {
  height: 180px; /* Adjust this value to control how far down the background extends */
  width: 100%;
}

.left-section {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.logo {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: var(--text-light);
  font-size: 1.25rem;
  font-weight: 500;
  margin-right: 0.5rem;
}

.logo-icon {
  color: var(--text-light);
  font-size: 1.25rem;
}

.menu-toggle {
  background: none;
  border: none;
  color: var(--text-light);
  font-size: 1.25rem;
  cursor: pointer;
  padding: 0.5rem;
  transition: color 0.2s;
  margin-left: 8rem;
}

.menu-toggle:hover {
  color: var(--icon-hover);
}

.search-section {
  margin-left: 0.5rem;
}

.search-input {
  width: 400px;
  padding: 0.5rem 1rem;
  background-color: var(--background-light);
  border: none;
  border-radius: 4px;
  color: var(--text-dark);
  font-size: 0.9rem;
}

.search-input::placeholder {
  color: var(--input-text);
}

.icons-section {
  display: flex;
  gap: 1rem;
  align-items: center;
}

.icon-btn {
  background: none;
  border: none;
  color: var(--text-light);
  font-size: 1.25rem;
  cursor: pointer;
  padding: 0.5rem;
  transition: color 0.2s;
}

.icon-btn:hover {
  color: var(--icon-hover);
}
</style>