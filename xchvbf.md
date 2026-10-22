代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggbmzyzt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2whreioag.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fuphiphz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ttjwxgmp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ekutrtkj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2vmqwkyke.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dnxwganp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oclmdtcw.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2gchchqub.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2agdbzhay.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2iitduzte.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wdcqewyv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2wpkyckvw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wqyiwxsq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tziygajd.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2oxfbfffs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jwersklv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rlbvdrcs.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2kpvdjfkb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2utoaacwl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2uwphmhgu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ktulxepc.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nkzybyvf.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fjszdryu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cprkyuwk.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rfjxeiys.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2pjixeshd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyubhzyh.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ywjevnjk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yihlsrdz.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gospliqz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xcldqecg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2gsnnvyhb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2utnryvzh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cmcsetgx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2msifvdmy.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gordpveg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bpbgowpn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ibnplfqf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kqpobfqs.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2gwwdolwz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hwkrxkqa.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2prxmpirm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rvpvuqto.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lhxxrsed.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2aynttsfy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2jxohsevc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dsubbdob.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2sabplsgi.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2npsuteaw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hpxhojxq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ouarwwld.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2knbvptrt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2ybcsifsp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2razbbftz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iztkrfej.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lmigqjxi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2rfhbapie.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2syykkrie.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2clvslonn.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2izzckpjm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2vnpyqrgn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2bwlxhwey.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2agonziek.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ugyfjsum.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wtopurag.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2suwsexcq.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zakuopbb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2lwydnnwo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2luykamxd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2lyxhdhvt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ammqxmet.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2nsixkmdh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ebjkzriu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zscrandc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogevaavg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwgxif.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ghwtrdjy.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2hekwufyx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jqsddtuc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2bzqlujcg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2svhdvjhz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2nypsmpyh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2gbuexuan.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cqvgnbsz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2opbzkpkz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vrxpvbnw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2erkfqdsi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2sbkojejg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hunjtrpy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2pzwuagll.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kaklxhxh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rrfnambl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2fddtocmd.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwjwewng.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2txbjsvkx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ojytmdvt.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2zfwfoitm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtxcpujc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2odnelgap.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bcqhthty.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2smxvnjbp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hnqyhlab.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkegopzt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2peqioedg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2skvdzasy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2auxbpade.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ioxrsopx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2eapkgjhg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ptqrekxo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nbflkxso.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dyawabsx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2nmqtqbwg.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2szdpdbuv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ghgmmrmq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yjqqvtbq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yknfwdgx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ixfmhaxf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2swtyqiat.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2twsehbwc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zpxjmzqb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2letjtowy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghmrlods.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gfqgzcnx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nljrqgdu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdaaqpa.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fdvwnwbw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2swkmhgdv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iuxvkoqs.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kozxaxaw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2sprypnas.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kwfmyipb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vwiqckin.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2itehtlra.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2vztrfanx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdbtunr.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vftfgtml.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kcgzxybv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2umttelnq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xcbgvkow.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xjumvopb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2txhrusjq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2beabzqpn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txvoujxi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kmatnuwz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dxbyziip.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jbnwziju.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2koagqrgl.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qkvnevur.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2gozjvjad.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qwuaxjek.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mzonsocz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxdnwgeh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2etgvhedh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2meoxlhci.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hopnhdgr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lghiwqhv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gfvyudfp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2nubpbadu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2rvtwpixm.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mstlzunz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2clgrazjm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lrhpaspb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2trrlkton.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ojwitssv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ctkupgvn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vkgyasdh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mmlqkwsu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gdszmzsz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mxwsxgtq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2iagxqdcc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ycgapear.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cfrcewrp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2prijovcs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lggurbxi.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jcdjswuk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dwgspmiq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kmatzosj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mefvtwzi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jcjabmon.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rprukwcm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ipznkdkv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vvahnkdf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xdkzdhbw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2swskwjmi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pyegfyhe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kfiqgnwj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vgwebxqa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hzbpasdv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lnfnpupc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vyserjlk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rwurbpel.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tpygoixm.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2awtywrgw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rzjrkcnr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2luovnkfx.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2derngwcu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bwtlfgwd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2buzhvpxa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ambzbkxa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ydsaimjb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ivlrjata.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2cphonock.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2iiqqwtkq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ekmuttfi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2bcivjctm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2oyogsnfd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fddxavrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axjwlorf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qpxableg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dkqfbpcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvwihysk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2irwuajlc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2fzbzwrko.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2cvtipstv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2bwvskksq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2phtcdcxn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pyfxhiwe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pgkighrr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2aabcztce.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2iheaqbse.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xlftdyuy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2oatfqvrd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2iqphmbdg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2luitxwvv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2ucllrsmn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2omnluzyd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rzhletqe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2bfabojmo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dpixsufz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2kopshgse.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2gjmczxxd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2htkhorze.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2wldziael.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iivxmwdj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qfujnetw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ymhsqunw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znkhyrzn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpciojjc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vfmrtjwl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogrbylsr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eugdcvwl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qyixshkn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eszyybvv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wwlsfvbc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hhvwfnka.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xexnjxxk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kbubnwfx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xosvrzae.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xkifmspx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hyplwyqd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jhnirqam.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kgtbtcpv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fipufpqs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bopubgul.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utxcuicd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svlhgyzh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewtojbbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxxaxiwp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ltllquju.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xdxuxpao.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2wcchgnku.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xkzixrdl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kdiwtzoe.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mssmmlaw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sayhuxtd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uckhfxqv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2eyrnihwm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ywbpyfsn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fqyrdurh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cliutuio.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2djhuzhdh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ptpzrzjy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2znzvcezr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jqaghrpo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2eqmujwnt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nofxdgjh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ozwblvne.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2smlldwsg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ojqycoja.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fybvmnva.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kduojdjw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wpfniwkz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ihhmiala.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xyggcbmf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wqgarqvh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2teopfjho.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2cfxubhef.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqxgrpuh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bytjtnxa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zqpulipe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wsbijqhk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vbfzurud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hehhjthi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zxsvhwho.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2apamfxwf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bwrpatte.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iplsxlei.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtxwevhl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dajahqlq.html


<!-- 参考信息 -->