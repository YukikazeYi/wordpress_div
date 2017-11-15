<?php
/**
 * The base configuration for WordPress
 *
 * The wp-config.php creation script uses this file during the
 * installation. You don't have to use the web site, you can
 * copy this file to "wp-config.php" and fill in the values.
 *
 * This file contains the following configurations:
 *
 * * MySQL settings
 * * Secret keys
 * * Database table prefix
 * * ABSPATH
 *
 * @link https://codex.wordpress.org/Editing_wp-config.php
 *
 * @package WordPress
 */

// ** MySQL settings - You can get this info from your web host ** //
/** The name of the database for WordPress */
define('DB_NAME', 'blog');

/** MySQL database username */
define('DB_USER', 'admit_lin90217');

/** MySQL database password */
define('DB_PASSWORD', 'abcd1234');

/** MySQL hostname */
define('DB_HOST', 'localhost');

/** Database Charset to use in creating database tables. */
define('DB_CHARSET', 'utf8mb4');

/** The Database Collate type. Don't change this if in doubt. */
define('DB_COLLATE', '');

/**#@+
 * Authentication Unique Keys and Salts.
 *
 * Change these to different unique phrases!
 * You can generate these using the {@link https://api.wordpress.org/secret-key/1.1/salt/ WordPress.org secret-key service}
 * You can change these at any point in time to invalidate all existing cookies. This will force all users to have to log in again.
 *
 * @since 2.6.0
 */
define('AUTH_KEY',         'CT15C0m,&zp$qaAQ%q{-E}hJ Zc#jTj[t.6szqS.yo+!1z$;JvZqcMzccL4?@~,x');
define('SECURE_AUTH_KEY',  '2|}kfq^bQR.FEw=iIQv_O<GPi5^{@N6OY78GR=.l;yOi%-;d#@X06stSy6EG9HCn');
define('LOGGED_IN_KEY',    'miHGr|>J&7s=#ZHB eC.r*AiEA}hW<e2P520o$m@ZaN+M@e5o<wz,/$}gPU#X@-F');
define('NONCE_KEY',        '=%gs>{0lwXVk(S/U~2]g_e4]zI:/Ax0.K=wwa<XGv&,%J|CV[=++xmr~Z(/N5[7X');
define('AUTH_SALT',        '%gkpABL( OQ=!{LaEghkfJz}[.7Z9MzL4]tN^oYT6hn1 zqc|JhXV]p5X_3cpx~3');
define('SECURE_AUTH_SALT', 'Z9%a$l#.bur?@b,>4{73Z=`ii&mi>.;|h]5S_<J6^?o@.=gd9B?;U_~%4A?z4#26');
define('LOGGED_IN_SALT',   '3}#f8!S&]2/4}..KxJ#&,y^*)Zey=*DB.OKJ44I(*3zp>@Lf RtE(_BCr0L<|x:2');
define('NONCE_SALT',       ') OoLu2lRf@Z>ZTZ8c=h*<llFRg7jKJ4h&9vlaw(K%:mUM@}#!|{8AC/-#i^Fw!]');

/**#@-*/

/**
 * WordPress Database Table prefix.
 *
 * You can have multiple installations in one database if you give each
 * a unique prefix. Only numbers, letters, and underscores please!
 */
$table_prefix  = 'wp_';

/**
 * For developers: WordPress debugging mode.
 *
 * Change this to true to enable the display of notices during development.
 * It is strongly recommended that plugin and theme developers use WP_DEBUG
 * in their development environments.
 *
 * For information on other constants that can be used for debugging,
 * visit the Codex.
 *
 * @link https://codex.wordpress.org/Debugging_in_WordPress
 */
define('WP_DEBUG', false);

/* That's all, stop editing! Happy blogging. */

/** Absolute path to the WordPress directory. */
if ( !defined('ABSPATH') )
	define('ABSPATH', dirname(__FILE__) . '/');

/** Sets up WordPress vars and included files. */
require_once(ABSPATH . 'wp-settings.php');
