<template xmlns="http://www.w3.org/1999/html">
  <div class="wrapper">
        <!-- 헤더시작 -->
        <Header></Header>
        <!-- 헤더끝 -->
        <div class="detail-container">
            <div class="detail-contents">
                <div class="page-location">
                    <a class="page-location-home" href=""></a>
                    <ul class="page-nav">
                        <li>
                            <a class="page-nav-a" href="">
                                헤어케어
                            </a>
                        </li>
                        <li>
                            <a class="page-nav-a" href="">원
                                트리트먼트/팩
                            </a>
                        </li>
                        <li>
                            <a class="page-nav-a" href="">
                                헤어 트리트먼트
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- 이미지 영역 시작 -->
        <div class="product-detail-wrapper">
            <div class="product-detail">
                <div class="left-area">
                    <div class="img-area">
                        <img :src="detailInfo.product_main_img" alt="">
                    </div>
                    <ul class="left-area-mini">
                        <li>
                            <a href="">
                                <img :src="detailInfo.product_sub_img" alt="">
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="right-area">
                    <p class="product-info">
                        <a href="">{{ detailInfo.product_brand_name }}</a>
                    </p>
                    <p class="product-info-main-tit">
                      {{ detailInfo.product_sell_name }}
                    </p>
                    <p class="product-price-info">
                        <span class="bf-price">{{ detailInfo.product_orgin_price }}원</span>
                        <span class="aft-price">{{ detailInfo.product_sell_price }}원</span>
                        <span class="advantage-info">혜택정보</span>
                    </p>
                    <p class="icon-area">
                        <span class="coupon-icon">
                            쿠폰
                        </span>
                    </p>
                    <div class="watcher-area">
                        <span class="watcher">
                            <span>3</span>
                            명이 보고있어요
                        </span>
                    </div>
                    <div class="prd-more-info">
                        <div class="row">
                            <p class="prd-more-tit">
                                배송정보
                                <a href=""></a>
                            </p>
                            <ul class="delivery-info">
                                <li>
                                    <span style="display:inline-block;vertical-align:top;">일반배송</span>
                                    <div class="delivery-div">
                                        3,000원 (30,000원 이상 무료배송) <br>
                                        <b class="dt1">업체배송</b>
                                        <b class="dt2">합배송불가</b>
                                        <p class="dt3">평균 3일 이내 배송</p>
                                    </div>
                                </li>
                            </ul>
                        </div>
                        <div class="row">
                            <p class="prd-sub-tit2">
                                결제혜택
                            </p>
                            <div class="benefit-list">
                                <p>
                                    THE CJ 카드 추가 10% 할인
                                    <a class="info-tab1" href=""></a>
                                </p>
                                <p>
                                    CJ ONE 포인트 최대 1% 적립 예상
                                    <a class="info-tab1" href=""></a>
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="prd-select-list">
                        <a href="" class="prd-select-area">
                            상품을 선택해주세요
                        </a>
                    </div>
                    <div class="prd-price-total">
                        <span class="prd-price1">
                            상품금액합계
                        </span>
                        <span class="prd-price2">0원</span>
                    </div>
                    <div class="buy-btns">
                        <button class="cart-btn">
                            장바구니
                        </button>
                        <button class="cart-btn2" @click="buyNow">
                            바로구매
                        </button>
                        <button class="cart-btn3">
                        </button>
                        <button class="cart-btn4">
                        </button>
                    </div>
                </div>
            </div>
        </div>
        <!-- 이미지 영역 끝 -->

        <!-- 구매 가능 매장 확인시작 -->
        <div class="buy-able-wrapper">
            <div class="buy-able-area">
                <p class="buy-able-left">
                    <em class="buy-able-img"></em>
                    <span class="buy-able-span">구매가능한 매장을 확인해보세요</span>
                    <em class="buy-able-arrow"></em>
                    <em class="vertical-line">

                    </em>
                </p>
                <p class="buy-able-right">
                    <span class="buy-able-right-img"></span>
                    <span class="brand-name">수플린 브랜드관</span>
                    <em class="buy-able-arrow2"></em>
                </p>
            </div>
        </div>
        <!-- 구매 가능 매장 확인끝 -->

        <!-- 추천상품 '어때요' 시작 -->
        <div class="recommend-wrapper">
            <div class="recommend-tit">
                <h4 class="recommend-tit-left">
                    이런 <strong class="recommend-word">디저트/간식 상품은</strong> 어때요?
                </h4>
                <button class="recommend-tit-right">
                    <span class="recommend-more-btn">더보기</span> 
                </button>
            </div>

            <div class="recommend-img-area">
                <ul class="recommend-img-ul">
                    <li>
                        <div style="margin-left:10px;">
                            <img style="margin-right:10px; float:left; width:100px; height:100px;" src="https://image.oliveyoung.co.kr/uploads/images/goods/400/10/0000/0018/B00000018990601ko.jpg?l=ko" alt="">
                            <span class="recommend-img-tit1">23년 첫수확 프리미엄 고당도 샤인머스캣 1송이 과일선물 (650g)</span>
                            <p class="prd_price" style="margin-top:8px;">
                                <span class="tx_org">
                                    <span class="tx_num">35,000</span>
                                    원
                                </span>
                                <span class="tx_cur">
                                    <span class="tx_num">23,900</span>
                                    원
                                </span>
                            </p>
                            <p class="prd_flag">
                                <span class="icon_flag sale">세일</span>
                                <span class="icon_flag coupon">쿠폰</span>
                                <span class="icon_flag delivery">오늘드림</span>
                            </p>
                        </div>
                    </li>
                    <li>
                        <div style="margin-left:10px;">
                            <img style="margin-right:10px; float:left; width:100px; height:100px;" src="https://image.oliveyoung.co.kr/uploads/images/goods/400/10/0000/0018/B00000018383002ko.jpg?l=ko" alt="">
                            <span class="recommend-img-tit1">23년 첫수확 프리미엄 고당도 샤인머스캣 1송이 과일선물 (650g)</span>
                            <p class="prd_price" style="margin-top:8px;">
                                <span class="tx_org">
                                    <span class="tx_num">62,900</span>
                                    원
                                </span>
                                <span class="tx_cur">
                                    <span class="tx_num">59,700</span>
                                    원
                                </span>
                            </p>
                            <p class="prd_flag">
                                <!-- <span class="icon_flag sale">세일</span> -->
                                <span class="icon_flag coupon">쿠폰</span>
                                <span class="icon_flag free">무배</span>
                                <!-- <span class="icon_flag delivery">오늘드림</span> -->

                            </p>
                        </div>
                    </li>
                    <li>
                        <div style="margin-left:10px;">
                            <img style="margin-right:10px; float:left; width:100px; height:100px;" src="https://image.oliveyoung.co.kr/uploads/images/goods/400/10/0000/0018/B00000018247004ko.jpg?l=ko" alt="">
                            <span class="recommend-img-tit1">[수플린] 풍성한과일선물 프리미엄 혼합과일 11입 선물세트 (11입, 총 4.3kg 이상)</span>
                            <p class="prd_price" style="margin-top:8px;">
                                <span class="tx_org">
                                    <span class="tx_num">72,900</span>
                                    원
                                </span>
                                <span class="tx_cur">
                                    <span class="tx_num">69,900</span>
                                    원
                                </span>
                            </p>
                            <p class="prd_flag">
                                <!-- <span class="icon_flag sale">세일</span> -->
                                <span class="icon_flag coupon">쿠폰</span>
                                <span class="icon_flag free">무배</span>
                                <!-- <span class="icon_flag delivery">오늘드림</span> -->
                            </p>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
        <!-- 추천상품 '어때요' 끝 -->
        
        <!-- 상품설명, 구매정보, 리뷰, Q&A 시작 -->
        <div class="product-btns-wrapper">
            <ul class="product-btns-ul">
                <li class="product-desc-li" @click="chgTab(1)" :class="tab == 1? 'active-product-btn' : ''">
                    <p>상품설명</p>
                </li>
                <li class="product-buyinfo-li" @click="chgTab(2)" :class="tab == 2 ? 'active-product-btn' : ''">
                    <p>구매정보</p>
                </li>
                <li class="product-rvw-li" @click="chgTab(3)" :class="tab == 3 ? 'active-product-btn' : ''">
                    <p>리뷰</p>
                </li>
                <li class="product-qna-li" @click="chgTab(4)" :class="tab == 4 ? 'active-product-btn' : ''">
                    <p>Q&A</p>
                </li>
            </ul>
        </div>

        <div class="contents-wrapper">
          <!--상품설명시작-->
          <div v-if="tab == 1" class="contents-area">
              <div class="advertise-area-wrapper">
                <div class="advertise-area-wrapper-inner">
                  <a href="" class="advertise-area">
                      <img :src="detailInfo.product_desc1_img" class="advertise-img">
                  </a>
                </div>
              </div>
              <div class="contents-area-main">
                  <img :src="detailInfo.product_desc2_img"  alt="" class="contents-main-img">
                  <img :src="detailInfo.product_desc3_img"  alt="" class="contents-sub-img">
              </div>
              <div class="notice-text">
                  <p>
                      본 상품 정보(상품 상세, 상품 설명 등)의 내용은 협력사가 직접 등록한 것 입니다.
                  </p>
              </div>
          </div>
          <!--상품설명끝-->

          <!--리뷰시작-->
          <div v-if="tab == 3" class="contents-area">
            <div class="rvw-write-wrapper">
              <button @click="goRvwWrite" class="rvw-write">
                리뷰쓰기
              </button>
            </div>
            <div class="rvw-supervise-wrapper">
              <div class="rvw-supervise-area">
                <!--얼굴부분시작-->
                <div class="grade-img">
                  <p class="img-face">
                    <span class="grade5">
                      <em class="grade5-em">최고</em>
                    </span>
                  </p>
                </div>
                <!--얼굴부분끝-->

                <!--점수부분시작-->
                <div class="score-area">
                  <p class="score-total">
                    <span>총 1,676건</span>
                  </p>

                  <p class="score-avg">
                    <strong>4.4</strong>
                    <span>점</span>
                  </p>

                  <ul class="star-num-area">
                    <li>
                      <span class="star-fill"></span>
                      <img class="star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="">
                    </li>
                    <li>
                      <span class="star-fill"></span>
                      <img class="star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="">
                    </li>
                    <li>
                      <span class="star-fill"></span>
                      <img class="star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="">
                    </li>
                    <li>
                      <span class="star-fill"></span>
                      <img class="star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="">
                    </li>
                    <li>
                      <span class="star-fill"></span>
                      <img class="star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="">
                    </li>
                  </ul>

                </div>
                <div class="graph-area-wrapper">
                  <ul class="graph-area">
                    <li class="graph-li">
                      <span class="graph-percent">66%</span>
                      <div class="graph-gray-area">
                        <span class="graph-red-area" :style="styleSet.redArea1"></span>
                      </div>
                      <span class="score-type1">5점</span>
                    </li>
                    <li class="graph-li">
                      <span class="graph-percent">21%</span>
                      <div class="graph-gray-area">
                        <span class="graph-red-area" :style="styleSet.redArea2"></span>
                      </div>
                      <span class="score-type1">4점</span>
                    </li>
                    <li class="graph-li">
                      <span class="graph-percent">8%</span>
                      <div class="graph-gray-area">
                        <span class="graph-red-area" :style="styleSet.redArea3"></span>
                      </div>
                      <span class="score-type1">3점</span>
                    </li>
                    <li class="graph-li">
                      <span class="graph-percent">3%</span>
                      <div class="graph-gray-area">
                        <span class="graph-red-area" :style="styleSet.redArea4"></span>
                      </div>
                      <span class="score-type1">2점</span>
                    </li>
                    <li class="graph-li">
                      <span class="graph-percent">3%</span>
                      <div class="graph-gray-area">
                        <span class="graph-red-area" :style="styleSet.redArea5"></span>
                      </div>
                      <span class="score-type1">1점</span>
                    </li>
                  </ul>
                </div>

                <!--점수부분끝-->

              </div>
            </div>

        <!--들어갈자리-->
        <!-- 상품 특징 3가지 시작 -->
        <div class="poll-wrapper" v-if="tab==3">
          <div class="poll-area">
            <dl class="poll-dl">
              <dt class="poll-dt">
                <span class="poll-dd-span">
                  피부타입
                </span>
              </dt>
              <dd class="poll-dd">
                <ul class="dd-ul">
                  <li class="dd-ul-li">
                    <span>건성에 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:30px"></span>
                    </div>
                    <em class="poll-em">30%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>복합성 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:62px"></span>
                    </div>
                    <em class="poll-em">62%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>지성에 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:8px"></span>
                    </div>
                    <em class="poll-em">8%</em>
                  </li>
                </ul>
              </dd>
            </dl>
            <dl class="poll-dl">
              <dt class="poll-dt">
                <span class="poll-dd-span">
                  피부고민
                </span>
              </dt>
              <dd class="poll-dd">
                <ul class="dd-ul">
                  <li class="dd-ul-li">
                    <span>보습에 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:74px"></span>
                    </div>
                    <em class="poll-em">74%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>진정에 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:20px"></span>
                    </div>
                    <em class="poll-em">20%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>주름/미백에 좋아요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:6px"></span>
                    </div>
                    <em class="poll-em">6%</em>
                  </li>
                </ul>
              </dd>
            </dl>
            <dl class="poll-dl">
              <dt class="poll-dt">
                <span class="poll-dd-span">
                  자극도
                </span>
              </dt>
              <dd class="poll-dd">
                <ul class="dd-ul">
                  <li class="dd-ul-li">
                    <span>자극없이 순해요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:90px"></span>
                    </div>
                    <em class="poll-em">90%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>보통이에요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:10px"></span>
                    </div>
                    <em class="poll-em">10%</em>
                  </li>
                  <li class="dd-ul-li">
                    <span>자극이 느껴져요</span>
                    <div class="dd-ul-li-div">
                      <span style="width:0px"></span>
                    </div>
                    <em class="poll-em">0%</em>
                  </li>
                </ul>
              </dd>
            </dl>
          </div>
        </div>
        <!-- 상품 특징 3가지 끝 -->

        
        <!-- 상품 리뷰 시작 -->
        <div class="prd-rvw-list-wrapper">
          <div class="prd-rvw-list-area">
              <ul class="prd-rvw-ul">
                <!--하나의 리뷰 시작-->
                  <li class="prd-rvw-li"  v-for="(item, idx) in reviewList" :key="idx">
                  <div class="prd-rvw-left">
                    <div class="prd-rvw-left-wrapper">
                      <a href="" class="prd-rvw-left-img-wrapper">
                        <img src="https://image.oliveyoung.co.kr/uploads/images/mbrProfile/2023/01/02/1672646269565.png?RS=79x60&CS=60x60" alt="">
                      </a>
                      <p class="user-nickname">
                        <span>{{ item.mid }}</span>
                      </p>
                      <p class="user-rank-area">
                        <span class="user-rank">TOP4</span>
                      </p>
                      <p class="tag">
                        <span class="tag1">건성</span>
                        <span class="tag2">여름쿨톤</span>
                        <span class="tag3">모공</span>
                        <span class="tag4">미백</span>
                      </p>
                    </div>
                  </div>
                  <!--리뷰사진영역시작-->
                  <div class="prd-rvw-right">
                    <div class="prd-rvw-right-wrapper">
                      <div class="rvw-score-area">
                        <span class="star-area">
                          <span class="star-point" :style="{ width: (item.review_score * 20) + '%' }"></span>
                        </span>
                        <span class="score-date">{{ item.review_reg_date }}</span>
                        <span class="icon-offline-store">
                          매장
                        </span>
                      </div>
                      <div class="rvw-poll-area">
                        <dl class="poll-type1">
                          <dt class="poll-type1-dt">
                            <span>피부타입</span>
                          </dt>
                          <dd class="poll-type1-dd">
                            <span>복합성에 좋아요</span>
                          </dd>
                        </dl>
                        <dl class="poll-type1">
                          <dt class="poll-type1-dt">
                            <span>피부타입</span>
                          </dt>
                          <dd class="poll-type1-dd">
                            <span>복합성에 좋아요</span>
                          </dd>
                        </dl>
                        <dl class="poll-type1">
                          <dt class="poll-type1-dt">
                            <span>피부타입</span>
                          </dt>
                          <dd class="poll-type1-dd">
                            <span>복합성에 좋아요</span>
                          </dd>
                        </dl>
                      </div>
                      <div class="rvw-txt-inner">
                        {{ item.review_content }}
                      </div>
                      <div class="rvw-tag">
                        <span>완전히달라진리뷰</span>
                        <span>뒤집어놓으셨다</span>
                        <span>SNS에서난리난그제품</span>
                      </div>
                      <div class="rvw-img-div">
                        <ul class="rvw-img-ul">
                          <li>
                            <img src="https://image.oliveyoung.co.kr/uploads/images/gdasEditor/2023/08/16/1692170934661.png?RS=165x0&CS=165x165" alt="">
                          </li>
                        </ul>
                      </div>
                    </div>
                  </div>
                  <!--리뷰사진영역끝-->
                </li>
                <div class="review_no" v-if="this.reviewList == 0">
                  <span>리뷰가 존재하지 않습니다.</span>
                </div>
                <!--하나의 리뷰 끝-->

              </ul>
          </div>
        </div>
        <!-- 상품 리뷰 끝 -->
        <!--들어갈자리-->
          </div>
          <!--리뷰끝-->
        </div>

    <!-- 상품설명, 구매정보, 리뷰, Q&A 끝-->
        <!-- 푸터시작 -->
    <Footer></Footer>
        <!-- 푸터끝 -->
    <ModalWrapper ref="modal" :width="500" :height="871">
      <div class="rvw-popup-wrapper">
        <div class="rvw-popup-tit">
          <span>리뷰쓰기</span>
        </div>
        <div class="rvw-main-area">
          <div class="rvw-main-left">
