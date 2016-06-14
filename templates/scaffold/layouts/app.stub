<!DOCTYPE html>
<!--[if IE 8]>
<html lang="en" class="ie8 no-js"> <![endif]-->
<!--[if IE 9]>
<html lang="en" class="ie9 no-js"> <![endif]-->
<!--[if !IE]><!-->
<html lang="en">
<!--<![endif]-->
<!-- BEGIN HEAD -->

<head>
    <meta charset="utf-8"/>
    <title>InfyOm Metronic Template</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta content="width=device-width, initial-scale=1" name="viewport"/>
    <meta content="" name="description"/>
    <meta content="" name="author"/>
    
    <!-- BEGIN GLOBAL MANDATORY STYLES -->
    <link href="http://fonts.googleapis.com/css?family=Open+Sans:400,300,600,700&subset=all" rel="stylesheet"
          type="text/css"/>

    <link href="path-to-metronic/assets/global/plugins/font-awesome/css/font-awesome.min.css" rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/simple-line-icons/simple-line-icons.min.css" rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/bootstrap/css/bootstrap.min.css" rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/uniform/css/uniform.default.css" rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/bootstrap-switch/css/bootstrap-switch.min.css" rel="stylesheet"
          type="text/css"/>
    <!-- END GLOBAL MANDATORY STYLES -->
    
    <!-- BEGIN PAGE LEVEL PLUGINS -->
    <link href="path-to-metronic/assets/global/plugins/bootstrap-daterangepicker/daterangepicker.min.css"
          rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/morris/morris.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/fullcalendar/fullcalendar.min.css" rel="stylesheet"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/jqvmap.css" rel="stylesheet" type="text/css"/>
    <!-- END PAGE LEVEL PLUGINS -->
    
    <!-- BEGIN THEME GLOBAL STYLES -->
    <link href="path-to-metronic/assets/global/css/components.min.css" rel="stylesheet" id="style_components"
          type="text/css"/>
    <link href="path-to-metronic/assets/global/css/plugins.min.css"" rel="stylesheet" type="text/css"/>
    <!-- END THEME GLOBAL STYLES -->
    
    <!-- BEGIN THEME LAYOUT STYLES -->
    <link href="path-to-metronic/assets/layouts/layout/css/layout.min.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/layouts/layout/css/themes/darkblue.min.css" rel="stylesheet" type="text/css"
          id="style_color"/>
    <link href="path-to-metronic/assets/layouts/layout/css/custom.min.css" rel="stylesheet" type="text/css"/>
    <!-- END THEME LAYOUT STYLES -->
    
    <link rel="shortcut icon" href="favicon.ico"/>
</head>
<!-- END HEAD -->

<body class="page-header-fixed page-sidebar-closed-hide-logo page-container-bg-solid page-content-white">
@if (!Auth::guest())
<!-- BEGIN HEADER -->
<div class="page-header navbar navbar-fixed-top">
    <!-- BEGIN HEADER INNER -->
    <div class="page-header-inner ">
    
        <!-- BEGIN LOGO -->
        <div class="page-logo">
            <a href="index.html">
                <img src="path-to-metronic/assets/layouts/layout/img/logo.png" alt="logo" class="logo-default"/>
            </a>
            <div class="menu-toggler sidebar-toggler"></div>
        </div>
        <!-- END LOGO -->
        
        <!-- BEGIN RESPONSIVE MENU TOGGLER -->
        <a href="javascript:;" class="menu-toggler responsive-toggler" data-toggle="collapse"
           data-target=".navbar-collapse"> </a>
        <!-- END RESPONSIVE MENU TOGGLER -->
        
        <!-- BEGIN TOP NAVIGATION MENU -->
        <div class="top-menu">
            <ul class="nav navbar-nav pull-right">
                <!-- BEGIN USER LOGIN DROPDOWN -->
                <!-- DOC: Apply "dropdown-dark" class after below "dropdown-extended" to change the dropdown styte -->
                <li class="dropdown dropdown-user">
                    <a href="javascript:;" class="dropdown-toggle" data-toggle="dropdown" data-hover="dropdown"
                       data-close-others="true">
                        <img alt="" class="img-circle"
                             src="http://infyom.com/images/logo/blue_logo_150x150.jpg"/>
                        @if (Auth::guest())
                            <span class="username username-hide-on-mobile">  InfyOm</span>
                        @else
                            <span class="username username-hide-on-mobile"> {!! Auth::user()->name !!}</span>
                            <i class="fa fa-angle-down"></i>
                        @endif
                    </a>
                    <ul class="dropdown-menu dropdown-menu-default">
                        <li class="divider"></li>
                        <li>
                            <a href="{!! url('/logout') !!}">
                                <i class="icon-key"></i> Log Out </a>
                        </li>
                    </ul>
                </li>
                <!-- END USER LOGIN DROPDOWN -->
            </ul>
        </div>
        <!-- END TOP NAVIGATION MENU -->
    </div>
    <!-- END HEADER INNER -->
