// стандарт кнопка
.button
	display: inline-block
	border: none
	color: #fff
	text-decoration: none
	background-color: $accent
	padding: 16px 45px
	font-size: 13px
	text-transform: uppercase
	font-weight: 600
	letter-spacing: 3px
	border-radius: 2px
	text-align: center
	position: relative
	outline: none
	transition: background-color .1s ease
	&::after
		transition: background-color .2s ease
		position: absolute
		content: ''
		height: 4px
		bottom: 0
		width: 100%
		background-color: darken($accent, 50%)
		opacity: .18
		border-bottom-left-radius: 2px
		border-bottom-right-radius: 2px
		left: 0
	&:focus, &:hover
		text-decoration: none
		color: #fff
	&:hover
		background-color: lighten($accent, 5%)
		&::after
			opacity: .22
	&:active
		background-color: darken($accent, 5%)
		&::after
			opacity: .32
