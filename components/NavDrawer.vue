<template>
  <section>
    <!-- Navigation Drawer -->
    <div class="layout-drawer is-open">
      <div class="drawer-header drawer-header-cover" style="background-color: #3b1a50; color: #FFFFFF;">
        <div class="drawer-user">
          <div class="drawer-avatar">
            <img
              src="https://lh3.googleusercontent.com/Lq_SheAKhz2hGawK5jvt0B32y8d0OXiDy3dL8518Ksg4kVWocrWtJibaADYhlGTnfMaq75ySmiSfpOEs=s220-rw">
          </div>
          <div class="drawer-meta">
            <span class="drawer-name">Beth Johnston</span>
            <span class="drawer-email">bjohnston@suvoda.com</span>
          </div>
        </div>
      </div>
      <nav class="drawer-navigation drawer-border">
        <a class="drawer-list-item" href="javascript:"><span>Reports</span><i class="material-icons">expand_more</i></a>


        <a class="drawer-list-item" href="javascript:"><span>Changes</span><i class="material-icons">expand_more</i></a>

        <a class="drawer-list-item" href="javascript:"><span>Settings</span><i
            class="material-icons">expand_more</i></a>


      </nav>



      <nav class="drawer-navigation">
        <a class="drawer-list-item drawer-icon-right" href="javascript:">
          <span>Need Help</span><i class="material-icons">sms</i>
        </a>
      </nav>
    </div>



    <!-- Other contents (not included) -->
    <header class="layout-header">
      <button class="header-drawer-toggle">
        <i class="material-icons">menu</i>
      </button>
      <span class="header-title hidden">Navigation Drawer</span>
      <span class="header-title default">Material — Navigation Drawer</span>
    </header>
  </section>
</template>

<script>

export default {
  name: 'NavDrawer',
  setup() {
    const handleScroll = () => {
      window.scrollTo(0, document.body.scrollHeight);
    }
    return {
      handleScroll
    }
  }
}
</script>
<style>
/**
 * Material — Navigation Drawer
 */
.elevation{
  box-shadow: 0 16px 24px 2px rgba(0, 0, 0, 0.14), 0 6px 30px 5px rgba(0, 0, 0, 0.12), 0 8px 10px -5px rgba(0, 0, 0, 0.2);
}

body {
  color: #000000;
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
  font-weight: 400;
  letter-spacing: 1px;
  margin: 0;
  min-height: 100%;
  width: 100%;
}

.layout-drawer {
  background-color: #FFFFFF;
  box-shadow: 0 16px 24px 2px rgba(0, 0, 0, 0.14), 0 6px 30px 5px rgba(0, 0, 0, 0.12), 0 8px 10px -5px rgba(0, 0, 0, 0.2);
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  overflow-x: hidden;
  overflow-y: auto;
  position: fixed;
  left: 0;
  top: 0;
  transform: translateX(-296px);
  transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  height: 100%;
  max-width: 280px;
  min-width: 280px;
  width: 280px;
  z-index: 4;
}

.layout-drawer.is-open {
  transform: translateX(0);
}

.layout-drawer * {
  flex-shrink: 0;
}

.layout-drawer .drawer-header {
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  padding: 8px 0;
  position: relative;
}

.layout-drawer .drawer-header.drawer-border {
  border-bottom: 1px solid #CCCCCC;
}

.layout-drawer .drawer-header.drawer-header-cover {
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}

.layout-drawer .drawer-header .drawer-user {
  display: flex;
  flex-direction: column;
  position: relative;
}

.layout-drawer .drawer-header .drawer-user .drawer-avatar {
  box-sizing: border-box;
  background: #EEEEEE;
  border-radius: 50%;
  margin: 16px 0 8px 24px;
  height: 64px;
  width: 64px;
}

.layout-drawer .drawer-header .drawer-user .drawer-avatar img {
  border-radius: inherit;
  height: 100%;
  width: 100%;
}

