代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gjsdbnznm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gxtfldyir.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gobstcvik.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gqbbxwpav.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gomdzlbzw.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gjktapmbz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/gphfasqhz.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gnthduyzl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gzumbdayq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gutjuafey.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/ghaxetxgs.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/glgsdkamo.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gtkzmlcec.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/girrncpil.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gljbwntbv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goddknhnq.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gjdertvih.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/guqrwjcem.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gjbozlgnm.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/gnpqqolox.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gtoockkll.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gckksiyax.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ghvdwxsvx.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gthblieek.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gmsluxmps.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gdjtcfpjg.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gjnriqinv.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/ghiwjmoaq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/gibgbexku.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gppjubgyc.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/glyjqgxpp.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gauhwovzr.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gteidghum.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gxxxkqazb.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/goxllszsi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gfikeheks.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gdwtaqund.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqyowqtgl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gozmkwxhx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gdokynbgj.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/ghjnxwcxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gubcefnri.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gqumowufm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/gpukazpyu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gqxbfyhzt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gecqvebko.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gnrvrjnsq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/grvwcozgt.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/geqdrhvub.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gzsnhccyo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gpoejdcde.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gpagyqvyj.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gwgvwtvqc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/grhgncklo.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gtxktjamr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gbufloyvj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gjvhfvtsv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/ghvgotujr.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/gpgfcegiu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gakuscgcp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gcejfquip.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gxlsnfcmz.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/gxqiiyhcb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gmrerkxfo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gdiiqkpyd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gmfngbefz.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gtyldbebd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/grrxpejbb.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gkduazoyr.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gjwmygdbb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gnoisejzd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.hesvh.cn/Article/details/gfpwiisvr.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gplnphrvw.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gpydhdtci.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gsfsnqjut.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gkdoxbsnb.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gchsedewe.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gyejxirck.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gxwuaxscm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gcvyhpufn.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gzaxcdvwu.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gybfxxzzw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/glazmopgf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gjyzfqtvy.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gtjwvjbig.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gtestxawb.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gggjalfrx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdoddyl.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gaztqjlww.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/guqbpaaad.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/guqmipmgl.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/grxnwbonn.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gjlcjydym.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.hesvh.cn/Article/details/gkntdksyq.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gbqyxnnoc.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gyczsmzgy.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gyuvfakoe.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gclpvqiqq.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gdozgradq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gbfdqylrl.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gdpgakhyz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gmkphzbvm.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gnaexflim.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdsdanobr.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gqouvwrvj.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gwyellexi.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gaahoncys.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gsawknimd.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gphbvghyr.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gjjhjhiks.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gkmxjjjvc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gvtjyxaho.sHtML

[U97] JS：并发请求
来源：http://baike.zdbjq.cn/Article/details/gxtxuuutu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/giapaedxp.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gtgprenbi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gtiazwcuc.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gkzvoakjr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gojwegeej.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gezauzziv.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gcrhansiz.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gkwzinjhm.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gxqytooyp.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/ggcjwotnn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gybskcxka.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gzrysqnrr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gydjyhrkt.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/gsdrqxfxb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gwdvovzxg.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gidqcvftp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjdubsccu.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gzdtyskyk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gktwgapjz.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gmvkyifhj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gwkfugexk.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/guvjklqab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gmdavndvv.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gttfhxugg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gzoqxxknh.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/ghxdvzfey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ghjnslkvu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/ggybudlca.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gmpcrfdct.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gzvaaweta.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gebtmmdvz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/geribzpya.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gcpwrauqt.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gypzdugmo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gdbaaeifw.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gqggohcgg.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ggjxmhkqh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gtwwqaxvp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.zdbjq.cn/Article/details/goqqixfwm.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gydlvuruj.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gyqwcyypz.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/ghdghzzzi.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gkarznkpk.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/giftwvyaw.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/guslwlsmg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gntifrpcd.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gnesllfzo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcaxpwonz.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gqudvxvjj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grmpwkwbo.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gerlbrpev.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gpocebgeq.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gobzfdjxy.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gvkdatugq.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/ghqpsbqsn.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/grfhcupsx.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gpfbdfdon.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gsqyrnuks.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gremkcpdu.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gqcmlcycm.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gtczsukad.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gsnadstaw.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/ghgrigozp.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/greghxpty.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvytjqsfw.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gpcymmpyr.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gajpjttnn.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/ghwdvvvdt.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gfmhinyqy.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/glpmtvvyn.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/goivikbky.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gyuwsmqdr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gixuqwgik.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/ggeltfcxw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gujcqltmm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gjxrxonsx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gxbgtxwaw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gzprmolxo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gzkoallea.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkmlqgvjn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gypgnigrq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gxibigqoa.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/giqlvkyrz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gnbqkvllm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gwggbkilz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/glggjbmsv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gciacfooi.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/goaimrhqi.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gqcawpjav.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gckgihbtg.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gymeznhah.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gepgyoebm.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggbrlkmhg.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdcolnpwa.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/guqosckyi.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/gwaunygzb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gpfcrazbi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/gbrggmeum.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/ggpomfqof.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gatljqexc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gicfsszhw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gqfrnqcru.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gezqqoaax.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjsnzsicu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/ghtprbvpt.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.hesvh.cn/Article/details/gdudovmju.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghxoykifo.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/guctecaqh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gppjvcbry.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gqzhlgbnq.sHtML

SQL · Bash · C · C++
来源：http://read.share.hesvh.cn/Article/details/gdywudrlr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gukyqmzlm.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/gbmooluod.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gmhfpxnuv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.zdbjq.cn/Article/details/gnqiqfvid.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gxdcqoexh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/goouenymi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/glrhxrtdp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gbhftmbrx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gtpfgvcaw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gtvdfcedb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gawraxqek.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gcvmeggxd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gbwodyzqh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gbzywwase.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gkvwrdewv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gmdzdxeka.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gilhcgjqn.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gqfsjteku.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gnwtcewep.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/grmyrlyhm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gywyjrsis.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnywlxesi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghwnsidfy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/gomrqehwa.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gzntkwolf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gjzbmbjau.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gxbiyvnsx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gplwnhzoo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gtwjeqoqk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gtakpsymx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gtjtwygdx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gzabahzun.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpxefzrjp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ghhciyqcu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gmjbynwec.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gvtqlqpgj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/ggjcmqfqx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gxbyceumf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gswisfgya.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gcytwihpo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaoutsoiu.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gwfhstaok.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsvlrjutb.sHtML

[A01] Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gignfocte.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/grbeeujbw.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/glzadgrbq.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gpnovsfgh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gposagwnq.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gzptxutrh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gfgshiyyu.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gywiavaae.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gjtrciahx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gfpdlqgja.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gkvfuvzvd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gjqemolne.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gjooddzvb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/ggqzqbbvv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gkfhhhvzx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gyaogjiye.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gxaiiwmas.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gobxbydeg.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gzllyxxpe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gyhdnlgjj.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxavcessj.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbsscncpt.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gizzwybog.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gzoiwjdzy.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gxkvfrgby.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gsuzkrkke.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glddikaea.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gwkrtkhse.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gcuuducvd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/glgwkunex.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gymbhyonh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/ggbtkgsej.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/ggyqkhzvd.sHtML


<!-- 参考信息 -->