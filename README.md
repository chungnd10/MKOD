Bai tap tao theme MKOD

1. Header
2. Footer
-----------------------------------------------------
1. Header
    - Tạo mới block:
        1.Block Promotion:<br/>
            - Title: Header Promotion Block<br/>
            - Identifier: header-promotion-block<br/>
            - All store views<br/>
            - Contents:
            
            <div class="header-promotion">
                <div class="promotion-item">FREE DELIVERY IN UK</div>
                <div class="promotion-item">30% OFF IN ALL PRODUCTS</div>
                <div class="promotion-item">30% STUDENT DISCOUNTS</div>
            </div>
            
        2.Block Header Contact<br/>
            - Title: Header Contact <br/>
            - Identifier: header-contact<br/>
            - All store views<br/>
            - Contents:
            
            <a class="mini-conntact" href="{{store url=""}}contact"><img src="{{media url="wysiwyg/contact.png"}}" alt="">&nbsp;&nbsp;contact</a>
            
        _(*2 Ảnh lấy trong thư mục AHT/MKOD/web/images/)_

2. Footer
3. Phần HomePage:
	3.1.Banner:
	- Tạo block:
		+Title: banner.
		+Id: banner.
		+Content: lấy ảnh bannerx2.png trong web/images

			<div class="banner">
				<div class="banner__img"><a href="#"><img src="{{media url="wysiwyg/bannerx2.png"}}" alt=""></a></div>
				<div class="banner__content">
					<div class="slogan">
						<p>step into summer</p>
					</div>
					<div class="button"><a href="#">shop now</a></div>
				</div>
			</div>

	3.2.Banner:
		- Tạo block:
			+Title: featured products.
			+Id: featured-products.
			+Content: lấy ảnh theo tên trong thẻ img trong web/images

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
		-Type widget: Catalog product list.
		-Sau khi add sẽ thấy như dưới (lưu ý thay đổi file template grid.phtml thành file ta thay đổi, như bên dưới là test.phtml):
			<p>{{widget type="Magento\CatalogWidget\Block\Product\ProductsList" title="trending now" show_pager="0" products_count="10" template="Magento_CatalogWidget::product/widget/content/test.phtml" conditions_encoded="^[`1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Combine`,`aggregator`:`all`,`value`:`1`,`new_child`:``^],`1--1`:^[`type`:`Magento||CatalogWidget||Model||Rule||Condition||Product`,`attribute`:`category_ids`,`operator`:`==`,`value`:`43`^]^]"}}</p>
    