</div>
<!-- END HEADER -->
<!-- BEGIN HEADER & CONTENT DIVIDER -->
<div class="clearfix"></div>
<!-- END HEADER & CONTENT DIVIDER -->
<!-- BEGIN CONTAINER -->
<div class="page-container">
    <!-- BEGIN SIDEBAR -->
    @include('layouts.sidebar')
    <!-- BEGIN CONTENT -->
    <div class="page-content-wrapper">
        <!-- BEGIN CONTENT BODY -->
        <div class="page-content">
            <!-- BEGIN PAGE HEADER-->

            <!-- BEGIN PAGE BAR -->

            <div class="page-toolbar">
                <div id="dashboard-report-range" class="pull-right tooltips btn btn-sm" data-container="body"
                     data-placement="bottom" data-original-title="Change dashboard date range">
                </div>
            </div>

            <!-- END PAGE BAR -->

            <!-- END PAGE HEADER-->

            <div class="row">
                <div class="col-lg-12">
                    @yield('content')
                </div>
            </div>

        </div>
        <!-- END CONTENT BODY -->
    </div>
    <!-- END CONTENT -->
</div>
<!-- END CONTAINER -->
<!-- BEGIN FOOTER -->
@else

<!-- BEGIN HEADER -->
<div class="page-header navbar navbar-fixed-top">
    <!-- BEGIN HEADER INNER -->
    <div class="page-header-inner ">
        <!-- BEGIN LOGO -->
        <div class="page-logo">
            <a href="index.html">
                <img src="path-to-metronic/assets/layouts/layout/img/logo.png" alt="logo" class="logo-default"/> </a>
            <div class="menu-toggler sidebar-toggler"></div>
        </div>
        <!-- END LOGO -->
        <!-- BEGIN RESPONSIVE MENU TOGGLER -->
        <a href="javascript:;" class="menu-toggler responsive-toggler" data-toggle="collapse"
           data-target=".navbar-collapse"> </a>
        <!-- END RESPONSIVE MENU TOGGLER -->
        <!-- BEGIN TOP NAVIGATION MENU -->
        <div class="top-menu">
            <ul class="nav navbar-nav pull-right">
                <!-- BEGIN USER LOGIN DROPDOWN -->
                <!-- DOC: Apply "dropdown-dark" class after below "dropdown-extended" to change the dropdown styte -->
                <li class="dropdown dropdown-user">
                    <a href="{!! url('/login') !!}" class="dropdown-toggle" data-hover="dropdown"
                       data-close-others="true">
                        <span class="username ">  login</span></a>
                </li>
                <li class="dropdown dropdown-user">
                    <a href="{!! url('/register') !!}" class="dropdown-toggle" data-hover="dropdown"
                       data-close-others="true">
                        <span class="username"> Register</span></a>
                </li>
            </ul>
        </div>
        <!-- END TOP NAVIGATION MENU -->
    </div>
    <!-- END HEADER INNER -->
