<template>
  <div class="main-page">
    <!-- Header Component -->
    <Header :isLoggedIn="false" />
    
    <!-- Main Content 1 -->
    <div class="main-content">
      <!-- Left Section - Text Content -->
      <div class="text-section">
        <div class="text-wrapper-2">아이의 속마음을</div>
        <div class="text-wrapper-3">쏙 알아듣는 AI 애착인형</div>
        <p class="description">
          아이와 자연스럽게 대화하며 감정을 분석하고
          <br />
          부모님께 실시간 성장 리포트를 전달합니다
        </p>
        <div class="button-wrapper">
          <button class="service-button">서비스 시작하기</button>
        </div>
      </div>

      <!-- Right Section - Image -->
      <div class="image-section">
        <img class="main-image" alt="Main Image" src="/images/main_1.png" />
        
        <!-- Pagination Dots -->
        <div class="pagination-dots">
          <div class="dot active"></div>
          <div class="dot"></div>
          <div class="dot"></div>
        </div>
      </div>
      
      <!-- Scroll Indicator 1 -->
      <div class="scroll-indicator-wrapper">
        <div class="scroll-indicator">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M7 10L12 15L17 10" stroke="#9E9E9E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
      </div>
    </div>

    <!-- Main Content 2 - 두 번째 페이지 -->
    <div class="main-content-2">
      <div class="pentagon-container">
        <!-- 중앙 오각형 -->
        <div class="pentagon">
          <div class="pentagon-text">
            <div class="pentagon-title">"감정을 이해하는</div>
            <div class="pentagon-subtitle">아이 맞춤형 AI 친구"</div>
          </div>
        </div>
        
        <!-- 점들 (오각형 꼭지점에 위치) -->
        <div class="feature-dot dot-top"></div>
        <div class="feature-dot dot-top-right"></div>
        <div class="feature-dot dot-bottom-right"></div>
        <div class="feature-dot dot-bottom-left"></div>
        <div class="feature-dot dot-left"></div>
        
        <!-- 텍스트들 (점에서 조금 떨어진 위치) -->
        <div class="feature-text text-top" 
             data-index="0" 
             data-original="이상행동 정밀 감지" 
             data-detailed="부모가 설정한 키워드로<br/>이상 행동을 정밀 감지합니다">이상행동 정밀 감지</div>
        <div class="feature-text text-top-right" 
             data-index="1" 
             data-original="스마트 시스템" 
             data-detailed="여러 명의 아이를 동시에 <br/>관리할 수 있는스마트 시스템입니다">스마트 시스템</div>
        <div class="feature-text text-bottom-right" 
             data-index="2" 
             data-original="친근한 목소리" 
             data-detailed="아이가 친근함을 느낄 수 있는<br/>자연스러운 목소리로 대화합니다">친근한 목소리</div>
        <div class="feature-text text-bottom-left" 
             data-index="3" 
             data-original="성장리포트" 
             data-detailed="매일 아이의 감정 변화를 분석하여<br/>성장 리포트를 제공합니다">성장리포트</div>
        <div class="feature-text text-left" 
             data-index="4" 
             data-original="맞춤형 케어" 
             data-detailed="아이의 개별 특성에 맞춘<br/>맞춤형 케어를 제공합니다">맞춤형 케어</div>
        
        <!-- 원형 배경 -->
        <div class="circle-background"></div>
      </div>
      
      <!-- Scroll Indicator 2 -->
      <div class="scroll-indicator-wrapper-2">
        <div class="scroll-indicator">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M7 10L12 15L17 10" stroke="#9E9E9E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
      </div>
    </div>

    <!-- Main Content 3 - 세 번째 페이지 -->
    <div class="main-content-3">
      <!-- 제목 섹션 -->
      <div class="title-section-3">
        <h1 class="main-title-3">
          <span class="highlight-text">쏙닥</span>과 함께하는 방법
        </h1>
        <p class="subtitle-3">간단한 3단계로 시작하는 특별한 친구 관계</p>
      </div>

      <!-- 구분선 -->
      <div class="divider-line"></div>

      <!-- 단계 카드들 -->
      <div class="steps-container">
        <!-- 1단계 -->
        <div class="step-card step-1">
          <div class="step-number-wrapper">
            <div class="step-number">1</div>
          </div>
          <h3 class="step-title">회원가입 & 설정</h3>
          <p class="step-description">
            쏙닥 서비스에 가입하고<br/>
            아이의 기본 정보를 등록해주세요.<br/>
            개인맞춤 서비스를 위한<br/>
            첫걸음입니다.
          </p>
        </div>

        <!-- 2단계 -->
        <div class="step-card step-2">
          <div class="step-number-wrapper">
            <div class="step-number">2</div>
          </div>
          <h3 class="step-title">AI 인형과 만나기</h3>
          <p class="step-description">
            귀여운 애착인형을 받고<br/>
            아이와 함께 첫 만남을 가져보세요.<br/>
            쏙닥이 아이만의<br/>
            특별한 친구가 됩니다.
          </p>
        </div>

        <!-- 3단계 -->
        <div class="step-card step-3">
          <div class="step-number-wrapper">
            <div class="step-number">3</div>
          </div>
          <h3 class="step-title">대화하고 성장하기</h3>
          <p class="step-description">
            아이가 쏙닥과 자연스럽게<br/>
            대화하며 감정을 표현해보세요.<br/>
            실시간 성장 리포트를<br/>
            확인할 수 있습니다.
          </p>
        </div>
      </div>

      <!-- Scroll Indicator 3 -->
      <div class="scroll-indicator-wrapper-3">
        <div class="scroll-indicator">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M7 10L12 15L17 10" stroke="#9E9E9E" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
      </div>
    </div>

    <!-- Main Content 4 - 네 번째 페이지 -->
    <div class="main-content-4">
      <!-- 상단 통계 섹션 -->
      <div class="stats-section">
        <h1 class="main-title-4">
          <span class="highlight-text-white">믿을 수 있는 </span>
          <span class="highlight-text-red">쏙닥</span>
        </h1>
        
        <div class="stats-container">
          <div class="stat-item">
            <div class="stat-number">98%</div>
            <div class="stat-label">부모 만족도</div>
          </div>
          <div class="stat-item">
            <div class="stat-number">15000+</div>
            <div class="stat-label">누적 사용자</div>
          </div>
          <div class="stat-item">
            <div class="stat-number">24/7</div>
            <div class="stat-label">케어서비스</div>
          </div>
          <div class="stat-item">
            <div class="stat-number">100%</div>
            <div class="stat-label">데이터 보안</div>
          </div>
        </div>
      </div>

      <!-- 후기 섹션 -->
      <div class="testimonial-section">
        <!-- 후기 카드 1 -->
        <div class="testimonial-card">
          <div class="testimonial-icon">
            <div class="family-icon family-1"></div>
          </div>
          <div class="testimonial-content">
            <p class="testimonial-text">
              "쏙닥 덕분에 아이가 요즘 어떤 생각을 하는지 처음으로 알게 되었어요. 대화가 깊어졌고, 아이의 마음을 더 잘 이해하게 됐습니다."
            </p>
            <p class="testimonial-author">- 김OO 부모님 -</p>
          </div>
        </div>

        <!-- 후기 카드 2 -->
        <div class="testimonial-card">
          <div class="testimonial-icon">
            <div class="family-icon family-2"></div>
          </div>
          <div class="testimonial-content">
            <p class="testimonial-text">
              "아이도 자기 마음을 털어놓을 누군가가 필요했던 거더라고요. 쏙닥이 그 친구가 되어줬어요."
            </p>
            <p class="testimonial-author">- 이OO 부모님 -</p>
          </div>
        </div>

        <!-- 후기 카드 3 -->
        <div class="testimonial-card">
          <div class="testimonial-icon">
            <div class="family-icon family-3"></div>
          </div>
          <div class="testimonial-content">
            <p class="testimonial-text">
              "혼자서 고민하던 아이가 쏙닥을 통해 '요즘 내가 이런 감정이었구나'를 스스로 말하게 됐어요."
            </p>
            <p class="testimonial-author">- 박OO 부모님 -</p>
          </div>
        </div>

        <!-- 후기 카드 4 -->
        <div class="testimonial-card">
          <div class="testimonial-icon">
            <div class="family-icon family-4"></div>
          </div>
          <div class="testimonial-content">
            <p class="testimonial-text">
              "막연했던 교육 방향이 쏙닥 덕분에 구체적인 방향성을 찾게 되었어요. 우리 아이만을 위한 맞춤 가이드를 받은 느낌이에요."
            </p>
            <p class="testimonial-author">- 정OO 부모님 -</p>
          </div>
        </div>
      </div>

      <!-- 하단 구분선과 저작권 -->
      <div class="footer-section">
        <div class="footer-line"></div>
        <p class="copyright">© 2025 쏙닥 by 팀 아이좋아. All rights reserved.</p>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './Header.vue'

