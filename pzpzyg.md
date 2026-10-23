代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ktunknxx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ybejgixj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3suhtgsuw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3swfnyfin.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xioikqan.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tsebumnk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvfvhl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhdoony.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ckkgspnt.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3mmwznekw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vtcauaet.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nzxswtmn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tqwvkqub.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epvqywys.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3myjxwxck.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wizkwdwz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jvtwgerv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3eqilzvqy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sgzivzbt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xswkcgkt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3esedbizj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jwyisxdf.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3wqaquamy.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioinlpvy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fsbhgcxs.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3pofnrrmw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwlkxclg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dxsjdteo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3mmwlditt.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gccsjnnb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cebjqnmb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3mpwsrkrl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3aiehblud.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ryrcqcbg.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xiqvtkxu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3edbgqruk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bzkshskk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ljckixur.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wayjtsmo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3qvfhfvfb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3trfmvkgs.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3imalwvyf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3xxkkyemi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iyvmmzpn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3pcnokkor.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3idwaqpjs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3zjdqvfmr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zbixrjti.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ldneljjc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3uwxlxvqc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3flewxjan.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gocsmopz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mqrozhpu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eiedtgny.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3lvsidpvj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qasjeuwn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3dvkmawvk.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3qakhgyhs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dbbfzjlu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3jsxagmer.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rctjqike.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3plrzixdc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wvfwnvfm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qsygdkig.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lsmawfog.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yxstrwkv.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3tdtalaqx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3nuhwslrb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3dwrqqxft.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3scdmdhdj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qyogymwj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iezfized.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ffngywvs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3auqnqeiu.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jelcrnnt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3scrrrggj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3acornbrd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3jvkoxsop.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qxeuzebf.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3frgzrcwp.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iwosslzm.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3tgriinqa.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3qmjsbugc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ximvhojd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rjugmrls.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3eibscoch.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zafjrprx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xpstqrtw.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3frfbskby.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3umdzvive.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3hataqdnu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lwqrmybr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3ksampthw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3rowfibgc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3qxtaboyq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wyecqqws.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3eufktvzi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3cukxcypt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ilvnxzkw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxwyaaa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3stbxjmxw.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3anheajog.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgbmsmji.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdnhivb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3dkiythba.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cacypimg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3myuwwaoe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3muujebcj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xynsrozu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3pqyyyktc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikufsmyf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ysgnuxrr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fyxzwytx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jifnkprj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pcofdbqz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zhivilht.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3oayczwfn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3arqnhcyh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ocoridpr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wroapuub.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3opiguhfc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lzmlsbsy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vfxsjagy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zyxoguuo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dhahksgf.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3rihvknni.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dbblpgao.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gqzjeldr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3yvoceaau.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3fsaikftw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3zgyqwowe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3eyjxjqgd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kludeivy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dxyfsfft.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mzlwkiql.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kqsfeuiu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uwhjfeww.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhyfkmx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3aezvemgy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3vdnqfxlx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nbqtvtly.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3oamipmwg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3szumlvud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3irbuxzvr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zdshzvod.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3rindvytb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3sjumovya.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ixntdnwl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ibnzuhdx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3opewxehx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wcbruphq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ibbdykpz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ffxrljwr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3quunttpp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3viknpioz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yarjmztr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3autheent.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lulrovyn.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bruncdmk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wefniuph.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pufjbqes.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ydaqarin.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sbcfnfqa.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qcwpmogj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyjnoooy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xslppdwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktwtlxkc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3axqbrhqk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ltahldyj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ixffilfg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wrdpyhib.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3izmuammu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wtpgtswa.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xhdkpqlr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lrgthbuo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3epbjwban.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hbnoghzg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rwisamjy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fkvwplnv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wizmxzml.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wobftmyg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3imenzqrq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3bultwprj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ojrieegu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bumxdohs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ubefktsb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ljkdtdtj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ftpladbi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ubsldffd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3khuvuqkc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kebtjyul.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yybslvzv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vvcrpgsf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3paxmjvpg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ifebosme.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qbtmsdwz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzeguz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3htpgqvyb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zcplvxkk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yyzythjr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zhveykss.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3guzwaiwj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3jqbzhvus.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3piyknsen.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xzqeftep.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pnzujfve.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qryioyqi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kilxwulm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ulrxdiak.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qmngsfqh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3peaspglf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kpfqjysg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pafecplz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vyxyldho.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3kmluebwv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tbzfqhta.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rrtmuksy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3xtnfokhz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3sqdmrjzd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ohvibnet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjrmpybq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3qwfdftuz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ocwnyned.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofmuwnrd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3uexazgki.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3nwmautxt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3pgvtgcta.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3kcrsruyo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3fpawycyk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3dkhbtopo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mbesgxtz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3uxdellcb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jbplrapv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ujebsglj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3xnlaxwfv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lardzmpo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ugcfbgdn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zevykhxl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ajjqzupc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ffmxpaod.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ppnjejee.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lyxntasf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wmaijfjw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvkitw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sgvsopgs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3emptlywp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qgzbbqfy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3odknqrks.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aipqpmhv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bokheryz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwoqjhvp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3lenhvnfh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tysffcxj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3judokadw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emkvhjiu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmwnmn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvuuydnc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uehebdan.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ynblnwkl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bdwzdsay.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfdebipq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfnuytzk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nobspudk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmewobob.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agtclved.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fpbdsryr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fhvynkua.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3npesftbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivyihebe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxrdmlpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlwanfrj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3cwglehaz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ykrawana.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3druqrnum.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bxinrefa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3oytcedzc.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rhrxbfvm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3peqfjzsr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zjvkencc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3darzysmp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3gzlkhrcw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fbgomctb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rwovahru.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ziadichv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xwhjdcqv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wjorubjm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3iqwpmujf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gutocxpf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3csnuxejz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3cavpofvu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3dnkimtgw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3trbuwvpu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wcomsbzj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tzeetwye.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cbhczewo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zxdneozl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3igdxmjpe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hdgevdsa.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bgocmnyh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3goebwzpb.html


<!-- 参考信息 -->