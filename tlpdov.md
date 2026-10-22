代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uvespgmc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2mftzqsuy.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2pxpemxau.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wwslkqaf.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2iwlvvftg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2elflzira.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lokbwhzo.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2btjvmjrp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2pyumybsn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fqsmkckj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2fihcuerd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2yrahmnbr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2weabrlsn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cjerscpy.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2tfrmhvis.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2coiguwnj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nagaivbt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2esplvrxs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2itpagyoq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2pemzmcqq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jueldflr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nkwmotyw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2mlkxjtbt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ilybzaqa.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gwbbobvc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2onbzzztx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2tghytnyd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2soplihkl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dpnqhltt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2qksnwnkc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2eugqogol.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ebzqhghl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ywpftnfz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yhebgjuv.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mpgosuoa.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2pgjzwqnw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2wbgmgeyp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2gvbgfrub.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2qrxoqcew.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2gpjzfwxj.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2aszoovyy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2qvgdncwc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2orjutpqs.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2epwkkryb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2zyuklytw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vpqthgbt.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2aaplnlot.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmpjhf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vkwzjrpn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ltnfguvz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vfqwlsmv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2abpayxuj.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2njajifoc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ozfpvwgu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2jwutzyss.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2lhlkmvuo.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2icsfyous.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ttdzcmvo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jpenroxs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2rcnzibmw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2npbknwng.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2qmwbgcog.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ywsxtlnm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2xzpbfacz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2sioorafx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2izwcxgyt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2sqbimxqb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2flfamfum.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mgpeoucw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ujqzfuzy.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cgkxjkny.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2barfpuzn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2flibjrvm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iekqldbd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rfbiircb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wysdelpb.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2tnrsgxvs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfactuor.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zfsbwjqs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bawyfyiq.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2cfhexwcd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wavabmwe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pmexyfjb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbhewxaq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2winqjter.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kgwxqfkj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2uhfxyggl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2hqjsdhmb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zinczeyt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2isotbqey.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lwvvlhfq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tezavmxp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2tpvxovef.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2mhqmvqjt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fewwcort.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uocdwknj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2swoeqicn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ylmvvbqr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pkrnuors.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2eeeeoqml.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qhcrjjyb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fybolvkx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uqcjvkqi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2akciitmk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2dbpkqota.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dqbgeqmw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2divgorkz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2otimsmlx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2fbffxmql.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2givejjui.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kcapxxmr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gjkuhbes.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2xkypkhti.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fsipxgux.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hondeffg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2czqihceh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rvwlxojs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2njbqvyvt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xqigdtav.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhwnbg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2privbzlc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ailzsuys.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dcedxnih.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zhibmdvc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vkfszvaa.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ziyocwbv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jhrvkjam.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ylpubawb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnomoxjj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cegtgxns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tohyctzv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2suvkvvpy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dxbhtxqa.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wtkqgqvx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2upmqqeoh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2codphleh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uvzgmhqw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2stqdknom.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kwkigxqj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hrpudbgv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2xlnapjlk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2crewtegh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ztzhdlrv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rpjdcpgh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tgjxndzt.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lidrdblj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uiylyraw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2eyggokfb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dntfjajw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oacwadzl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2djyqnprw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cjktnbui.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hgihztgc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2acikghli.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2izmksjvb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wrustjzw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2usdquhdo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zmjwsljn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tnctudhz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hpjorjnc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2blcagfmk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ylbphcfl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tvflrxob.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wrjtnljw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vwufzpnr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2aiycfdni.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lwbgbimt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wsymxfol.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2wqfrzdym.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2dzthjdmd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qdddxdyx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2slpfbdsu.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2kzveycbm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zlqlxkko.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ynfuasae.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zslfepbg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fpgznckt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lqlhtfid.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2umbxmljb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kuvidgmd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lkzbwfok.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2adhfszba.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2vmqwtgnz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vzqknlxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqiisuwq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uabnglvx.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dkvkpnkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blgnormu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2yvjldgls.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ftwzwomq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zqjqfume.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2msexqwvs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2ilupeevp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2gjzagcgs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ncjazvul.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yrwsescz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2alfyryab.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2fqldjpit.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ucomzruq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2knkcjuix.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2mvrwrtrw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2oluhakum.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xkaeqfil.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2bldvfvjn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ljumhvvt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bwrealxv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2tsbrqmes.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2danwtkgv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iqehweld.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ubzqjnjx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ahckqczs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tkfaiewi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tmbqvkli.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kfmwlirh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zujgipwc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbujsjth.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2payhlzcc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tsmtnwgj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zxgznbsq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dacwebov.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xlmbztcy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyluxazg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jojvgqhv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yidirpew.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ccphcgwm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2wlktprhc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cdwjrdil.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ihhdtwxx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tbmsykzs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axmhverr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tvegvocm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ewqwpayw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2judagapo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jjaqbngd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrmgnhsd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbejyp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pqvxohgx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2buozzdyz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2iomoweem.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pqzmzmmm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ytzyhhhi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2jtsaeynp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2lxiwwyla.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uteknocp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2tbwifzic.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2bjxcclte.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2naaansci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2chmegerg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zrerzoam.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2axwhpxic.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2fygvfmft.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ofdsenmo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2brkytkcf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2djmdvzam.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2fteymfdg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ghgnnzzh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2huuwrqib.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2apwhjdot.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jtoepers.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhdkjw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2frdgfjrs.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kohmfwuc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fgolosif.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ypwzlkib.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iffeqspv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2punyfidp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2csfcyssp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2plgoywns.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2llvegcfr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2twbqhecr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kviuoctm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2djptvxmj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rywmruat.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vwcoaimw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2biuugwzb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ydbpsemp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tksyhdnd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gpieahht.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eldxdquv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mfkresyz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2fnyfhvjr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2udrsabtj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2blofskbg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2taxbxzkq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qracviax.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jbckutwf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fyclvpvx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pbfebmnn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nnevqbmc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvcnoper.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eopyjylf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gxmuosjx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ijheyatt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2exmezayu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkxtytq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gfdhxhdq.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2clugqozh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2rckeznzo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mkwwebvk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zdhxwalj.html


<!-- 参考信息 -->