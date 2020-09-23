// even pada saat link diklik

// sintak dibawah ini artinta jequery ($) tolong carikan sebuah elemen yang namanya class page-scroll
$('.page-scroll').on('click', function(e) {
	// bisa masukan console.log('ok'); di sini untuk mencoba apakah evenya jalan di link dengan class page-scroll. dan lihat dengan inspek elemen console
	

	// ambil isi href atau tujuan, attr adalah atribut, this adalah elemen a nya
	var tujuan = $(this).attr('href');
	// tangkap elemen ybs dalam hal ini sectionya yg punya id #
	var elemenTujuan = $(tujuan);
	// mencoba hasil penangkapan eleman dengan console.log(elementujuan);
	// mencoab mengetahui jarak defaul sebuah objek kebagian paling atas halaman dengan console.log(elementujuan.offset().top);
	// untuk mencoba mengetahui jarak sebuah elemen saat scroll bar di geser adalah degan menambahkan karakter e
	// pada fuction (e), panggil function e dengan e.preventDefault dan buat conlose.log ($('body').scrollTop());
	
	// pindah scrolltop sebuah eleman

	$('html , body').animate({
		scrollTop: elemenTujuan.offset().top - 50
	}, 1500, 'easeInOutExpo');


	e.preventDefault ();
	
	

});

// efek paralax

// untuk about
$(window).on('load', function(){
	$('.pKiri').addClass('pMuncul');
	$('.pKanan').addClass('pMuncul');
});

$(window).scroll(function(){
	// efek pada jumbotron scrolltop

	var wscroll = $(this).scrollTop();
	$('.jumbotron img').css({
		'transform' : 'translate(0px, '+ wscroll/2 +'%)'

	});



	$('.jumbotron h1').css({
		'transform' : 'translate(0px, '+ wscroll/4 +'%)'

	});

	// efek leanding objek pada portfolio
		// mencari jarak elemen portfolio dari halaman paling atas
		// dapat menggunakan if( wscroll>1000 ){console.log('ok');}
		// atau mencari secara spesifik objek portfolionya dengan
		// if( wscroll> $('.portfolio').offset().top ){console.log('ok');}

	if( wscroll> $('.portfolio').offset().top -250){

		$('.portfolio .thumbnail').each(function(i){
			setTimeout(function(){
				$('.portfolio .thumbnail').eq(i).addClass('muncul')
			}, 500 * (i+1));

		});




		
	}
	
	


});