export default {
  name: "MainPage",
  components: {
    Header
  },
  data() {
    return {
      currentTextIndex: -1, // 현재 강조된 텍스트 인덱스 (-1은 아무것도 강조되지 않음)
      totalTexts: 5 // 총 텍스트 개수
    }
  },
  mounted() {
    this.initScrollAnimation()
  },
  methods: {
    initScrollAnimation() {
      let isScrolling = false
      let currentPage = 0
      const pages = document.querySelectorAll('.main-content, .main-content-2, .main-content-3, .main-content-4')
      
      const scrollToPage = (pageIndex) => {
        if (pageIndex >= 0 && pageIndex < pages.length) {
          // 부드러운 전환을 위한 CSS 애니메이션 적용
          pages.forEach((page, index) => {
            if (index === pageIndex) {
              page.style.transform = 'translateY(0)'
              page.style.opacity = '1'
            } else if (index < pageIndex) {
              page.style.transform = 'translateY(-100vh)'
              page.style.opacity = '0'
            } else {
              page.style.transform = 'translateY(100vh)'
              page.style.opacity = '0'
            }
          })
          currentPage = pageIndex
          
          // 페이지 변경 시 텍스트 강조 상태 초기화
          if (pageIndex !== 1) {
            this.resetTextEmphasis()
          }
        }
      }
      
      const handleWheel = (e) => {
        e.preventDefault() // 기본 스크롤 방지
        
        if (isScrolling) return
        
        isScrolling = true
        
        // 두 번째 페이지에서의 특별한 처리
        if (currentPage === 1) {
          if (e.deltaY > 0) {
            // 아래로 스크롤 - 텍스트 강조
            if (this.currentTextIndex < this.totalTexts - 1) {
              this.currentTextIndex++
              this.emphasizeText(this.currentTextIndex)
            } else {
              // 마지막 텍스트까지 강조했으면 다음 페이지로 (만약 있다면)
              if (currentPage < pages.length - 1) {
                currentPage++
                scrollToPage(currentPage)
              }
            }
          } else if (e.deltaY < 0) {
            // 위로 스크롤 - 텍스트 강조 해제
            if (this.currentTextIndex >= 0) {
              this.deemphasizeText(this.currentTextIndex)
              this.currentTextIndex--
            } else {
              // 첫 번째 텍스트보다 위로 가면 이전 페이지로
              if (currentPage > 0) {
                currentPage--
                scrollToPage(currentPage)
              }
            }
          }
        } else {
          // 다른 페이지에서는 기존 로직
          if (e.deltaY > 0 && currentPage < pages.length - 1) {
            // 아래로 스크롤 (슈-웅 효과)
            currentPage++
            scrollToPage(currentPage)
          } else if (e.deltaY < 0 && currentPage > 0) {
            // 위로 스크롤 (슈-웅 효과)
            currentPage--
            scrollToPage(currentPage)
          }
        }
        
        setTimeout(() => {
          isScrolling = false
        }, 600) // 쿨다운 시간 단축
      }
      
      // 키보드 지원 추가 (화살표 키)
      const handleKeydown = (e) => {
        if (isScrolling) return
        
        if (currentPage === 1) {
          // 두 번째 페이지에서 키보드 처리
          if (e.key === 'ArrowDown' || e.key === 'ArrowRight') {
            isScrolling = true
            if (this.currentTextIndex < this.totalTexts - 1) {
              this.currentTextIndex++
              this.emphasizeText(this.currentTextIndex)
            }
            setTimeout(() => { isScrolling = false }, 600)
          } else if (e.key === 'ArrowUp' || e.key === 'ArrowLeft') {
            isScrolling = true
            if (this.currentTextIndex >= 0) {
              this.deemphasizeText(this.currentTextIndex)
              this.currentTextIndex--
            }
            setTimeout(() => { isScrolling = false }, 600)
          }
        } else {
          // 다른 페이지에서는 기존 로직
          if (e.key === 'ArrowDown' && currentPage < pages.length - 1) {
            isScrolling = true
            currentPage++
            scrollToPage(currentPage)
            setTimeout(() => { isScrolling = false }, 900)
          } else if (e.key === 'ArrowUp' && currentPage > 0) {
            isScrolling = true
            currentPage--
            scrollToPage(currentPage)
            setTimeout(() => { isScrolling = false }, 900)
          }
        }
      }
      
      window.addEventListener('wheel', handleWheel, { passive: false })
      window.addEventListener('keydown', handleKeydown)
      
      // 초기 페이지 설정
      scrollToPage(0)
      
      // 컴포넌트 제거 시 이벤트 리스너 정리
      this.$once('hook:beforeDestroy', () => {
        window.removeEventListener('wheel', handleWheel)
        window.removeEventListener('keydown', handleKeydown)
      })
    },
    
    emphasizeText(index) {
      // 모든 텍스트 처리
      const allTexts = document.querySelectorAll('.feature-text')
      allTexts.forEach((text, i) => {
        const textIndex = parseInt(text.getAttribute('data-index'))
        
        if (textIndex === index) {
          // 현재 강조할 텍스트
          const detailedText = text.getAttribute('data-detailed')
          text.innerHTML = detailedText
          text.classList.add('emphasized')
          text.classList.remove('dimmed')
        } else {
          // 나머지 텍스트들 - 작게 만들기
          const originalText = text.getAttribute('data-original')
          text.innerHTML = originalText
          text.classList.remove('emphasized')
          text.classList.add('dimmed')
        }
      })
      
      // Pentagon과 Circle 축소
      this.scaleElements(true)
    },
    
    deemphasizeText(index) {
      const targetText = document.querySelector(`.feature-text[data-index="${index}"]`)
      if (targetText) {
        const originalText = targetText.getAttribute('data-original')
        targetText.innerHTML = originalText
        targetText.classList.remove('emphasized')
        targetText.classList.remove('dimmed')
      }
      
      // Pentagon과 Circle 복원 (다른 강조된 텍스트가 없다면)
      if (this.currentTextIndex < 0) {
        this.scaleElements(false)
        // 모든 텍스트를 원래 상태로 복원
        const allTexts = document.querySelectorAll('.feature-text')
        allTexts.forEach(text => {
          text.classList.remove('dimmed')
        })
      }
    },
    
    resetTextEmphasis() {
      // 모든 텍스트를 원래 상태로 복원
      const allTexts = document.querySelectorAll('.feature-text')
      allTexts.forEach(text => {
        const originalText = text.getAttribute('data-original')
        text.innerHTML = originalText
        text.classList.remove('emphasized')
        text.classList.remove('dimmed')
      })
      
      // Pentagon과 Circle 원래 크기로 복원
      this.scaleElements(false)
      this.currentTextIndex = -1
    },
    
    scaleElements(shouldScale) {
      const pentagon = document.querySelector('.pentagon')
      const circle = document.querySelector('.circle-background')
      const pentagonContainer = document.querySelector('.pentagon-container')
      
      if (shouldScale) {
        // 텍스트가 강조되면 Pentagon과 Circle 60% 축소
        if (pentagon) {
          pentagon.classList.add('scaled')
        }
        if (circle) {
          circle.classList.add('scaled')
        }
        if (pentagonContainer) {
          pentagonContainer.classList.add('scaled')
        }
      } else {
        // 강조된 텍스트가 없으면 원래 크기로 복원
        if (pentagon) {
          pentagon.classList.remove('scaled')
        }
        if (circle) {
          circle.classList.remove('scaled')
        }
        if (pentagonContainer) {
          pentagonContainer.classList.remove('scaled')
        }
      }
    }
  }
}
</script>

