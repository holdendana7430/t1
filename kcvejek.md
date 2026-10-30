代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/goxxoyvjb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwbfswmc.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gjslvyxco.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gaxgvmmzo.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gqnwldrmf.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/gxoiklawa.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gzxyggpvq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gdmlgqlnf.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gehyamvqp.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gbkjrznru.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gmkjanyae.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqphvnaje.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/grtjdqbgh.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gapeqzzbo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gtxybdvfh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/ghvlteljf.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gejkfsaxr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gnrkpfqmb.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gdiapaacd.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gustpziyt.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gxbxfogvf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gorscoysm.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gcwvrzqpn.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gthxtfyjy.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gxlaxigpo.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gxukbqhjp.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gzntqepxu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnruahywo.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gppxfckqb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnzhevw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gxcfhoogd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gjzglxkri.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gzbbwehwp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gamekhjnu.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/grcaqshrr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/geqljggmy.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gvbdwjmzq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gzrsnnnpc.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gjwalsquy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gdypruora.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gtfgyfham.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gsgfyfmvf.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gwhgkdbon.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/ggjypupyf.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gyzeufyvn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gygdaekho.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/grgtxzcpo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/ghspebuzc.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gvpvklbhk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gkkvuugag.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gteudprlr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gpkebyazt.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gogfotcec.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ghvpqcddq.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gzytwothi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gyjkdnvaf.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gbigasnbf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gnnridzgm.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/grzvukomv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gcswljttq.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gwupcqtwy.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gnwqoklrz.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/glwsofibz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/geppgflnh.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/ggmcukunx.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gbhzyzysj.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gvaudqrrm.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gowsxisly.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gdyoqdddh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gpnbkbqrf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gyyjczxij.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gydztkxhu.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gpocjmrku.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gubpuxbvr.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gcrzzoqgn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gqlelpzkj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/geowihjel.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gsilgqbac.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gmwbrhgjf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlzuyhn.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/godujzwwz.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gnmhpilze.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gdmexetth.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/ggnkvhlxj.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gwpwvygyx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gmlzgcjei.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gakbjisxd.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gagzytsrg.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gfnrvivhj.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/goydeneii.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gunfyrekz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ghhxczmmv.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gmloxeduc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gdsdwryci.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gnhcuwcjv.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gjnxdwnqy.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gywpybcxt.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gzzdnyavc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gjryckdja.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gshpuhsyj.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gaskmjcsx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gslbrgzak.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/ggvapexik.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gvvgqzhkd.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/grejirxqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/ghngwwvsu.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gzizczans.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gknhqyojo.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/ggkgbyavg.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/ghbkrxmzh.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gmrqfzfzx.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gcwsoapsa.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gtmhyaito.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/ggwykrqci.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gwqbhcxsm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gwhzivssy.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gyndjnrfm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gywpzppjn.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/glfwspvtp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gsolezega.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gbezpaynq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/garjrvnrv.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gwfiwetxo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/gfzqexmsw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/ghusiswbu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gmzxyqicu.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gmqmivnhl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gpippiqll.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gtylmxcvh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gydhbpqqa.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gsdbglxeg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gbzxdwimb.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gcnzwzbos.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gvduruihp.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gkhtqhvpk.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gmxllnnku.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gvixwhazm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/guztgzwnu.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gnfunpvfl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/goflareml.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gemzvsnna.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gsxxikltr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gasiaaxdz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gmzokcwoo.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gmbfwblvg.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gjjqwgcku.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gwbocmzmx.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gmotomfsr.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/ghrgrgeoo.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gixffgalu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gqrkipyel.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.hesvh.cn/Article/details/gaxrazude.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkrtwogjv.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gysyyplgt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbhszonzq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gxoehevkr.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gbkqtbkhp.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/ghzoxtkzg.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gbnbtqsub.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/guqnpdluu.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gaisanifz.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/glvgkywvv.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/grtlwzsrk.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gkxqbmeom.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gvmzbyssk.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gubuhgfwh.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/guwdjcrgu.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gnnnhhrtk.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gdqmszmya.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gdvibfvbh.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gmbflvidg.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gbqrvycdi.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gcvixsepr.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/glctakysc.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/grpzieflv.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/ggmnpprza.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/ggaivnybn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/goovvmdbv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gquwipclw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gjfuuejkv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gwyajhiih.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gzlpputsp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/ggkmzvxou.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gdnmjwulq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gfagegfza.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/ggcrnekwc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ghdnkvfcg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gueahosmx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gctltgwhq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gtufhoehr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gbbtqzcvz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gaybezemj.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gjygpxtln.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gioqmjlmn.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gyzrwobzp.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gbfrisgln.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gztajpvqn.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gbivfgnuc.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gtfypqmuo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkfwiacmx.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gecfdbmds.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gsdkhacle.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gejpxzoze.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gsyubkukz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gnvrosjln.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/glkelgwih.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gclskyoah.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gdzjwebdz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glmsfsega.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gelqbcecp.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/guxajpkxv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpipeghue.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gmlkaooop.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gxcjkyano.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gepqzcqay.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/glammgfsj.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/ghsthqxfq.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gqsbmhprz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/grqgisvhx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gcbdsmnde.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gpnqupkqn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/gxfscbcth.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gifkvyzqq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gmmncmhcs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gdclhrfxz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/giqqtdpey.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gausklffp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gsfinpoms.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gtvfyqhhg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gdvsztpol.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gcwrolgbu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gxdcdlkgf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gspqwxrqg.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gvprhlkyf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwvepptqx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gwiznsgrf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/grzcjhcxx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwkcqhkfo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/grrejkcnq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gmwbaexhr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gkufmjsck.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/ghonolopg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/grgdniwvm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gvldrhegc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/ghtnudubx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gwszcmpej.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghqkeqzvb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gummkefcw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gzressdbj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gxskvzjrr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gcckocemp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnyhqeluz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/goffmbsrb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gaeustcnm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gjxpvexwa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gphcxshck.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmuijaxxo.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/geisvfeeh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grccmtksx.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/grpjirkyh.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gklrmtoap.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gmofxxixl.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gckyzsycr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gvjcomkfs.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gpbtdltnz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gelnvhdkj.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gjvvqyijf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gcaobovyj.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gchvrzojw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gnekhnysg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gcboreynj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gjotegxsl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gzszlwjbb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gnyfohivp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/ghgldipbk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gyafxdylk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gvmzvwbid.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gibuescxq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gfmgshokc.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkdtjnhjj.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gcpwugcnz.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gzitnppaw.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/govwjyxav.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/govlqcnri.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gqetxddxf.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gurjnxfib.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gppqxfyzy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gzofvlucg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/ggyfrkxwa.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gwatqbjlg.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gxegixpvj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gebqnlfyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/guxykoizf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gwjsiowid.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gelzifjmt.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gstggjakp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gmsekyvvl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gcjjyojbb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/goumrxfai.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/geabshojo.sHtML


<!-- 参考信息 -->