<!--            <img src="https://image.oliveyoung.co.kr/uploads/images/goods/400/10/0000/0014/B00000014658854ko.jpg?l=ko" alt="">-->
            <img :src="detailInfo.product_main_img" alt="">
          </div>
          <div class="rvw-main-right">
            <span>{{detailInfo.product_sell_name}}</span>
          </div>
          <div class="rvw-select-star">
            <div class="rvw-select-subtit-wrapper">
              <span>상품을 사용해 보셨나요?</span>
              <input type="hidden" v-model="review_score">
              <br>
              <div class="rvw-star-area">
                <ul>
                  <li>
                    <span class="rvw-star-fill" :style="{ width: starWidth[0] }"></span>
                    <img class="rvw-star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="" @click="fillStar(0)">
                  </li>
                  <li>
                    <span class="rvw-star-fill" :style="{ width: starWidth[1] }"></span>
                    <img class="rvw-star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="" @click="fillStar(1)">
                  </li>
                  <li>
                    <span class="rvw-star-fill" :style="{ width: starWidth[2] }" ></span>
                    <img class="rvw-star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="" @click="fillStar(2)">
                  </li>
                  <li>
                    <span class="rvw-star-fill" :style="{ width: starWidth[3] }" ></span>
                    <img class="rvw-star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt=""  @click="fillStar(3)">
                  </li>
                  <li>
                    <span class="rvw-star-fill" :style="{ width: starWidth[4] }" ></span>
                    <img class="rvw-star-empty" src="https://static.oliveyoung.co.kr/pc-static-root/image//product/bg_rating_star.png" alt="" @click="fillStar(4)">
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <div class="rvw-text-area">
            <div class="rvw-text-subtit">
              <span>어떤 점이 좋았나요?</span>
            </div>
            <div class="rvw-text-textarea">
              <textarea class="rvw-input-textarea" v-model="review_content"></textarea>
            </div>
          </div>

          <div class="rvw-photo-upload">
            <p>사진 첨부하기</p>
          </div>

          <div class="rvw-btns-bundle">
            <button class="btn-cancel" @click="closeModal">
              취소
            </button>
            <button class="btn-enroll" @click="reviewInsert">
              등록
            </button>
          </div>
        </div>
      </div>
    </ModalWrapper>
