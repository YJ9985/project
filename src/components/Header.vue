<template>
  <header class="header">
    <div class="header-container">
      <!-- Logo Section -->
      <div class="logo-section">
        <div class="logo-wrapper">
          <img
            class="logo-image"
            alt="SSOKDAK Logo"
            src="/images/header_1.png"
          />
          <img
            class="logo-text"
            alt="SSOKDAK Text"
            src="/images/header_2.png"
          />
        </div>
      </div>

      <!-- Center Section -->
      <div class="center-section">
        <!-- Navigation Links -->
        <nav class="navigation">
          <!-- 비로그인 상태 네비게이션 -->
          <template v-if="!isLoggedIn">
            <a href="#" class="nav-link">쏙닥 소개</a>
            <a href="#" class="nav-link">왜 필요할까요?</a>
            <a href="#" class="nav-link">이용 방법</a>
            <a href="#" class="nav-link">우리가 만든 변화</a>
          </template>
          
          <!-- 로그인 상태 네비게이션 -->
          <template v-else>
            <a href="#" class="nav-link">메인페이지</a>
            <a href="#" class="nav-link">대시보드</a>
          </template>
        </nav>
      </div>

      <!-- Action Buttons -->
      <div class="action-buttons">
        <div class="divider"></div>
        
        <!-- 비로그인 상태 버튼 -->
        <template v-if="!isLoggedIn">
          <div class="button-group">
            <button class="primary-btn">{{ actionButtonText.primary }}</button>
            <button class="secondary-btn">{{ actionButtonText.secondary }}</button>
          </div>
        </template>
        
        <!-- 로그인 상태 사용자 정보 -->
        <template v-else>
          <div class="user-info">
            <div class="logout-text">
              <span class="logout-label">로그아웃</span>
              <span class="user-name">홍길동님</span>
            </div>
            <div class="user-icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 12C14.7614 12 17 9.76142 17 7C17 4.23858 14.7614 2 12 2C9.23858 2 7 4.23858 7 7C7 9.76142 9.23858 12 12 12Z" fill="#07294E"/>
                <path d="M12 14C7.58172 14 4 17.5817 4 22H20C20 17.5817 16.4183 14 12 14Z" fill="#07294E"/>
              </svg>
            </div>
          </div>
        </template>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: {
    isLoggedIn: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    // 로그인 상태에 따라 다른 텍스트 반환
    actionButtonText() {
      return this.isLoggedIn ? {
        primary: "마이페이지",
        secondary: "로그아웃"
      } : {
        primary: "회원가입",
        secondary: "로그인"
      }
    }
  }
}
</script>

<style scoped>
.header {
  background-color: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(10px);
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.1);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  height: 6vh; /* 반응형 높이로 변경 */
  min-height: 50px; /* 최소 높이 설정 */
  max-height: 80px; /* 최대 높이 설정 */
}

.header-container {
  max-width: 1920px;
  margin: 0 auto;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between; /* 3개 섹션을 균등 분배 */
  padding: 0 60px;
}

/* Logo Section */
.logo-section {
  display: flex;
  align-items: center;
  flex: 0 0 auto; /* 고정 크기 */
}

.logo-wrapper {
  display: flex;
  align-items: center;
  gap: 8px;
}

.logo-image {
  width: 48px;
  height: 48px;
  object-fit: contain;
}

.logo-text {
  height: 32px;
  object-fit: contain;
}

/* Center Section */
.center-section {
  display: flex;
  align-items: center;
  justify-content: center;
  /* flex: 1; 남은 공간 차지 */
}

/* Navigation */
.navigation {
  display: flex;
  align-items: center;
  gap: 80px;
}

.nav-link {
  color: #07294E;
  font-family: "Pretendard", -apple-system, BlinkMacSystemFont, sans-serif;
  font-size: 16px;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.2s ease;
  white-space: nowrap;
}

.nav-link:hover {
  color: #FF6B35;
}

/* Action Buttons */
.action-buttons {
  display: flex;
  align-items: center;
  gap: 30px;
  flex: 0 0 auto; /* 고정 크기 */
}

.divider {
  width: 1px;
  height: 28px;
  background-color: #B8B8BC;
}

.button-group {
  display: flex;
}

.primary-btn, .secondary-btn {
  background: none;
  border: none;
  font-family: "Pretendard", -apple-system, BlinkMacSystemFont, sans-serif;
  font-size: 16px;
  font-weight: 500;
  cursor: pointer;
  transition: color 0.2s ease;
  white-space: nowrap;
}

.primary-btn {
  color: #FF6B35;
}

.secondary-btn {
  color: #9E9E9E;
}

.primary-btn:hover {
  color: #E55A2B;
}

.secondary-btn:hover {
  color: #757575;
}

/* User Info (로그인 상태) */
.user-info {
  display: flex;
  align-items: center;
  gap: 15px;
}

.logout-text {
  display: flex;
  align-items: center;
  gap: 12px; /* 로그아웃과 홍길동님 사이 간격 */
  color: #9E9E9E;
  font-family: "Pretendard", -apple-system, BlinkMacSystemFont, sans-serif;
  font-size: 16px;
  font-weight: 500;
  white-space: nowrap;
}

.logout-label {
  color: #9E9E9E;
}

.user-name {
  color: #9E9E9E;
}

.user-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 24px;
  height: 24px;
}

.user-icon svg {
  width: 100%;
  height: 100%;
}

/* Responsive Design */
@media (max-width: 1200px) {
  .header-container {
    padding: 0 40px;
  }
  
  .navigation {
    gap: 50px;
  }
  
  .nav-link {
    font-size: 16px;
  }
  
  .primary-btn, .secondary-btn {
    font-size: 16px;
  }
  
  .button-group {
    gap: 25px;
  }
  
  .logout-text {
    font-size: 16px;
    gap: 10px; /* 태블릿에서는 간격 조정 */
  }
  
  .user-info {
    gap: 12px;
  }
}

@media (max-width: 768px) {
  .header {
    height: 10vh;
    min-height: 60px;
  }
  
  .header-container {
    padding: 0 20px;
  }
  
  .center-section {
    display: none; /* 모바일에서는 중앙 섹션 숨김 */
  }
  
  .logo-image {
    width: 40px;
    height: 40px;
  }
  
  .logo-text {
    height: 28px;
  }
  
  .action-buttons {
    gap: 20px;
  }
  
  .button-group {
    gap: 20px;
  }
  
  .primary-btn, .secondary-btn {
    font-size: 16px;
  }
  
  .logout-text {
    font-size: 14px;
    gap: 8px; /* 모바일에서는 간격 조정 */
  }
  
  .user-icon {
    width: 20px;
    height: 20px;
  }
  
  .user-info {
    gap: 10px;
  }
}

@media (max-width: 480px) {
  .header {
    height: 12vh;
    min-height: 70px;
  }
  
  .header-container {
    padding: 0 15px;
  }
  
  .logo-image {
    width: 36px;
    height: 36px;
  }
  
  .logo-text {
    height: 24px;
  }
  
  .action-buttons {
    gap: 15px;
  }
  
  .button-group {
    gap: 15px;
  }
  
  .primary-btn, .secondary-btn {
    font-size: 14px;
  }
  
  .logout-text {
    font-size: 12px;
    gap: 6px; /* 소형 모바일에서는 간격 조정 */
  }
  
  .user-icon {
    width: 18px;
    height: 18px;
  }
  
  .user-info {
    gap: 8px;
  }
}
</style> 