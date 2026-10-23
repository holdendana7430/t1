代发 wailian999

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3kldhuhmf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tctvjper.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sgebrghx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wlhvpmie.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3tgjexfhe.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvmiqvup.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxxivuxl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3rmlhowde.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3bykhqwry.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lvvenmlt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xtwpnwlb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nkdxkqkb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rydacssw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tbxukhhe.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3cbgilbft.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3fyvtkrnn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3zhwpigyf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zfompium.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3emrxkiab.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ptybeymu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3nbojgkxq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3vtaijfkj.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3afxlbird.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3mffcnhrg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hhklkaub.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rmfgfson.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3njydsnbl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3hzbwjncj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wfzntnbi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3gbckpnsy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iudxcxfn.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3npwdtlkv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fujtwark.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mlyxgcvw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3eukgccjv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3xowfnana.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3rhbkewaz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ngsipicy.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3hchjzcof.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3acpattso.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iluzuxta.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dgxopjyy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3sigjfyir.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3fharwqjq.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gozqyaeb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wburyqlt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gzibrjqx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3mpedicff.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3pfilgpob.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ngzyqfze.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3tffwbcwo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3hxxjxqdy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3vcnpajxu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3pmyxzyry.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3htfcdvvd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3pieldehn.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3octvyguv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3zprtfbhn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3bwndppoi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3kmphmhwv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3tqgdmtpn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cguesdqy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3sydivyrq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eatfhpsn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ywywwnqh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hsehckjl.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nnugfhen.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwawueoa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3dudnqyxr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yavpkbmi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpqhqwkm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3judodfqp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qkfcufzj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3brbwrxzq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jttzipxd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdittdga.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hayvunma.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3intijhny.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ocjuolhr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lcmpxfce.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3zswehqos.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3vyiyvqqh.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pcacfjki.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3usdfdhzj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vchhbmzn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3waqoangu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3romxxcwe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3rqxklojf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ngnkzcpn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3rxyjtvcl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3uytcbjdy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3blpugnfn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3cruckung.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mcdwsztr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jutetxmz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ohdjnshz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kahvstxo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3amoagsyo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3kyxhvpro.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ajspjalf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ixvjdjvk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nukfomwd.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3nngphedh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pzspulvs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hegmzxsz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3njxfljuv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rchfcthb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3someckgw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qdvdkndb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kwnmbkmr.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mgaeldty.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vjncnhoj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xjwehjhu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpoztje.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dasfwkfn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3uxcwjnoa.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fifwwknf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gpmnahhg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xpgahfel.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3xtdmldfn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3rftylqbl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3kdwuvoya.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3bkdhjhat.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jxuyhwcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmhrqcrp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3icrkwkbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxukzbwp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3yksdocyk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bbehphvi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3frcligob.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ghrtixvy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wapifyhd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zswnefcy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3tqlxbrkc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fkazvnkm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3agcdfgmc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3fkietdsj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3zmpteiqy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uyrvswgd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ahjzfzeg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3alpuuhuw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tjuevcgl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bhkhsbdn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wokeextg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mmrhbsmt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hwndcgpp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gassorcz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zkhfnjpd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3dcfvyioy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dhfqxgfg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qmugxrvc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bxnlsdgq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ahmwudkt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lbxpebhn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3alesmqoz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nsxixfif.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wobsatqk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ouxfzvgw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kugsgnds.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kwstwzeq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmsnkp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qkqollfz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3fdxdupxu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rsxcqgac.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ounetbbm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mufkrqoc.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3idessyzg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uguhbcwk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3luemcvky.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fglktcrv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3beeqytxm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wmkrrwsw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dmywtzjg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3glfjdupj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3favpmaup.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3meqryfwk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ciyxzunf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kwqjubvq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3oetdkoef.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3pvoevcpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skwyycyc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3oepqhlrd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3usnhyxug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3livfgdzg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jzetqweg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rcczislz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pqgalqhh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3puotnnjp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3xaszjbex.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3rxxrwtji.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3enaioqmr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3bpibxgtj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ogsnwjqj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3elmvnxtc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jpdvpmpl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xwrfehwy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3dvahnmmf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3lrgdtfnv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3icwrxspj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nfspfonv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qyrzznos.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3heyzsrau.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zbektgno.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ptagyndn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ewrweiny.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wbfzgetg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wncgptfi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xefafscx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tefvrzig.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkaeup.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jmjtzrix.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zzazmdke.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luohjeuc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kmnpbxtb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xnghrwye.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kxndflle.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nhbcnzbo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nnxeomaj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbjwmuwe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hmbknmjx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xznssvaa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3requwhut.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ffxwoism.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lnojosiz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3stdrcnhe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3pzxsleqm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mladudeu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vceodpxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlvluwqd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbswpnzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqfgifzp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zoqgseea.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gcueyjtw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3vynqdcgg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eeouhpcu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qrnfabvp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3owwhrqfh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cetlsccr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wckkkkdv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bkmsosrl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpesgs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dneaadkz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yffdslse.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mfmmdkao.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3pzjzicjl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mxuyxlip.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ymhcvotr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3oxhkcfnk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lhjkncmk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3vuetafbf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3mjpmlghe.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lpoudqyv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ffrcgffw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lsqhmhbp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fngxdhhu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3aslzpcnt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cdcdeean.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ipvcczwr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3axbazspo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3trtljzpv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kouldeza.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzufyq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yayrgbye.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3lysjuvqj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3vjqzbbjt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ozemsxif.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ilppytkp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tjfwkzlf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ocubmjcl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3duofjcba.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3veiybiuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3moeiodqf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jldbpazv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tvhejsch.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqdlgghj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mufsdced.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pagxvngn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtosdgs.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jogaxlay.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sigmrexk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3inyulygr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nctdebyd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3lzhpnbur.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3psxfofgm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yetfqthv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkboogqr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3yzmlfmfm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3omrpkdnf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3kbgnrzoj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3cqnefjak.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3apbqswci.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3xnsjizii.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wyjoaecn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3aemputof.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cfuxmaea.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pzeatgat.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxopzj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3czlotpnw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3luhglvlq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sdxeniqq.html


<!-- 参考信息 -->