</div>
</template>

<script>
import ModalWrapper from '@/components/ModalWrapper.vue';
import axios from "axios";
import basicMixin from "@/mixin/basicMixin.js";
import Footer from "@/components/Footer";
import Header from "@/components/Header";

export default {
  mixins: [basicMixin],
  components:{
    ModalWrapper,
      Footer,
      Header
  },
  data() {
    return {
      tab: 1,
      detailInfo: {},
      styleSet: {
        redArea1: {height: '66px'},
        redArea2: {height: '21px'},
        redArea3: {height: '8px'},
        redArea4: {height: '3px'},
        redArea5: {height: '3px'},
      },
      mid: localStorage.getItem('mid'),
      product_sell_name: '',
      review_content: '',
      review_score: '1',
      starWidth: ["100%", "0%", "0%", "0%", "0%"],
      reviewList: [],
      review_reg_date: '',
    };
  },
  async mounted() {
    let { data } = await axios.post('http://oliveyoungproject.shop/getProduct', {product_idx: this.$route.query.prdId});

    if (!data) {
      this.toastMsg('데이터가 없습니다.');
      return;
    }

    this.detailInfo = data;

    axios.post('/reviewList', {product_sell_name: this.detailInfo.product_sell_name})
        .then(response => { this.reviewList = response.data, console.log(this.reviewList)})
        .catch(error => {console.log("에러 : ", error)})

  },
  methods: {
    goStackLayer() {
      this.$pushContents('TestStack');
    },
    buyNow() {
      this.requestPay();
    },
    goRvwWrite() {
      this.$refs.modal.modalOpen();
    },
    chgTab(tab) {
      this.tab = tab;
    },
    requestPay() {
      let IMP = window.IMP;
      IMP.init('imp15187333'); //iamport 대신 자신의 "가맹점 식별코드"를 사용
      IMP.request_pay({
        pg: "kicc",
        pay_method: "card",
        merchant_uid : 'merchant_'+new Date().getTime(),
        name : '결제테스트', // 상품명
        amount : 1, // 가격
        buyer_email : 'iamport@siot.do',
        buyer_name : '구매자',
        buyer_tel : '010-1234-5678',
        buyer_addr : '서울특별시 강남구 삼성동',
        buyer_postcode : '123-456'
      }, function (rsp) { // callback
        if (rsp.success) {
          // 결제 성공 시 로직,
          console.log('성공 ', rsp);
        } else {
          // 결제 실패 시 로직,
          console.log('실패 ', rsp);
        }
      });
    },
    closeModal() {
      this.$refs.modal.closeModal();

    },
    fillStar(index) {
      // 클릭한 별 이전 별까지만 채움
      if(index == 0){
        this.starWidth[0] = '100%'
        this.starWidth[1] = this.starWidth[2] = this.starWidth[3] = this.starWidth[4] = '0%'
        this.review_score= '1'
      }
      if(index == 1){
        this.starWidth[0] = this.starWidth[1] = '100%'
        this.starWidth[2] = this.starWidth[3] = this.starWidth[4] = '0%'
        this.review_score= '2'
      }
      if(index == 2){
        this.starWidth[0] = this.starWidth[1] = this.starWidth[2] = '100%'
        this.starWidth[3] = this.starWidth[4] = '0%'
        this.review_score= '3'
      }
      if(index == 3){
        this.starWidth[0] = this.starWidth[1] = this.starWidth[2] = this.starWidth[3] = '100%'
        this.starWidth[4] = '0%'
        this.review_score= '4'
      }
      if(index == 4){
        this.starWidth[0] = this.starWidth[1] = this.starWidth[2] = this.starWidth[3] = this.starWidth[4] = '100%'
        this.review_score= '5'
      }
    },
    async reviewInsert() {
      this.toastMsg('등록.');
      let review등록 = {
        mid: localStorage.getItem('mid'),
        product_sell_name: this.detailInfo.product_sell_name,
        review_content: this.review_content,
        review_score: this.review_score,
      }
      let result = await axios.post("http://oliveyoungproject.shop/reviewInsert",review등록 );
      console.log('result >> ', result.data);
      this.$refs.modal.closeModal();
    },
  }
}
</script>
<style scoped src="@/assets/styles/productdetail.css">

</style>