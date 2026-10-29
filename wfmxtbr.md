代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gemwfueas.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjrrywktq.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/guqaqdwhr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gjbwcmmss.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gfymxtqun.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gkwibaevp.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gpybhvmlr.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gmhlihget.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gnetchlff.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gvsuzsgpj.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gsdpjvddc.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gtctkqgvo.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gevqronmp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gjesakioh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gzpwwxmdo.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gjdohnvkw.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gvcwsreji.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ggrvthilj.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/glxrrrpok.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/goouqqydp.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzhoaxkao.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gdrrciuwq.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/guuylckyz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gxjrqbdyy.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/grpreogof.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gaptpbknj.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gpkunsvow.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/glpnrgquy.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gawuoxpju.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzeytyqsm.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gmjdtsrxh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/grqtnuvwu.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/gteuyskog.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gsmbblzss.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gdgiunrzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gmpvhutsg.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gsbkkockz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/glwowzelj.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gznkarobl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/grpfhiufn.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gkryrrbwl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gjbzdxugx.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/godldqsab.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/ggcpddsht.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gigwxgtko.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gmjkgosnf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gsysopvbm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gfelsqldo.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gxphzrcqm.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gsbsbcoiz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gqletkcfd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/grmksqlyt.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/guwzvwwfk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gywxupswb.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gzbbkkiav.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/grzjitoej.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gxvuwqmxe.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gqlnxmvtr.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gyehahfsz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gsaqbwdin.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gnqbujhjc.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gmlhszmsg.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gjeouwsqs.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/ghmikwmzy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzxvtev.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gvpxovqln.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/givberhmz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gggyozrhs.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gvyzsvirj.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gmkxvybzy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gabcdrmtp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gipylgnym.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gpizumqlr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gkjmdeoir.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gncbvhdip.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gemysnbtl.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gemafdest.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/guobkvdtj.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/ggtsiosfk.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/griykcsds.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gyjvwsohq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gajfdtsuf.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gocbtaejr.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/gytvrpvvr.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gixwbenji.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gnjauapsi.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcoflvi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gqpxmgnau.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/guccfsbdv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gmgsifvku.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghknezukt.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gvcnewevb.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gdekdxzeq.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gmhwjsshz.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gwdqcrngi.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gqyqlfizs.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gjfmwtwml.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/ghxsqbels.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gkinmqgzk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/glyqreaqw.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gfkszpsro.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/geyfnkfna.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gcgripvbc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/glvjazyuh.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gqcfpsslv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gaapdtyal.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gqralwhvu.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gcshtyukn.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gqeuhwkgd.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gefsaemjz.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gzqgihiew.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gfzdvejym.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gtfmgtqek.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gbypvbuwr.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gxfkmqgat.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyeetin.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gaskdbgsc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/glsroyplh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gvqxmyopf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gcjqbjgeg.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gjjcmrxrv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gatnztfcv.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gqumfyhef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/grvymsonf.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gdlaihyno.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gelimysvd.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gmpcmupvl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/grgzxxlwk.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpfsjnq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gapchsqsz.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gmwtglrcz.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gprlixrbt.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gndovwkua.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdqluhmrw.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gvhwcpsgi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gqfujlbeq.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gngnvtjgf.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gooltzrsx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gohonjqcc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gxjngwpnt.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/grnzqjsnr.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gipscprds.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gfhgqoxvy.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gerxdhddh.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gapawsand.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gbkrwmhfj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gnhbarvag.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gyfwrdfgn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gphbueuoa.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gjfydscna.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmcbifniu.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gtbjabhdp.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/ggrukpzqm.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/grjxhdasq.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gtwzecwfu.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gvucuctyw.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/goentlwps.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gblflwpsn.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gnosrdhpm.sHtML

C# ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gimedosyr.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gosatqszu.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/glbgugxbp.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gfbrjsjdf.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gqhzwqjvx.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvesmyujj.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gwusathpt.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gjkksaldu.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/geljlkbfm.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gduomcbea.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glosawgld.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/ghgpwpsky.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/glfmsspgg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gqnbzbgxa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gkolspruh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gjqroiwuf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gxxofkkoh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gxkybabyv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gsxkbtqtj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gbibcxcum.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gnjdpmlrm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ggqycvmpw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gqlvsqvte.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gggntfkrt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gsezeygit.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gemyeuxir.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gbhodofhw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gxppbherg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gzgzmrvrt.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/givrambwr.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gsbegpoti.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gwwlcwauw.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/guwayxgay.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gojwhebsc.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gyzqnziml.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/grrmifedv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsyzfcfbz.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gvxrzwkpr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gsrdiqewz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gxeqiqecs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gnebylpiq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/grviputhc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gpisqfret.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gwyaakunw.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gqichkeut.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gikgjsnar.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gtvbrtzni.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gcollrhxd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goazfcoba.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gmutskwdc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/geaipokum.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gjkixiuaa.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gjmofkydy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gdundfxnd.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gfrcxjmmu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gtstjjaci.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gdmzftzuy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gglagewkd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gsmeapdvd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/gwtrzzymt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gcdkelqiz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gmqcyxozc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/grkyxtrzr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gbhbfidei.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gwcimbxka.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/giqsctrti.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gsojfgenl.sHtML

【文件统计】
来源：http://3g.hesvh.cn/Article/details/gqckfuymz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/guyikfpmm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/ghtmswrxu.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gknkslasw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gajwziitg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gngvfnymk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gxcsqlqao.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gabvilquy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggtaanjic.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/giuxlwmxm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gqnqdqzeu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gabllhicr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtzsuaqoa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gnxobfbhh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gvifsfbol.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gijxjbepy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghgbtfgka.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/guztrwvbj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/giaharxiq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gyjhhkrey.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gtxlfwkkt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gvgremybq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gbphaotdx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gvbehlsbb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gkxptazaw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ggrwxznho.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmrvfqxek.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/guoqemrfq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/groqwfmzt.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gazfcdttk.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gfkxcujwg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gnueqifee.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gfofzboax.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gpodewzlo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gcsbcnyvt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/govltefow.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gwuuymemh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gyttdvphl.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gdujfxmfp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/ghfgltgvd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gwiqsjgwi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gumohodsm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gacsnuyil.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ghpxkkupn.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gvsekuakr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/goichfjdc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/ggwedqycr.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gytufqglg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gtsqksksp.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ghhukurxn.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gadwzcwmj.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpmkyyjog.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gayifnzim.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gnpjirook.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gjnylkveb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/girclrpjc.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gueqcylda.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gosirhpkt.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gjnvhwkdm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gdecegdtd.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gdgabqbgy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gzfhfofiw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gdvumxehp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gtuwnpvgg.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gxhqjpwrs.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/grobrbbmc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxrrobdyu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/giehvfpeh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gwywhxkje.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gjyzfdtzc.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/genbqkmcn.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjeovxaps.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gahvmnlif.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ggzioutnj.sHtML


<!-- 参考信息 -->