<style scoped>
.main-page {
  background-color: #ffffff;
  height: 100vh;
  width: 100vw;
  max-width: 100vw;
  min-width: 100vw;
  margin: 0;
  padding: 0;
  overflow: hidden;
  position: relative;
  top: 0;
  left: 0;
}

.main-content {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100vw;
  max-width: 100vw;
  height: 100vh;
  gap: 60px;
  margin: 0;
  padding: 0 8vw;
  position: fixed;
  top: 0;
  left: 0;
  box-sizing: border-box;
  transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.075), opacity 0.6s ease;
  z-index: 1;
}

/* Text Section */
.text-section {
  flex: 1;
  max-width: 600px;
  padding-right: 40px;
  text-align: left;
}

.text-wrapper-2 {
  color: #000000;
  font-family: "Pretendard-SemiBold";
  font-size: 52px;
  font-weight: 600;
  line-height: 1;
  margin-bottom: 20px;
  white-space: nowrap;
  margin-left: 0;
  text-align: left;
}

.text-wrapper-3 {
  color: #000000;
  font-family: "Pretendard-SemiBold";
  font-size: 52px;
  font-weight: 600;
  line-height: 1;
  margin-bottom: 40px;
  white-space: nowrap;
  margin-left: 0;
  text-align: left;
}

