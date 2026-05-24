---
title: Universal Total Table — 전체 Auction Open API 고유 UDS 속성
channel: Auction Open API
type: api-doc-extraction
extracted_at: 2026-05-24T22:02:43
rows_including_header: 1610
csv_backup: ../../_csv/Auction Open API/01 - Universal Total Table — 전체 Auction Open API 고유 UDS 속성.csv
source_urls:
  - http://api.auction.co.kr/APIv1/AuctionService.asmx?WSDL
  - http://api.auction.co.kr/APIv1/ShoppingService.asmx?WSDL
  - http://api.auction.co.kr/APIv1/SecurityService.asmx?WSDL
---

# Universal Total Table — 전체 Auction Open API 고유 UDS 속성

- Channel: [[Auction Open API Index|Auction Open API]]
- Rows including header: **1610**
- Data rows: **1609**
- CSV backup: `../../_csv/Auction Open API/01 - Universal Total Table — 전체 Auction Open API 고유 UDS 속성.csv`
- Source: legacy Auction SOAP/XML Open API WSDL + operation pages.
- Caveat: this is legacy Auction Open API, not the newer ESM Trading API. Use it as a supplementary Auction-only source and reconcile with `Gmarket Auction` before connector implementation.

| UDS 속성명 | Auction 필드명 | API 영역 | 사용 Operation 수 | UDS 필요도 | 설명 |
| --- | --- | --- | --- | --- | --- |
| Inform 상태 | @InformStatus, InformStatus | CS API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Inform 일자 | @InformDate, InformDate | CS API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Question 일자 | @QuestionDate, QuestionDate | CS API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQuestionToHelpDesk |
| Reply Limit 일자 | @ReplyLimitDate, ReplyLimitDate | CS API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Reply 일자 | @ReplyDate, ReplyDate | CS API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| 상품 번호 And Question 건수 | ItemNoAndQuestionCount | CS API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAListHistory, GetSellerQnAList |
| Answer 일자 | @AnswerDate, AnswerDate | CS API, 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQuestionToHelpDesk |
| Register 일자 | @RegisterDate, RegisterDate | CS API, 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQnAList |
| Reply 상태 | @ReplyStatus, ReplyStatus | CS API, 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteDetailBySeqno, BuyerNoteList, SellerNoteDetailBySeqno, SellerNoteList |
| Pagination | Pagination | CS API, 기타 API, 상품 API | 20 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteList, GetAvailableSellerCouponList, GetEmergencyInformList, GetISBNSearchResults, GetItemQnAList 외 15개 |
| 판매자 Nick 명 | @SellerNickName, SellerNickName | CS API, 기타 API, 상품 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetMyQnAList, GetSohoBest50, GetSohoHotKeyword 외 8개 |
| Authentication 티켓 | AuthenticationTicket | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 187 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddEmergencyInformReply, AddFeedbackSecond, AddGroupToFavoriteGroupList, AddInterestItem, AddItem 외 182개 |
| Value | @Value, Value | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 212 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddEmergencyInformReply, AddFavoriteAuctionItem, AddFeedbackSecond, AddGroupToFavoriteGroupList, AddInterestItem 외 207개 |
| 암호화 티켓 | EncryptedTicket, encryptedTicket | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 212 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, SecurityService, ShoppingService; 사용 operation: AddEmergencyInformReply, AddFavoriteAuctionItem, AddFeedbackSecond, AddGroupToFavoriteGroupList, AddInterestItem 외 207개 |
| 인증티켓 | Ticket | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 134 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddGroupToFavoriteGroupList, AddInterestItem, AddItem, AddItemMobile 외 129개 |
| 페이지 번호 | @PageIndex, PageIndex, @PageNo, PageNo, @PageNumber, PageNumber | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 43 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BidList, BuyerNoteList, FavoriteAuctionItemList, FavoriteItemList, FavoriteModelList 외 38개 |
| 회원 티켓 | MemberTicket, memberTicket | CS API, 기타 API, 상품 API, 인증 API, 정산 API, 주문/배송 API, 클레임 API | 125 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddGroupToFavoriteGroupList, AddInterestItem, AddItem, AddItemMobile 외 120개 |
| 페이지 크기 | @PageSize, PageSize, pageSize | CS API, 기타 API, 상품 API, 인증 API, 클레임 API | 37 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BuyerNoteList, FavoriteAuctionItemList, FavoriteItemList, FavoriteModelList, FavoriteStoreList 외 32개 |
| 결과 | @Result, Result | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API | 16 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddEmergencyInformReply, AddFavoriteAuctionItem, AddFeedbackSecond, AlertShippingDelay, DeleteFavoriteAuctionItem 외 11개 |
| 구매자 ID | @BuyerID, @BuyerId, BuyerID, BuyerId | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 28 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BidList, BuyerNoteDetailBySeqno, BuyerNoteList, GetBidCancelList, GetCancelApprovalList 외 23개 |
| 상품 ID | @ItemID, ItemID | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 79 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddInterestItem, AddItem, AddItemMobile, AddItemToFavoriteItemList 외 74개 |
| 상품 번호 | @ItemNo, ItemNo, itemNo, itemno | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 60 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, BuyerNoteDetailBySeqno, BuyerNoteList 외 55개 |
| 상품명 | @ItemName, ItemName, @Name, Name | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 88 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, BuyerNoteDetailBySeqno, BuyerNoteList 외 83개 |
| 조회 시작일 | @FromDate, FromDate, @StartDate, StartDate | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 24 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BuyerNoteList, GetAvailableSellerCouponList, GetCancelApprovalList, GetCancelNotReceivedList, GetCompletedRemittanceList 외 19개 |
| 조회 종료일 | @EndDate, EndDate, @ToDate, ToDate | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 24 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BuyerNoteList, GetAvailableSellerCouponList, GetCancelApprovalList, GetCancelNotReceivedList, GetCompletedRemittanceList 외 19개 |
| 주문번호 | @OrderNo, OrderNo | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 67 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFeedbackSecond, AddItem, AddItemMobile, AddUsedItem, AlertShippingDelay 외 62개 |
| 주문일시 | @OrderDate, OrderDate | CS API, 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetEmergencyInformList, GetExpectedRemittanceList 외 8개 |
| 판매자 ID | @SellerID, @SellerId, SellerID, SellerId | CS API, 기타 API, 상품 API, 주문/배송 API | 46 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, BuyerNoteDetailBySeqno, BuyerNoteList 외 41개 |
| Seq 번호 | @SeqNo, SeqNo | CS API, 기타 API, 상품 API, 주문/배송 API, 클레임 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, BuyerNoteDetailBySeqno, BuyerNoteList 외 17개 |
| 상태 | @Status, Status | CS API, 기타 API, 상품 API, 주문/배송 API, 클레임 API | 20 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddInterestItem, AddItemMobile, AddItemToFavoriteItemList, AddQnAReply, Bid 외 15개 |
| 판매가 | @Price, Price | CS API, 기타 API, 상품 API, 주문/배송 API, 클레임 API | 32 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, BidList, Cart 외 27개 |
| Total 건수 | @TotalCount, TotalCount | CS API, 기타 API, 상품 API, 클레임 API | 16 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteAuctionItemList, FavoriteItemList, FavoriteModelList, FavoriteStoreList, GetBidCancelList 외 11개 |
| 사유 | @Reason, Reason | CS API, 기타 API, 상품 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddQnAReply, GetBidCancelList, RemoveQnAList, ReviseAttribute |
| 반품 코드 | @ReturnCode, ReturnCode | CS API, 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SellerNoteReply, SendNoteToSeller |
| 상품 IDs | ItemIDs | CS API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerQnAList |
| 상품 Image Path | @ItemImagePath, ItemImagePath | CS API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQnAList |
| Apply End 일자 | ApplyEndDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Apply 일자 | ApplyDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Auto Buying Decision 일자 | @AutoBuyingDecisionDate, AutoBuyingDecisionDate | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Available 판매자 Coupon | AvailableSellerCoupon | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Balance 수량 | @BalanceQty, BalanceQty | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Bid 상태 | @BidStatus, BidStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BidList |
| Bid 일자 | @BidDate, BidDate | 기타 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BidList, GetBiddingHistory |
| Bidding 상태 | @BiddingStatus, BiddingStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| Book 판매자 | BookSeller | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Buying 일자 | BuyingDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| buying 전화번호 번호 | buyingTelNo | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Cert End 일자 | CertEndDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Cert Start 일자 | CertStartDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification 상태 | CertificationStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification 일자 | CertificationDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Comment 이메일 여부 | @CommentEmailYN, CommentEmailYN | 기타 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, SetFeedbackSecond |
| Display End 일자 | @DisplayEndDate, DisplayEndDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Display Start 일자 | @DisplayStartDate, DisplayStartDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Display 상태 | @DisplayStatus, DisplayStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Feedback End 일자 | @FeedbackEndDate, FeedbackEndDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| Feedback 상태 | @FeedbackStatus, FeedbackStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| Feedback 일자 | @FeedbackDate, FeedbackDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyFeedbackList |
| Import 택배사 | ImportAgency | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Insert 일자 | @InsertDate, InsertDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Limited Feedback First 일자 | @LimitedFeedbackFirstDate, LimitedFeedbackFirstDate | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Limited Feedback 일자 | @LimitedFeedbackDate, LimitedFeedbackDate | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Made 일자 From | MadeDateFrom | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Made 일자 To | MadeDateTo | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Office 전화번호 | OfficeTel | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| ow 수량 | owQty | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Pay Expire 일자 | @PayExpireDate, PayExpireDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmingReceiptList |
| Payment Due 일자 | @PaymentDueDate, PaymentDueDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| Power 판매자 | PowerSeller | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Publish 일자 | @PublishDate, PublishDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Publish 일자 From | PublishDateFrom | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Publish 일자 To | PublishDateTo | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Receipt 상태 | @ReceiptStatus, ReceiptStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmingReceiptList |
| Reg 일자 | @RegDate, RegDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Sale Close 일자 | @SaleCloseDate, SaleCloseDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Sale Open 일자 | @SaleOpenDate, SaleOpenDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Sell 상태 | @SellStatus, SellStatus | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SellerNoteList |
| Smile Cash Smile Pay Expect Save 금액 | @SmileCashSmilePayExpectSaveAmount, SmileCashSmilePayExpectSaveAmount | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cash Smile Pay Expect Save 일자 | @SmileCashSmilePayExpectSaveDate, SmileCashSmilePayExpectSaveDate | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cash Total Expect Save 금액 | @SmileCashTotalExpectSaveAmount, SmileCashTotalExpectSaveAmount | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cash 판매자 Expect Save 금액 | @SmileCashSellerExpectSaveAmount, SmileCashSellerExpectSaveAmount | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cash 판매자 Expect Save 일자 | @SmileCashSellerExpectSaveDate, SmileCashSellerExpectSaveDate | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Soho 판매자 여부 | @SohoSellerYN, SohoSellerYN | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| Write 일자 | @WriteDate, WriteDate | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst |
| 발송 Note | SendNote | 기타 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteDetailBySeqno, BuyerNoteList |
| 여부 Custom 응답 Great 판매자 | IsCustomResponseGreatSeller | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 여부 Feedback Great 판매자 | IsFeedbackGreatSeller | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 여부 Top 판매자 | IsTopSeller | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 요청 수량 | @RequestQty, RequestQty | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCartDetail |
| 판매자 Addr | SellerAddr | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses |
| 판매자 Coupon | SellerCoupon | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerCoupon |
| 판매자 Feedback 유형 | @SellerFeedbackType, SellerFeedbackType | 기타 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst, SetBuyingDecisionAndFeedbackFirst |
| 판매자 IDs | SellerIDs | 기타 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| 판매자 Level | SellerLevel | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 판매자 Point | @SellerPoint, SellerPoint | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 판매자 Register 번호 | SellerRegisterNo | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 페이지 | page | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 페이지 Index | pageIndex | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 휴대폰번호 | Mobile | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| 휴대폰번호 Join Apln URL | MobileJoinAplnURL | 기타 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 휴대폰번호 Search Option | MobileSearchOption | 기타 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Ad Successful Bid Seqno | @AdSuccessfulBidSeqno, AdSuccessfulBidSeqno | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid, GetPowerRegisteredItems, GetTodayRecommandBestItems, GetTodayRecommandItems |
| Ad 메시지 | @AdMessage, AdMessage | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Ad 카테고리 Seqno 코드 | @AdCategorySeqnoCode, AdCategorySeqnoCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid |
| Add line1 | Add_line1 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, ReviseitemLocationBroad |
| Add line2 | Add_line2 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, ReviseitemLocationBroad |
| Addon Service 유형 | @AddonServiceType, AddonServiceType | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Admin Staff Tag | @AdminStaffTag, AdminStaffTag | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Adult | @Adult, Adult | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Advertise 메시지 | @AdvertiseMessage, AdvertiseMessage | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| After Service | @AfterService, AfterService | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Apply Lump Sum 할인 | @ApplyLumpSumDiscount, ApplyLumpSumDiscount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Applying Coupon | @ApplyingCoupon, ApplyingCoupon | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Area 코드 | AreaCode | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad, ReviseitemLocationkorea |
| ASInfo | @ASInfo, ASInfo | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Attr ID | @AttrID, AttrID | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseAttribute, ReviseItem 외 4개 |
| Attr Seq 번호 | @AttrSeqNo, AttrSeqNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Attr Value Seq 번호 | @AttrValueSeqNo, AttrValueSeqNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Attr 유형 | @AttrType, AttrType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Auct Stat | @AuctStat, AuctStat | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: FavoriteAuctionItemList, GetMyAuctionItemList |
| Auction 할인 | @AuctionDiscount, AuctionDiscount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Auto Extend | AutoExtend | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Award Amnt | @AwardAmnt, AwardAmnt | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory, GetMyAuctionItemList, GetMyAuctionSellingItemList |
| Bar 코드 | @BarCode, BarCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Bid 건수 | @BidCount, BidCount | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory, GetMyAuctionSellingItemList, ViewItem, ViewItem_old |
| Bidder 건수 | @BidderCount, BidderCount | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetMyAuctionItemList, ReviseItemForUsedMarket, ViewItem, ViewItemForUsedMarket, ViewItem_old |
| Bonus | @Bonus, Bonus | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit, ViewClosedItem, ViewItem |
| Bonus Base | @BonusBase, BonusBase | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit, ViewClosedItem, ViewItem |
| Bonus 코드 | @BonusCode, BonusCode | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit, ViewClosedItem, ViewItem |
| Book Info | BookInfo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Broadcast Equipment | BroadcastEquipment | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Bulk 할인 수량 | @BulkDiscountQty, BulkDiscountQty | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Buy It Now Available | @BuyItNowAvailable, BuyItNowAvailable | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Buy It Now 가격 | @BuyItNowPrice, BuyItNowPrice | 기타 API, 상품 API | 19 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 14개 |
| Buy Limit Period | @BuyLimitPeriod, BuyLimitPeriod | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Buy Limit 유형 코드 | @BuyLimitTypeCode, BuyLimitTypeCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Callback Info | CallbackInfo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Callback 유형 | @CallbackType, CallbackType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Card 할인 | CardDiscount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Cash | @Cash, Cash | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Charged Wish Keyword | ChargedWishKeyword | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Chart Detail 카테고리 | ChartDetailCategory | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Child | Child | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerSellingCategories |
| Child Product Safe Cert | ChildProductSafeCert | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Clase Name1 | @ClaseName1, ClaseName1 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Clase Name2 | @ClaseName2, ClaseName2 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Clase Name3 | @ClaseName3, ClaseName3 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Clase Name4 | @ClaseName4, ClaseName4 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Clase Name5 | @ClaseName5, ClaseName5 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Click Check Image URL | @ClickCheckImageUrl, ClickCheckImageUrl | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid, GetPowerRegisteredItems, GetTodayRecommandBestItems, GetTodayRecommandItems |
| Close 일자 | @CloseDate, CloseDate | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: FavoriteAuctionItemList, GetBiddingHistory, GetFinishedItemList, GetMyAuctionItemList |
| Comment 건수 | @CommentCount, CommentCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Condition | Condition | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ViewItem, ViewItem_old |
| Condition 유형 | ConditionType | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Core Asrt 코드 | @CoreAsrtCode, CoreAsrtCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Country | Country | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, ReviseitemLocationBroad |
| Coupon 할인 가격 | @CouponDiscountPrice, CouponDiscountPrice | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| Current 페이지 번호 | @CurrentPageNumber, CurrentPageNumber | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList, GetSellPlusItemList, GetSellingItemList |
| DCategory | DCategory | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Del 여부 | @DelYn, DelYn | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSohoShopStyleTrendList, ReviseItem 외 2개 |
| Deliberation | Deliberation | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Description | @Description, Description | 기타 API, 상품 API | 24 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 19개 |
| Description Ver 유형 | @DescriptionVerType, DescriptionVerType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Descriptive Option | DescriptiveOption | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Descriptive Text | @DescriptiveText, DescriptiveText | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Detail Consulting | DetailConsulting | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Discounted 가격 | @DiscountedPrice, DiscountedPrice | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Display Attr 명 | @DisplayAttrName, DisplayAttrName | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseAttribute, ReviseItem 외 4개 |
| Display Limit | DisplayLimit | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Display Limit 사유 | @DisplayLimitReason, DisplayLimitReason | 기타 API, 상품 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 8개 |
| Display Limit 여부 | @DisplayLimitYn, DisplayLimitYn | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Display Limit 일자 | @DisplayLimitDate, DisplayLimitDate | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Distr 유형 | @DistrType, DistrType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Dongmyun | Dongmyun | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeKorea, GetItemLocationKorea, ReviseitemLocationkorea |
| Donor Shopping From 일자 | @DonorShoppingFromDate, DonorShoppingFromDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Donor Shopping Search 코드 | @DonorShoppingSearchCode, DonorShoppingSearchCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Donor Shopping To 일자 | @DonorShoppingToDate, DonorShoppingToDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Duty 사용 Months | @DutyUseMonths, DutyUseMonths | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Ecoupon Effective Period | @EcouponEffectivePeriod, EcouponEffectivePeriod | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Element ID | @ElementID, ElementID | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseAttribute, ReviseItem 외 4개 |
| Element List | ElementList | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Element 명 | @ElementName, ElementName | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseAttribute, ReviseItem 외 4개 |
| Elements | Elements | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Enable Free Phone URL | @EnableFreePhoneUrl, EnableFreePhoneUrl | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Enable PCSCoupon | @EnablePCSCoupon, EnablePCSCoupon | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| End 시간 | @EndTime, EndTime | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemForUsedMarket, ViewItem, ViewItemForUsedMarket, ViewItem_old |
| Entity 명 | @EntityName, EntityName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID |
| Entry Close 여부 | @EntryCloseYN, EntryCloseYN | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList |
| Entry Close 일자 | @EntryCloseDate, EntryCloseDate | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetItemFreeExperienceList, ReviseItem 외 2개 |
| Entry Start 일자 | @EntryStartDate, EntryStartDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Entry 건수 | @EntryCount, EntryCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList |
| Environment Friendly License | EnvironmentFriendlyLicense | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Epin Info | EpinInfo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Epin 코드 | @EpinCode, EpinCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Equal | @Equal, Equal | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID |
| Essen 여부 | @EssenIs, EssenIs, @EssenYn, EssenYn | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetOfficialNoticeInfo, ReviseAttribute 외 5개 |
| Etc Business Registration | EtcBusinessRegistration | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Exclude Mart On 상품 | @ExcludeMartOnItem, ExcludeMartOnItem | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 4개 |
| Exclude 카테고리 ID | ExcludeCategoryID | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Exist Related 상품 | @ExistRelatedItem, ExistRelatedItem | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 17개 |
| Expense 할인 | ExpenseDiscount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Expense 할인 Cards | ExpenseDiscountCards | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Expense 할인 금액 | ExpenseDiscountAmount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Expose 여부 | @ExposeYn, ExposeYn | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Extra Info | ExtraInfo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Favorite Auction Model | FavoriteAuctionModel | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| Feature | Feature | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Feature 유형 | @FeatureType, FeatureType | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Feedback 건수 | @FeedbackCount, FeedbackCount | 기타 API, 상품 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword 외 6개 |
| First Bid 가격 | @FirstBidPrice, FirstBidPrice | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| Fix Image | FixImage | 기타 API, 상품 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 3개 |
| Fix Image B | FixImageB | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| Fix Image Path | @FixImagePath, FixImagePath | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteAuctionItemList, FavoriteItemList |
| Fix Image300 | FixImage300 | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Focus | @Focus, Focus | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| Food License | FoodLicense | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Free Gift 코드 | @FreeGiftCode, FreeGiftCode | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit, ViewClosedItem, ViewItem |
| Free Phone Apply URL | @FreePhoneApplyUrl, FreePhoneApplyUrl | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Fst Image Path | @FstImagePath, FstImagePath | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: FavoriteAuctionItemList, GetMyAuctionItemList, GetMyAuctionSellingItemList |
| Group 번호 | @GroupNo, GroupNo | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddGroupToFavoriteGroupList, AddItemToFavoriteItemList, DeleteItemFromFavoriteItemList, DoFavoriteModelAdd 외 12개 |
| Has Acceleration | @HasAcceleration, HasAcceleration | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Has Favorite Card | @HasFavoriteCard, HasFavoriteCard | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Has Matching 상품 | @HasMatchingItem, HasMatchingItem | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Has Upward Point | @HasUpwardPoint, HasUpwardPoint | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Health Food Import Business Registration | HealthFoodImportBusinessRegistration | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Health Food License | HealthFoodLicense | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Height | @Height, Height | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemForBrandShop |
| ID | @ID, ID | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetAuthenticate, GetCatalog, GetCategories, GetISBNSearchResults, GetSearchResultsMartOn 외 1개 |
| Image | @Image, Image | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList, FavoriteStoreList |
| Image Matching Finish 여부 | @ImageMatchingFinishYN, ImageMatchingFinishYN | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Image1 Path | @Image1Path, Image1Path | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList |
| Image2 Path | @Image2Path, Image2Path | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList |
| Immediately 여부 | @ImmediatelyYN, ImmediatelyYN | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| Input Channel | @InputChannel, InputChannel | 기타 API, 상품 API | 20 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 15개 |
| Input Channel 코드 | @InputChannelCode, InputChannelCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Ins Oprt | @InsOprt, InsOprt | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Install | Install | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Install Maker ID | @InstallMakerId, InstallMakerId | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Integrate Safe Cert | IntegrateSafeCert | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Interest Free | @InterestFree, InterestFree | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Interest Free3 Months | @InterestFree3Months, InterestFree3Months | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Interest Free6 Months | @InterestFree6Months, InterestFree6Months | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| ISBN | @ISBN, ISBN | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetISBNSearchResults, ReviseItem 외 2개 |
| ISBN 코드 허용 여부 | @IsbnCodeAllowYn, IsbnCodeAllowYn | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Join 수수료 유형 | @JoinFeeType, JoinFeeType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Keywords | @Keywords, Keywords | 기타 API, 상품 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 10개 |
| Landing URL | @LandingUrl, LandingURL, LandingUrl | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoCategoryBox, GetSohoLookbook, GetSohoShopHomeNewArrival 외 2개 |
| Large 코드 | @LargeCode, LargeCode | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoCategoryBox, GetSohoShopSearchResults, GetSohoShopSearchResultsCategoryBox |
| Latitude | Latitude | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemGeocodeKorea, GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad 외 1개 |
| LCategory | LCategory | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Leaf 카테고리 | @LeafCategory, LeafCategory | 기타 API, 상품 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 10개 |
| Less Than Close Days | @LessThanCloseDays, LessThanCloseDays | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Level 유형 | @LevelType, LevelType | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoCategoryBox, GetSohoShopSearchResults, GetSohoShopSearchResultsCategoryBox |
| List 가격 | @ListPrice, ListPrice | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Listing Begin 일자 | @ListingBeginDate, ListingBeginDate | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Listing Begin 일자 Reservation | @ListingBeginDateReservation, ListingBeginDateReservation | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Listing Details | ListingDetails | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Listing End 일자 | @ListingEndDate, ListingEndDate | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Listing End 일자 Reservation | @ListingEndDateReservation, ListingEndDateReservation | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Listing Enhancement | ListingEnhancement | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Listing Picture | ListingPicture | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Listing Picture B | ListingPictureB | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| Listing Picture URL | @ListingPictureUrl, ListingPictureUrl | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Listing 상태 | ListingStatus | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Listing 여부 | @ListingYn, ListingYn | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Local Chain | @LocalChain, LocalChain | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Location 번호 | @LocationNo, LocationNo | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad, ReviseitemLocationkorea |
| Longitude | Longitude | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemGeocodeKorea, GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad 외 1개 |
| Lotte Sale 가격 | @LotteSalePrice, LotteSalePrice | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Lowest 가격 | @LowestPrice, LowestPrice | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList, GetISBNSearchResults |
| Lowest 상품 번호 | @LowestItemNo, LowestItemNo | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList, GetISBNSearchResults |
| Luxury Goods Corner | LuxuryGoodsCorner | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Made 일자 | @MadeDate, MadeDate | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Main Description | @MainDescription, MainDescription | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList, GetISBNSearchResults |
| Make 명 | @MakeName, MakeName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| Maker ID | @MakerID, MakerID | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 4개 |
| Management 코드 | @ManagementCode, ManagementCode | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Manufacturer | @Manufacturer, Manufacturer | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID, ViewItem, ViewItem_old |
| Mart On Asrt Level 유형 | @MartOnAsrtLevelType, MartOnAsrtLevelType | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Mart On Asrt 명 | @MartOnAsrtName, MartOnAsrtName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Mart On Asrt 코드 | @MartOnAsrtCode, MartOnAsrtCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Mart On End 일자 | @MartOnEndDate, MartOnEndDate | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Mart On Start 일자 | @MartOnStartDate, MartOnStartDate | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Mart On 카테고리 Array | MartOnCategoryArray | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsMartOn, GetSearchResultsMartOnBest100 |
| Mart On 카테고리 ID | MartOnCategoryID | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsMartOn, GetSearchResultsMartOnBest100 |
| Match 건수 | @MatchCount, MatchCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Matched 건수 | @MatchedCount, MatchedCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Matching 상품 건수 | @MatchingItemCount, MatchingItemCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Max Bin 가격 | @MaxBinPrice, MaxBinPrice | 기타 API, 상품 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetISBNSearchResults, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults 외 7개 |
| Max Sale 가격 | @MaxSalePrice, MaxSalePrice | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| MCategory | MCategory | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Media 속성 Set | MediaAttributeSet | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, ViewItem, ViewItem_old |
| Medical Instrument Import Business Registration | MedicalInstrumentImportBusinessRegistration | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Medical Instrument License | MedicalInstrumentLicense | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Method 코드 | @MethodCode, MethodCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList |
| Min | Min | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Min Bin 가격 | @MinBinPrice, MinBinPrice | 기타 API, 상품 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetISBNSearchResults, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults 외 7개 |
| Min Buy 수량 | @MinBuyQty, MinBuyQty | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, ReviseItem 외 2개 |
| Min Sale 가격 | @MinSalePrice, MinSalePrice | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Min Sell Amnt | @MinSellAmnt, MinSellAmnt | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Min Sell 수량 | @MinSellQty, MinSellQty | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Model 명 | @ModelName, ModelName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Motors Dealer | @MotorsDealer, MotorsDealer | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Moving Picture URL | @MovingPictureURL, MovingPictureURL | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Multi Matching Enable 여부 | @MultiMatchingEnableYn, MultiMatchingEnableYn | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseAttribute, ReviseItem 외 4개 |
| My Favorite Store Best 상품 List | MyFavoriteStoreBestItemList | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| My Favorite Store 상품 List | MyFavoriteStoreItemList | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| Noti 상품 Group | NotiItemGroup | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetOfficialNoticeInfo |
| Noti 상품 Group 명 | @NotiItemGroupName, NotiItemGroupName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetOfficialNoticeInfo |
| Noti 상품 Group 번호 | @NotiItemGroupNo, NotiItemGroupNo | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, GetOfficialNoticeInfo, ViewOfficialNotice |
| Noti 상품 Value | @NotiItemValue, NotiItemValue | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, ViewOfficialNotice |
| Noti 상품 코드 | @NotiItemCode, NotiItemCode | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, GetOfficialNoticeInfo, ViewOfficialNotice |
| Noti 상품 코드 명 | @NotiItemCodeName, NotiItemCodeName | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetOfficialNoticeInfo |
| Now 가격 | @NowPrice, NowPrice | 기타 API, 상품 API | 21 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteAuctionItemList, FavoriteItemList, GetBiddingHistory, GetMyAuctionItemList, GetPowerRegisteredItems 외 16개 |
| Num Of Items | @NumOfItems, NumOfItems | 기타 API, 상품 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 10개 |
| Obj Opt Clase 번호 | @ObjOptClaseNo, ObjOptClaseNo | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Obj Opt No1 | @ObjOptNo1, ObjOptNo1 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Obj Opt No2 | @ObjOptNo2, ObjOptNo2 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Obj Opt No3 | @ObjOptNo3, ObjOptNo3 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Obj Opt No4 | @ObjOptNo4, ObjOptNo4 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Obj Opt No5 | @ObjOptNo5, ObjOptNo5 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Offering After Service | @OfferingAfterService, OfferingAfterService | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| On Going | @OnGoing, OnGoing | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteItemList |
| Opt Detail Image Level | @OptDetailImageLevel, OptDetailImageLevel | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Opt Rep Image Level | @OptRepImageLevel, OptRepImageLevel | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Opt Ver 유형 | @OptVerType, OptVerType | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Option Buy | OptionBuy | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Option Buy 유형 | @OptionBuyType, OptionBuyType | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Option Object 명 | OptionObjectName | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Option Required | @OptionRequired, OptionRequired | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Option 유형 | @OptionType, OptionType | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Option 유형 코드 | @OptionTypeCode, OptionTypeCode | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Origin | Origin | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Ownership Days | @OwnershipDays, OwnershipDays | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Pay 건수 | @PayCount, PayCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Payer 건수 | @PayerCount, PayerCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Penalty 여부 | @PenaltyYn, PenaltyYn | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, ReviseItem 외 2개 |
| Period | Period | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Pickup Favor Cash | @PickupFavorCash, PickupFavorCash | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Pickup Favor Gift | @PickupFavorGift, PickupFavorGift | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Pickup Favor 유형 | @PickupFavorType, PickupFavorType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Pickup 주소 번호 | @PickupAddressNo, PickupAddressNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture Details | PictureDetails | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Picture Expansion | PictureExpansion | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Picture URL | PictureUrl | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Picture1 | Picture1 | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| Picture1 300 | Picture1_300 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture1 600 | Picture1_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture1 B | Picture1B | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| Picture10 | Picture10 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture10 600 | Picture10_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture11 | Picture11 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture11 600 | Picture11_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture12 | Picture12 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture12 600 | Picture12_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture13 | Picture13 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture13 600 | Picture13_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture14 | Picture14 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture14 600 | Picture14_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture15 | Picture15 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture15 600 | Picture15_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture2 | Picture2 | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| Picture2 600 | Picture2_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture2 B | Picture2B | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| Picture3 | Picture3 | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| Picture3 600 | Picture3_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture3 B | Picture3B | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| Picture4 | Picture4 | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| Picture4 600 | Picture4_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture5 | Picture5 | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| Picture5 600 | Picture5_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture6 | Picture6 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture6 600 | Picture6_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture7 | Picture7 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture7 600 | Picture7_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture8 | Picture8 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture8 600 | Picture8_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Picture9 | Picture9 | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemPictures 외 2개 |
| Picture9 600 | Picture9_600 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Place | @Place, Place | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Post Script 건수 | @PostScriptCount, PostScriptCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Post 수수료 | @PostFee, PostFee | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Premium | @Premium, Premium | 기타 API, 상품 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSellPlusItemList, GetSohoBest50, GetSohoHotKeyword 외 6개 |
| Premium Condition | @PremiumCondition, PremiumCondition | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Premium Plus | @PremiumPlus, PremiumPlus | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Prod Satisfaction | @ProdSatisfaction, ProdSatisfaction | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Prod 일자 | @ProdDate, ProdDate | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| Prod 일자 Attr | @ProdDateAttr, ProdDateAttr | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| Product ID | @ProductID, ProductID | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Product Listing Details | ProductListingDetails | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Quick Available Area | @QuickAvailableArea, QuickAvailableArea | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Quick Available Area Str | @QuickAvailableAreaStr, QuickAvailableAreaStr | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Quick Company Phone | @QuickCompanyPhone, QuickCompanyPhone | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Quick Company 명 | @QuickCompanyName, QuickCompanyName | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Quick Service Area | QuickServiceArea | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSearchResults, GetSearchResultsExtMedia 외 5개 |
| Receipt | @Receipt, Receipt | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Recent Bidder 건수 | @RecentBidderCount, RecentBidderCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Recent Payer 건수 | @RecentPayerCount, RecentPayerCount | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Recommend | @Recommend, Recommend | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Recommend Condition | @RecommendCondition, RecommendCondition | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Regional 시중 Area 코드 | @RegionalMarketAreaCode, RegionalMarketAreaCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Regional 시중 Corner | RegionalMarketCorner | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Register Channel | @RegisterChannel, RegisterChannel | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFeedbackSecond, ReviseItemForUsedMarket, SetBuyingDecisionAndFeedbackFirst, SetFeedbackSecond, ViewItemForUsedMarket |
| Rule Seq | @RuleSeq, RuleSeq | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Rule 명 | @RuleName, RuleName | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Safe Auth | SafeAuth | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Satisfaction Rate | @SatisfactionRate, SatisfactionRate | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| SCategory | SCategory | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Sd Attr Matching Info | SdAttrMatchingInfo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Sd Maker 코드 | @SdMakerCode, SdMakerCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Search Auct 상태 | @SearchAuctStatus, SearchAuctStatus | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionItemList, GetMyOnSaleItemCount |
| Search Condition | SearchCondition | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList, GetSellPlusItemList, GetSellingItemList |
| Search Term | @SearchTerm, SearchTerm | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionItemList, GetMyAuctionSellingItemList, GetMyOnSaleItemCount |
| Search Term From | @SearchTermFrom, SearchTermFrom | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Search Term To | @SearchTermTo, SearchTermTo | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Search Term 유형 | @SearchTermType, SearchTermType | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Search 결과 상품 | SearchResultItem | 기타 API, 상품 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 6개 |
| Search 결과 상품 Array | SearchResultItemArray | 기타 API, 상품 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 6개 |
| Selective Option | SelectiveOption | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Sell Range Max Value1 | @SellRangeMaxValue1, SellRangeMaxValue1 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Range Max Value2 | @SellRangeMaxValue2, SellRangeMaxValue2 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Range Min Value1 | @SellRangeMinValue1, SellRangeMinValue1 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Range Min Value2 | @SellRangeMinValue2, SellRangeMinValue2 | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Unit Value | @SellUnitValue, SellUnitValue | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Unit Volume | @SellUnitVolume, SellUnitVolume | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Sell Unit 유형 | @SellUnitType, SellUnitType | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Sell Unit 코드 | @SellUnitCode, SellUnitCode | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Sell 가격 | @SellPrice, SellPrice | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteStoreList, GetFinishedItemList |
| Sell 수수료 유형 | @SellFeeType, SellFeeType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Selling 상태 | SellingStatus | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Selling 상품 건수 | @SellingItemCount, SellingItemCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| Selling 유형 | @SellingType, SellingType | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetAvailableSellerCouponList, GetConfirmingReceiptList, GetFinishedItemList, GetPowerRegisteredItems, GetRelatedItems 외 17개 |
| Seq | @Seq, Seq | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemForBrandShop |
| Seqno | @Seqno, Seqno | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Shiping 수수료 유형 | @ShipingFeeType, ShipingFeeType | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, ReviseItem 외 2개 |
| Shop Catg Prod | ShopCatgProd | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Shop 명 | ShopName | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad, ReviseitemLocationkorea |
| Shop 전화번호 번호 | ShopTelNo | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, GetItemLocationKorea, ReviseitemLocationBroad, ReviseitemLocationkorea |
| Sido | Sido | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeKorea, GetItemLocationKorea, ReviseitemLocationkorea |
| Sigugun | Sigugun | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeKorea, GetItemLocationKorea, ReviseitemLocationkorea |
| Site Goods 번호 | @SiteGoodsNo, SiteGoodsNo | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddOfficialNotice, AddUsedItem, ReviseItem 외 5개 |
| Slot 번호 | @SlotNo, SlotNo | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| Smile Cash 상품 Expect Save 금액 | @SmileCashItemExpectSaveAmount, SmileCashItemExpectSaveAmount | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cash 상품 Expect Save 일자 | @SmileCashItemExpectSaveDate, SmileCashItemExpectSaveDate | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Smile Cashback 금액 | SmileCashbackAmount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Smile Cashback 일자 | SmileCashbackDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Soho Best50 상품 | SohoBest50Item | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50 |
| Soho Home Hot Keyword 상품 Details | SohoHomeHotKeywordItemDetails | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoHotKeyword |
| Soho Large 카테고리 | @SohoLargeCategory, SohoLargeCategory | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Soho Middle 카테고리 | @SohoMiddleCategory, SohoMiddleCategory | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Soho Shop Best 상품 List | SohoShopBestItemList | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoRanking |
| Soho Shop 상품 | SohoShopItem | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoRanking, GetSohoShopBest50 |
| Soho Shop 상품 List | SohoShopItemList | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoHotKeyword, GetSohoLookbook, GetSohoSaleItems 외 2개 |
| Soho Shop 카테고리 Index Entry | SohoShopCategoryIndexEntry | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoCategoryBox, GetSohoShopSearchResults, GetSohoShopSearchResultsCategoryBox |
| Soho Style Finder 카테고리 | SohoStyleFinderCategory | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Soho 상품 Color List | SohoItemColorList | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| Soho 상품 Icon List | SohoItemIconList | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| Soho 카테고리 | @SohoCategory, SohoCategory | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Soho 카테고리 Gender | @SohoCategoryGender, SohoCategoryGender | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoRanking, GetSohoShopBest50 |
| Soho 카테고리 코드 | @SohoCategoryCode, SohoCategoryCode | 기타 API, 상품 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoCategoryBox, GetSohoRanking, GetSohoSaleItems, GetSohoShopBest50 |
| Soho 카테고리 코드 Array List | @SohoCategoryCodeArrayList, SohoCategoryCodeArrayList | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50 |
| Sort Condition | @SortCondition, SortCondition | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemFreeExperienceList, GetSellPlusItemList |
| Start 가격 | @StartPrice, StartPrice | 기타 API, 상품 API | 21 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteAuctionItemList, GetMyAuctionItemList, GetPowerRegisteredItems, GetRelatedItems, GetSearchResults 외 16개 |
| Start 시간 | @StartTime, StartTime | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemForUsedMarket, ViewItem, ViewItemForUsedMarket, ViewItem_old |
| State | State | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad, GetItemLocationBroad, ReviseitemLocationBroad |
| Stipulation Period | @StipulationPeriod, StipulationPeriod | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Store Pickup 주소 | StorePickupAddress | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Supply 가격 | @SupplyPrice, SupplyPrice | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Total 번호 Of Entries | @TotalNumberOfEntries, TotalNumberOfEntries | 기타 API, 상품 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia 외 7개 |
| Trade Description | @TradeDescription, TradeDescription | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Traditional Goods Corner | TraditionalGoodsCorner | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Trans Policy 번호 | @TransPolicyNo, TransPolicyNo | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, GetTransPolicyList 외 5개 |
| Unit | @Unit, Unit | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Uri | @Uri, Uri | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemForBrandShop |
| Used History | UsedHistory | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Used Month | @UsedMonth, UsedMonth | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| User ID | @UserID, UserID | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Vehicle 속성 | VehicleAttribute | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Vertical Display 유형 | @VerticalDisplayType, VerticalDisplayType | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| Vertical 유형 | @VerticalType, VerticalType | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| View Check Image URL | @ViewCheckImageUrl, ViewCheckImageUrl | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid, GetPowerRegisteredItems, GetTodayRecommandBestItems, GetTodayRecommandItems |
| View 건수 | @ViewCount, ViewCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetRelatedItems |
| Vip URL | @VipUrl, VipUrl | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| Width | @Width, Width | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemForBrandShop |
| Wish Keyword | @WishKeyword, WishKeyword | 기타 API, 상품 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemSelling 외 3개 |
| Wish Keyword Opt In | @WishKeywordOptIn, WishKeywordOptIn | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 가격 Range Filter | PriceRangeFilter | 기타 API, 상품 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults, GetSearchResultsBest100 외 6개 |
| 가격 결과 | PriceResult | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 4개 |
| 건수 | @Count, Count | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetMyAuctionBuyingSellingCount, GetMyOnSaleItemCount, GetSearchTrendCenter 외 4개 |
| 검색용 상품명 | @NameSearch, NameSearch | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 결과 Max 가격 | @ResultMaxPrice, ResultMaxPrice | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 4개 |
| 결과 Min 가격 | @ResultMinPrice, ResultMinPrice | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 4개 |
| 결과 Msg | @ResultMsg, ResultMsg | 기타 API, 상품 API | 19 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddGroupToFavoriteGroupList, AddItemToFavoriteItemList, DeleteFavoriteAuctionItem, DeleteItemFromFavoriteItemList 외 14개 |
| 구매가능수량 | @BuyableQuantity, BuyableQuantity | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 17개 |
| 구매자 Charge Cell Phone Amnt | @BuyerChargeCellPhoneAmnt, BuyerChargeCellPhoneAmnt | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 구매자 Descriptive Text | @BuyerDescriptiveText, BuyerDescriptiveText | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 발송 By 휴대폰번호 수수료 | @SendByMobileFee, SendByMobileFee | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 브랜드 | Brand | 기타 API, 상품 API | 18 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID, GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100 외 13개 |
| 브랜드 ID | @BrandID, BrandID | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID, GetCatalog, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst 외 5개 |
| 사용 By 일자 | @UseByDate, UseByDate | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 사용 Option Buy 수량 | @UseOptionBuyQty, UseOptionBuyQty | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 사용 여부 | @UseYN, UseYN | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 상태 코드 | @StatusCode, StatusCode | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| 상품 Feedback 유형 | @ItemFeedbackType, ItemFeedbackType | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SetBuyingDecisionAndFeedbackFirst |
| 상품 Image Path List | ItemImagePathList | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| 상품 Landing URL | @ItemLandingUrl, ItemLandingUrl | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 5개 |
| 상품 Official Noti Value | ItemOfficialNotiValue | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, ViewOfficialNotice |
| 상품 Official Notice | ItemOfficialNotice | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, ViewOfficialNotice |
| 상품 Option | @ItemOption, ItemOption | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst |
| 상품 건수 | @ItemCount, ItemCount | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteGroupList |
| 상품 수량 | ItemQty | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| 상품 유형 | ItemType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| 속성 Set Array | AttributeSetArray | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 수량 Sold | @QuantitySold, QuantitySold | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 수수료 Plan Seq 번호 | @FeePlanSeqNo, FeePlanSeqNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 수입신고번호 | @ImportNo, ImportNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 시중가 | @MarketPrice, MarketPrice | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 17개 |
| 여부 Adult | @IsAdult, IsAdult | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Bulk 할인 | @IsBulkDiscount, IsBulkDiscount | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| 여부 C2 C | @IsC2C, IsC2C | 기타 API, 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetFeedbackFirst, GetFeedbackSecondRemainList 외 5개 |
| 여부 Convert 요청 | @IsConvertRequest, IsConvertRequest | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Default 수수료 Plan | @IsDefaultFeePlan, IsDefaultFeePlan | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Discounted | @IsDiscounted, IsDiscounted | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Donor Shopping | @IsDonorShopping, IsDonorShopping | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Exception Allkill | @IsExceptionAllkill, IsExceptionAllkill | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| 여부 Exclude35 Policy | @IsExclude35Policy, IsExclude35Policy | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Free Experience | @IsFreeExperience, IsFreeExperience | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 17개 |
| 여부 General Call Plan | @IsGeneralCallPlan, IsGeneralCallPlan | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Install | @IsInstall, IsInstall | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Lease | @IsLease, IsLease | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Marton | @IsMarton, IsMarton | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Moving Picture | @IsMovingPicture, IsMovingPicture | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 여부 Multiple Sell Unit | @IsMultipleSellUnit, IsMultipleSellUnit | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Only Brnad Shop | @IsOnlyBrnadShop, IsOnlyBrnadShop | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID, ViewItem, ViewItem_old |
| 여부 PCS | @IsPCS, IsPCS | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Quick Service | @IsQuickService, IsQuickService | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 여부 Representation | @IsRepresentation, IsRepresentation | 기타 API, 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| 여부 Reward Exclude 상품 | @IsRewardExcludeItem, IsRewardExcludeItem | 기타 API, 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Sold Out | @IsSoldOut, IsSoldOut | 기타 API, 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 여부 Store Pickup | @IsStorePickup, IsStorePickup | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 여부 Trust 판매자 | @IsTrustSeller, IsTrustSeller | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 여부 VATFree | @IsVATFree, IsVATFree | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 판매자 DCException | @IsSellerDCException, IsSellerDCException | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 판매자 Point Amnt | @IsSellerPointAmnt, IsSellerPointAmnt | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 판매자 Point Rate | @IsSellerPointRate, IsSellerPointRate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 할인 In Full | @IsDiscountInFull, IsDiscountInFull | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 여부 회원 할인 | @IsMemberDiscount, IsMemberDiscount | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 2개 |
| 여부 휴대폰번호 | @IsMobile, IsMobile | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 휴대폰번호 Only | @IsMobileOnly, IsMobileOnly | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 요청 가격 | @RequestPrice, RequestPrice | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart, ViewCartDetail |
| 원산지 | @PlaceOfOrigin, PlaceOfOrigin | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 원재료 유형 | @RawMaterialsType, RawMaterialsType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 유통기한 | @Expiry, Expiry | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 유형 | @Type, Type, type | 기타 API, 상품 API | 19 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, GetBrandID, GetISBNSearchResults, GetPromotionMasterInfo, GetSearchResults 외 14개 |
| 제조일자 | @ProductionDate, ProductionDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 카테고리 | @Category, Category | 기타 API, 상품 API | 23 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCatalog, GetISBNSearchResults, GetPowerRegisteredItems, GetPromotionMasterInfo, GetRelatedItems 외 18개 |
| 카테고리 Array | CategoryArray | 기타 API, 상품 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetPowerRegisteredItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 10개 |
| 카테고리 Level | @CategoryLevel, CategoryLevel | 기타 API, 상품 API | 22 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetCategories, GetISBNSearchResults 외 17개 |
| 카테고리 코드 | @CategoryCode, CategoryCode, categoryCode | 기타 API, 상품 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetAvailableSellerCouponList, GetBuyingDecisionInfo 외 10개 |
| 판매자 | @Seller, Seller | 기타 API, 상품 API | 34 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetFeedbackSecondRemainList, GetPowerRegisteredItems 외 29개 |
| 판매자 Discount2 | @SellerDiscount2, SellerDiscount2 | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Info | SellerInfo | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 판매자 Ins Attr Value | @SellerInsAttrValue, SellerInsAttrValue | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Point Group 번호 | @SellerPointGroupNo, SellerPointGroupNo | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Smile Cash Rate | @SellerSmileCashRate, SellerSmileCashRate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 주소 | SellerAddress | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 할인 | @SellerDiscount, SellerDiscount | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 할인 From 일자 | @SellerDiscountFromDate, SellerDiscountFromDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 할인 To 일자 | @SellerDiscountToDate, SellerDiscountToDate | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 할인 유형 | @SellerDiscountType, SellerDiscountType | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 할인 | @Discount, Discount | 기타 API, 상품 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoBest50, GetSohoHotKeyword, GetSohoLookbook 외 7개 |
| 할인 Array | DiscountArray | 기타 API, 상품 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 할인가 | @DiscountPrice, DiscountPrice | 기타 API, 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewCart 외 2개 |
| 홍보용 상품명 | @NamePrmt, NamePrmt | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 휴대폰번호 Description | @MobileDescription, MobileDescription | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 휴대폰번호 Only 상품 건수 | MobileOnlyItemCount | 기타 API, 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia, GetSearchResultsExtMediaByItemNos 외 4개 |
| 휴대폰번호 Phone Installment | MobilePhoneInstallment | 기타 API, 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 휴대폰번호 Vip URL | @MobileVipUrl, MobileVipUrl | 기타 API, 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| Keyword | @Keyword, Keyword | 기타 API, 상품 API, 인증 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetISBNSearchResults, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults 외 12개 |
| Max 가격 | @MaxPrice, MaxPrice | 기타 API, 상품 API, 인증 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteAuctionItemList, FavoriteItemList, GetBiddingHistory, GetCatalog, GetISBNSearchResults 외 12개 |
| Min 가격 | @MinPrice, MinPrice | 기타 API, 상품 API, 인증 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetISBNSearchResults, GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults 외 8개 |
| Total 번호 Of Pages | @TotalNumberOfPages, TotalNumberOfPages | 기타 API, 상품 API, 인증 API | 14 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos, GetSearchResultsExtMedia 외 9개 |
| Total 상품 건수 | @TotalItemCount, TotalItemCount | 기타 API, 상품 API, 인증 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResultsLodge, GetSearchResultsTicket, GetSohoLookbook 외 2개 |
| 할인 Begin 일자 | @DiscountBeginDate, DiscountBeginDate | 기타 API, 상품 API, 인증 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSearchResultsTicket, ReviseItem 외 2개 |
| 할인 End 일자 | @DiscountEndDate, DiscountEndDate | 기타 API, 상품 API, 인증 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSearchResultsTicket, ReviseItem 외 2개 |
| Option 가격 | @OptionPrice, OptionPrice | 기타 API, 상품 API, 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetSettlementDetail, ViewCart |
| 회원 ID | @MemberID, MemberID | 기타 API, 상품 API, 정산 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetConfirmedAccountNumbers, ReviseItem 외 12개 |
| Prod Option | ProdOption | 기타 API, 상품 API, 정산 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail, GetShippingAddressList, GetShippingDetail, ViewItem, ViewItem_old |
| 카테고리 ID | @CategoryID, CategoryID | 기타 API, 상품 API, 정산 API, 주문/배송 API | 31 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetCompletedRemittanceList, GetDeliveryPrepareList, GetFinishedItemList, GetISBNSearchResults 외 26개 |
| Search Duration | SearchDuration | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestListBySearchCondition, GetFinishedItemList 외 6개 |
| Search Value | @SearchValue, SearchValue | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCancelNotReceivedList, GetCompletedRemittanceList, GetDeliveryPrepareList, GetFinishedItemList, GetOrderInfoList 외 6개 |
| Search 유형 | @SearchType, SearchType | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 16 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCancelApprovalList, GetCancelNotReceivedList, GetCompletedRemittanceList, GetDeliveryPrepareList, GetExchangeRequestListBySearchCondition 외 11개 |
| 요청 Option 가격 | @RequestOptionPrice, RequestOptionPrice | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExpectedRemittanceList, GetOrderCanceledList 외 6개 |
| 주문수량 | @AwardQty, AwardQty | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory, GetCancelApprovalList, GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList 외 12개 |
| 판매자 재고코드 | @SellerStockCode, SellerStockCode | 기타 API, 상품 API, 정산 API, 주문/배송 API, 클레임 API | 14 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExpectedRemittanceList 외 9개 |
| Add 수수료 Exclude Jeju | @AddFeeExcludeJeju, AddFeeExcludeJeju | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, ReviseItem 외 2개 |
| Add 수수료 Jeju | @AddFeeJeju, AddFeeJeju | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, ReviseItem 외 2개 |
| Additional 배송 유형 | @AdditionalShippingType, AdditionalShippingType | 기타 API, 상품 API, 주문/배송 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, Cart, Carts 외 6개 |
| Award 수량 | @AwardQuantity, AwardQuantity | 기타 API, 상품 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList, GetShippingAddressList |
| Change 유형 | @ChangeType, ChangeType | 기타 API, 상품 API, 주문/배송 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, ReviseTransPolicy 외 7개 |
| Condition Level1 | ConditionLevel1 | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| Condition Level2 | ConditionLevel2 | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| Condition Level3 | ConditionLevel3 | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| Condition Level4 | ConditionLevel4 | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| Condition Level5 | ConditionLevel5 | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| Epin Matching Ver 번호 | @EpinMatchingVerNo, EpinMatchingVerNo | 기타 API, 상품 API, 주문/배송 API | 14 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, Cart, Carts 외 9개 |
| Error 메시지 | @ErrorMessage, ErrorMessage | 기타 API, 상품 API, 주문/배송 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddInterestItem, Bid, Cart, Carts, GetShippingPolicyInfoList 외 10개 |
| Etc | @Etc, Etc | 기타 API, 상품 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: DoshippingConnected, GetItemGeocodeKorea, GetItemLocationKorea, ReviseitemLocationkorea |
| Gitem 번호 | @GitemNo, GitemNo | 기타 API, 상품 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Image Height | @ImageHeight, ImageHeight | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Image Width | @ImageWidth, ImageWidth | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Impose 유형 | @ImposeType, ImposeType | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, ReviseItem 외 2개 |
| Install Model 코드 | @InstallModelCode, InstallModelCode | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPaidOrderList, GetShippingAddressList 외 4개 |
| Obj Opt Clase No1 | @ObjOptClaseNo1, ObjOptClaseNo1 | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Obj Opt Clase No2 | @ObjOptClaseNo2, ObjOptClaseNo2 | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Obj Opt Clase No3 | @ObjOptClaseNo3, ObjOptClaseNo3 | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Payment 유형 | @PaymentType, PaymentType | 기타 API, 상품 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingAddressList, ReviseItemForUsedMarket, ViewItem, ViewItemForUsedMarket, ViewItem_old |
| Receipt 유형 | @ReceiptType, ReceiptType | 기타 API, 상품 API, 주문/배송 API | 18 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 13개 |
| Section | @Section, Section | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Shipment Place | @ShipmentPlace, ShipmentPlace | 기타 API, 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, FavoriteGroupList, GetShippingPlaceCode 외 3개 |
| Single Opt Seq 번호 | @SingleOptSeqNo, SingleOptSeqNo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Sku Info | SkuInfo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Sku Matching Ver 번호 | @SkuMatchingVerNo, SkuMatchingVerNo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Stand Alone 재고 Seq 번호 | @StandAloneStockSeqNo, StandAloneStockSeqNo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Text | @Text, Text | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Text2 | @Text2, Text2 | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| Version | @Version, Version | 기타 API, 상품 API, 주문/배송 API | 56 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddFavoriteAuctionItem, AddGroupToFavoriteGroupList, AddItem, AddItemMobile, AddItemToFavoriteItemList 외 51개 |
| 배송 | Shipping | 기타 API, 상품 API, 주문/배송 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 배송 Place Seq | @ShippingPlaceSeq, ShippingPlaceSeq | 기타 API, 상품 API, 주문/배송 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, FavoriteGroupList, GetSearchResults 외 8개 |
| 배송 Regions | @ShippingRegions, ShippingRegions | 기타 API, 상품 API, 주문/배송 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| 사은품 | @FreeGift, FreeGift | 기타 API, 상품 API, 주문/배송 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, GetShippingAddressList 외 5개 |
| 상품 재고 Calc 번호 | @ItemStockCalcNo, ItemStockCalcNo | 기타 API, 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 3개 |
| 상품 재고 번호 | @ItemStockNo, ItemStockNo | 기타 API, 상품 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 수수료 | @Fee, Fee, fee | 기타 API, 상품 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, GetShippingPlaceCode, GetShippingPolicyInfoList, ReviseItemSelling |
| 수수료 Free Condition 유형 | @FeeFreeConditionType, FeeFreeConditionType | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| 여부 Arrival | @IsArrival, IsArrival | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, GetShippingPlaceCode 외 4개 |
| 여부 Default Place | @IsDefaultPlace, IsDefaultPlace | 기타 API, 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, ReviseItem 외 2개 |
| 여부 Displayable | @IsDisplayable, IsDisplayable | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| 여부 Prepayable | @IsPrepayable, IsPrepayable | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, GetShippingPolicyInfoList 외 4개 |
| 재고 ID | @StockId, StockId | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| 재고 Master Seq 번호 | @StockMasterSeqNo, StockMasterSeqNo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| 재고 Text 번호 | @StockTextNo, StockTextNo | 기타 API, 상품 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, SetCart, SmileShippingCart |
| 재고 번호 | @StockNo, StockNo | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| 재고수량 | @StockQty, StockQty | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, ReviseItemStock, SetCart 외 4개 |
| 주소 | @Address, Address | 기타 API, 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetItemGeocodeBroad, GetItemGeocodeKorea 외 4개 |
| 카테고리 명 | @CategoryName, CategoryName | 기타 API, 상품 API, 주문/배송 API | 21 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetFinishedItemList, GetISBNSearchResults, GetOrderCanceledList, GetSearchResults 외 16개 |
| 코드 | @Code, Code | 기타 API, 상품 API, 주문/배송 API | 14 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, GetMobileSohoBest100, GetMobileSohoSrpLp 외 9개 |
| 판매자 Addr 번호 | @SellerAddrNo, SellerAddrNo | 기타 API, 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellerAddresses, GetShippingPlaceCode 외 3개 |
| Image URL | @ImageUrl, ImageUrl | 기타 API, 상품 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, Cart, Carts, GetBidCancelList, GetSearchTrendCenter 외 6개 |
| 수량 | @Qty, Qty, qty, @Quantity, Quantity | 기타 API, 상품 API, 주문/배송 API, 클레임 API | 32 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, Bid, BidList, Cart, Carts 외 27개 |
| 주문 | Order | 기타 API, 상품 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetReturnList, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst 외 5개 |
| Staff 번호 | @StaffNo, StaffNo | 기타 API, 상품 API, 클레임 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItemMobile, GetReturningList, GetSohoShopHomeNewArrival, GetSohoShopStyleTrendList, ReviseItemStock 외 1개 |
| 반품 | Return | 기타 API, 상품 API, 클레임 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetRelatedItems, GetSearchResults, GetSearchResultsBest100, GetSearchResultsByItemNos 외 12개 |
| Home 페이지 | @HomePage, HomePage | 기타 API, 인증 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge, GetSearchResultsTicket |
| Performance Begin 일자 | @PerformanceBeginDate, PerformanceBeginDate | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance End 일자 | @PerformanceEndDate, PerformanceEndDate | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance End 일자 From | @PerformanceEndDateFrom, PerformanceEndDateFrom | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance End 일자 To | @PerformanceEndDateTo, PerformanceEndDateTo | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance 일자 From | @PerformanceDateFrom, PerformanceDateFrom | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance 일자 To | @PerformanceDateTo, PerformanceDateTo | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance 전화번호 | @PerformanceTel, PerformanceTel | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| 할인 금액 | @DiscountAmount, DiscountAmount | 기타 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Bank 명 | @BankName, BankName | 기타 API, 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers, GetMyAccount |
| Bank 코드 | @BankCode, BankCode | 기타 API, 정산 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoChangeRemittanceMethod, GetConfirmedAccountNumbers, GetMyAccount |
| Best 회원 할인 | @BestMemberDiscount, BestMemberDiscount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Bulk 할인 | @BulkDiscount, BulkDiscount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Comment | @Comment, Comment | 기타 API, 정산 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetFeedbackFirst, GetSellerEmoneyDepositList, PurchaseBenefit, SetBuyingDecisionAndFeedbackFirst |
| Direct 할인 금액 | @DirectDiscountAmount, DirectDiscountAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Etc 수수료 금액 | @EtcFeeAmount, EtcFeeAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Event Emoney | @EventEmoney, EventEmoney | 기타 API, 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableEmoney, GetISBNSearchResults |
| Expected Remit 금액 | @ExpectedRemitAmount, ExpectedRemitAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Expected Remit 상태 | @ExpectedRemitStatus, ExpectedRemitStatus | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Expected Remit 일자 | @ExpectedRemitDate, ExpectedRemitDate | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Occur 유형 | @OccurType, OccurType | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| Occur 일자 | @OccurDate, OccurDate | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| Options | Options | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Pay By | @PayBy, PayBy | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| Pay It Once 할인 | @PayItOnceDiscount, PayItOnceDiscount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Regist 일자 | @RegistDate, RegistDate | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers |
| Search Acc 유형 | SearchAccType | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| Search 일자 From | @SearchDateFrom, SearchDateFrom | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Search 일자 To | @SearchDateTo, SearchDateTo | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Sell 수수료 금액 | @SellFeeAmount, SellFeeAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Trans Money | @TransMoney, TransMoney | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| 번호 Interest 수수료 금액 | @NoInterestFeeAmount, NoInterestFeeAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 판매자 Coupon Discount1 | @SellerCouponDiscount1, SellerCouponDiscount1 | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 판매자 Coupon Discount2 | @SellerCouponDiscount2, SellerCouponDiscount2 | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 판매자 Coupon 할인 | @SellerCouponDiscount, SellerCouponDiscount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 판매자 Point 금액 | @SellerPointAmount, SellerPointAmount | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 회원 명 | @MemberName, MemberName | 기타 API, 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers |
| Acct 일자 | @AcctDate, AcctDate | 기타 API, 정산 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetOrderInfoList |
| Buy Award 유형 | @BuyAwardType, BuyAwardType | 기타 API, 정산 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExpectedRemittanceList, GetShippingAddressList, GetShippingOrderList |
| Duration 유형 | @DurationType, DurationType | 기타 API, 정산 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList, GetShippingOrderList |
| Option 명 | @OptionName, OptionName | 기타 API, 정산 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember, GetSettlementDetail 외 2개 |
| Option 수량 | @OptionQty, OptionQty, @OptionQuantity, OptionQuantity | 기타 API, 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail, GetShippingAddressList, GetShippingDetail |
| Trans 수수료 | TransFee | 기타 API, 정산 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail, GetShippingDetail |
| 금액 | @Amount, Amount | 기타 API, 정산 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList, GetShippingDetailInfoList |
| 발송 유형 | @SendType, SendType | 기타 API, 정산 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExpectedRemittanceList, GetShippingAddressList, GetShippingOrderList |
| 수취인 | @Receiver, Receiver | 기타 API, 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExpectedRemittanceList, GetShippingOrderList |
| 입금/접수일시 | @ReceiptDate, ReceiptDate | 기타 API, 정산 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList |
| 주문 Base | OrderBase | 기타 API, 정산 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExpectedRemittanceList, GetOrderCanceledList 외 4개 |
| Fail 사유 | @FailReason, FailReason | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AlertShippingDelay, AppoveBidCancel, BidCancel, ChangeShippingType, ChangeShippingTypeBeforeOrder 외 12개 |
| Group 주문 Seqno | @GroupOrderSeqno, GroupOrderSeqno | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExpectedRemittanceList, GetOrderCanceledList 외 8개 |
| Pay 번호 | @PayNo, PayNo | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExpectedRemittanceList, GetPaidOrderList, GetReturnList, GetSellerEmoneyDepositList 외 4개 |
| 구매자명 | @BuyerName, BuyerName | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 18 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList, GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestDetailInfo 외 13개 |
| 발송일시 | @SendDate, SendDate | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeSwitch, DoShippingBundle, DoShippingGeneral, GetCompletedRemittanceList, GetExpectedRemittanceList 외 2개 |
| 배송 요청사항 | @RequestOption, RequestOption | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 17 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Bid, Cart, Carts, GetCompletedRemittanceList, GetConfirmingReceiptList 외 12개 |
| 배송비 금액 | @DeliveryFeeAmount, DeliveryFeeAmount | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExpectedRemittanceList, GetOrderCanceledList 외 6개 |
| 주문금액 | @AwardAmount, AwardAmount | 기타 API, 정산 API, 주문/배송 API, 클레임 API | 15 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList, GetCompletedRemittanceList, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList 외 10개 |
| Search Keyword | @SearchKeyword, SearchKeyword | 기타 API, 정산 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestListBySearchCondition, GetReturnList, GetSellerEmoneyDepositList, GetSohoShopStyleFinder |
| 결과 메시지 | @ResultMessage, ResultMessage | 기타 API, 정산 API, 클레임 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetFeedbackExceptionType, GetSellerEmoneyDepositList, ReviseTransPolicy, SetCancelNotReceived, SetOKCashBagSave |
| Acode | @Acode, Acode | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Addr Desc | @AddrDesc, AddrDesc | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Addr Detail | @AddrDetail, AddrDetail | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| Addr Image Path | @AddrImagePath, AddrImagePath | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Addr Post | @AddrPost, AddrPost | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| Addr 유형 | @AddrType, AddrType | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| Adversting 메시지 | @AdverstingMessage, AdverstingMessage | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| App 유형 | @AppType, AppType | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Apply Gift Packing | @ApplyGiftPacking, ApplyGiftPacking | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Bid Seq 번호 | @BidSeqNo, BidSeqNo | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Bluechip 판매자 할인 금액 | @BluechipSellerDiscountAmount, BluechipSellerDiscountAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Book One Day 배송 Desc URL | @BookOneDayShippingDescURL, BookOneDayShippingDescURL | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Book One Day 배송 End 시간 | @BookOneDayShippingEndTime, BookOneDayShippingEndTime | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Book One Day 배송 Service Area | @BookOneDayShippingServiceArea, BookOneDayShippingServiceArea | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Book One Day 배송 Start 시간 | @BookOneDayShippingStartTime, BookOneDayShippingStartTime | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Book One Day 배송 여부 | @BookOneDayShippingIs, BookOneDayShippingIs | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Canc 일자 | @CancDate, CancDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Card Payment 금액 | @CardPaymentAmount, CardPaymentAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Cart 배송 | CartShipping | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Cart 번호 | @CartNo, CartNo | 기타 API, 주문/배송 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Cart, Carts, ChangeShippingTypeBeforeOrder, GetBiddingHistory, LoadCart 외 7개 |
| Cart 상품 배송 | CartItemShipping | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Cart 요청 T | CartRequestT | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Carts, SmileShippingCarts |
| Cart 응답 T | CartResponseT | 기타 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCarts |
| Charge 유형 코드 | @ChargeTypeCode, ChargeTypeCode | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| Check Card 여부 | @CheckCardYN, CheckCardYN | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Comp 명 | @CompName, CompName | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryList |
| Comp 코드 | @CompCode, CompCode | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryList |
| Condition From | @ConditionFrom, ConditionFrom | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPlaceCode, GetShippingPolicyInfoList |
| Condition Level10 | ConditionLevel10 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| Condition Level6 | ConditionLevel6 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| Condition Level7 | ConditionLevel7 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| Condition Level8 | ConditionLevel8 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| Condition Level9 | ConditionLevel9 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| Condition To | @ConditionTo, ConditionTo | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPlaceCode, GetShippingPolicyInfoList |
| Contact Info Na | @ContactInfoNa, ContactInfoNa | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Contract 번호 | @ContractNo, ContractNo | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoEcouponOrderConfirm |
| Cur Smile 배송 건수 | @CurSmileShippingCount, CurSmileShippingCount | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| Cur Smile 배송 금액 | @CurSmileShippingAmount, CurSmileShippingAmount | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| Cur Total 건수 | @CurTotalCount, CurTotalCount | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| Default Addr 여부 | @DefaultAddrYN, DefaultAddrYN | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Default Shipment Place Addr 여부 | @DefaultShipmentPlaceAddrYN, DefaultShipmentPlaceAddrYN | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Default Visit Take Addr 여부 | @DefaultVisitTakeAddrYN, DefaultVisitTakeAddrYN | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Del 수수료 Commission | @DelFeeCommission, DelFeeCommission | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetailInfoList |
| Descriptive 요청 Option | @DescriptiveRequestOption, DescriptiveRequestOption | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Device 유형 | @DeviceType, DeviceType | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Dist Post 번호 | @DistPostNo, DistPostNo | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Dist 전화번호 | @DistTel, DistTel | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Dist 주소 Post | @DistAddressPost, DistAddressPost | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Dist 휴대폰번호 전화번호 | @DistMobileTel, DistMobileTel | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Error 유형 | @ErrorType, ErrorType | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| Error 코드 | @ErrorCode, ErrorCode | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingPolicyInfoList |
| Event 일자 | @EventDate, EventDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| General 요청 | GeneralRequest | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle |
| Gift Packing 여부 | @GiftPackingYN, GiftPackingYN | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Gmkt Gd 번호 | @GmktGdNo, GmktGdNo | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoEcouponOrderConfirm |
| Group Decision 주문 | GroupDecisionOrder | 기타 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Group Decision 주문 상품 | GroupDecisionOrderItem | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Info Ad1 | @InfoAd1, InfoAd1 | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Info Ad2 | @InfoAd2, InfoAd2 | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Info Cp | @InfoCp, InfoCp | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Info Ht | @InfoHt, InfoHt | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Ins 일자 | @InsDate, InsDate | 기타 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: BuyerNoteDetailBySeqno, BuyerNoteList, GetShippingPlaceCode, GetSohoShopHomeNewArrival, GetSohoShopStyleTrendList 외 4개 |
| Install 일자 | @InstallDate, InstallDate | 기타 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPaidOrderList, GetShippingAddressList, GetShippingDetail |
| Islands Add 수수료 | @IslandsAddFee, IslandsAddFee | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| List 건수 | @ListCount, ListCount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSendingDetailList |
| Local Chain 명 | @LocalChainName, LocalChainName | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Local Chain 코드 | @LocalChainCode, LocalChainCode | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Map URL | @MapUrl, MapURL, MapUrl | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Mart Branch 명 | @MartBranchName, MartBranchName | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Mart Branch 코드 | @MartBranchCode, MartBranchCode | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Mart 코드 | @MartCode, MartCode | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Memb ID | @MembId, MembId | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Noint Offering 수수료 금액 | @NointOfferingFeeAmount, NointOfferingFeeAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| NPage | @NPage, NPage | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSendingDetailList |
| Option Content | @OptionContent, OptionContent | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList, GetShippingDetail |
| Others | @Others, Others | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Pay For | @PayFor, PayFor | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetailInfoList |
| Payment 수수료 유형 | @PaymentFeeType, PaymentFeeType | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| Payment 일자 | @PaymentDate, PaymentDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| Platform 유형 | @PlatformType, PlatformType | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Pre Remit 금액 | @PreRemitAmount, PreRemitAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Pre Smile 배송 금액 | @PreSmileShippingAmount, PreSmileShippingAmount | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| Pre Trans 금액 | @PreTransAmount, PreTransAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Processes | Processes | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| Receive 유형 | @ReceiveType, ReceiveType | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Remark | @Remark, Remark | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| Remit 일자 | @RemitDate, RemitDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Ret Appr 일자 | @RetApprDate, RetApprDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Search Duration2 | SearchDuration2 | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Search Sort 주문 | SearchSortOrder | 기타 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResultsMartOn, GetSohoShopSearchResults |
| Search 일자 Condtion 유형 | SearchDateCondtionType | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| Site ID | @SiteID, SiteID | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Tracking Ver | @TrackingVer, TrackingVer | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Trans Policy 유형 | @TransPolicyType, TransPolicyType | 기타 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList |
| Trans 수수료 Pre Paid 여부 | @TransFeePrePaidYN, TransFeePrePaidYN | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Bid, Cart, Carts, SetCart, SmileShippingCart 외 1개 |
| Upd 일자 | @UpdDate, UpdDate | 기타 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPlaceCode, GetSohoShopHomeNewArrival, GetSohoShopStyleTrendList |
| URL | @Url, Url | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| User 유형 | @UserType, UserType | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSendingDetailList |
| Wish 배송 AMPM | @WishDeliveryAMPM, WishDeliveryAMPM | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| Wish 배송 일자 | @WishDeliveryDate, WishDeliveryDate | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Cart, Carts, GetShippingAddressList, SetCart, SmileShippingCart 외 1개 |
| 결과 유형 | @ResultType, ResultType | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, RemoveCarts, RemoveCartsByNos, SmileShippingCart 외 1개 |
| 결제일시 | @PayDate, PayDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetailInfoList |
| 구매자 Ins Value1 | @BuyerInsValue1, BuyerInsValue1 | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 구매자 Ins Value2 | @BuyerInsValue2, BuyerInsValue2 | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 구매자 Post 번호 | @BuyerPostNo, BuyerPostNo | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 구매자 Reject | @BuyerReject, BuyerReject | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingOrderList |
| 구매자 Writing | @BuyerWriting, BuyerWriting | 기타 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, SetCart, SmileShippingCart |
| 기본주소 | AddressBase | 기타 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmingReceiptList, GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList |
| 반품지 기본주소 | @RetFrontAddr, RetFrontAddr | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| 반품지 상세주소 | @RetBackAddr, RetBackAddr | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| 반품지 우편번호 | @RetPostNo, RetPostNo | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| 반품지 전화번호 | @RetTelNo, RetTelNo | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| 반품지 휴대폰번호 | @RetMobileNo, RetMobileNo | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| 발송 Expected 일자 | @SendExpectedDate, SendExpectedDate | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AlertShippingDelay |
| 발송마감일 | @TransDueDate, TransDueDate | 기타 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList |
| 배송 Method Filter | ShippingMethodFilter | 기타 API, 주문/배송 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| 수량 판매자 할인 금액 | @QuantitySellerDiscountAmount, QuantitySellerDiscountAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 여부 Certification | @IsCertification, IsCertification | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoEcouponOrderConfirm |
| 여부 Default | @IsDefault, IsDefault | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingPolicyInfoList |
| 여부 Default Policy | @IsDefaultPolicy, IsDefaultPolicy | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 여부 Receipt 요청 | @IsReceiptRequest, IsReceiptRequest | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 여부 배송 Prepay | @IsShippingPrepay, IsShippingPrepay | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| 여부 배송 수수료 Pre Pay | @IsShippingFeePrePay, IsShippingFeePrePay | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| 요청 Option Calculation | RequestOptionCalculation | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 요청 Prod Option | RequestProdOption | 기타 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Bid, Cart, Carts, SetCart, SmileShippingCart 외 3개 |
| 요청 메시지 | @RequestMessage, RequestMessage, requestMessage | 기타 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: Bid, Cart, Carts, SetCart, SmileShippingCart 외 1개 |
| 요청 배송 | RequestShipping | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: Cart, Carts, SetCart, SmileShippingCart, SmileShippingCarts |
| 주문 Nos | OrderNos | 기타 API, 주문/배송 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember, SetBuyingDecisionAndFeedbackFirst |
| 판매자 Addr Post 번호 | @SellerAddrPostNo, SellerAddrPostNo | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 판매자 Addr 명 | @SellerAddrName, SellerAddrName | 기타 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| 판매자 Book Cash 금액 | @SellerBookCashAmount, SellerBookCashAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 판매자 Coupon 수수료 금액 | @SellerCouponFeeAmount, SellerCouponFeeAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 판매자 Point 수수료 금액 | @SellerPointFeeAmount, SellerPointFeeAmount | 기타 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Canc 사유 | @CancReason, CancReason | 기타 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList, GetOrderInfoList |
| Comp 유형 | @CompType, CompType | 기타 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetDeliveryList |
| Default 반품 Addr 여부 | @DefaultReturnAddrYN, DefaultReturnAddrYN | 기타 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellerAddresses, GetShippingPlaceCode |
| Reciever | Reciever | 기타 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetShippingDetail |
| Reciever 명 | @RecieverName, RecieverName | 기타 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnList, GetShippingAddressList |
| Recp 일자 | @RecpDate, RecpDate | 기타 API, 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList, GetOrderInfoList, GetReturnAdditionalFee |
| Ret Pickup 유형 | @RetPickupType, RetPickupType | 기타 API, 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, GetReturnList |
| 구매자 | Buyer | 기타 API, 주문/배송 API, 클레임 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnDetail, GetReturnList, GetShippingDetail |
| 구매자 메시지 | @MessageForBuyer, MessageForBuyer | 기타 API, 주문/배송 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| 상세주소 | @AddressDetail, AddressDetail | 기타 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 5개 |
| 우편번호 | @PostNo, PostNo, ZipCode | 기타 API, 주문/배송 API, 클레임 API | 12 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 7개 |
| 이메일 | @Email, Email | 기타 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 5개 |
| 전화번호 | @Tel, Tel | 기타 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 6개 |
| 주소 Post | @AddressPost, AddressPost | 기타 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 5개 |
| 주소 Road 명 | @AddressRoadName, AddressRoadName | 기타 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 5개 |
| 휴대폰번호 전화번호 | @MobileTel, MobileTel | 기타 API, 주문/배송 API, 클레임 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: DoReturnRequestBySeller, GetConfirmingReceiptList, GetDeliveryPrepareList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition 외 5개 |
| Auto Approval 일자 | @AutoApprovalDate, AutoApprovalDate | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnDetail |
| Canc 사유 Detail | @CancReasonDetail, CancReasonDetail | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| Cell Phone 번호 | @CellPhoneNumber, CellPhoneNumber | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| Fail With 응답 | @FailWithResponse, FailWithResponse | 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnApproval, DoReturnHold |
| Payment Choice | @PaymentChoice, PaymentChoice | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnList |
| Phone 번호 | @PhoneNumber, PhoneNumber | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| Requested 일자 | @RequestedDate, RequestedDate | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnDetail, GetReturnList, GetReturningList |
| Reward 상태 | @RewardStatus, RewardStatus | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturningList |
| Search Flags | SearchFlags | 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestListBySearchCondition, GetReturnList |
| Search String | @SearchString, SearchString | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| Sender | Sender | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| Trust 판매자 유형 | @TrustSellerType, TrustSellerType | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnList |
| Withdraw 일자 | @WithdrawDate, WithdrawDate | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnList |
| 결과코드 | @ResultCode, ResultCode | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: PurchaseBenefit, SetCancelNotReceived, SetOKCashBagSave |
| 구매자 Phone | @BuyerPhone, BuyerPhone | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| 구매자 요청 Memo | @BuyerRequestMemo, BuyerRequestMemo | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnList |
| 구매자 이메일 | @BuyerEmail, BuyerEmail | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 구매자 휴대폰번호 | @BuyerMobile, BuyerMobile | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| 메시지 | @Message, Message | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoSellingCancel, GetCheckMessageBeforeSellingCancel, SetCancelNotReceived |
| 메시지 코드 | @MessageCode, MessageCode | 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoSellingCancel, GetCheckMessageBeforeSellingCancel |
| 사유 Detail | @ReasonDetail, ReasonDetail | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoSellingCancel |
| 수취인명 | @ReceiverName, ReceiverName | 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 여부 Success | @IsSuccess, IsSuccess | 기타 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AppoveBidCancel, BidCancel |
| 요청 일자 | @RequestDate, RequestDate | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| 조회일자 유형 | @SearchDateType, SearchDateType | 기타 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList, GetExchangeRequestListBySearchCondition, GetReturnList |
| 판매자 메시지 | @SellerMessage, SellerMessage | 기타 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| Auction Low 가격 | @AuctionLowPrice, AuctionLowPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Auction Low 가격 상품 번호 | @AuctionLowPriceItemNo, AuctionLowPriceItemNo | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Auth 상품 Num | AuthItemNum | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Auth 상품 유형 | AuthItemType | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Book 가격 | BookPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Bulk 할인 가격 | @BulkDiscountPrice, BulkDiscountPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Buy 가격 | BuyPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Buying Selling 유형 | BuyingSellingType | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionBuyingSellingCount |
| Child 카테고리 | ChildCategory | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Child 카테고리 List | ChildCategoryList | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalogCategory |
| Consulting 상품 Info | ConsultingItemInfo | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Consulting 상품 Value | ConsultingItemValue | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Consulting 상품 유형 | ConsultingItemType | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Coupon Applied 가격 | @CouponAppliedPrice, CouponAppliedPrice | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Current 가격 | @CurrentPrice, CurrentPrice | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Duty 사용 Days 가격 | @DutyUseDaysPrice, DutyUseDaysPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Entry 상품 건수 | @EntryItemCount, EntryItemCount | 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetItemFreeExperienceList, ReviseItem 외 2개 |
| Favorite Auction 상품 | FavoriteAuctionItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: FavoriteAuctionItemList |
| Favorite 상품 | FavoriteItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteItemList |
| Finished 상품 | FinishedItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList |
| fixed 가격 상품 여부 | fixedPriceItemYN | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| From Selling 가격 | @FromSellingPrice, FromSellingPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Get 상품 Geocode Broad 응답 T | GetItemGeocodeBroadResponseT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeBroad |
| Get 상품 Geocode Korea 응답 T | GetItemGeocodeKoreaResponseT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemGeocodeKorea |
| Get 상품 Location Broad 응답 T | GetItemLocationBroadResponseT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemLocationBroad |
| Get 상품 Location Korea 응답 T | GetItemLocationKoreaResponseT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetItemLocationKorea |
| Group Buy 속성 Set | GroupBuyAttributeSet | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Imported 상품 | ImportedItem | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Install 가격 | @InstallPrice, InstallPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Installment 속성 Set | InstallmentAttributeSet | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Interest 상품 | InterestItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddInterestItem |
| Internet Low 가격 | @InternetLowPrice, InternetLowPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| ISBNAttribute Set | ISBNAttributeSet | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| License 속성 Set | LicenseAttributeSet | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Mart On 카테고리 명 Mapping Info T | MartOnCategoryNameMappingInfoT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMartOnCategoryBox |
| Matching 상품 Cnt | @MatchingItemCnt, MatchingItemCnt | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| Month Rental 가격 | @MonthRentalPrice, MonthRentalPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| My Auction Selling 상품 | MyAuctionSellingItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionSellingItemList |
| My Auction 상품 | MyAuctionItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionItemList |
| Option 상품 Flag | OptionItemFlag | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Option 상품 번호 | OptionItemNo | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Option 재고 | OptionStock | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Option 재고 유형 | @OptionStockType, OptionStockType | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| Org 카탈로그 ID | @OrgCatalogID, OrgCatalogID | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Ow 가격 | @OwPrice, OwPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Ownership Days 가격 | @OwnershipDaysPrice, OwnershipDaysPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Price1 | Price1 | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Price2 | Price2 | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Price3 | Price3 | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Promotion 상품 List T | PromotionItemListT | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionItemList |
| Reg 가격 | @RegPrice, RegPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Related 상품 Array | RelatedItemArray | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetRelatedItems |
| Rep 상품 명 | RepItemName | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Rep 속성 Set | RepAttributeSet | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Sd Product 브랜드 코드 | @SdProductBrandCode, SdProductBrandCode | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Sd 브랜드 코드 | @SdBrandCode, SdBrandCode | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Sd 카테고리 코드 | @SdCategoryCode, SdCategoryCode | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Search ADItem Array | SearchADItemArray | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPowerRegisteredItems, GetTodayRecommandBestItems, GetTodayRecommandItems |
| Search 결과 | SearchResult | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Selling Priod | @SellingPriod, SellingPriod | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList |
| Selling 가격 | @SellingPrice, SellingPrice | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Selling 상태 코드 | @SellingStatusCode, SellingStatusCode | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| Shop 카테고리 코드 | @ShopCategoryCode, ShopCategoryCode | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Single 상품 여부 | @SingleItemYn, SingleItemYn | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Start 가격 여부 | StartPriceYn | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Sub Catalogs | SubCatalogs | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| Sum 재고 수량 | @SumStockQty, SumStockQty | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| To Selling 가격 | @ToSellingPrice, ToSellingPrice | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Unit 가격 | @UnitPrice, UnitPrice | 상품 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemStock 외 3개 |
| Vehicle 속성 Set | VehicleAttributeSet | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| Vertical 상품 Info | VerticalItemInfo | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| View 상품 URL | @ViewItemURL, ViewItemURL | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 가격 Expose 여부 | PriceExposeYn | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 가격 Per Month | PricePerMonth | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 가격 Range | PriceRange | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| 브랜드 List | BrandList | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| 브랜드 Shop 상품 | BrandShopItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemForBrandShop |
| 브랜드 Shop 카테고리 코드 | @BrandShopCategoryCode, BrandShopCategoryCode | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 브랜드 코드 | @BrandCode, BrandCode | 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForBrandShop 외 2개 |
| 브랜드명 | @BrandName, BrandName | 상품 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, FavoriteModelList, GetBrandID 외 5개 |
| 사용자정의 브랜드명 | @UserDefineBrandName, UserDefineBrandName | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 | Item | 상품 API | 13 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetPowerRegisteredItems, GetRelatedItems 외 8개 |
| 상품 Add Html | @ItemAddHtml, ItemAddHtml | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Auction 할인 | ItemAuctionDiscount | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Book Cash | ItemBookCash | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Call Plan | ItemCallPlan | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Class | @ItemClass, ItemClass | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 상품 Consulting | ItemConsulting | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Contents Html | ItemContentsHtml | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Display 여부 | @ItemDisplayYN, ItemDisplayYN | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| 상품 Extra | ItemExtra | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Free Experience | ItemFreeExperience | 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetItemFreeExperienceList, ReviseItem 외 2개 |
| 상품 Html | @ItemHtml, ItemHtml | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Image | ItemImage | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: ReviseItemPictures |
| 상품 License 번호 | ItemLicenseNo | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 상품 List | ItemList | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList, GetSellingItemList |
| 상품 Nos | itemNos | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 상품 Picture | ItemPicture | 상품 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 4개 |
| 상품 Promotion Html | @ItemPromotionHtml, ItemPromotionHtml | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Regist 일자 | @ItemRegistDate, ItemRegistDate | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 상품 Rental | ItemRental | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 Selling | ItemSelling | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemSelling, ViewItemSelling |
| 상품 Selling 상태 | ItemSellingStatus | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemSellingStatus |
| 상품 Total 수량 | @ItemTotalQuantity, ItemTotalQuantity | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList |
| 상품 브랜드 Shop Picture | ItemBrandShopPicture | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemForBrandShop |
| 상품 상태 | @ItemStatus, ItemStatus | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionItemList |
| 상품 재고 | ItemStock | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 상품 재고 Stand Alone 번호 | @ItemStockStandAloneNo, ItemStockStandAloneNo | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 상품 재고 Text 번호 | @ItemStockTextNo, ItemStockTextNo | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 상품 카테고리 Attr | ItemCategoryAttr | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseAttribute, ViewAttribute |
| 상품 카테고리 속성 | ItemCategoryAttribute | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 판매자 Shop | ItemSellerShop | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품 할인 | ItemDiscount | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 상품상태 | @ItemStatusType, ItemStatusType | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 속성 Element 명 | @AttributeElementName, AttributeElementName | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteModelList |
| 속성 List | AttributeList | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| 속성 Sets | AttributeSets | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog |
| 여부 Available Donor Shop 상품 | @IsAvailableDonorShopItem, IsAvailableDonorShopItem | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 여부 Fixed 상품 | @IsFixedItem, IsFixedItem | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionSellingItemList |
| 여부 Item20 SPS | IsItem20SPS | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 여부 Vertical 상품 | @IsVerticalItem, IsVerticalItem | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| 여부 브랜드 Shop | @IsBrandShop, IsBrandShop | 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForBrandShop 외 2개 |
| 여부 재고 수량 Mng | @IsStockQtyMng, IsStockQtyMng | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 여부 카탈로그 | @IsCatalog, IsCatalog | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList |
| 여부 판매자 Regist 브랜드 | @IsSellerRegistBrand, IsSellerRegistBrand | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBrandID, ViewItem, ViewItem_old |
| 재고 Calculation | StockCalculation | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 재고 Stand Alone | StockStandAlone | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 재고 Text | StockText | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 재고 상태 | @StockStatus, StockStatus | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 카탈로그 | Catalog | 상품 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCatalog, ReviseItemForUsedMarket, ViewItemForUsedMarket |
| 카탈로그 Attr 여부 | @CatalogAttrYn, CatalogAttrYn | 상품 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewCategoryAttribute 외 2개 |
| 카탈로그 ID | @CatalogID, CatalogID | 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: DoFavoriteModelAdd, DoFavoriteModelDelete, FavoriteModelList, GetCatalog |
| 카탈로그 명 | @CatalogName, CatalogName | 상품 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteModelList, GetCatalog, ReviseItemForUsedMarket, ViewItemForUsedMarket |
| 카탈로그 코드 | @CatalogCode, CatalogCode | 상품 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 3개 |
| 카테고리 Attr | CategoryAttr | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCategoryAttribute |
| 카테고리 List | CategoryList | 상품 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCatalog, GetCatalogCategory |
| 카테고리 Node | CategoryNode | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerSellingCategories |
| 카테고리 Node Array | CategoryNodeArray | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerSellingCategories |
| 카테고리 속성 | CategoryAttribute | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Shop 브랜드 | SellerShopBrand | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Shop 브랜드 명 | SellerShopBrandName | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 판매자 Shop 브랜드 코드 | SellerShopBrandCode | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 판매자 Shop 카테고리 | SellerShopCategory | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 판매자 Shop 카테고리 명 | SellerShopCategoryName | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 판매자 Shop 카테고리 코드 | SellerShopCategoryCode | 상품 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 판매지역 | @SellingArea, SellingArea | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 회원 할인 가격 | @MemberDiscountPrice, MemberDiscountPrice | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 휴대폰번호 Phone Real 가격 Installment | MobilePhoneRealPriceInstallment | 상품 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 가격 Info | @PriceInfo, PriceInfo | 상품 API, 인증 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Option 상품 가격 | @OptionItemPrice, OptionItemPrice | 상품 API, 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail, GetShippingAddressList, GetShippingDetail |
| Option 상품 명 | @OptionItemName, OptionItemName | 상품 API, 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail, GetShippingAddressList, GetShippingDetail |
| 상품코드 | @ItemCode, ItemCode | 상품 API, 정산 API, 주문/배송 API | 10 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetCompletedRemittanceList, GetOrderInfoList 외 5개 |
| 배송 번호 | @DeliveryNo, DeliveryNo | 상품 API, 정산 API, 주문/배송 API, 클레임 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetMyAuctionSellingItemList, GetReturnDetail 외 4개 |
| Backwoods 배송 여부 | @BackwoodsDeliveryYn, BackwoodsDeliveryYn | 상품 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Faster 배송 여부 | @FasterDeliveryYn, FasterDeliveryYn | 상품 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| Presale 배송 일자 | @PresaleShippingDate, PresaleShippingDate | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| Prod Option 상품 | @ProdOptionItem, ProdOptionItem | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 배송 Amnt | @ShippingAmnt, ShippingAmnt | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionSellingItemList |
| 배송 Condition | @ShippingCondition, ShippingCondition | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 배송 Cost | @ShippingCost, ShippingCost | 상품 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetFinishedItemList, GetSellPlusItemList, GetShippingAddressList |
| 배송 Place | ShippingPlace | 상품 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 배송 Policy | ShippingPolicy | 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPlaceCode, GetShippingPolicyInfoList 외 3개 |
| 배송 Policy 번호 | @ShippingPolicyNo, ShippingPolicyNo | 상품 API, 주문/배송 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetShippingPolicyInfoList, ReviseItem 외 2개 |
| 배송 수수료 | ShippingFee | 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ReviseItemForUsedMarket 외 3개 |
| 배송 수수료 Additional | ShippingFeeAdditional | 상품 API, 주문/배송 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 배송 수수료 Charge 유형 | @ShippingFeeChargeType, ShippingFeeChargeType | 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, GetShippingPolicyInfoList 외 3개 |
| 배송 수수료 유형 | @DeliveryFeeType, DeliveryFeeType, @ShippingFeeType, ShippingFeeType | 상품 API, 주문/배송 API | 8 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, GetSellPlusItemList, GetSendingDetailList 외 3개 |
| 배송 유형 | @ShippingDeliveryType, ShippingDeliveryType, @ShippingType, ShippingType | 상품 API, 주문/배송 API | 9 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ChangeShippingType, FavoriteItemList 외 4개 |
| 여부 Bundle 배송 | IsBundleShipping | 상품 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 여부 배송 Pre Payable | @IsShippingPrePayable, IsShippingPrePayable | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 주문 By 유형 | @OrderByType, OrderByType | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFinishedItemList |
| 주문 Complete 수량 | @OrderCompleteQty, OrderCompleteQty | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 주문 상태 | @OrderStatus, OrderStatus | 상품 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAuctionSellingItemList, GetOrderInfoList |
| 주문 수량 | @OrderQty, OrderQty | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 주문 유형 코드 | @OrderTypeCode, OrderTypeCode | 상품 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetSellPlusItemList |
| 주문 재고 | OrderStock | 상품 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItemMobile, ReviseItemStock, ViewItemStock |
| 판매자 상품번호 | @SellerItemNo, SellerItemNo | 상품 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ConfirmReceivingOrder, DoShippingBundle, DoShippingGeneral |
| 배송 Company | @DeliveryCompany, DeliveryCompany, @ShippingCompany, ShippingCompany | 상품 API, 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo, GetMyAuctionSellingItemList |
| 송장 | @Invoice, Invoice | 상품 API, 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SetCancelNotReceived, ViewItem, ViewItem_old |
| 택배사 코드 | @DeliveryAgency, DeliveryAgency | 상품 API, 주문/배송 API, 클레임 API | 11 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ChangeShippingType, DoExchangeSwitch 외 6개 |
| 반품 주소 | ReturnAddress | 상품 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ViewItem, ViewItem_old |
| 상품 반품 | ItemReturn | 상품 API, 클레임 API | 6 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddItem, AddItemMobile, AddUsedItem, ReviseItem, ViewClosedItem 외 1개 |
| 취소 여부 | @CancelYN, CancelYN | 상품 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ReviseItemVertical, ViewItemVertical |
| Account Numb | @AccountNumb, AccountNumb | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoChangeRemittanceMethod |
| Account 명 | @AccountName, AccountName | 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers, GetMyAccount |
| Account 번호 | @AccountNumber, AccountNumber | 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers, GetMyAccount |
| Cash Emoney | @CashEmoney, CashEmoney | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableEmoney |
| Completed 송금 | CompletedRemittance | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList |
| Do Change 송금 Method 응답 유형 | @DoChangeRemittanceMethodResponseType, DoChangeRemittanceMethodResponseType | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoChangeRemittanceMethod |
| Emoney 유형 | @EmoneyType, EmoneyType | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| Expected 송금 | ExpectedRemittance | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExpectedRemittanceList |
| Minus Emoney | @MinusEmoney, MinusEmoney | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| Money Transfer Method | @MoneyTransferMethod, MoneyTransferMethod | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| My Account | MyAccount | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyAccount |
| Remit Account T | RemitAccountT | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmedAccountNumbers |
| Remit Expected Money | @RemitExpectedMoney, RemitExpectedMoney | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSettlementDetail |
| 구매자 Cash Emoney | @BuyerCashEmoney, BuyerCashEmoney | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableEmoney |
| 구매자 Event Emoney | @BuyerEventEmoney, BuyerEventEmoney | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableEmoney |
| 송금 유형 | @RemittanceType, RemittanceType | 정산 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoChangeRemittanceMethod, GetCompletedRemittanceList |
| 송금금액 | @RemittanceAmount, RemittanceAmount | 정산 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList |
| Group 주문 Seq 번호 | @GroupOrderSeqNo, GroupOrderSeqNo | 정산 API, 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSellerEmoneyDepositList |
| 배송 Cost 유형 | @ShippingCostType, ShippingCostType | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExpectedRemittanceList, GetShippingOrderList |
| 송금 Account 명 | @RemittanceAccountName, RemittanceAccountName | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, DoshippingConnected |
| 송금 Account 번호 | @RemittanceAccountNumber, RemittanceAccountNumber | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, DoshippingConnected |
| 송금 Bank 코드 | @RemittanceBankCode, RemittanceBankCode | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, DoshippingConnected |
| 송금 Method | RemittanceMethod | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, DoshippingConnected |
| 송금 Method 유형 | @RemittanceMethodType, RemittanceMethodType | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral, DoshippingConnected |
| 송금일자 | @RemittanceDate, RemittanceDate | 정산 API, 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetShippingDetailInfoList |
| 주문 배송 Payment 유형 | @OrderShippingPaymentType, OrderShippingPaymentType | 정산 API, 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingTypeBeforeOrder, GetSettlementDetail, GetShippingDetail |
| 배송 Company 명 | @DeliveryCompanyName, DeliveryCompanyName | 정산 API, 주문/배송 API, 클레임 API | 7 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCompletedRemittanceList, GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnDetail, GetReturnList 외 2개 |
| 배송 Finish 일자 | @DeliveryFinishDate, DeliveryFinishDate | 정산 API, 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList, GetCompletedRemittanceList, GetOrderInfoList |
| Bundle Delviery 요청 번호 | @BundleDelvieryRequestNo, BundleDelvieryRequestNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPaidOrderList |
| Bundle 배송 번호 | @BundleDeliveryNo, BundleDeliveryNo | 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, GetSendingDetailList, GetShippingDetail |
| Bundle 배송 여부 | @BundleDeliveryYN, BundleDeliveryYN | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| Bundle 요청 번호 | @BundleRequestNo, BundleRequestNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle |
| Change 배송 유형 응답 유형 | @ChangeShippingTypeResponseType, ChangeShippingTypeResponseType | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, ChangeShippingTypeBeforeOrder |
| Cmp Aid Amnt | CmpAidAmnt | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Delay 사유 Detail | @DelayReasonDetail, DelayReasonDetail | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AlertShippingDelay, DoExchangeDelayNotice |
| Delay 사유 유형 | @DelayReasonType, DelayReasonType | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AlertShippingDelay, DoExchangeDelayNotice |
| Deny Sell 사유 | @DenySellReason, DenySellReason | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DenySell |
| Deny Sell 응답 유형 | @DenySellResponseType, DenySellResponseType | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DenySell |
| Display 주문 | DisplayOrder | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Do Ecoupon 주문 Confirm 응답 유형 | @DoEcouponOrderConfirmResponseType, DoEcouponOrderConfirmResponseType | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoEcouponOrderConfirm |
| Do 교환 Delay Notice 응답 유형 | @DoExchangeDelayNoticeResponseType, DoExchangeDelayNoticeResponseType | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeDelayNotice |
| Do 배송 Connected 응답 유형 | @DoShippingConnectedResponseType, DoShippingConnectedResponseType | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoshippingConnected |
| Do 배송 General 응답 유형 | @DoShippingGeneralResponseType, DoShippingGeneralResponseType | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoShippingBundle, DoShippingGeneral |
| Expected Re 배송 일자 | @ExpectedReDeliveryDate, ExpectedReDeliveryDate | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeDelayNotice |
| Gmkt 주문 번호 | @GmktOrderNo, GmktOrderNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoEcouponOrderConfirm |
| Paid 주문 | PaidOrder | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPaidOrderList |
| Pre Sale 배송 일자 | PreSaleShippingDate | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Sending Detail | SendingDetail | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSendingDetailList |
| trans 수수료 Pre Paid 여부 | transFeePrePaidYN | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 구매자 Choice 배송 명 | @BuyerChoiceShippingName, BuyerChoiceShippingName | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 배송 Biz Error | ShippingBizError | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingPolicyInfoList |
| 배송 Comp List | DeliveryCompList | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryList |
| 배송 Company 코드 | @DeliveryCompanyCode, DeliveryCompanyCode | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoshippingConnected |
| 배송 Confirm 일자 | @DeliveryConfirmDate, DeliveryConfirmDate | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingAddressList |
| 배송 Delay Day | @DeliveryDelayDay, DeliveryDelayDay | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList |
| 배송 Delay Notify 일자 | @DeliveryDelayNotifyDate, DeliveryDelayNotifyDate | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList |
| 배송 Detail Info | ShippingDetailInfo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetailInfoList |
| 배송 Method Classfication | @ShippingMethodClassfication, ShippingMethodClassfication | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType |
| 배송 Place Seq 번호 | shippingPlaceSeqNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 배송 Place T | ShippingPlaceT | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 배송 Policy Seq 번호 | @ShippingPolicySeqNo, ShippingPolicySeqNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 배송 Prepare List 응답 T | DeliveryPrepareListResponseT | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList |
| 배송 Remark | @DeliveryRemark, DeliveryRemark | 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList, GetShippingAddressList |
| 배송 Seqno | @ShippingSeqno, ShippingSeqno | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetailInfoList |
| 배송 Traceable | @DeliveryTraceable, DeliveryTraceable | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingOrderList |
| 배송 일자 | @DeliveryDate, DeliveryDate | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingOrderList |
| 배송 주문 List | ShippingOrderList | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingOrderList |
| 배송 주소 | ShippingAddress | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetShippingAddressList, GetShippingPlaceCode |
| 배송 판매자 Detail | ShippingSellerDetail | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 배송비 유형 | @DeliveryFee, DeliveryFee | 주문/배송 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetDeliveryPrepareList, GetPaidOrderList |
| 여부 Bundle Free | @IsBundleFree, IsBundleFree | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetShippingPlaceCode |
| 여부 Install 주문 | @IsInstallOrder, IsInstallOrder | 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPaidOrderList, GetShippingAddressList, GetShippingDetail |
| 여부 배송 Great 판매자 | IsShippingGreatSeller | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 주문 Canceled | OrderCanceled | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderCanceledList |
| 주문 Confirm 일자 | @OrderConfirmDate, OrderConfirmDate | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| 주문 Info List | OrderInfoList | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| 주문 건수 | OrderCount | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 주문 번호 | orderNo | 주문/배송 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 판매자 주문번호 | @SellerOrderNo, SellerOrderNo | 주문/배송 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ConfirmReceivingOrder, DoShippingBundle, DoShippingGeneral |
| Auction 배송 | AuctionDelivery | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| Fast 환불 여부 | @FastRefundyn, FastRefundyn | 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList, GetReturnDetail, GetReturnList |
| First 배송 수수료 Charge | @FirstDeliveryFeeCharge, FirstDeliveryFeeCharge | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnList |
| Payment 교환 | PaymentExchange | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetShippingDetail |
| Re 배송 Comp 명 | @ReDeliveryCompName, ReDeliveryCompName | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| Re 송장 번호 | @ReInvoiceNo, ReInvoiceNo | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 교환 Delay 사유 | @ExchangeDelayReason, ExchangeDelayReason | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 교환 일자 | @ExchangeDate, ExchangeDate | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList |
| 반품 Approve 일자 | @ReturnApproveDate, ReturnApproveDate | 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturningList, GetShippingDetail |
| 반품 By 판매자 배송 Method | @ReturnBySellerDeliveryMethod, ReturnBySellerDeliveryMethod | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| 반품 배송 Method | @ReturnDeliveryMethod, ReturnDeliveryMethod | 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnList |
| 반품 일자 | @ReturnDate, ReturnDate | 주문/배송 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderInfoList, GetReturnDetail, GetReturnList, GetReturningList |
| 배송 Bill 번호 | @ShippingBillNo, ShippingBillNo | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 배송 Comp 명 | @DeliveryCompName, DeliveryCompName | 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList, SetCancelNotReceived |
| 배송 Etc Method | @ShippingEtcMethod, ShippingEtcMethod | 주문/배송 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| 배송 Etc 택배사 명 | @ShippingEtcAgencyName, ShippingEtcAgencyName | 주문/배송 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| 배송 Method | ShippingMethod | 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| 배송 발송 일자 | @DeliverySendDate, DeliverySendDate | 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList, GetOrderInfoList |
| 배송방법 구분 | @ShippingMethodClassficationType, ShippingMethodClassficationType | 주문/배송 API, 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| 송장번호 | @InvoiceNo, InvoiceNo | 주문/배송 API, 클레임 API | 5 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, DoExchangeSwitch, DoShippingBundle, DoShippingGeneral, GetCancelNotReceivedList |
| 취소 유형 | @CancelType, CancelType | 주문/배송 API, 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderCanceledList |
| 취소 일자 | @CancelDate, CancelDate | 주문/배송 API, 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetOrderCanceledList, GetShippingDetailInfoList |
| 택배사명 | @DeliveryAgencyName, DeliveryAgencyName | 주문/배송 API, 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ChangeShippingType, DoExchangeSwitch, DoShippingBundle, DoShippingGeneral |
| Add 반품 수수료 | @AddReturnFee, AddReturnFee | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnHold, GetReturnAdditionalFee, GetReturnDetail |
| Bid 취소 List | BidCancelList | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBidCancelList |
| Confirm 취소 Approval List 응답 유형 | @ConfirmCancelApprovalListResponseType, ConfirmCancelApprovalListResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: ConfirmCancelApprovalList |
| Do 교환 Switch 응답 유형 | @DoExchangeSwitchResponseType, DoExchangeSwitchResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeSwitch |
| Do 교환 To 반품 응답 유형 | @DoExchangeToReturnResponseType, DoExchangeToReturnResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeToReturn |
| Do 반품 요청 By 판매자 응답 유형 | @DoReturnRequestBySellerResponseType, DoReturnRequestBySellerResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| Selling 취소 | SellingCancel | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoSellingCancel |
| 교환 Arrival Over Day | @ExchangeArrivalOverDay, ExchangeArrivalOverDay | 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환 Arrival 일자 | @ExchangeArrivalDate, ExchangeArrivalDate | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo, GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환 Base | ExchangeBase | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo, GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환 Charge | @ExchangeCharge, ExchangeCharge | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoExchangeSwitch |
| 교환 Detail 사유 | @ExchangeDetailReason, ExchangeDetailReason | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 교환 발송 일자 | @ExchangeSendDate, ExchangeSendDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 교환 상태 | @ExchangeStatus, ExchangeStatus | 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환 수수료 금액 | @ExchangeFeeAmount, ExchangeFeeAmount | 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환 요청 일자 | @ExchangeRequestDate, ExchangeRequestDate | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo, GetExchangeRequestList, GetExchangeRequestListBySearchCondition |
| 교환사유 | @ExchangeReason, ExchangeReason | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 구매자 Pay Cancelable 일자 | @BuyerPayCancelableDate, BuyerPayCancelableDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestDetailInfo |
| 반품 Approval 응답 유형 | @ReturnApprovalResponseType, ReturnApprovalResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnApproval |
| 반품 Arrival 일자 | @ReturnArrivalDate, ReturnArrivalDate | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnDetail, GetReturnList, GetReturningList |
| 반품 By 판매자 사유 코드 | @ReturnBySellerReasonCode, ReturnBySellerReasonCode | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| 반품 Detail 사유 | @ReturnDetailReason, ReturnDetailReason | 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnDetail, GetReturnList |
| 반품 Hold Detail | @ReturnHoldDetail, ReturnHoldDetail | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnHold |
| 반품 Hold 유형 | @ReturnHoldType, ReturnHoldType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnHold |
| 반품 Hold 응답 유형 | @ReturnHoldResponseType, ReturnHoldResponseType | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnHold |
| 반품 Hold 일자 | @ReturnHoldDate, ReturnHoldDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturningList |
| 반품 List | ReturnList | 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnList, GetReturningList |
| 반품 Notice | ReturnNotice | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 반품 Requester | @ReturnRequester, ReturnRequester | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnList |
| 반품 사유 Detail | @ReturnReasonDetail, ReturnReasonDetail | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: DoReturnRequestBySeller |
| 반품 사유 코드 | @ReturnReasonCode, ReturnReasonCode | 클레임 API | 4 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetExchangeRequestList, GetExchangeRequestListBySearchCondition, GetReturnDetail, GetReturnList |
| 반품 상태 | @ReturnStatus, ReturnStatus | 클레임 API | 3 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnDetail, GetReturnList, GetReturningList |
| 반품 수수료 | ReturnFee | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 반품 수수료 Charge | @ReturnFeeCharge, ReturnFeeCharge | 클레임 API | 2 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnDetail, GetReturnList |
| 반품 수수료 금액 | @ReturnFeeAmount, ReturnFeeAmount | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturnList |
| 반품 전화번호 | ReturnTel | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 반품 취소 일자 | @ReturnCancelDate, ReturnCancelDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetReturningList |
| 취소 Approval | CancelApproval | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelApprovalList |
| 취소 Not Received Detail 사유 | @CancelNotReceivedDetailReason, CancelNotReceivedDetailReason | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received List | CancelNotReceivedList | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received Withdraw Exception 여부 | @CancelNotReceivedWithdrawExceptionYN, CancelNotReceivedWithdrawExceptionYN | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received Withdraw Exception 일자 | @CancelNotReceivedWithdrawExceptionDate, CancelNotReceivedWithdrawExceptionDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received Withdraw 일자 | @CancelNotReceivedWithdrawDate, CancelNotReceivedWithdrawDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received 사유 | @CancelNotReceivedReason, CancelNotReceivedReason | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Not Received 요청 | cancelNotReceivedRequest | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 취소 Not Received 일자 | @CancelNotReceivedDate, CancelNotReceivedDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCancelNotReceivedList |
| 취소 Text | cancelText | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 취소 요청 일자 | @CancelRequestDate, CancelRequestDate | 클레임 API | 1 | ✅ 핵심 UDS | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBidCancelList |
| Question 유형 | @QuestionType, QuestionType | CS API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQuestionToHelpDesk |
| Assort Menu 유형 | @AssortMenuType, AssortMenuType | CS API, 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Contact 유형 | @ContactType, ContactType | CS API, 기타 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddEmergencyInformReply, GetEmergencyInformList |
| Query 유형 | @QueryType, QueryType | CS API, 기타 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetSellerQnAList |
| Search Query 유형 | @SearchQueryType, SearchQueryType | CS API, 기타 API | 7 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteDetailBySeqno, BuyerNoteList, GetItemQnAList, GetSellerQnAList, SellerNoteDetailBySeqno 외 2개 |
| Sort 유형 | @SortType, SortType | CS API, 기타 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetSellerQnAList |
| 결과 Description | @ResultDescription, ResultDescription | CS API, 기타 API | 5 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddEmergencyInformReply, AddFeedbackSecond, SellerNoteReply, SendNoteToSeller, SetFeedbackSecond |
| Writer ID 여부 회원 티켓 ID | @WriterIdIsMemberTicketId, WriterIdIsMemberTicketId | CS API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList |
| Additional Service 수수료 유형 | @AdditionalServiceFeeType, AdditionalServiceFeeType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Addtional Condition 여부 | AddtionalConditionYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Adult 여부 | @AdultYN, AdultYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Affiliate 유형 | @AffiliateType, AffiliateType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SetBuyingDecisionAndFeedbackFirst |
| Broadcast Equipment 여부 | BroadcastEquipmentYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Car 유형 | @CarType, CarType | 기타 API | 6 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Cert Biz 유형 | CertBizType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Cert Group 유형 | CertGroupType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification Target 코드 | CertificationTargetCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification 유형 | CertificationType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Channel 코드 | @ChannelCode, ChannelCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SetOKCashBagSave |
| Coupon Select 유형 | @CouponSelectType, CouponSelectType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Default 여부 | @DefaultIs, DefaultIs | 기타 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Duty Included 여부 | @DutyIncludedYn, DutyIncludedYn | 기타 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Element 유형 | @ElementType, ElementType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Extra Mark 여부 | @ExtraMarkIs, ExtraMarkIs | 기타 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddOfficialNotice, ViewOfficialNotice |
| Exts Limit 여부 | ExtsLimitYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Feedback Exception 유형 | @FeedbackExceptionType, FeedbackExceptionType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackExceptionType |
| Feedback 유형 | @FeedbackType, FeedbackType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| Food Import Cert 여부 | FoodImportCertIs | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Get Bidding History 응답 T | GetBiddingHistoryResponseT | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBiddingHistory |
| Image 유형 | ImageType | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoRanking, GetSohoShopSearchResults |
| Input 유형 | InputType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Ins 유형 | InsType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Junk 여부 | @JunkYN, JunkYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyFeedbackList |
| Landing Target 여부 | @LandingTargetYn, LandingTargetYn | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Listing Asrt 코드 | ListingAsrtCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Listing Title 유형 | ListingTitleType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Lodge 유형 | @LodgeType, LodgeType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Lodge 유형 Idx | @LodgeTypeIdx, LodgeTypeIdx | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| OKCash Bag Save Channel 코드 | @OKCashBagSaveChannelCode, OKCashBagSaveChannelCode | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Origin 코드 | @OriginCode, OriginCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetNationCode |
| Pagination 사용 여부 | PaginationUseYn | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsBest100 |
| Preview 여부 | @PreviewYN, PreviewYN | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Preview 유형 | @PreviewType, PreviewType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Preview 코드 | @PreviewCode, PreviewCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Recommend 유형 | @RecommendType, RecommendType | 기타 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, GetMyFeedbackList, SetFeedbackSecond |
| Revise 유형 | ReviseType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Safe Auth 유형 | SafeAuthType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Search 요청 | SearchRequest | 기타 API | 6 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Series 코드 | @SeriesCode, SeriesCode | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Sex 유형 | @SexType, SexType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Soho Style 코드 | @SohoStyleCode, SohoStyleCode | 기타 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50 |
| Style 유형 | @StyleType, StyleType | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Tab 유형 | @TabType, TabType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Template 유형 | @TemplateType, TemplateType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Trans 유형 | @TransType, TransType | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetBiddingHistory, GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Up Down 유형 | @UpDownType, UpDownType | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoHotKeyword |
| 여부 Ad Deliberation | IsAdDeliberation | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 여부 Auto Decision | @IsAutoDecision, IsAutoDecision | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Award | @IsAward, IsAward | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: Bid |
| 여부 Base Benefit | @IsBaseBenefit, IsBaseBenefit | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Bonus | @IsBonus, IsBonus | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit |
| 여부 Charity Shopping | @IsCharityShopping, IsCharityShopping | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Charity Shopping Point | @IsCharityShoppingPoint, IsCharityShoppingPoint | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Daum Reserve | @IsDaumReserve, IsDaumReserve | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Daum Site | @IsDaumSite, IsDaumSite | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Decision | @IsDecision, IsDecision | 기타 API | 5 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember, SetBuyingDecisionAndFeedbackFirst |
| 여부 Decision Complete | @IsDecisionComplete, IsDecisionComplete | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Double Promotion | @IsDoublePromotion, IsDoublePromotion | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Feedback | @IsFeedback, IsFeedback | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Feedback First | @IsFeedbackFirst, IsFeedbackFirst | 기타 API | 5 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember, SetBuyingDecisionAndFeedbackFirst |
| 여부 Feedback First Pass | @IsFeedbackFirstPass, IsFeedbackFirstPass | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Food Cert 여부 | IsFoodCertIs | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 여부 Free Gift | @IsFreeGift, IsFreeGift | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: PurchaseBenefit |
| 여부 Health Food | IsHealthFood | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 여부 Home Double Promotion | @IsHomeDoublePromotion, IsHomeDoublePromotion | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Mart On | @IsMartOn, IsMartOn | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| 여부 Medical Instrument | IsMedicalInstrument | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 여부 Multiple | IsMultiple | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| 여부 OKCash Bag Save | @IsOKCashBagSave, IsOKCashBagSave | 기타 API | 4 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| 여부 Shared Sns | @IsSharedSns, IsSharedSns | 기타 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, SetFeedbackSecond |
| 여부 Soho Sale And Coupon | IsSohoSaleAndCoupon | 기타 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoShopSearchResults |
| 요청 명 | @RequestName, RequestName | 기타 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCartDetail |
| Area 명 | @AreaName, AreaName | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Blog Main Image | @BlogMainImage, BlogMainImage | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Creation 시간 | @CreationTime, CreationTime | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Image Path | @ImagePath, ImagePath | 기타 API, 인증 API | 8 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetBiddingHistory, GetSearchResultsTicket, GetSohoBest50, GetSohoLookbook, GetSohoShopBest50 외 3개 |
| Jenre | @Jenre, Jenre | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Jenre 코드 | @JenreCode, JenreCode | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance ID | @PerformanceId, PerformanceId | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance Notice | @PerformanceNotice, PerformanceNotice | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance Org | @PerformanceOrg, PerformanceOrg | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance Sub 명 | @PerformanceSubName, PerformanceSubName | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Performance 명 | @PerformanceName, PerformanceName | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| req | req | 기타 API, 인증 API | 3 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, SecurityService, ShoppingService; 사용 operation: |
| Search Results | SearchResults | 기타 API, 인증 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge, GetSearchResultsTicket |
| Sort | @Sort, Sort | 기타 API, 인증 API | 2 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge, GetSearchResultsTicket |
| Theater ID | @TheaterId, TheaterId | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| Theater 명 | @TheaterName, TheaterName | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| 시간 Info | @TimeInfo, TimeInfo | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| 할인 Rate | @DiscountRate, DiscountRate | 기타 API, 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsTicket |
| App Password | @AppPassword, AppPassword | 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: SecurityService; 사용 operation: RequestApplicationTicket |
| 개발자 ID | @DevID, DevID | 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: SecurityService; 사용 operation: RequestApplicationTicket |
| 암호화 Auth Info | encryptedAuthInfo | 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: SecurityService; 사용 operation: |
| 애플리케이션 ID | @AppID, AppID | 인증 API | 1 | 🟡 후보 | Auction legacy SOAP Open API 필드. 서비스: SecurityService; 사용 operation: RequestApplicationTicket |
| Emergency Inform List | EmergencyInformList | CS API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Inform 번호 | @InformNo, InformNo | CS API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddEmergencyInformReply, GetEmergencyInformList |
| My Question List | MyQuestionList | CS API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQuestionToHelpDesk |
| Qn A | QnA | CS API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyQnAList |
| Qn AList | QnAList | CS API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAListHistory, GetMyQnAList, GetSellerQnAList |
| Question 번호 | @QuestionNo, QuestionNo | CS API | 8 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddQnAReply, AddQnAReply_origin, GetItemQnAList, GetItemQnAListHistory, GetMyQnAList 외 3개 |
| Reply List | ReplyList | CS API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList |
| Total Question 건수 | @TotalQuestionCount, TotalQuestionCount | CS API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetSellerQnAList |
| VIPQn AList T | VIPQnAListT | CS API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList |
| Answer 번호 | @AnswerNo, AnswerNo | CS API, 기타 API | 5 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddQnAReply, AddQnAReply_origin, GetItemQnAListHistory, GetMyQuestionToHelpDesk, GetSellerQnAList |
| Answered State | @AnsweredState, AnsweredState | CS API, 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetSellerQnAList |
| Answers | Answers | CS API, 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetMyQuestionToHelpDesk, GetSellerQnAList |
| Content | @Content, Content | CS API, 기타 API | 13 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddEmergencyInformReply, AddQnAReply, AddQnAReply_origin, BuyerNoteDetailBySeqno, BuyerNoteList 외 8개 |
| Contents | @Contents, Contents | CS API, 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, GetFeedbackSecondForTest, GetISBNSearchResults, GetMyFeedbackList, GetMyQuestionToHelpDesk 외 2개 |
| Duration | Duration | CS API, 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList, GetSellerQnAList |
| Listing Img URL | @ListingImgUrl, ListingImgUrl | CS API, 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAListHistory, GetSellerQnAList |
| Nick 명 | @NickName, NickName | CS API, 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: FavoriteStoreList, GetItemQnAListHistory, GetSellerQnAList, GetSohoRanking |
| Open To Public State | @OpenToPublicState, OpenToPublicState | CS API, 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList |
| Regdate | @Regdate, Regdate | CS API, 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetSellerQnAList |
| Reply Note | ReplyNote | CS API, 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteDetailBySeqno, SellerNoteDetailBySeqno |
| Reply 번호 | @ReplyNo, ReplyNo | CS API, 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BuyerNoteDetailBySeqno, SellerNoteDetailBySeqno |
| Search Filter Answered State | @SearchFilterAnsweredState, SearchFilterAnsweredState | CS API, 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList |
| Staff 명 | @StaffName, StaffName | CS API, 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetEmergencyInformList, GetSohoShopHomeNewArrival, GetSohoShopStyleTrendList |
| Title | @Title, Title | CS API, 기타 API | 16 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, AddQnAReply, AddQnAReply_origin, BuyerNoteDetailBySeqno, BuyerNoteList 외 11개 |
| VIPImg URL | @VIPImgUrl, VIPImgUrl | CS API, 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAListHistory, GetSellerQnAList |
| Writer ID | @WriterID, WriterID | CS API, 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetItemQnAList, GetItemQnAListHistory, GetSellerQnAList, RemoveQnAList |
| Actor | Actor | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Ad Deliberation 번호 | AdDeliberationNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Ad Successful Bid | AdSuccessfulBid | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid |
| Add Point | @AddPoint, AddPoint | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| Add 할인 Amnt | AddDiscountAmnt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Address1 | @Address1, Address1 | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Address2 | @Address2, Address2 | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Age | Age | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsBest100 |
| Age Limit | AgeLimit | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Aid Amnt | AidAmnt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Allow Shortage | @AllowShortage, AllowShortage | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BidList |
| Apply Period | ApplyPeriod | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Asiana Mileage | @AsianaMileage, AsianaMileage | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Auction Image Path | AuctionImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Auction Image Path Big | AuctionImagePathBig | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Auction Point | @AuctionPoint, AuctionPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Authentication 번호 | AuthenticationNO | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Author | @Author, Author | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Banner HTML | @BannerHTML, BannerHTML | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Banner Image Path | @BannerImagePath, BannerImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopHomeNewArrival |
| Basic Point | @BasicPoint, BasicPoint | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| bid Seq 번호 | bidSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| bidder ID | bidderID | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Biz Plus Point | @BizPlusPoint, BizPlusPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Book Cash | @BookCash, BookCash | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Buy Admin Staff ID | BuyAdminStaffId | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Card Numb | @CardNumb, CardNumb | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SetOKCashBagSave |
| Cart Detail | CartDetail | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart, ViewCartDetail |
| Cart Detail Text | CartDetailText | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCartDetail |
| Cart Detail 번호 | @CartDetailNo, CartDetailNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCartDetail |
| cart Nos | cartNos | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Cart Text 번호 | @CartTextNo, CartTextNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCartDetail |
| Cart View T | CartViewT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| cart 번호 | cartNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Cart 번호 T | CartNoT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: RemoveCartsByNos |
| Categories | Categories | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetCategories |
| Certification Group 번호 | CertificationGroupNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification Img URL | CertificationImgUrl | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification Office 명 | CertificationOfficeName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Certification 번호 | CertificationNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Chart Detail | @ChartDetail, ChartDetail | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Chart Detail Age | ChartDetailAge | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Chart Detail Region | ChartDetailRegion | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Chart Detail Sex | ChartDetailSex | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Chart Detail 시간 Span | ChartDetailTimeSpan | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Chart Kind | @ChartKind, ChartKind | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Check Image Path | @CheckImagePath, CheckImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Child Product Safe Cert Detail Info List | ChildProductSafeCertDetailInfoList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Color | @Color, Color | 기타 API | 9 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst 외 4개 |
| Color Index | @ColorIndex, ColorIndex | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: Bid |
| Color Seqno | @ColorSeqno, ColorSeqno | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Color 명 | @ColorName, ColorName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Commercial | @Commercial, Commercial | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Confirming Receipt | ConfirmingReceipt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmingReceiptList |
| Consulting Seq | ConsultingSeq | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Cost | Cost | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Coupon Period | CouponPeriod | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Coupon Point | @CouponPoint, CouponPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Coupon 번호 | @CouponNo, CouponNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAvailableSellerCouponList |
| Daum Point | @DaumPoint, DaumPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Daum Reward Point | @DaumRewardPoint, DaumRewardPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Deliberation 번호 | DeliberationNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Detail | Detail | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Detail Level | DetailLevel | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Detail View | DetailView | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Display Column | DisplayColumn | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Double Comment After Decision | @DoubleCommentAfterDecision, DoubleCommentAfterDecision | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Double Comment Before Decision | @DoubleCommentBeforeDecision, DoubleCommentBeforeDecision | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Editor | @Editor, Editor | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Element Seq 번호 | @ElementSeqNo, ElementSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| End 시간 From | EndTimeFrom | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| End 시간 To | EndTimeTo | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Exclude Keyword | ExcludeKeyword | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsMartOn 외 1개 |
| Ext Media Filter | ExtMediaFilter | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Exts Days | ExtsDays | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Exts Expire Dt | ExtsExpireDt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Favorite Auction Store Group | FavoriteAuctionStoreGroup | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreGroupList |
| Favorite Card | @FavoriteCard, FavoriteCard | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| Favorite Card Info | @FavoriteCardInfo, FavoriteCardInfo | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Favorite Group | FavoriteGroup | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteGroupList |
| Feedback Second Remain List | FeedbackSecondRemainList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackSecondRemainList |
| First Certification 번호 | FirstCertificationNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| First Step Max 건수 | FirstStepMaxCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Free Experience Coupon | @FreeExperienceCoupon, FreeExperienceCoupon | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Front Tag Value | FrontTagValue | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Fuel | @Fuel, Fuel | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Gender | Gender | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsBest100 |
| Gift Mileage | @GiftMileage, GiftMileage | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Gift Packing 수수료 | GiftPackingFee | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Group 명 | @GroupName, GroupName | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: AddGroupToFavoriteGroupList, DoFavoriteStoreGroupAdd, FavoriteGroupList, FavoriteStoreGroupList, FavoriteStoreList 외 2개 |
| Guide Text | @GuideText, GuideText | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetOfficialNoticeInfo |
| Happy Point | @HappyPoint, HappyPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Has Preview | HasPreview | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Hotel Grade | @HotelGrade, HotelGrade | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Html | @Html, Html | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Images | Images | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Img Path | @ImgPath, ImgPath | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst, GetFeedbackSecondRemainList, GetMyFeedbackList |
| Info A | InfoA | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Info AD | InfoAD | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Info B | InfoB | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Info C | InfoC | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Info EM | InfoEM | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Info HT | InfoHT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Ins ID | InsID | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Inspected | @Inspected, Inspected | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Inst Pricipal | InstPricipal | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Installment 건수 | InstallmentCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Integrate Safe Cert Detail List | IntegrateSafeCertDetailList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Integrate Safe Cert Group List | IntegrateSafeCertGroupList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Is3 PL | @Is3PL, Is3PL | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: ViewCart |
| Isbn | Isbn | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| ISBNCode | @ISBNCode, ISBNCode | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Join Apln URL | JoinAplnURL | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Join Product Cnt | JoinProductCnt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| KDSeq 번호 | @KDSeqNo, KDSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoHotKeyword |
| Key Word Landing URL | @KeyWordLandingUrl, KeyWordLandingUrl | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoHotKeyword |
| keyword | keyword | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Keyword Chart T | KeywordChartT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Level | @Level, Level | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetCategories, GetSearchResultsMartOn, GetSearchResultsMartOnBest100 |
| listing Seq 번호 | listingSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Listing Seq 번호 | ListingSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Listing Sort Seq | ListingSortSeq | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Listing Title | ListingTitle | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Location | @Location, Location | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 2개 |
| Location Explain | LocationExplain | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Location To | LocationTo | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Lookup Condition | @LookupCondition, LookupCondition | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAdSuccessfulBid |
| Main Image | @MainImage, MainImage | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Main Image Path | MainImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Maker | Maker | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Maker Aid Amnt | MakerAidAmnt | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Mandatory Safety Sign | MandatorySafetySign | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Map Image Path | MapImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| max 건수 | maxCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Max 할인 Rate | MaxDiscountRate | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| md ID | mdID | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| MDID | @MDID, MDID | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionMasterInfo |
| MHtml | @MHtml, MHtml | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionMasterInfo |
| Mileage | Mileage | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Mileage From | @MileageFrom, MileageFrom | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Mileage To | @MileageTo, MileageTo | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| MImage | @MImage, MImage | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionMasterInfo |
| Min 할인 Rate | MinDiscountRate | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Model | Model | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Model ID | ModelID | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Month | Month | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| MType | @MType, MType | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionMasterInfo |
| Music Title | MusicTitle | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| My Favorite Store List | MyFavoriteStoreList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreList |
| My Feedback List | MyFeedbackList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMyFeedbackList |
| Nation | Nation | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Nation List T | NationListT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetNationCode |
| OKCashbag | @OKCashbag, OKCashbag | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Option | Option | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Option Flag | OptionFlag | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Option Set | OptionSet | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Option 번호 | OptionNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Org Title | @OrgTitle, OrgTitle | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Origin 명 | @OriginName, OriginName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetNationCode |
| Origin 명 Detail | @OriginNameDetail, OriginNameDetail | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetNationCode |
| Original Title | OriginalTitle | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Over Image Path | @OverImagePath, OverImagePath | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| pageindex | pageindex | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Pages | @Pages, Pages | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Painter | @Painter, Painter | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Password | Password | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetAuthenticate |
| Payment | Payment | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Payment 시간 Limit | @PaymentTimeLimit, PaymentTimeLimit | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetConfirmingReceiptList |
| Plantation 명 | PlantationName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| President | President | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| President Info NA | PresidentInfoNA | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Principal | Principal | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Prod Option Seq 번호 | @ProdOptionSeqNo, ProdOptionSeqNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: Bid |
| Producer 명 | ProducerName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Product Filter | ProductFilter | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Product 명 | ProductName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Promotion Sub Title T | PromotionSubTitleT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetPromotionSubTitleInfo |
| Publisher | @Publisher, Publisher | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Query | Query | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Ranking | @Ranking, Ranking | 기타 API | 5 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter, GetSohoBest50, GetSohoHotKeyword, GetSohoRanking, GetSohoShopBest50 |
| Ranking Range | @RankingRange, RankingRange | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Ranking Rate | @RankingRate, RankingRate | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoHotKeyword |
| Ranking State | @RankingState, RankingState | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchTrendCenter |
| Rate | Rate | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Ready Duration Day | @ReadyDurationDay, ReadyDurationDay | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Receive Note | ReceiveNote | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: SellerNoteDetailBySeqno, SellerNoteList |
| Recommend Type2 | @RecommendType2, RecommendType2 | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, SetFeedbackSecond |
| Register Office 명 | RegisterOfficeName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Registration Office 명 | RegistrationOfficeName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Registration 번호 | RegistrationNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| requests | requests | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Review | @Review, Review | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Review Master Point | @ReviewMasterPoint, ReviewMasterPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| row 건수 | rowCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| RT | RT | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: AddFeedbackSecond, SetFeedbackSecond |
| Satisfaction | @Satisfaction, Satisfaction | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst |
| Search ISBNResult Array | SearchISBNResultArray | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Second Step Max 건수 | SecondStepMaxCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Selected | @Selected, Selected | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Seq No2 | @SeqNo2, SeqNo2 | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: TestDTC1, TestDTC2, TestDTC3 |
| Series Title | @SeriesTitle, SeriesTitle | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Service Area | ServiceArea | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Shape | Shape | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetMobileSohoBest100, GetMobileSohoSrpLp, GetSohoShopSearchResults |
| Shape Description | @ShapeDescription, ShapeDescription | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Shape Seqno | @ShapeSeqno, ShapeSeqno | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Shape 명 | @ShapeName, ShapeName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| sku ID | skuId | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Smile Pay Point | @SmilePayPoint, SmilePayPoint | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetBuyingDecisionInfo, GetBuyingDecisionInfoNonMember, GetBuyingDecisionSmartInfo, GetBuyingDecisionSmartInfoNonMember |
| Soho Color | SohoColor | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Soho Home New Arrival T | SohoHomeNewArrivalT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopHomeNewArrival |
| Soho Home Style Trend T | SohoHomeStyleTrendT | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleTrendList |
| Soho New Arriaval | @SohoNewArriaval, SohoNewArriaval | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50 |
| Soho Shape | SohoShape | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Soho Shop Description | @SohoShopDescription, SohoShopDescription | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Soho Shop Look Book Intro Element List | SohoShopLookBookIntroElementList | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Soho Shop 명 | @SohoShopName, SohoShopName | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoLookbook |
| Soho Style | @SohoStyle, SohoStyle | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Sold Out | SoldOut | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Spec | Spec | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Start 시간 From | StartTimeFrom | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Start 시간 To | StartTimeTo | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Store Class | StoreClass | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Store Filter | StoreFilter | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Store ID | @StoreID, StoreID | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Store Pickup Area | StorePickupArea | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Store URL | StoreUrl | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Store 건수 | @StoreCount, StoreCount | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: FavoriteStoreGroupList, FavoriteStoreList |
| Store 명 | @StoreName, StoreName | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Street | Street | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: |
| Style | Style | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Style Description | @StyleDescription, StyleDescription | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Style Finder | StyleFinder | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Style Seqno | @StyleSeqno, StyleSeqno | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| Style 명 | @StyleName, StyleName | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoBest50, GetSohoShopBest50, GetSohoShopBest50Tab, GetSohoShopStyleFinder |
| sub Favorite Auction Model | subFavoriteAuctionModel | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Subsidy | Subsidy | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Tab 번호 | @TabNo, TabNo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopHomeNewArrival |
| Tip | @Tip, Tip | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResultsLodge |
| Tool Tip Image Path | @ToolTipImagePath, ToolTipImagePath | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSohoShopStyleFinder |
| Total Bid 건수 | @TotalBidCount, TotalBidCount | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: BidList |
| Total Only | TotalOnly | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Trans Close 시간 | @TransCloseTime, TransCloseTime | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Trans Policy | TransPolicy | 기타 API | 2 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest |
| Trans Policy 명 | @TransPolicyName, TransPolicyName | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: GetTransPolicyList, RedisTest, ReviseTransPolicy |
| Translator | @Translator, Translator | 기타 API | 7 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService, ShoppingService; 사용 operation: GetISBNSearchResults, GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst 외 2개 |
| Transmission | @Transmission, Transmission | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Upd ID | UpdID | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: |
| Used | Used | 기타 API | 4 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst |
| Value2 | @Value2, Value2 | 기타 API | 3 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: ShoppingService; 사용 operation: TestDTC1, TestDTC2, TestDTC3 |
| Warranty | @Warranty, Warranty | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Weight | @Weight, Weight | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Writer | @Writer, Writer | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetFeedbackFirst |
| Writer Info | @WriterInfo, WriterInfo | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetISBNSearchResults |
| Year | Year | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| Year From | @YearFrom, YearFrom | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Year To | @YearTo, YearTo | 기타 API | 6 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: GetSearchResults, GetSearchResultsExtMedia, GetSearchResultsExtMediaSortByPremiumFirst, GetSearchResultsSortByPremiumFirst, GetSearchResultsUsedMarket 외 1개 |
| Zip | Zip | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 명 Value | NameValue | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 크기 | Size | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: |
| 크기 Index | @SizeIndex, SizeIndex | 기타 API | 1 | ⚪ 선택 / 낮음 | Auction legacy SOAP Open API 필드. 서비스: AuctionService; 사용 operation: Bid |
