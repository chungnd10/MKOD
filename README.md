Bai tap theme MKOD

1. Header
2. Footer
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
<<<<<<< HEAD

3. Phần HomePage:<br/>
	3.1.Banner:<br/>
	- Tạo block:<br/>
		+Title: banner.<br/>
		+Id: banner.<br/>
		+Content: lấy ảnh bannerx2.png trong web/images:<br/>
        
            <div class="banner">
                <div class="banner__img"><a href="#"><img src="{{media url="wysiwyg/bannerx2.png"}}" alt=""></a></div>
                <div class="banner__content">
                    <div class="slogan">
                        <p>step into summer</p>
                    </div>
                    <div class="button"><a href="#">shop now</a></div>
                </div>
            </div>

	3.2.Banner:<br/>
		- Tạo block:<br/>
			+Title: featured products.<br/>
			+Id: featured-products.<br/>
			+Content: lấy ảnh theo tên trong thẻ img trong web/images:<br/>

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

	3.3. Thêm widget vào Homepage:<br/>
		-Type widget: Catalog product list.<br/>
		-Sau khi add sẽ thấy như dưới (lưu ý thay đổi file template grid.phtml thành file ta thay đổi, như bên dưới là test.phtml):<br/>
			<div>
                <p>{{widget type="Magento\CatalogWidget\Block\Product\ProductsList" title="trending now" show_pager="0" products_count="10" template="Magento_CatalogWidget::product/widget/content/test.phtml" conditions_encoded="^[`1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Combine`,`aggregator`:`all`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Product`,`attribute`:`category_ids`,`operator`:`==`,`value`:`43`^]^]"}}</p>
            </div>
    