.description {
  color: #000000;
  font-family: "Pretendard-Thin";
  font-size: 20px;
  font-weight: 100;
  line-height: 1.2;
  margin-bottom: 55px;
  max-width: 555px;
  width: 100%;
  margin-left: 0;
  text-align: left;
}

.button-wrapper {
  margin-top: 40px;
  text-align: left;
  margin-left: 0;
}

.service-button {
  background-color: #07294E;
  border: none;
  border-radius: 40px;
  color: #ffffff;
  font-family: "Pretendard", -apple-system, BlinkMacSystemFont, sans-serif;
  font-size: 18px;
  font-weight: 500;
  padding: 12px 32px;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.service-button:hover {
  background-color: #051f3a;
  transform: translateY(-2px);
  box-shadow: 0px 6px 8px rgba(0, 0, 0, 0.3);
}

/* Image Section */
.image-section {
  flex: 1;
  max-width: 450px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding-left: 40px;
  margin-top: 50px;
}

.main-image {
  width: 400px;
  height: 400px;
  object-fit: cover;
  border-radius: 12px;
}

/* Pagination Dots */
.pagination-dots {
  position: relative;
  margin-top: 20px;
  display: flex;
  justify-content: center;
  gap: 20px;
}

.dot {
  width: 8px;
  height: 8px;
  border-radius: 6px;
  background-color: #d9d9d9;
  transition: background-color 0.3s ease;
}

.dot.active {
  background-color: #07294E;
}

/* Scroll Indicator (첫 번째 페이지 하단에 위치) */
.scroll-indicator-wrapper {
  position: absolute;
  bottom: 40px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  justify-content: center;
  z-index: 20;
}

.scroll-indicator {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 24px;
  height: 24px;
}

/* 두 번째 페이지 스타일 */
.main-content-2 {
  background-color: #FFEDE5;
  width: 100vw;
  max-width: 100vw;
  height: 100vh;
  margin: 0;
  padding: 0;
  display: flex;
  align-items: center;
  padding-top: 40px;
  justify-content: center;
  position: fixed;
  top: 0;
  left: 0;
  overflow: hidden;
  box-sizing: border-box;
  transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.075), opacity 0.6s ease;
  z-index: 1;
  transform: translateY(100vh);
  opacity: 0;
}

