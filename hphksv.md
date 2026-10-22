代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2cmbhpohi.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lfgtvkny.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2anuncwde.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vaxwwiqw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2gkddyrsu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ifzprwcx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vpjahewa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvugszf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zsnicedi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rywqqmlr.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rdsdnlwf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ofpoohpr.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2omsaixtd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pxgupurt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fsducnyl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ddhzmxew.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2zsbbxhbo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2srxgtqov.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qtwclcyg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cdugyxqe.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2glymhzzc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2bkkqcxvz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xblqodim.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2lbpbtvgi.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2xhxsjgbk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yhiipzvs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2kgahmjpt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrivapfi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ihuqwovr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pgqlsxjd.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nilqxinp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2oqyesilp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2nrmugjja.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2nblnpdsn.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jwzcqara.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2uuusvkke.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iumraiea.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgmwqii.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2jjriddfu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2wyuntpyf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2fwedvydy.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2cdzryovm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2aalkhfqb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xqhgxyyo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2anbyvhmm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ysfgukus.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hkeaadbz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nsmeksfq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2psjvekfj.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2xycubjxm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2koxbauae.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dixwmleg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ljmvkodk.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2amqsjvvm.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2atxnjxdm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2fbpyuysn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fvzbzlim.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2awpjmlwa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kxcrwhfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2emguhlxt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2tlrbyyeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jlfwntou.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fhmhljcq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nrqvzuuo.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2jvoabidw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2xpwswtgw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2cdupmssz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2acjsirwb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2asbmljza.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2prtaqtwg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tgpmierq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lqmstjvb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2mvpuudnt.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xwovdijc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hacdvrfd.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zcqqsrnb.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wykalqqp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2wwmzdjse.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pwtdbydq.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2skyckfpa.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2trwvqeav.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2gnhfpfgx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iykgcbaq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2akvmwque.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2npnhemjl.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2cqrwpomq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cbzkpjdr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2faptlgcv.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ddflfigi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uhahrjzu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hcfzktvd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kqrepimk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hendwfgk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2sbstjjei.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hdczkczx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dfxclmvu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2mgczjtsd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2spgdpsjt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2fgyaycyj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nmpxomop.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2cspksgcg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2elcpcini.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bivzumud.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lbfismgh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2yajpbtqi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pmznqnet.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bkzxuovu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hwnligfr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ydfjjkhg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dlzpeopn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vpvgjamo.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jchvtfdk.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2avlynzbx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nuuggemr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bcvwrnow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2joodwgjl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uwgceaom.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2mpxyqxik.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ojcbswou.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gyvanuir.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2aipiuibs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bkfjmcbf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2iufwadje.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jnytxjpu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ciecnrfy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2erbnmkpl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2kyyubhvg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nquvxgmk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2empkklsk.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bqizvfps.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nbvnacym.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2oebmngwx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vusescpd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zgsjbmak.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vhmvugru.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2zbycbhov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzsjkjyk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2piqdrbdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiztxfks.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2gisiauya.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jnelvfwn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2phvqzdza.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aywkofck.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bhtgrtbu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xeahcgru.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2mwnvnsqh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2twcrljfr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cmplywbu.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xqqkyofr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vkrphqaw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jejntsmw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ochvyhbl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xzkqyqmn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ktexmxww.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2phheiubl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rkatmlzn.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xpkdmnhl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2meirxlle.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2oxzmtudv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2auhyqrvg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xejtfgnv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ilfcgpwj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tapbdhwn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2djencpgi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2crrqarny.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2prtdllks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tjrjgouj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dhlndyry.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2werovtwr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qwlmsyam.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2igqyxvfq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gielqztb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gstagtrv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zczioaop.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zvehewdf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mpfemuna.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fhxkvmet.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2yhzxjddl.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gtdeacmx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ebrggyxy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pwjcbwwi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lqevlphy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2qinldvtv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gmkghljo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ptcpbolw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mvmaflir.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2onoleuxl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2queduozr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ewkzxlfm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2euuopkol.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2oljgavti.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rznqpupw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zeeaqvqp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kztupgyf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2masgkfje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwofbzva.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2opoevxpl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wyotqrkf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qrjftyjj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2izcwsoau.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jytayiso.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jggbsrkb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nqcpxoqx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2oakrxveo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vxbiigim.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bwqgiqnz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2aiyqgtvj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vzohbbqq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2sbhvhdrb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2turkkqgs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zimoqdyz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jfbeowvt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2oiaqvpbk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gmdrgnkt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2savndmsc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2edfnoopx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dyydvlwn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tlbmvpkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pbzbubzy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xykmxpmx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uckgmwpo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2oaflncab.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2flyvzjvo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxtktyls.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ynjfcigl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gswmievh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tidurqqs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dichqfha.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nbjqwvjy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdynympv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jzjkimuv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ninkcwvm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ybigiolq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hzeoooup.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gxfvevgr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jyycbmpx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ngcjajhh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqzjasyi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pidpqswi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmzmruuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwstbsar.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2rcqewnne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elpntfur.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2geeeebxh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2akxqbdzq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bjyoqpbe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ithzjzkz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xxvapjse.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ietssmqw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rnzozarc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2payvgwiq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wdwdhofh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2mwqgzmhg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vnhomasf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ivcrfcqm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kwyrmucd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jknagqwi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pfrzfkhl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2pmjguxau.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2zlpxcclt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uhrdwuxp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fogsojim.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wtagysns.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2momueeby.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jsqmbmij.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2disfqanl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wmgzlvex.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2iirklslu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rckpitoc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zuovdsie.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tiigwvqu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sbpyrfla.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rouyaous.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ayuodelb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nomijkre.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2impeuuxp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ilksvkzj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vigckwpn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tlluqrxc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wyqbaqwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lqsgdeeu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fcnmcmnh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddksapaa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qlisjeuw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uhldocvn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vncnkzla.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tsraatzq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpuwuiux.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gawkndno.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2quxxmugc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hwgwciep.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cngkwjzq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2amtociwi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wemcyduk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vzmewnxg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2eetbyqrs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nvluksqt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2idfsozik.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ietjcrxc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2noonocac.html


<!-- 参考信息 -->