.layout-drawer .drawer-header .drawer-user .drawer-meta {
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
  height: 56px;
}

.layout-drawer .drawer-header .drawer-user .drawer-meta .drawer-name,
.layout-drawer .drawer-header .drawer-user .drawer-meta .drawer-email {
  padding-left: 24px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.layout-drawer .drawer-header .drawer-user .drawer-meta .drawer-name {
  font-family: 'Roboto', sans-serif;
  font-weight: 500;
}

.layout-drawer .drawer-navigation {
  display: flex;
  flex-direction: column;
  padding: 8px 0;
}

.layout-drawer .drawer-navigation.drawer-border {
  border-bottom: 1px solid #CCCCCC;
}

.layout-drawer .drawer-navigation .drawer-navigation {
  padding: 0;
}

.layout-drawer .drawer-navigation .drawer-navigation.drawer-border {
  border-bottom: none;
}

.layout-drawer .drawer-navigation .drawer-navigation .drawer-list-item {
  color: rgba(0, 0, 0, 0.74);
  padding-left: 48px;
  height: 36px;
}

.layout-drawer .drawer-navigation .drawer-navigation .drawer-list-item:focus {
  color: rgba(0, 0, 0, 0.87);
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle,
.layout-drawer .drawer-navigation .drawer-list-item,
.layout-drawer .drawer-navigation .drawer-subtitle {
  box-sizing: border-box;
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
  font-weight: 500;
  padding-left: 24px;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle,
.layout-drawer .drawer-navigation .drawer-list-item {
  color: rgba(0, 0, 0, 0.87);
  display: flex;
  align-items: center;
  position: relative;
  transition: background-color 0.3s cubic-bezier(0.4, 0, 0.2, 1), color 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  height: 48px;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle:focus,
.layout-drawer .drawer-navigation .drawer-list-item:focus {
  background-color: #E0E0E0;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle:focus .drawer-badge,
.layout-drawer .drawer-navigation .drawer-list-item:focus .drawer-badge {
  background-color: rgba(0, 0, 0, 0.87);
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle:focus .material-icons,
.layout-drawer .drawer-navigation .drawer-list-item:focus .material-icons {
  color: rgba(0, 0, 0, 0.87);
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle.is-active,
.layout-drawer .drawer-navigation .drawer-list-item.is-active {
  color: #3B1A50;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle.is-active .drawer-badge,
.layout-drawer .drawer-navigation .drawer-list-item.is-active .drawer-badge {
  background-color: #3B1A50;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle.is-active .material-icons,
.layout-drawer .drawer-navigation .drawer-list-item.is-active .material-icons {
  color: inherit;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle span,
.layout-drawer .drawer-navigation .drawer-list-item span {
  flex-grow: 1;
  flex-shrink: 1;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle .material-icons,
.layout-drawer .drawer-navigation .drawer-list-item .material-icons {
  color: rgba(0, 0, 0, 0.54);
  margin-right: 24px !important;
  transition: color 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle .drawer-badge,
.layout-drawer .drawer-navigation .drawer-list-item .drawer-badge {
  background-color: rgba(0, 0, 0, 0.54);
  border-radius: 2px;
  box-sizing: border-box;
  color: #FFFFFF;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-family: 'Roboto', sans-serif;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  margin-right: 24px;
  padding: 0 4px;
  transition: background-color 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  height: 24px;
  min-width: 24px;
}

.layout-drawer .drawer-navigation .drawer-dropdown-toggle {
  background-color: transparent;
  border: none;
  cursor: pointer;
  margin: 0;
  outline: 0;
  padding: 0 0 0 24px;
  text-align: left;
}

.layout-drawer .drawer-navigation .drawer-list-item {
  text-decoration: none;
}

.layout-drawer .drawer-navigation .drawer-subtitle {
  color: rgba(0, 0, 0, 0.54);
  overflow: hidden;
  padding-top: 8px;
  text-overflow: ellipsis;
  height: 40px;
  white-space: nowrap;
}
</style>
