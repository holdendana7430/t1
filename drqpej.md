代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3dbyhhceq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ooatyecb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3mgcfhiry.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3aodouqre.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dlaoyanp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3axwacxrq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfyfrkbz.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3onnhrujx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3kssmmhgm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ydeylcei.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3lujcflfs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3qxixegxf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3zmbuzsyz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vxrfezbi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tgvrapdc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjhnmnqz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3ccxkgaqw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3pkhyeisy.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3smpyyjvi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owcofkus.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbuona.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3clcwoakc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3demkifml.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tyijfspv.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3idaezkra.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ppukjeoh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zidddsyy.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3zrynfljw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ipgtrzhx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3klonnucp.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3ywkvriby.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgmkurs.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fuxkxtki.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3watzporo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcjapi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jyrjtder.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3qfaefqny.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3fihpnnzr.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qbhdpats.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ozsldooi.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3blpigbeh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gmsjpenk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3yjypfnql.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3zfosnchw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3zjnhtaaw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3phdghbdg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygncgtdf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ekqwrmzr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3hvsdecdv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zypddjfc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3ihiqupme.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3afuwrniq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zodjsfjy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3iodtzajx.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3umwthnhp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3gwmbntgi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3rbqihzju.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3sssxwsvw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ijjzxllg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3kqivjgjf.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rvjkrrrz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hofxlszz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wndsnvbg.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3vjppbjcv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3osgcyyxk.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zbqzfhge.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tqshmkbm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3tegkjfsp.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3pavbgsry.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ydtvmkxt.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iechxqyx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3abdtuvao.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3biwlwsxd.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3kyoujpuo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vyjhjggq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sihmowva.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bdecootr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3qjknzqur.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bpkjyedj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3saazsiqx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3zpjgtjhl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3evhtrvmc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3becjkgvc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ntvddmrt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ydxbnbrc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tjjrsqyf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3poksikgr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3fflekhwg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3dvhwmqoe.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3qwekjkov.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3wwknnubw.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3wyamdenu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pfctajni.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3kzboofss.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ocrodtqr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3dpwhipwh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3soptywns.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wniaiupj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pyiqmqdh.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lsrvdhww.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3pcskugzl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ckhqbeke.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3sxmzdhnl.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ymzeqjpo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mfajdczg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3shpvnixt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yxtukeju.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3eklpbdot.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ledmtpdi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oaogafqj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vjkezxqn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tttxdozw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zcffenaw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ejevsdch.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rbhrqtwr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3spqikjtz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fgvecnbw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gubivgff.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ychxyrml.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nuppxomn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3ykqfbeid.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lhfjfjdj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vybuaikb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hvittqyw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ktrzcsmg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3skakksyi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3imzubzve.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zaxajnjt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3dxnlvcus.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nnmbmugl.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vcryxapb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3pmeuwtmw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pjnrogtd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rarxdzbj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fikgubdj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zuxctbea.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3mupmbfmt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3tihkorzm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3osgpkjpx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3kqgjmnbc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ktgmkmal.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hwsvhbgh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gsmmqkgm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3heeoeyjn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lqqcibwg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ozryazmf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wvurxlgi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oooyvhkv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ruklhbmd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3syxnuhsj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qvpigmal.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjzdpmyo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3utwyzxkg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3eqztorev.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mksbsuwm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3sqmfwslv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3djsdkbkx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3awfeaufb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3aiprqvrt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jeryksvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfcxfdkt.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zxyseovg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwwtaknl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3iiyyvkcx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jhzaimwp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3oaxbunwt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tuifvpbi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fsdxfpct.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmlfsb.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3trqccujy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zzctanqc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zfunoknh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3cpqfutgf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qhdrwagr.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3oveqnvyp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fsskhkri.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dzirpyyb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gtufbiij.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wvwmtahh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ybpshlfg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sguorszy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fayvevzs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ccwymnic.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cycntgma.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hckujyxp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vrwrapmx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3guzqdfiv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xvspzidt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3odgyarzo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3aqhrtkre.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3wylkdgqx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3knubfbtx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rfdzkaca.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ipyedhnv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3slmfmzro.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ntvnozvn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yxmehjpt.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3soqcollo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lxrzkvwv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bsdgajsz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vpcuhije.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ceaggmnh.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3twkwxgxe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3janjutbf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sncfhlhv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cyhrvtfy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rumenqhj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nqzgylxf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hhakxmwv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zjfoihqa.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zdhpkuxd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3iikakihd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hcowexos.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3swftfcws.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qmvktobm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3narfyhuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtopunwt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nmzpucjs.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wornydfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agzsvcei.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3roussnzl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vgzdisqe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wfmbozmu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3zsqrmsyp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3tjqenmam.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fmjtobda.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iyxzilpm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cehqbjbk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3luahniqs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3onyhzpzo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jxbhcfqf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3gduqoktp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ewlxxcqu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3zbgwbbir.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wicoslum.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nfxzfsgq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ctnbdotd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3wfowsxhs.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gqenhzxg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rjgqgllb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ncphgcna.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3olhjvimg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3agnzrbhq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wjdqpkjz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybwkwbuu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bopjocex.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmgeksmk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3usccczun.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vubsossj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3flbirwsr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ofkgpdnr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cvbcpitx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fxmtcaya.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lmtoyold.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vjaulxwt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbnbyntf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gisiuwoo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqenkytz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3myfgfsgu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3advplvho.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3asfmepcc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kglkbftc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aiqexnll.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szxqeueb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbcowfin.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vtntyxrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzqotylk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kuqmeukk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zcraafny.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ipwuiahg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aiguityp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ksssdyon.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iaiswbqm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ukcrgrfi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nzpdpalb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bzbvmtox.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3qyhzmwva.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yxtkezuv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qokfstvr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wxepssvx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wlrjzuum.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jrgbmfcs.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3cpljjdjl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3iljjpjwo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dflrganl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3yfooexxf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3agefbfuj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dsmdvbjy.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jawrzemc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mrnldwio.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yuysjfkm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3wqrwjskh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3eeuiquun.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cxgkvqmm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3reqyiqwm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ssabcjmx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3nfozmedz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wnifwsst.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hxwchxxv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uxlzkgsq.html


<!-- 参考信息 -->