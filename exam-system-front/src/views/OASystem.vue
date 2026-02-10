<template>
  <div class="oa-system-container">
    <div class="oa-header">
      <h1>OA系统</h1>
      <p>办公自动化管理平台</p>
      <button class="back-btn" @click="goBack">返回中心</button>
    </div>
    
    <div class="oa-content">
      <div class="nav-menu">
        <ul>
          <li>
            <router-link to="/oa/dashboard">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect>
                <line x1="3" y1="9" x2="21" y2="9"></line>
                <line x1="9" y1="21" x2="9" y2="9"></line>
              </svg>
              <span>仪表盘</span>
            </router-link>
          </li>
          <li>
            <router-link to="/oa/users">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
                <circle cx="9" cy="7" r="4"></circle>
                <path d="M23 21v-2a4 4 0 0 0-3-3.87"></path>
                <path d="M16 3.13a4 4 0 0 1 0 7.75"></path>
              </svg>
              <span>用户管理</span>
            </router-link>
          </li>
          <li>
            <router-link to="/oa/departments">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M3 6h18"></path>
                <path d="M3 12h18"></path>
                <path d="M3 18h18"></path>
              </svg>
              <span>部门管理</span>
            </router-link>
          </li>
          <li>
            <router-link to="/oa/documents">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect>
                <line x1="16" y1="2" x2="16" y2="6"></line>
                <line x1="8" y1="2" x2="8" y2="6"></line>
                <line x1="3" y1="10" x2="21" y2="10"></line>
              </svg>
              <span>公文管理</span>
            </router-link>
          </li>
          <li>
            <router-link to="/oa/approvals">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path>
                <polyline points="22 4 12 14.01 9 11.01"></polyline>
              </svg>
              <span>审批管理</span>
            </router-link>
          </li>
          <li>
            <router-link to="/oa/schedules">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <circle cx="12" cy="12" r="10"></circle>
                <polyline points="12 6 12 12 16 14"></polyline>
              </svg>
              <span>日程管理</span>
            </router-link>
          </li>
        </ul>
      </div>
      
      <div class="feature-grid">
        <div class="feature-card" @click="navigateTo('/oa/dashboard')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect>
              <line x1="3" y1="9" x2="21" y2="9"></line>
              <line x1="9" y1="21" x2="9" y2="9"></line>
            </svg>
          </div>
          <h3>仪表盘</h3>
          <p>系统概览和数据统计</p>
        </div>
        
        <div class="feature-card" @click="navigateTo('/oa/users')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
              <circle cx="9" cy="7" r="4"></circle>
              <path d="M23 21v-2a4 4 0 0 0-3-3.87"></path>
              <path d="M16 3.13a4 4 0 0 1 0 7.75"></path>
            </svg>
          </div>
          <h3>用户管理</h3>
          <p>员工信息和权限管理</p>
        </div>
        
        <div class="feature-card" @click="navigateTo('/oa/departments')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M3 6h18"></path>
              <path d="M3 12h18"></path>
              <path d="M3 18h18"></path>
            </svg>
          </div>
          <h3>部门管理</h3>
          <p>组织架构和部门设置</p>
        </div>
        
        <div class="feature-card" @click="navigateTo('/oa/documents')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <rect x="3" y="4" width="18" height="18" rx="2" ry="2"></rect>
              <line x1="16" y1="2" x2="16" y2="6"></line>
              <line x1="8" y1="2" x2="8" y2="6"></line>
              <line x1="3" y1="10" x2="21" y2="10"></line>
            </svg>
          </div>
          <h3>公文管理</h3>
          <p>文档审批、流转和归档</p>
        </div>
        
        <div class="feature-card" @click="navigateTo('/oa/approvals')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path>
              <polyline points="22 4 12 14.01 9 11.01"></polyline>
            </svg>
          </div>
          <h3>审批流程</h3>
          <p>请假、报销等审批管理</p>
        </div>
        
        <div class="feature-card" @click="navigateTo('/oa/schedules')">
          <div class="feature-icon">
            <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="12" cy="12" r="10"></circle>
              <polyline points="12 6 12 12 16 14"></polyline>
            </svg>
          </div>
          <h3>日程安排</h3>
          <p>会议、任务和活动管理</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { useRouter } from 'vue-router'

const router = useRouter()

const goBack = () => {
  router.push('/')
}

const navigateTo = (path: string) => {
  router.push(path)
}
</script>

<style scoped>
.oa-system-container {
  min-height: 100vh;
  background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
  padding: 40px 20px;
}

.oa-header {
  text-align: center;
  margin-bottom: 40px;
}

.oa-header h1 {
  font-size: 2.5rem;
  color: #333;
  margin-bottom: 10px;
}

.oa-header p {
  font-size: 1.2rem;
  color: #666;
  margin-bottom: 20px;
}

.back-btn {
  background: #667eea;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1rem;
  transition: background 0.3s ease;
}

.back-btn:hover {
  background: #764ba2;
}

.oa-content {
  max-width: 1200px;
  margin: 0 auto;
}

.nav-menu {
  background: white;
  border-radius: 12px;
  padding: 20px;
  margin-bottom: 40px;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
}

.nav-menu ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.nav-menu li {
  flex: 1;
  min-width: 120px;
}

.nav-menu a {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  padding: 12px;
  background: #f8f9fa;
  border-radius: 8px;
  text-decoration: none;
  color: #333;
  transition: all 0.3s ease;
  font-weight: 500;
}

.nav-menu a:hover {
  background: #667eea;
  color: white;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(102, 126, 234, 0.3);
}

.feature-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
}

.feature-card {
  background: white;
  border-radius: 12px;
  padding: 30px;
  text-align: center;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  cursor: pointer;
}

.feature-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
}

.feature-icon {
  margin-bottom: 20px;
  color: #667eea;
}

.feature-card h3 {
  font-size: 1.3rem;
  color: #333;
  margin-bottom: 10px;
}

.feature-card p {
  color: #666;
  line-height: 1.5;
}

@media (max-width: 768px) {
  .oa-header h1 {
    font-size: 2rem;
  }
  
  .nav-menu ul {
    flex-direction: column;
  }
  
  .nav-menu li {
    min-width: 100%;
  }
  
  .feature-grid {
    grid-template-columns: 1fr;
  }
}
</style>