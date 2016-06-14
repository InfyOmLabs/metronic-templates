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
    <title>Metronic | User Login 2</title>
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta content="width=device-width, initial-scale=1" name="viewport"/>
    <meta content="" name="description"/>
    <meta content="" name="author"/>
    
    <!-- BEGIN GLOBAL MANDATORY STYLES -->
    <link href="http://fonts.googleapis.com/css?family=Open+Sans:400,300,600,700&subset=all" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/font-awesome/css/font-awesome.min.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/simple-line-icons/simple-line-icons.min.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/bootstrap/css/bootstrap.min.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/uniform/css/uniform.default.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/bootstrap-switch/css/bootstrap-switch.min.css" rel="stylesheet" type="text/css"/>
    <!-- END GLOBAL MANDATORY STYLES -->
    
    <!-- BEGIN PAGE LEVEL PLUGINS -->
    <link href="path-to-metronic/assets/global/plugins/select2/css/select2.min.css" rel="stylesheet" type="text/css"/>
    <link href="path-to-metronic/assets/global/plugins/select2/css/select2-bootstrap.min.css" rel="stylesheet" type="text/css"/>
    <!-- END PAGE LEVEL PLUGINS -->
    
    <!-- BEGIN THEME GLOBAL STYLES -->
    <link href="path-to-metronic/assets/global/css/components.min.css" rel="stylesheet" id="style_components" type="text/css"/>
    <link href="path-to-metronic/assets/global/css/plugins.min.css" rel="stylesheet" type="text/css"/>
    <!-- END THEME GLOBAL STYLES -->
    
    <!-- BEGIN PAGE LEVEL STYLES -->
    <link href="path-to-metronic/assets/pages/css/login-2.min.css" rel="stylesheet" type="text/css"/>
    <!-- END PAGE LEVEL STYLES -->
    
    <!-- BEGIN THEME LAYOUT STYLES -->
    <!-- END THEME LAYOUT STYLES -->
    <link rel="shortcut icon" href="favicon.ico"/>
</head>
<!-- END HEAD -->

<body class=" login">
<!-- BEGIN LOGO -->
<div class="logo">
    <a href="index.html">
        <img src="path-to-metronic/assets/pages/img/logo-big-white.png" style="height: 17px;" alt=""/> </a>
</div>
<!-- END LOGO -->
<!-- BEGIN LOGIN -->
<div class="content">
    <!-- BEGIN LOGIN FORM -->
    <form class="login-form" action="{!! url('/login') !!}" method="post">
        {!! csrf_field() !!}
        <div class="form-title">
            <span class="form-title">Welcome.</span>
            <span class="form-subtitle">Please login.</span>
        </div>
        <div class="alert alert-danger display-hide">
            <button class="close" data-close="alert"></button>
            <span> Enter any username and password. </span>
        </div>
        <div class="form-group">
            <!--ie8, ie9 does not support html5 placeholder, so we just show field title for that-->
            <label class="control-label visible-ie8 visible-ie9">Username</label>
            <input class="form-control form-control-solid placeholder-no-fix" type="text" autocomplete="off"
                   placeholder="Username" name="email"/></div>
        <div class="form-group">
            <label class="control-label visible-ie8 visible-ie9">Password</label>
            <input class="form-control form-control-solid placeholder-no-fix" type="password" autocomplete="off"
                   placeholder="Password" name="password"/></div>
        <div class="form-actions">
            <button type="submit" class="btn btn red btn-block btn-flat">Sign In</button>
        </div>
        <div class="form-actions">
            <div class="pull-left">
                <label class="rememberme check">
                    <input type="checkbox" name="remember" value="1"/>Remember me </label>
            </div>
            <div class="pull-right forget-password-block">
                <a href="javascript:;" id="forget-password" class="forget-password">Forgot Password?</a>
            </div>
        </div>
        <div class="create-account">
            <p>
                <a href="javascript:;" class="btn-primary btn" id="register-btn">Create an account</a>
            </p>
        </div>
    </form>
    <!-- END LOGIN FORM -->
    <!-- BEGIN FORGOT PASSWORD FORM -->
    <form class="forget-form" action="{!! url('/password/reset') !!}" method="post">
        <div class="form-title">
            <span class="form-title">Forget Password ?</span>
            <span class="form-subtitle">Enter your e-mail to reset it.</span>
        </div>
        <div class="form-group">
            <input class="form-control placeholder-no-fix" type="text" autocomplete="off" placeholder="Email"
                   name="email"/></div>
        <div class="form-actions">
            <button type="button" id="back-btn" class="btn btn-default">Back</button>
            <button type="submit" class="btn btn-primary uppercase pull-right">Submit</button>
        </div>
    </form>

    <form class="register-form" method="post" action="{!! url('/register') !!}">

        {!! csrf_field() !!}
        <div class="form-title">
            <span class="form-title">Sign Up</span>
        </div>
        <p class="hint"> Enter your personal details below: </p>

        <div class="form-group ">
            <input type="text" class="form-control" name="name" value="{!! old('name') !!}" placeholder="Full Name">
        </div>

        <div class="form-group ">
            <input type="email" class="form-control" name="email" value="{!! old('email') !!}" placeholder="Email">
        </div>

        <div class="form-group ">
            <input type="password" class="form-control" name="password" placeholder="Password">
        </div>

        <div class="form-group ">
            <input type="password" name="password_confirmation" class="form-control" placeholder="Confirm password">
        </div>

        <div class="form-group margin-top-20 margin-bottom-20">
            <label class="check">
                <input type="checkbox"> I agree to the <a href="#">terms</a>
            </label>
        </div>

        <!-- /.col -->
        <div class="form-group ">
            <button type="submit" class="btn btn red btn-block btn-flat">Register</button>
        </div>
        <!-- /.col -->

    </form>
<!-- END REGISTRATION FORM -->
</div>
<div class="copyright hide"> 2014 © Metronic. Admin Dashboard Template.</div>
<!-- END LOGIN -->

<!--[if lt IE 9]>
<script src="path-to-metronic/assets/global/plugins/respond.min.js"></script>
<script src="path-to-metronic/assets/global/plugins/excanvas.min.js"></script>
<![endif]-->

<!-- BEGIN CORE PLUGINS -->
<script src="path-to-metronic/assets/global/plugins/jquery.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap/js/bootstrap.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/js.cookie.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap-hover-dropdown/bootstrap-hover-dropdown.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery-slimscroll/jquery.slimscroll.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery.blockui.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/uniform/jquery.uniform.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/bootstrap-switch/js/bootstrap-switch.min.js" type="text/javascript"></script>
<!-- END CORE PLUGINS -->

<!-- BEGIN PAGE LEVEL PLUGINS -->
<script src="path-to-metronic/assets/global/plugins/jquery-validation/js/jquery.validate.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/jquery-validation/js/additional-methods.min.js" type="text/javascript"></script>
<script src="path-to-metronic/assets/global/plugins/select2/js/select2.full.min.js" type="text/javascript"></script>
<!-- END PAGE LEVEL PLUGINS -->

<!-- BEGIN THEME GLOBAL SCRIPTS -->
<script src="path-to-metronic/assets/global/scripts/app.min.js" type="text/javascript"></script>
<!-- END THEME GLOBAL SCRIPTS -->

<!-- BEGIN PAGE LEVEL SCRIPTS -->
<script src="path-to-metronic/assets/pages/scripts/login.min.js" type="text/javascript"></script>
<!-- END PAGE LEVEL SCRIPTS -->
<!-- BEGIN THEME LAYOUT SCRIPTS -->
<!-- END THEME LAYOUT SCRIPTS -->
</body>

</html>