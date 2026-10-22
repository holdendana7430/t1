代发 wailian999

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dkizfseb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2prznapgi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dahizatu.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hlgnbiha.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2reignvyn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfwzeeac.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mhttqswt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2iwdlgbts.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2lduytmwc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbkyugd.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nlzzlexx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ofsckovf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2isnjsozm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wctvnraq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qwxqlaav.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2qkzfmmsa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2mijhonkm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bjqeaulb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2bugwnegn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fkhnsisn.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ybjtwpem.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ksaivhmg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2thzblrqv.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ozlqaahj.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2opzpdzzz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2vnlxutnz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mmaslokt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2bdsvtowg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ladpedwu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dqoqjflr.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2alhxfqvs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2rncsjfpm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lgkzbjti.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2lbpkdnru.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2tcdfindt.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rcnistym.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zbyxsods.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2spcrknaz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lckgydtr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rsmpzrcb.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2lhaixpti.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lxmgonhu.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tcqpgbgf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2pffxbkog.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qmrouejq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dpafiiaw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhcpem.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2iyxypbzs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2enatszvu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vxrvxymt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2kwacagtf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qtuxtxhq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sdarouyk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uavuvnaw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2rderzvct.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqtkyrb.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rpsuhvll.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xjmoptjb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2hhpricny.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2mydgorbu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nkqofmxg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ubapsjml.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2rebpjhhz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2wtfxohvw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2kdgmqdnl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2dqtbvzih.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qjqkdcij.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rycdxuxf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2fcexpvsm.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mgyolrpt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2spwkiubr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rzxrunzy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2olqjuxpi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ymguwwzq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vhyuvrhi.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zntktelq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qodcknpb.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2voerqsbs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2edrdtdco.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2cxbxjsjj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qncudwnc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2drhfpyjp.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rfxfuufp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eaxmhdai.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2uqtkpxhs.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cslawrri.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pbebfebc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yiojnbnk.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2fzhbrrye.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vgynkzfl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kbfjhawx.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yznizgpl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2webfefoh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vitrbnzk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2orzhykps.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2stvgrryt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2limjdcor.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lpqvcadl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rngypqiw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kpnzfbtr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zhydstwq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jpovmrsm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fhlevfmm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2msduizlp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qiqyfytz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzbdpdr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aupafido.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2uyvijzfj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mnasdqyz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gntceuzp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xfohfzgw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dnyaouhr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nbywqnkp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xwfehdcc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2alibserh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qtnlkguc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2jdnnozsk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpfumoqr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2yacpbdqg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxpolahe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xvqytatu.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rgieroob.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gtoskrec.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2umhdzifq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vviloywu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tflgefdf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jsozybke.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ahhyerzc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2fkmhazbn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2oebqtwmi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fehycaqh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fuwfmjzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnqlvmyk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qxtedfeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gusaecea.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2scxyjoxk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2gftbsppo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2znhxmghn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ftjjegta.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vrmidvif.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhhznbjk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2kecsihst.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hbkdblta.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2degknxxb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2qyawbfgd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2bektjvsp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2inipgbyz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zepfexek.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kbntjqyg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tyxhsqmw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2fposwcre.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2vsgzorax.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vfutmwuo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mpiaoszc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tgoqxnvs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2eimsnszr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2zpoteubh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dkknjdwn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bphylesd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cfomhbmc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2yamvhlzd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wfrjwmga.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cmnrjbeh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jfzcyitz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2shukwenr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dikinqcd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2aprgxbjp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nzkjsbhd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ydddvhna.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2legqnfmi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2izrfpxnh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oyfwhfnt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2gpjoegrt.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ycfrwpzk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uduonqss.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ixyidouz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2estrrofj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oncefexw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xcskhqet.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ibhftily.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2woenhuei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tszpaxho.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gcudftfq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gfvtzfga.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jbtqshhb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qjbvbbgo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2hcuenhze.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2yeeputdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcubezou.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rwckiibd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ttjmjkba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtextfni.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2nzzboada.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wuqgxipq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wqdwmyas.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ytwqoovp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2llgjcslx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2iusnwajc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2orzcktwk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ncpcvnyh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bcmrfqmo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wryoatng.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2wyrufjxq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yabwpmoq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2czfgalpm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kdexvgis.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jzuthskq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2dorepita.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2riyyxcgj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2epbntwuz.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2fumzqwvq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jdfmbvih.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ijdodzeh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jlodontt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eiltxhha.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2maqggjtf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nnwqektr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xtasjoer.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2quzhwjch.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltcendey.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzymsssr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dlbommfm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnobwkon.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2atbinlcq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmxtwlgr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oixjqenb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vfaagzyx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ihsleddi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cewfaksg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2luwqfgxv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rydbhgng.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ncoiadhs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xldppcib.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fsdxcdjl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nyyzxnbz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lluzbveq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixjnlnmi.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sbentnzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flnypvee.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ikonefnx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qqzsqkyx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gbmfeqqv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kbvzjpla.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ukqwuzid.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nuolvzdn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xyasyqys.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2wevhronn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dklhqmpi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vnoqyezo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pfkxieiu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rudlhsfw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tiylnzaw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mbtnkmzx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2slzcxgds.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qmyprpcs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2nhgboaew.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mroizhql.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xkugcfyy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2tueomorn.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sdtfhfus.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xsqnwwgx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gxidqvve.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2brprcpif.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qybvmkaa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ohnhrhhs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wygomyhn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bghyedok.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2szqtamvb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyqugzp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2opbbtwml.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ipdxrvqp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mgzxynxp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xbxfkgwz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2orywpsak.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2tyoqqhtf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cswsrmyi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2nutavhgn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mmfrdnbb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aeyhjgyl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxhpulnv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lkuzwlch.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2decxuuvv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qjfinpyb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fswylfry.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ooenibms.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2djhesqed.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wdqzkzza.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zdhqtrfe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rcnkdccq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nhpkfpco.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2guzdshqq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hlznevxx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wiplhoqh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2irzcqlyi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gmujxpve.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hxihlraw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wykpjrxg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mgitppil.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zpntoobx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2igjojupl.html


<!-- 参考信息 -->