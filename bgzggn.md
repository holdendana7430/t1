代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2fqeablnh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uqobivnh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmaxvmgs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vqnjrlpi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbrgmexx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2puazngzn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mkbwwbqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjdxgqta.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nzynufpy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2adqeqyrh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kmxhkfwh.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plgqprch.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rxxydkcp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kavgohpx.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2atgvdouw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yemlkmzj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2pmbsdqph.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2okdnfklo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ukpjuoif.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2wfhcsmjn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dpscesni.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2epdgrigz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ropzyxpg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2megwfdhx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2agrfaxwq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2zgtdpyno.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2uwkpufpy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zavbcwer.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2qovnlela.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2peboqtqs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2xannzpmk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zecnyifh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2yqmqrmax.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kzyhkfwd.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvdbku.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rahdqdei.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2spovplsg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hknndujn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2npgtshlo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2qmmeynfu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2sclghgti.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xuqlnhhd.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2ghrjgfoh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eyshcndy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yuqobofr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2azjvdkpr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2voeqmitb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2tinikdda.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2meueagot.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2fevsusgg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2mepylgqd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hmkylnav.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kxgggzwn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2esnztrxr.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdxtgf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nhetstam.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dlbjowyo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2qzsleydj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ffneggmv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2xugjcrbe.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pqelswon.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2yrtnxzke.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vujpfcfi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2hzzaflgl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ktthlrgw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cxwyjkiw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2avsoucej.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2vottwxkx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2kejvmdlc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2alkdxtwf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tmlijcpl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gpmogkru.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kxbypufq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ywpourdb.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kaxyecol.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2egcykgow.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2xwrevmor.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mogebpvq.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ywqaebis.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uqjaynqf.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2shtfcuoc.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zhndrzhf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2kpegjyvd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xdzcmfmf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qsakgwma.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ahooskjk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kmcgveoe.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pcprwpet.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2itkndsjz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2idmfeebt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2suhvhnzd.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfjcgqbs.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2feptjgxg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ndhxgqeg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ybxqzpkm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2irlvkdjd.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2vhubdhgw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jkonnvxz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dgbllmqg.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2syoljnrn.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2rancsmzm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2okowecrb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2blqrtolz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjepuef.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jywazami.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pcwqrflb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2eaolfmuj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qbeitjas.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ywcwukvs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2yyfokhxd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pcpjsdlq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2trwbfrsb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lmfjftaw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qakiootg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2quislnge.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2czmbrugh.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2dpfzebkl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2owxuvfzc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ufagodrq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2svzodrbh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2aztsblwg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dpqqhkgi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ccyoqthu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2letjmkyy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zkdbtkpq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2oauhofah.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ucmgcmyq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rzwfbwuh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wfrihcja.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uiazrras.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ixmmckjc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2jqlwsuoy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ejzqaldw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oagusrpx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ejuftcvd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kocfgnup.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ohcqrfmp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2twtmadpj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ecerhcer.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxmzkoe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yhrgxkop.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2totnvrev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2htkfkbqf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2asjezcwf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rbeyuhxz.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2gfiliule.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dyyttqrr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jhnovapi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2mqxporuz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oeoqmrwq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2dplakskz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gojbopzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkwgmiit.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wasaildl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgdxptpz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2hmmdpnaq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2srljcbne.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hpbjgxaf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2fypxmqby.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dxykknys.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zazvywzl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iqvjcbtc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ovjxpzoa.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2guzjmzpg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2gskvkapr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tthnmzpg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ilgzdalv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bcsiwzga.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bykcxaho.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kvclyouy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2vilgdury.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kuaumpsj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hozyzysy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2exppcjgd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2creskkly.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jfvtqhii.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jqvpvwsa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gxyalpsc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ycfrjvyo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2anmsatfd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cmlnelij.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dwxqbdbn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fgyhqcdx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qgdbxmad.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rtmqesoz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nksyengh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mpechtqc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2utxvqykg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wgfrfoei.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xnvcjbeq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2yqcyqjff.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kosttosg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gteciilb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xgolsvby.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2okcasmfe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2whdifrfw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lcxjvdxg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zamqtwyf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tknxcfyk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kfegfewa.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2knrgmret.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2icgyamrq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ceowympo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2amujkrro.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2aqpbdeny.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2spchfmxn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wsbdymny.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fgaxaeph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgrbjbku.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2utaxshbu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dzpvatvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phzndryf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jtzqhttn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2yjzeapgk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2aoujamoj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yryhfosz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2pjmuqnyh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnrqzy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yrdzjlae.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2iwvxaewc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mahvcycp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gactmzaj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zyzliifz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2tnypasxu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2avkbpjkg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tauvginb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2djtsggts.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jwdxyijw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2qrlhpabv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ytmtgfdc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2uejyubqn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dwkslptu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eigukyxg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2axukloto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mksrxyhh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mohpmgpu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eexmhxnm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bjkerdpz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ftejjfhf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cxrmbjnh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2luifllol.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2apyhkuil.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zphjkeot.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jebdajtd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcrfrmnj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bephwqjv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xyerqztf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrspzuon.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gxyxhetk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2akclnwiv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wclfedtk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2irvqpbut.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gwrzypsu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bvjnczsx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aydfiruj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jesmncmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwdvwask.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wetkiscv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzivhwfb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ovarafje.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vovcnwqp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2eahtvpcs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cmrpzakg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tqxffkee.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lgdawunr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bxhqpnup.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wfacllzz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bsflpmxd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2wwxnoole.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lboufviq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wddolhzm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sdlolrfu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vrpiwcks.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xesouoyd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2fkmefemq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2cwegzial.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fegdczgv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2eeuyyuwt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dozfikqr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qqsplrsg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pjmrptsp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qfppmjyc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ccdjprqe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oswxtpqg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2semurgji.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lchecmwm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ehnhxici.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jblpvsuy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rafvwsih.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xzqzzvti.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2avvarazp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lcgqhpmd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kdinjcbw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nqilhkse.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wwnktphe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2uowgylib.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ygonlkks.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhgmwztz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cfpphbas.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tobmbsuf.html


<!-- 参考信息 -->