</div>
<!-- END HEADER -->
<!-- BEGIN HEADER & CONTENT DIVIDER -->
<div class="clearfix"></div>
<!-- END HEADER & CONTENT DIVIDER -->
<!-- BEGIN CONTAINER -->
<div class="page-container">
    <!-- BEGIN SIDEBAR -->
    @include('layouts.sidebar')
            <!-- END SIDEBAR -->
    <!-- BEGIN CONTENT -->
    <div class="page-content-wrapper">
        <!-- BEGIN CONTENT BODY -->
        <div class="page-content">
            <!-- BEGIN PAGE HEADER-->
            <!-- BEGIN PAGE BAR -->
            <div class="page-toolbar">
                <div id="dashboard-report-range" class="pull-right tooltips btn btn-sm" data-container="body"
                     data-placement="bottom" data-original-title="Change dashboard date range">
                </div>
            </div>
            <!-- END PAGE BAR -->

            <!-- END PAGE HEADER-->

            <div class="row">
                <div class="col-lg-12">
                    @yield('content')
                </div>
            </div>

        </div>
        <!-- END CONTENT BODY -->
    </div>
    <!-- END CONTENT -->
</div>
<!-- END CONTAINER -->
<!-- BEGIN FOOTER -->
@endif

<div class="page-footer">
    <div class="page-footer-inner"> 2016 &copy; Generator by InfyOm
    </div>
    <div class="scroll-to-top">
        <i class="icon-arrow-up"></i>
    </div>
</div>
<!-- END FOOTER -->

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.0/jquery.min.js"></script>
<script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js"></script>
<script src="https://cdn.datatables.net/1.10.11/js/jquery.dataTables.min.js"></script>
<script src="https://cdn.datatables.net/1.10.11/js/dataTables.bootstrap.min.js"></script>
<!--[if lt IE 9]>
<script src="path-to-metronic/assets/global/plugins/respond.min.js')!!}></script>
<script src=" path-to-metronic/assets/global/plugins/excanvas.min.js')!!}></script>
<![endif]-->

<!-- BEGIN CORE PLUGINS -->
<script src="path-to-metronic/assets/global/plugins/js.cookie.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap-hover-dropdown/bootstrap-hover-dropdown.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery-slimscroll/jquery.slimscroll.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery.blockui.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/uniform/jquery.uniform.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap-switch/js/bootstrap-switch.min.js" type="text/javascript"></script>
<!-- END CORE PLUGINS -->

<!-- BEGIN PAGE LEVEL PLUGINS -->
<script src="path-to-metronic/assets/global/plugins/moment.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap-daterangepicker/daterangepicker.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/morris/morris.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/morris/raphael-min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/counterup/jquery.waypoints.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/counterup/jquery.counterup.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/amcharts.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/serial.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/pie.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/radar.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/themes/light.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/themes/patterns.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amcharts/themes/chalk.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/ammap/ammap.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/ammap/maps/js/worldLow.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/amcharts/amstockcharts/amstock.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/fullcalendar/fullcalendar.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/flot/jquery.flot.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/flot/jquery.flot.resize.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/flot/jquery.flot.categories.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery-easypiechart/jquery.easypiechart.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery.sparkline.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/jquery.vmap.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/maps/jquery.vmap.russia.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/maps/jquery.vmap.world.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/maps/jquery.vmap.europe.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/maps/jquery.vmap.germany.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/maps/jquery.vmap.usa.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jqvmap/jqvmap/data/jquery.vmap.sampledata.js" type="text/javascript"></script>
<!-- END PAGE LEVEL PLUGINS -->

<!-- BEGIN THEME GLOBAL SCRIPTS -->
<script src="path-to-metronic/assets/global/scripts/app.min.js" type="text/javascript"></script>
<!-- END THEME GLOBAL SCRIPTS -->

<!-- BEGIN PAGE LEVEL SCRIPTS -->
<script src="path-to-metronic/assets/pages/scripts/dashboard.min.js" type="text/javascript"></script>
<!-- END PAGE LEVEL SCRIPTS -->

<!-- BEGIN THEME LAYOUT SCRIPTS -->
<script src="path-to-metronic/assets/layouts/layout/scripts/layout.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/layouts/layout/scripts/demo.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/layouts/global/scripts/quick-sidebar.min.js" type="text/javascript"></script>
@yield('scripts')
<!-- Datatables -->

<!-- END THEME LAYOUT SCRIPTS -->
</body>
</html>