.pentagon-container {
  position: relative;
  width: 70vmin;
  height: 70vmin;
  max-width: 600px;
  max-height: 600px;
  min-width: 300px;
  min-height: 300px;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* 중앙 오각형 */
.pentagon {
  width: 80%;
  height: 75%;
  aspect-ratio: 1;
  background: linear-gradient(135deg, #FF1C1C 0%, #FF4848 38%, #ED6A6A 75%, #fab9b9 100%);
  clip-path: polygon(50% 0%, 100% 38%, 82% 100%, 18% 100%, 0% 38%);
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  z-index: 10;
  filter: drop-shadow(0 10px 20px rgba(255, 28, 28, 0.3));
}

.pentagon-text {
  text-align: center;
  color: #ffffff;
  font-family: "Pretendard-Bold";
  margin-top: 5%;
}

.pentagon-title {
  font-size: clamp(16px, 4.5vmin, 36px);
  font-weight: 600;
  margin-bottom: 0;
  line-height: normal;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

.pentagon-subtitle {
  font-size: clamp(16px, 4.5vmin, 36px);
  font-weight: 600;
  line-height: normal;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

/* Feature Dots - 오각형 꼭지점에 정확히 위치 */
.feature-dot {
  position: absolute;
  width: clamp(6px, 1.5vmin, 10px);
  height: clamp(6px, 1.5vmin, 10px);
  background-color: #E55A2B;
  border-radius: 50%;
  z-index: 15;
}

/* 점들의 위치 - 오각형 꼭지점에 맞춤 */
.dot-top {
  top: 5%;
  left: 50%;
  transform: translateX(-50%);
}

.dot-top-right {
  top: 38%;
  right: 4%;
}

.dot-bottom-right {
  bottom: 10%;
  right: 18%;
}

.dot-bottom-left {
  bottom: 10%;
  left: 18%;
}

.dot-left {
  top: 38%;
  left: 4%;
}

/* Feature Text - 점에서 떨어진 위치 */
.feature-text {
  position: absolute;
  font-family: "Pretendard-SemiBold";
  font-size: clamp(12px, 3.5vmin, 28px);
  font-weight: 600;
  color: #000000;
  white-space: nowrap;
  text-align: center;
  z-index: 15;
}

/* 텍스트들의 위치 - 점에서 10px 마진 */
.text-top {
  top: -4%;
  left: 50%;
  transform: translateX(-50%);
}

.text-top-right {
  top: 35%;
  right: -30%;
}

.text-bottom-right {
  bottom: 1%;
  right: -10%;
}

.text-bottom-left {
  bottom: 1%;
  left: -10%;
}

.text-left {
  top: 35%;
  left: -25%;
}

/* 강조된 텍스트 스타일 */
.feature-text.emphasized {
  font-size: clamp(20px, 3.5vmin, 48px) !important;
  font-weight: 500 !important;
  color: #07294E !important;
  text-shadow: 0px 2px 4px rgba(0, 0, 0, 0.1);
  transition: font-size 0.5s ease-in-out, font-weight 0.5s ease-in-out, color 0.5s ease-in-out, top 0.5s ease-in-out, bottom 0.5s ease-in-out, left 0.5s ease-in-out, right 0.5s ease-in-out;
  z-index: 10;
  line-height: 1.4;
}

/* 강조된 텍스트들의 새로운 위치 */
.feature-text.emphasized.text-top {
  top: 0% !important; /* 더 위로 이동 */
  left: 50% !important;
}

.feature-text.emphasized.text-top-right {
  top: 35% !important; /* 살짝 위로 */
  right: -60% !important; /* 더 바깥으로 */
}

.feature-text.emphasized.text-bottom-right {
  bottom: 5% !important; /* 더 아래로 */
  right: -40% !important; /* 더 바깥으로 */
}

.feature-text.emphasized.text-bottom-left {
  bottom: 5% !important; /* 더 아래로 */
  left: -40% !important; /* 더 바깥으로 */
}

.feature-text.emphasized.text-left {
  top: 30% !important; /* 살짝 위로 */
  left: -40% !important; /* 더 바깥으로 */
}

/* 강조되지 않은 텍스트 스타일 (다른 텍스트가 강조될 때) */
.feature-text.dimmed {
  font-size: 20px !important;
  font-weight: 400 !important;
  opacity: 0.7;
  transition: font-size 0.5s ease-in-out, font-weight 0.5s ease-in-out, opacity 0.5s ease-in-out, top 0.5s ease-in-out, bottom 0.5s ease-in-out, left 0.5s ease-in-out, right 0.5s ease-in-out;
}

/* 비강조 텍스트들의 새로운 위치 (더 안쪽으로 이동) */
.feature-text.dimmed.text-top {
  top: 10% !important; /* 아래로 이동 */
  left: 50% !important;
}

.feature-text.dimmed.text-top-right {
  top: 40% !important; /* 아래로 */
  right: -12% !important; /* 안쪽으로 */
}

.feature-text.dimmed.text-bottom-right {
  bottom: 16% !important; /* 위로 */
  right: -4% !important; /* 안쪽으로 */
}

.feature-text.dimmed.text-bottom-left {
  bottom: 15% !important; /* 위로 */
  left: 2% !important; /* 안쪽으로 */
}

.feature-text.dimmed.text-left {
  top: 40% !important; /* 아래로 */
  left: -8% !important; /* 안쪽으로 */
}

/* 원형 배경 */
.circle-background {
  position: absolute;
  width: 240%;
  height: 240%;
  border: 1px solid #E55A2B;
  border-radius: 50%;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 1;
  transition: transform 0.5s ease-in-out;
}

/* 축소된 Pentagon */
.pentagon.scaled {
  transform: scale(0.6) !important;
  transition: transform 0.5s ease-in-out !important;
}

/* 축소된 Circle */
.circle-background.scaled {
  transform: translate(-50%, -49%) scale(0.25) !important;
  transition: transform 0.5s ease-in-out !important;
}

/* Pentagon이 축소될 때 dot들도 함께 조정 */
.pentagon-container.scaled .feature-dot {
  transition: top 0.5s ease-in-out, bottom 0.5s ease-in-out, left 0.5s ease-in-out, right 0.5s ease-in-out;
}

/* 축소된 Pentagon에 맞춘 dot 위치 */
.pentagon-container.scaled .dot-top {
  top: 16% !important; /* 축소된 Pentagon의 위쪽 꼭지점 */
  left: 50% !important;
}

.pentagon-container.scaled .dot-top-right {
  top: 43% !important; /* 축소된 Pentagon의 오른쪽 위 꼭지점 */
  right: 16% !important;
}

.pentagon-container.scaled .dot-bottom-right {
  bottom: 20% !important; /* 축소된 Pentagon의 오른쪽 아래 꼭지점 */
  right: 28% !important;
}

.pentagon-container.scaled .dot-bottom-left {
  bottom: 20% !important; /* 축소된 Pentagon의 왼쪽 아래 꼭지점 */
  left: 28% !important;
}

.pentagon-container.scaled .dot-left {
  top: 43% !important; /* 축소된 Pentagon의 왼쪽 꼭지점 */
  left: 16% !important;
}

/* 두 번째 페이지 스크롤 인디케이터 */
.scroll-indicator-wrapper-2 {
  position: absolute;
  bottom: 40px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  justify-content: center;
}

/* 애니메이션 */
@keyframes float {
  0%, 100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes pulse {
  0%, 100% {
    transform: translate(-50%, -50%) scale(1);
    opacity: 0.7;
  }
  50% {
    transform: translate(-50%, -50%) scale(1.05);
    opacity: 0.9;
  }
}

/* 세 번째 페이지 스크롤 인디케이터 */
.scroll-indicator-wrapper-3 {
  position: absolute;
  bottom: 40px;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  justify-content: center;
}

/* 애니메이션 */
@keyframes float {
  0%, 100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-10px);
  }
}

@keyframes pulse {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: 0.5;
  }
}

@keyframes fadeInUp {
  0% {
    opacity: 0;
    transform: translateY(30px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

/* 세 번째 페이지 스타일 */
.main-content-3 {
  background-color: #ffffff;
  width: 100vw;
  max-width: 100vw;
  height: 100vh;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: fixed;
  top: 0;
  left: 0;
  overflow: hidden;
  box-sizing: border-box;
  transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.075), opacity 0.6s ease;
  z-index: 1;
  transform: translateY(100vh);
  opacity: 0;
  padding: 40px 20px;
  background-color: #FFFBE9;
}

/* 제목 섹션 */
.title-section-3 {
  text-align: center;
}

.main-title-3 {
  font-family: "Pretendard-Bold";
  font-size: clamp(28px, 4vw, 48px);
  font-weight: 700;
  line-height: normal;
  margin-top: 0;
  margin-bottom: 4px;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  color: #000000;
}

.highlight-text {
  color: #ff7272;
}

.subtitle-3 {
  font-family: "Pretendard-Thin";
  font-size: clamp(14px, 2vw, 20px);
  font-weight: 100;
  color: #000000;
  margin-top: 0;
  margin-bottom: 0;
}

/* 구분선 */
.divider-line {
  width: 90%;
  max-width: 1920px;
  height: 0.5px;
  background-color: #B8B8BC;
  margin: 40px 0 40px 0;
  border-radius: 2px;
}

/* 단계 컨테이너 */
.steps-container {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: clamp(40px, 7vw, 100px);
  width: 100%;
  max-width: 1920px;
  padding: 0 20px;
  box-sizing: border-box;
}

/* 단계 카드 */
.step-card {
  background: #F69E7B;
  border-radius: 20px;
  padding: 30px 20px;
  width: 100%;
  max-width: 320px;
  min-height: 320px;
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  box-shadow: 0px 8px 20px rgba(0, 0, 0, 0.15);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.step-card:hover {
  transform: translateY(-5px);
  box-shadow: 0px 12px 30px rgba(0, 0, 0, 0.2);
}


/* 단계 번호 */
.step-number-wrapper {
  position: absolute;
  top: 30px;
  left: 50%;
  transform: translateX(-50%);
  background-color: #FFFBE9;
  border-radius: 16px;
  box-shadow: -2px 2px 12px 2px rgba(0, 0, 0, 0.2);
  width: 60px;
  height: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.step-number {
  font-family: "Pretendard-ExtraBold";
  font-size: clamp(20px, 2.5vw, 32px);
  font-weight: 600;
  color: #333333;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

/* 단계 제목 */
.step-title {
  font-family: "Pretendard-SemiBold";
  font-size: clamp(16px, 2vw, 24px);
  font-weight: 600;
  color: #ffffff;
  margin: 80px 0 4px 0;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}

/* 단계 설명 */
.step-description {
  font-family: "Pretendard-Light";
  font-size: clamp(12px, 1.5vw, 16px);
  font-weight: 300;
      color: #ffffff;
    line-height: 1.4;
    flex-grow: 1;
    display: flex;
    align-items: center;
    word-wrap: break-word;
    white-space: normal;
    text-align: center;
  }

/* 네 번째 페이지 스타일 */
.main-content-4 {
  background: linear-gradient(180deg, #07294E 0%, #07294E 45%, #FFFBE9 45%, #FFFBE9 100%);
  width: 100vw;
  max-width: 100vw;
  height: 100vh;
  min-height: 100vh;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  position: fixed;
  top: 0;
  left: 0;
  overflow: hidden;
  box-sizing: border-box;
  transition: transform 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.075), opacity 0.6s ease;
  z-index: 1;
  transform: translateY(100vh);
  opacity: 0;
}

/* 상단 통계 섹션 */
.stats-section {
  width: 100%;
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  /* padding: 60px 0px; */
  box-sizing: border-box;
}

.main-title-4 {
  font-family: "Pretendard-Bold";
  font-size: clamp(28px, 4vw, 48px);
  font-weight: 600;
  line-height: normal;
  margin-top: 72px;
  margin-bottom: 32px;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  text-align: center;
}

.highlight-text-white {
  color: #ffffff;
}

.highlight-text-red {
  color: #ff7272;
}

.stats-container {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: clamp(60px, 16vw, 280px);
  width: 100%;
  max-width: 1920px;
  margin: 0 auto;
}

.stat-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.stat-number {
  color: #F69E7B;
  font-family: "Pretendard-Bold";
  font-size: clamp(28px, 4vw, 36px);
  font-weight: 600;
  line-height: normal;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  margin-bottom: 8px;
}

.stat-label {
  color: #ffffff;
  font-family: "Pretendard-Thin";
  font-size: clamp(8px, 2vw, 20px);
  font-weight: 100;
  line-height: normal;
}

/* 후기 섹션 */
.testimonial-section {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: clamp(20px, 4vw, 240px);
  padding: 60px 10px 10px 20px;
  box-sizing: border-box;
  max-width: 1920px;
  margin: 0 auto;
}

.testimonial-card {
  background-color: #ffffff;
  border-radius: 12px;
  box-shadow: -4px 4px 8px 2px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 280px;
  height: 280px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding: 32px 20px;
  box-sizing: border-box;
  position: relative;
}

.testimonial-icon {
  margin-bottom: 20px;
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
}

.family-icon {
  width: 60px;
  height: 60px;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.family-1 {
  background-image: url('/images/Family_1.png');
}

.family-2 {
  background-image: url('/images/Family_2.png');
}

.family-3 {
  background-image: url('/images/Family_3.png');
}

.family-4 {
  background-image: url('/images/Family_4.png');
}

.testimonial-content {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  text-align: center;
}

.testimonial-text {
  color: #000000;
  font-family: "Pretendard-Light";
  font-size: clamp(8px, 1vw, 16px);
  font-weight: 300;
  line-height: 1.4;
  /* margin: 0 0 20px 0; */
  text-align: center;
}

.testimonial-author {
  color: #000000;
  font-family: "Pretendard-Thin";
  font-size: clamp(8px, 1vw, 16px);
  font-weight: 100;
  line-height: normal;
  text-align: center;
  margin: 0;
}

/* 하단 푸터 섹션 */
.footer-section {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 8px;
  box-sizing: border-box;
  margin-top: auto;
}

.footer-line {
  width: 95%;
  max-width: 1850px;
  height: 1px;
  background-color: #B8B8BC;
  margin-bottom: 20px;
}

.copyright {
  color: #666666;
  font-family: "Pretendard-Thin";
  font-size: clamp(12px, 1vw, 16px);
  font-weight: 100;
  line-height: normal;
  text-align: center;
  margin: 0;
}

/* 반응형 조정 */
@media (max-width: 1200px) {
  .steps-container {
    flex-direction: column;
    align-items: center;
    gap: 30px;
  }
  
  .step-card {
    max-width: 400px;
    min-height: 300px;
  }
}

@media (max-width: 768px) {
  .divider-line {
    margin: 15px 0 25px 0;
  }
  
  .step-card {
    padding: 25px 15px;
    min-height: 280px;
    max-width: 350px;
  }

  /* 네 번째 페이지 반응형 */
  .testimonial-section {
    flex-direction: column;
    align-items: center;
    gap: 20px;
    padding: 20px;
  }

  .testimonial-card {
    max-width: 400px;
    height: 250px;
    padding: 20px 15px;
  }

  .stats-container {
    gap: clamp(30px, 6vw, 60px);
    flex-wrap: wrap;
  }
}

/* Responsive Design */
@media (max-width: 1200px) {
  .main-content {
    padding: 70px 40px 0 40px;
  }
  
  .text-wrapper-2,
  .text-wrapper-3 {
    font-size: 60px;
  }
  
  .description {
    font-size: 24px;
    width: 100%;
  }
  
  .main-image {
    width: 500px;
    height: 500px;
  }
}

@media (max-width: 768px) {
  .main-content {
    flex-direction: column;
    padding: 60px 20px 0 20px;
    text-align: center;
  }
  
  .text-section {
    padding-right: 0;
    margin-bottom: 40px;
  }
  
  .text-wrapper-2,
  .text-wrapper-3 {
    font-size: 40px;
    white-space: normal;
  }
  
  .description {
    font-size: 20px;
    width: 100%;
  }
  
  .main-image {
    width: 300px;
    height: 300px;
  }
  
  .indicators {
    bottom: 20px;
  }
}

@media (max-width: 480px) {
  .main-content {
    padding: 50px 15px 0 15px;
  }
  
  .text-wrapper-2,
  .text-wrapper-3 {
    font-size: 32px;
  }
  
  .description {
    font-size: 18px;
  }
  
  .service-button {
    font-size: 16px;
    padding: 14px 28px;
  }
  
  .main-image {
    width: 250px;
    height: 250px;
  }
  
  /* 두 번째 페이지 반응형 */
  .pentagon-container {
    width: 90%;
    height: 400px;
  }
  
  .pentagon {
    width: 200px;
    height: 180px;
  }
  
  .pentagon-title {
    font-size: 16px;
  }
  
  .pentagon-subtitle {
    font-size: 14px;
  }
  
  .feature-text {
    font-size: 14px;
  }
  
  .circle-background {
    width: 350px;
    height: 350px;
  }

  /* 네 번째 페이지 소형 화면 반응형 */
  .main-content-4 {
    background: linear-gradient(180deg, #07294E 0%, #07294E 60%, #FFFBE9 60%, #FFFBE9 100%);
  }

  .stats-section {
    height: 60%;
    padding: 20px;
  }

  .testimonial-section {
    height: 40%;
    padding: 10px 15px;
    overflow-y: auto;
  }

  .testimonial-card {
    max-width: 300px;
    height: 200px;
    padding: 15px 10px;
  }

  .family-icon {
    width: 60px;
    height: 60px;
  }

  .footer-section {
    padding: 10px;
  }
}
</style> 