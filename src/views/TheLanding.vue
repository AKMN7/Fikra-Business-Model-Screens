<template>
	<div class="flex flex-col items-center justify-center h-auto">
		<div class="flex flex-col w-full">
			<div class="flex flex-col flex-1 overflow-hidden pb-28">
				<!-- SECTION 1 -->
				<div class="flex flex-col items-center justify-center bg-[#BED8ED] pt-20 pb-28">
					<div
						class="w-[85%] md:w-[40%] xl:w-[30%] text-center text-[48px] md:text-[62px] leading-[68px] font-medium text-[#1E1E1E]">
						<h1><span class="text-[#307094]">فكـرة</span> لديك نحوّلها إلى كيان تجاري ابتكاري قـائـم وفعّـال</h1>
					</div>
					<p class="text-[20px] md:text-[24px] leading-[32px] text-[#1E1E1E] mt-4 mb-7 w-[80%] md:w-full text-center">
						من خلال تسخير خدمات أكثر من 100 جهة حكومية وخاصة
					</p>
					<div class="flex items-center justify-between w-[85%] lg:w-[23%]">
						<button type="submit" class="w-full py-2 mx-1 text-center text-white rounded-full bg-primary">التالي</button>
						<button type="button" class="w-full py-2 mx-1 text-center border border-black rounded-full text-balck">
							شاهد ماهي بوابة فكرة
						</button>
					</div>
				</div>
				<!-- SECTION 2 -->
				<div class="z-0 flex items-center justify-center px-6 bm_img h-[200px] md:h-[400px] md:-mt-2">
					<div class="hero_img h-[420px] w-[430px] md:h-[620px] md:w-[630px]"></div>
				</div>
				<!-- SECTION 11 (Logged In Only) -->
				<div
					v-if="isLoggedIn"
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[85%] xl:w-[70%] z-10 bg-white rounded-[10px] opacity-95 -mt-[128px] mb-12">
					<div class="flex flex-col items-start justify-between w-full mb-6 md:items-center md:flex-row">
						<div class="flex flex-col items-start justify-start">
							<h3 class="text-[22px] md:text-[32px] leading-9 text-[#042925]">شهادة المنشأة الابتكارية</h3>
							<p class="leading-[34px] text-primary text-[18px] w-full">6 طلبات</p>
						</div>
						<button type="button" class="text-[20px] hover:underline hover:text-primary">جميع الطلبات</button>
					</div>
					<div class="grid w-full grid-cols-1 gap-2 md:grid-cols-2">
						<div class="p-8 bg-white rounded-lg border border-[#EAECF0] hover:border-primary space-y-4">
							<div class="flex items-center justify-between">
								<img src="../assets/img/ns3a.svg" class="w-[137px] h-[50px]" />
								<p class="text-[18px]">تحت الدارسة</p>
							</div>
							<p class="text-[16px] text-[#78787A] w-[90%]">
								الاستثمار الجريء والدعم النشط للشركات المحفظة يتم الاستثمار بعد التحليل العميق للشركة المستهدف
							</p>
						</div>
						<div class="p-8 bg-white rounded-lg border border-[#EAECF0] hover:border-primary space-y-4">
							<div class="flex items-center justify-between">
								<img src="../assets/img/Al-baha.svg" class="w-[137px] h-[50px]" />
								<p class="text-[18px]">تم القبول</p>
							</div>
							<p class="text-[16px] text-[#78787A] w-[90%]">
								الاستثمار الجريء والدعم النشط للشركات المحفظة يتم الاستثمار بعد التحليل العميق للشركة المستهدف
							</p>
						</div>
					</div>
				</div>
				<!-- SECTION 3 -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[85%] xl:w-[70%] z-10 bg-[#96B2C8] rounded-[10px] mt-4 mb-10">
					<h3 class="mb-3 text-[32px] leading-9 text-white">ماهي بوابة فكرة؟</h3>
					<p class="mb-4 text-[20px] leading-8 text-white">
						لكون الابتكار التجاري لا ينشأ أو ينمو إلا على قاعدة معرفية رصينة وشبكة علاقات فعالة. تأتي بوابة الابتكار التجاري الوطنية
						“فكرة” لتقدم لك من خلال أقسامها المختلفة مجموعة من الأدوات غير المسبوقة في السوق السعودي. أدواتنا ستساند أفكارك
						الابتكارية في رحلة الازدهار أينما كان موقعك الجغرافي في المملكة.
					</p>
					<div class="grid w-full grid-cols-2 gap-4 md:grid-cols-3 lg:grid-cols-4">
						<div class="flex items-center justify-around p-2 bg-white rounded-lg md:p-5">
							<div class="flex flex-col items-start">
								<p class="text-[#042925] text-3xl md:text-4xl">60+</p>
								<p class="text-black font-bold text-md md:text-xl leading-[20px]">جهة</p>
							</div>
							<img src="../assets/img/reward.svg" class="w-[30px] h-[30px] md:w-[50px] md:h-[50px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-around p-2 bg-white rounded-lg md:p-5">
							<div class="flex flex-col items-start">
								<p class="text-[#042925] text-3xl md:text-4xl">220+</p>
								<p class="text-black font-bold text-md md:text-xl leading-[20px]">مبتكر تجاري</p>
							</div>
							<img src="../assets/img/businessman.svg" class="w-[30px] h-[30px] md:w-[50px] md:h-[50px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-around p-2 bg-white rounded-lg md:p-5">
							<div class="flex flex-col items-start">
								<p class="text-[#042925] text-3xl md:text-4xl">150+</p>
								<p class="text-black font-bold text-md md:text-xl leading-[20px]">الخدمات المنفذة</p>
							</div>
							<img src="../assets/img/event.svg" class="w-[30px] h-[30px] md:w-[50px] md:h-[50px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-around p-2 bg-white rounded-lg md:p-5">
							<div class="flex flex-col items-start">
								<p class="text-[#042925] text-3xl md:text-4xl">20+</p>
								<p class="text-black font-bold text-md md:text-xl leading-[20px]">قصص النجاح</p>
							</div>
							<img src="../assets/img/rocket.svg" class="w-[30px] h-[30px] md:w-[50px] md:h-[50px]" alt="Icon" />
						</div>
					</div>
				</div>
				<!-- SECTION 4 -->
				<div
					class="flex flex-col justify-start flex-1 py-8 mx-auto w-[85%] md:w-[85%] xl:w-[70%] z-10 bg-white rounded-[10px] mt-10 mb-8">
					<h3 class="mb-6 text-[32px] leading-9 text-[#042925]">قصص نجاح في بوابة فكرة</h3>
					<div class="grid w-full grid-cols-2 gap-4 md:grid-cols-3 lg:grid-cols-4">
						<div class="flex items-center justify-center p-5 bg-white rounded-lg border border-[#EAECF0]">
							<img src="../assets/img/fodex.svg" class="w-[140] h-[36px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-center p-5 bg-white rounded-lg border border-[#EAECF0]">
							<img src="../assets/img/jahez.svg" class="w-[140] h-[36px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-center p-5 bg-white rounded-lg border border-[#EAECF0]">
							<img src="../assets/img/highberbary.svg" class="w-[140] h-[36px]" alt="Icon" />
						</div>
						<div class="flex items-center justify-center p-5 bg-white rounded-lg border border-[#EAECF0]">
							<img src="../assets/img/marn.svg" class="w-[140] h-[36px]" alt="Icon" />
						</div>
					</div>
				</div>
				<!-- SECTION 5 -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[90%] xl:w-[70%] z-10 bg-white rounded-[10px] mt-4 mb-8">
					<div class="flex flex-col items-start justify-between w-full mb-6 md:items-center md:flex-row">
						<h3 class="text-[22px] md:text-[32px] leading-9 text-[#042925]">خدمات منظومة الابتكار</h3>
						<button type="button" class="px-4 py-2 text-center bg-white border rounded-full md:px-6 text-primary border-primary">
							عرض جميع الخدمات
						</button>
					</div>
					<div class="grid w-full grid-cols-1 gap-2 md:grid-cols-3 lg:grid-cols-4">
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/training_icon.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">التدريب</p>
									<p class="text-[15px] text-[#78787A]">يهدف اكتساب مهارات لبناء فكرتك</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/checkboard.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">دراسة السوق</p>
									<p class="text-[15px] text-[#78787A]">اكتشاف الفرص والاحتياجات لفكرتك</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/ruler.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">اختبار الافكار</p>
									<p class="text-[15px] text-[#78787A]">ابحث عن صحة فكرتك قبل الإطلاق</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/tv_input.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">التصميم والتنفيذ</p>
									<p class="text-[15px] text-[#78787A]">طور وابدأ بعملية اختبار فكرتك</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/training_icon.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">التدريب</p>
									<p class="text-[15px] text-[#78787A]">يهدف اكتساب مهارات لبناء فكرتك</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/checkboard.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">دراسة السوق</p>
									<p class="text-[15px] text-[#78787A]">اكتشاف الفرص والاحتياجات لفكرتك</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/ruler.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">اختبار الافكار</p>
									<p class="text-[15px] text-[#78787A]">ابحث عن صحة فكرتك قبل الإطلاق</p>
								</div>
							</div>
						</div>
						<div class="py-3 px-3 bg-[#E8F1F8] rounded-lg border border-[#BACDDB]">
							<p class="text-[14px] text-left w-full">10 جهات</p>
							<div class="flex items-start">
								<img src="../assets/img/tv_input.svg" class="w-[36px] h-[36px] ml-1" alt="Icon" />
								<div>
									<p class="text-[22px] text-[#042925] font-bold">التصميم والتنفيذ</p>
									<p class="text-[15px] text-[#78787A]">طور وابدأ بعملية اختبار فكرتك</p>
								</div>
							</div>
						</div>
					</div>
				</div>
				<!-- SECTION 6 -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[90%] xl:w-[70%] z-10 bg-white rounded-[10px] mt-4 mb-8">
					<div class="flex flex-col items-start justify-between w-full mb-6 md:items-center md:flex-row">
						<div class="flex flex-col items-start justify-start">
							<h3 class="text-[22px] md:text-[32px] leading-9 text-[#042925]">شهادة المنشأة الابتكارية</h3>
							<p class="md:text-[22px] leading-[26px] md:w-[70%] text-[19px] w-full">
								هل تمثل منشأة صغيرة أو متوسطة نجحت في تنفيذ ابتكار أو تقنية صاعدة؟ أحصل على الشهادة اليوم واستفد من المزايا!
							</p>
						</div>
						<button
							type="button"
							class="px-4 md:px-6 md:mt-0 mt-2 py-2 text-center bg-[#2A6490] rounded-full max-w-[150px text-white">
							اطلب الشهادة
						</button>
					</div>
					<div class="bg-[#E8F1F8] p-6 md:p-12 rounded-lg">
						<h1 class="text-center text-[22px] md:text-[32px] leading-9 text-[#042925] mb-6">الحاصلون على الشهادة</h1>
						<div class="grid w-full grid-cols-2 gap-8 md:grid-cols-3 lg:grid-cols-5">
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/dell.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/huwawai.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/jahez.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/highberbary.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/marn.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/tyme.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/sushi.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/fodex.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/dyson.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
							<div class="flex items-center justify-center py-7 px-4 bg-white rounded-lg border border-[#EAECF0]">
								<img src="../assets/img/sushi.svg" class="w-[140px] h-[36px]" alt="Icon" />
							</div>
						</div>
					</div>
				</div>
				<!-- SECTION 7 -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[90%] xl:w-[70%] z-10 bg-white rounded-[10px] mt-4">
					<div class="flex flex-col items-start justify-between w-full mb-6 md:items-center md:flex-row">
						<h3 class="text-[22px] md:text-[32px] leading-9 text-[#042925]">فعاليات الابتكار التجاري</h3>
					</div>
					<div class="grid w-full grid-cols-1 gap-4">
						<div
							class="py-5 px-4 bg-white rounded-lg border border-[#EAECF0] flex flex-col md:flex-row items-start md:items-center justify-between">
							<div class="flex items-center">
								<div class="bg-[#E1F2E8] border border-[#027A48] text-center py-4 px-2 rounded-lg ml-4">
									<p class="text-[#158456] text-[28px] leading-[26px]">28</p>
									<p class="text-[#158456] text-[16px] leading-[18px]">مارس</p>
								</div>
								<div class="flex flex-col items-start justify-center space-y-3">
									<p class="text-[#3F3F3F] text-[24px] leading-[18px] font-bold">كيف اختبر فكرتي؟</p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">ورشة عمل<span class="text-[#158456]">(قادمة)</span></p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">
										ورشة عمل مجانية لمدة ساعة في جدة بعنون “ابحث عن صحة فكرتك قبل اللإطلاق”
									</p>
								</div>
							</div>
							<button class="text-[16px] text-[#307094] hover:underline mt-3 md:mt-0">سجل الآن</button>
						</div>
						<div
							class="py-5 px-4 bg-white rounded-lg border border-[#EAECF0] flex flex-col md:flex-row items-start md:items-center justify-between">
							<div class="flex items-center">
								<div class="bg-[#E1F2E8] border border-[#027A48] text-center py-4 px-2 rounded-lg ml-4">
									<p class="text-[#158456] text-[28px] leading-[26px]">04</p>
									<p class="text-[#158456] text-[16px] leading-[18px]">مارس</p>
								</div>
								<div class="flex flex-col items-start justify-center space-y-3">
									<p class="text-[#3F3F3F] text-[24px] leading-[18px] font-bold">ورشة ذكاء: انترنت الأشياء في صناعة المستقبل</p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">ورشة عمل<span class="text-[#158456]">(قادمة)</span></p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">
										ورشة عمل مجانية لمدة ساعة في جدة بعنون “ابحث عن صحة فكرتك قبل اللإطلاق”
									</p>
								</div>
							</div>
							<button class="text-[16px] text-[#307094] hover:underline mt-3 md:mt-0">سجل الآن</button>
						</div>
						<div
							class="py-5 px-4 bg-white rounded-lg border border-[#EAECF0] flex flex-col md:flex-row items-start md:items-center justify-between">
							<div class="flex items-center">
								<div class="bg-[#FEF3F2] border border-[#FDA29B] text-center py-4 px-2 rounded-lg ml-4">
									<p class="text-[#912018] text-[28px] leading-[26px]">17</p>
									<p class="text-[#912018] text-[16px] leading-[18px]">فبراير</p>
								</div>
								<div class="flex flex-col items-start justify-center space-y-3">
									<p class="text-[#3F3F3F] text-[24px] leading-[18px] font-bold">استشارات للشركات الناشئة</p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">دورة تدريبية<span class="text-[#FF3A46]">(أنتهت)</span></p>
									<p class="text-[#3F3F3F] text-[16px] leading-[18px]">
										تبدأ عملية اختيار الفكرة بعد وضع الاساسيات واختبارها مع مجموعة من العملاء بطرق متنوعة ومختلفة.
									</p>
								</div>
							</div>
							<button class="text-[16px] text-[#FF3A46] hover:underline mt-3 md:mt-0">التسجيل مغلق</button>
						</div>
						<button class="py-5 bg-[#EAECF0] rounded-lg outline outline-[#EAECF0] hover:outline-1 hover:outline-primary">
							<p class="text-[16px] text-center w-full text-[#307094]">عرض جميع الفعاليات</p>
						</button>
					</div>
				</div>
				<!-- SECTION 8 Courasael -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[85%] xl:w-[70%] z-10 bg-white rounded-[10px] border-t border-t-[#F5F5F7] mt-20">
					<div class="flex items-center justify-between w-full mb-6">
						<h3 class="text-[20px] md:text-[32px] leading-9 text-[#042925]">مكتبة الابتكار</h3>
						<router-link
							to="/library"
							class="text-[14px] md:text-[16px] px-4 py-2 text-center bg-white border rounded-full md:px-6 text-primary border-primary">
							عرض محتويات المكتبة
						</router-link>
					</div>
					<Carousel
						:items-to-show="1"
						dir="rtl"
						:breakpoints="{
							768: {
								itemsToShow: 2,
							},
							1130: {
								itemsToShow: 3,
							},
						}">
						<template #addons>
							<Navigation />
						</template>
						<Slide v-for="item in carouselItems" :key="item.title">
							<div class="carousel__item">
								<div class="relative">
									<div class="text-[16px] leading-[22px] py-1 px-3 top-5 right-5 absolute bg-[#FFFFFFCC] rounded-xl">
										{{ item.category }}
									</div>
									<img :src="item.img" :alt="item.title" class="rounded-t-lg" />
									<div class="border rounded-b-lg border-[#EAECF0] p-4 text-right">
										<p class="text-[22px] leading-[26px] text-[#042925] mb-1">{{ item.title }}</p>
										<p class="text-[16px] leading-[22px] mb-7">
											{{ truncateString(item.desc) }}
										</p>
										<div class="flex items-center justify-between">
											<p class="text-[18px] leading-[22px] text-[#00000046]">{{ item.date }}</p>
											<router-link to="/article/1" class="text-[16px] leading-[22px] text-primary underline">قراءة المقال</router-link>
										</div>
									</div>
								</div>
							</div>
						</Slide>
					</Carousel>
				</div>
				<!-- SECTION 9 -->
				<div
					class="flex items-center justify-center mx-auto w-[95%] md:w-[85%] xl:w-[70%] z-10 bg-[#2A6490] rounded-[10px] mt-20 overflow-hidden">
					<img src="../assets/img/IntrestedIndividual.svg" alt="Coin In Hand" class="hidden h-full mx-3 -mb-1 md:block" />
					<div class="flex flex-col items-start justify-between mx-3 w-[85%] md:w-[50%] py-14">
						<h3 class="text-[22px] md:text-[36px] leading-10 text-white mb-8">
							هل لديك اهتمام بالاستثمار في الشركات الابتكارية؟ لدينا مجموعة من الفرص المتاحة..
						</h3>
						<button type="button" class="px-4 py-2 mx-1 text-center text-white border border-white rounded-full">
							شاهد ماهي بوابة فكرة
						</button>
					</div>
				</div>
				<!-- SECTION 10 -->
				<div
					class="flex flex-col justify-start flex-1 p-8 mx-auto w-[95%] md:w-[90%] xl:w-[72.5%] z-10 bg-white rounded-[10px] mt-20">
					<div class="flex flex-col items-start justify-between w-full mb-6 md:items-center md:flex-row">
						<h3 class="text-[22px] md:text-[32px] leading-9 text-[#042925]">الأسئلة الأكثر شيوعًا</h3>
					</div>
					<div class="flex flex-col gap-y-[12px]">
						<div
							v-for="(item, index) in faqs"
							:key="index"
							class="rounded-[8px] px-[32px] cursor-pointer border border-[#EAECF0] hover:border-primary transition-all duration-100 ease-in-out"
							:class="openIndex === index ? `border-[#BACDDB] bg-[#E8F1F8] py-[32px]` : 'bg-[#fff] py-[16px]'"
							@click="toggleFaq(index)">
							<div class="flex items-center justify-between mb-[8px]">
								<h3 class="text-[22px] leading-[26px] font-bold w-[75%]">
									{{ item.question }}
								</h3>
								<div class="flex">
									<img v-if="openIndex !== index" src="../assets/img/plus.svg" class="w-6 h-6" />
									<img v-if="openIndex === index" src="../assets/img/circle.svg" class="w-6 h-6" />
								</div>
							</div>
							<p v-if="openIndex === index" class="text-[16px] leading-[22px] font-medium w-[75%]">
								{{ item.answer }}
							</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script setup>
	import { Carousel, Slide, Navigation } from "vue3-carousel";
	import { ref } from "vue";
	const carouselItems = [
		{
			title: "كيف اختبر فكرتي؟",
			desc: "تبدأ عملية اختيار الفكرة بعد وضع الأساسيات واختبارها مع مجموعة من العملاء بطرق مختلفة ومتنوعة",
			date: "28 فبراير 2022",
			img: "https://images.pexels.com/photos/1314410/pexels-photo-1314410.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1",
			category: "مرحلة الفكرة",
		},
		{
			title: "كيف اختار الشركة المناسبة؟",
			desc: "من أهم المقومات لنجاح الفكرة هو اختيار الشركة المناسبة لتنفيذ وتصميم الفكرة",
			date: "28 فبراير 2022",
			img: "https://images.pexels.com/photos/207607/pexels-photo-207607.jpeg?auto=compress&cs=tinysrgb&w=1600",
			category: "تأسيس الشركات",
		},
		{
			title: "ما أهمية التدريب؟",
			desc: "لبناء فكرة معينة فأنت بحاجة إلى مجموعة من المهارات الي بدورها ستساعدك في بناء الفكرة",
			date: "28 فبراير 2022",
			img: "https://images.pexels.com/photos/45718/pexels-photo-45718.jpeg?auto=compress&cs=tinysrgb&w=1600",
			category: "التوجيه والارشاد",
		},
		{
			title: "ما أهمية التدريب؟",
			desc: "لبناء فكرة معينة فأنت بحاجة إلى مجموعة من المهارات الي بدورها ستساعدك في بناء الفكرة",
			date: "28 فبراير 2022",
			img: "https://images.pexels.com/photos/3153207/pexels-photo-3153207.jpeg?auto=compress&cs=tinysrgb&w=1600",
			category: "مرحلة الفكرة",
		},
		{
			title: "ما أهمية التدريب؟",
			desc: "لبناء فكرة معينة فأنت بحاجة إلى مجموعة من المهارات الي بدورها ستساعدك في بناء الفكرة",
			date: "28 فبراير 2022",
			img: "https://images.pexels.com/photos/3183190/pexels-photo-3183190.jpeg?auto=compress&cs=tinysrgb&w=1600",
			category: "تأسيس الشركات",
		},
	];

	const faqs = [
		{
			question: "ما هي المنشأة الابتكارية؟",
			answer:
				"هناك حقيقة مثبتة منذ زمن طويل وهي أن المحتوى المقروء لصفحة ما سيلهي القارئ عن التركيز على الشكل الخارجي للنص أو شكل توضع الفقرات في الصفحة التي يقرأها.",
		},
		{
			question: "ماهي الابتكارات؟",
			answer: `الابتكارات (Innovations) هي ما يقدمه الكيان من سلع (منتجات أو خدمات) أو عمليات (نموذج عمل تجاري أو بيئة عمل أو عمليات داخلية) أو مزيج من السلع والعمليات، بحيث تكون جديدة أو مطورة بشكل ملحوظ، وتكون جاهزة أو شبه جاهزة للاستخدام من قبل الكيان نفسه أو من خلال عملائه.`,
		},
		{
			question: "ماهي التقنيات الصاعدة؟",
			answer:
				"لوريم إيبسوم(Lorem Ipsum) هو ببساطة نص شكلي (بمعنى أن الغاية هي الشكل وليس المحتوى) ويُستخدم في صناعات المطابع ودور النشر. كان لوريم إيبسوم ولايزال المعيار للنص الشكلي منذ القرن الخامس عشر عندما قامت مطبعة مجهولة برص مجموعة من الأحرف بشكل عشوائي أخذتها من نص.",
		},
		{
			question: "ما هي آلية الانضمام إلى منصة فكرة؟",
			answer:
				'هنا يوجد محتوى نصي" فتجعلها تبدو (أي الأحرف) وكأنها نص مقروء. العديد من برامح النشر المكتبي وبرامح تحرير صفحات الويب تستخدم لوريم إيبسوم بشكل إفتراضي كنموذج عن النص، وإذا قمت بإدخال "lorem ipsum" في أي محرك بحث ستظهر العديد من المواقع الحديثة العهد في نتائج البحث.',
		},
		{
			question: "ما هي شروط المشاركة في جائزة ابتكر؟",
			answer:
				'للمهتمين قمنا بوضع نص لوريم إبسوم القياسي والمُستخدم منذ القرن الخامس عشر في الأسفل. وتم أيضاً توفير الأقسام 1.10.32 و 1.10.33 من "حول أقاصي الخير والشر" (de Finibus Bonorum et Malorum) لمؤلفه شيشيرون (Cicero) بصيغها الأصلية',
		},
		{
			question: "كيف يمكننا متابعة الفعاليات والإعلانات الجديدة؟",
			answer:
				'هنا يوجد محتوى نصي" فتجعلها تبدو (أي الأحرف) وكأنها نص مقروء. العديد من برامح النشر المكتبي وبرامح تحرير صفحات الويب تستخدم لوريم إيبسوم بشكل إفتراضي كنموذج عن النص، وإذا قمت بإدخال "lorem ipsum" في أي محرك بحث ستظهر العديد من المواقع الحديثة العهد في نتائج البحث.',
		},
		{
			question: "من هو المبتكر التجاري؟",
			answer:
				'هنا يوجد محتوى نصي" فتجعلها تبدو (أي الأحرف) وكأنها نص مقروء. العديد من برامح النشر المكتبي وبرامح تحرير صفحات الويب تستخدم لوريم إيبسوم بشكل إفتراضي كنموذج عن النص، وإذا قمت بإدخال "lorem ipsum" في أي محرك بحث ستظهر العديد من المواقع الحديثة العهد في نتائج البحث.',
		},
	];

	let isLoggedIn = ref(false);

	const openIndex = ref(null);

	function toggleFaq(index) {
		if (openIndex.value !== index) return (openIndex.value = index);
		openIndex.value = null;
	}

	function truncateString(str) {
		return str.length > 80 ? str.slice(0, 80) + "..." : str;
	}
</script>
