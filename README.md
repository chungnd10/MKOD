Bai tap theme MKOD

1. Header
2. Footer
3. HomePage
4. Listing product
5. Product detail
-----------------------------------------------------
1. Header
    - Tạo mới block:
        Block Promotion:<br/>
            - Title: Header Promotion Block<br/>
            - Identifier: header-promotion-block<br/>
            - All store views<br/>
            - Contents:
            
            <div class="header-promotion">
                <div class="promotion-item">FREE DELIVERY IN UK</div>
                <div class="promotion-item">30% OFF IN ALL PRODUCTS</div>
                <div class="promotion-item">30% STUDENT DISCOUNTS</div>
            </div>
            
        Block Account-Minicart<br/>
            - Title: Account-Minicart <br/>
            - Identifier: account-minicart<br/>
            - All store views<br/>
            - Contents:
            
            <a class="mini-conntact" href="{{store url=""}}contact"><img src="{{media url="wysiwyg/contact.png"}}" alt="">&nbsp;&nbsp;contact</a>
            <a class="mini-account" href="{{store url=""}}customer/account"><img src="{{media url="wysiwyg/account.png"}}" alt="">&nbsp;&nbsp;account</a>
            
        _(*2 Ảnh lấy trong thư mục AHT/MKOD/web/images/)_

2. Footer
    2.1. Tạo block MKOD Footer FEATURES :

        + title : MKOD Footer FEATURES
        + id    : mkod-footer-features
        + content:

            <div>
                <h2 class="footer-header">FEATURES</h2>
                <ul class="footer links footer-content">
                    <li class="nav item"><a href="{{store url="fasq"}}">fasq</a></li>
                    <li class="nav item"><a href="{{store url="about-us"}}">about us</a></li>
                    <li class="nav item"><a href="{{store url="privacy-policy"}}">privacy policy</a></li>
                    <li class="nav item"><a href="{{store url="delivery"}}">delivery</a></li>
                </ul>
            </div>

    2.2. Tạo block mkod footer customer service 1:

        + title : mkod footer customer service
        + id    : mkod-footer-customer-service
        + content:

            <div>
            <h2 class="footer-header">customer service</h2>
            <div class="footer-content">
            <p>customerservice@mykindofdress.com</p>
            <p>Unit 1, Fashion city, Balymount, D24</p>
            </div>
            </div>

    2.3. Tạo block MKOD footer copyright :

        + title : MKOD footer copyright
        + id    : mkod-footer-copyright
        + content:

            <div class="mkod-copyright">
            <h2 class="footer-header">YOUR ORDER</h2>
            <p class="footer-content">Copyright © 2018 - 2019 MyKindofDress</p>
            </div>

3. HomePage:
	
    3.1.Banner:

	    - Tạo block:
            + Title: banner.
            + Id: banner.
            + Content: lấy ảnh bannerx2.png trong web/images:
                <div class="banner">
                    <div class="banner__img">
                        <a href="#"><img src="{{media url="wysiwyg/bannerx2.png"}}" alt=""></a>
                    </div>
                    <div class="banner__content">
                        <div class="slogan">
                            <p>step into summer</p>
                        </div>
                        <div class="button">
                            <a href="#">shop now</a>
                        </div>
                    </div>
                </div>

	3.2. Banner:

		- Tạo block:

			+Title: featured products.
			+Id: featured-products.
			+Content: lấy ảnh theo tên trong thẻ img trong web/images:

        <div class="featured-products">
            <div class="featured-products__title">
                <h3>featured products</h3>
            </div>
            <div class="slide1 owl-carousel owl-theme">
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/left.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>summer shades</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/50"}}</div>
                    </div>
                </div>
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/center.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>occasion</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/51"}}</div>
                    </div>
                </div>
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/right.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>fashion</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/52"}}</div>
                    </div>
                </div>
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/left.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>summer shades</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/50"}}</div>
                    </div>
                </div>
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/center.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>occasion</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/51"}}</div>
                    </div>
                </div>
                <div class="item">
                    <div class="img-cate"><img src="{{media url=" wysiwyg/right.png "}}" alt=""></div>
                    <div class="item__content">
                        <div class="cate-name">
                            <h3>fashion</h3>
                        </div>
                        <div class="cate-link">{{widget type="Magento\Catalog\Block\Category\Widget\Link" template="Magento_Catalog::category/widget/link/link_block.phtml" id_path="category/52"}}</div>
                    </div>
                </div>
            </div>
        </div>

	3.3. Thêm widget vào Homepage:
    
        -Vào Content->Pages->Homepage > Tạo mới wwifget trong phần content
		-Type widget: Catalog product list.
		-Sau khi add sẽ thấy như dưới:
			<div>
                <p>{{widget type="Magento\CatalogWidget\Block\Product\ProductsList" title="trending now" show_pager="0" products_count="10" template="Magento_CatalogWidget::product/widget/content/grid.phtml" conditions_encoded="^[`1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Combine`,`aggregator`:`all`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Product`,`attribute`:`category_ids`,`operator`:`==`,`value`:`43`^]^]"}}</p>
            </div>
4. Listing product:

    4.1. tắt filter theo attribute section in layered navigation

            - Vào Admin Chọn Catalog > Categories
            - Chọn danh mục hiển thị sản phẩm 
            - Phần Display Settings > Anchor chọn No.
            - Phần content > thêm mô tả danh mục
            - Phần Design > Layout > chọn 1 column
       
5. Product detail

    5.1 Tạo attribute cho product
    
        5.1.1 Delivery
            - Defaul label: Delivery
            - Type: Text Area
            - Values Required: Yes
        5.1.1 Returns
            - Defaul label: Returns
            - Type: Text Area
            - Values Required: Yes
    5.2 Tạo attribute set
    
        - Name: Dress
        - Based On: Default
        
        Vào mục cài đặt store > attribute set > chọn attribute dress.
        Kéo 2 attribute vừa tạo từ Unassigned Attributes sang Groups > Products Details
        Nhấn Save
        
    5.3 Tạo block
    
        5.3.1 Block info-shipping
            - Title: Info shipping
            - identifier: info-shipping
            - all store view
            - content: "| Usually dispatched within 2 working days"
        5.3.2 Block Social Network
            - Title: Social Network
            - identifier: social-network
            - all store view
            - content:
                <ul>
                    <li><a href="#"><i class="fab fa-facebook-square" aria-hidden="true"></i>&nbsp;Share</a></li>
                    <li><a href="#"><i class="fab fa-twitter-square" aria-hidden="true"></i>&nbsp;Tweet</a></li>
                    <li><a href="#"><i class="fab fa-pinterest" aria-hidden="true"></i>&nbsp;Pin it</a></li>
                </ul>
        5.3.2 Block size guide
            - Title: Size guide
            - identifier: size-guide
            - all store view
            - content:
                <div class="product-size-guide">
                    <a id="click-me">size guide</a>
                </div>
                <div id="popup-modal" style="display: none;">
                    <img src="{{media url="wysiwyg/size-guide.png"}}" alt="">
                </div>
                
            _*(images lấy trong thư mục AHT/MKOD/web/images)
            
    5.4 Tạo sản phẩm
    
        - Tạo 6 sản phẩm Configure:
            - Thuộc Attribute Dress vừa tạo
            - Cấu hình cho sản phẩm có từ 4-7 size 

_*Lưu ý: ảnh dùng cho sản phẩm có kích cỡ 800*1200px_ <br>
_*Nếu ảnh không hiển thị đúng kích thước thì chạy lệnh bin/magento catalog:images:resize_ 
