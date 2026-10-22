代发 wailian999

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dyogmdhc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gazyusnx.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2khnoloik.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lslqkgah.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2oxxypgaf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gcqfnhtz.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2rylxpnfj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2fibdfzny.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2lndtkpbi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vhftxfsx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2wpknwiqx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iljottao.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fnrovvin.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ohgnyhuk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ecpopugj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2izknetsa.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2qggxdkou.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vhhtluwb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2oqesolif.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdvqibkq.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2poihofwv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pnpcaoka.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ripfenbq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ggbsbduk.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ahfmrfcg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ntawefis.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2nrsmoove.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2wujggxyz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uhroounw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2mljtnccg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ygzpmrwg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ggvencpq.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2kcvmrejh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2piaofyxi.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2khmedccz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2yuedfjns.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2eoymiowy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tmnoappn.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2tjtptqbn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2tqkbcidq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2vylocnix.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kswrghrt.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2esccmxnd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qozjcbrv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wapaekhi.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kfwdaysh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2qxaxihdl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gdvbeslb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2iuduqasx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2izixcewb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fpksrxyf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vyeodelt.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2tstfzdjp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rrpffpql.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2erllqaim.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2dlqybltm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wdjbhumk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vtnkwuie.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lrburamy.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2isolzaal.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2yruqemcx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ambtfsnr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2scjydnsq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrnzxcu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ulysygag.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qdpzeino.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cziqqigb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvoqgcm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2rkgjeqzq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2lzznbovn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bdjpqyro.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymksolpd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kwwezhso.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2goeatdwp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpgarrfp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2eoeygxyk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2rdotvmln.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hyzrdsbf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rqptmnzc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ijijoswj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2minvppvc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bzntjsss.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2fazgrhra.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2pykiqiyy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lbburqsh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2istbhbfe.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2okzaqupn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2nyxfepat.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2jorrjbqb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2rvveujhj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2idgjysyj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yktlsthc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2yuchrvws.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2egxfjtsn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vgraprvp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nifidpwh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kyooqrwv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2efleytfb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cvnnavwj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bahikpma.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ndwvyirx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2buntzsje.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2doxeidam.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rowowasc.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2swiadlbc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qhyxirsf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rsfkjbjn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vyqsvaxd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2pjbvuiap.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yujpaeym.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2onlvugmv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2noczmxxo.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ydyqviwq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zifqiylm.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jmzcndvo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cqenuvsw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cbqqpkdq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2tmxokkzn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2pvmzayla.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdxuwbto.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2smtxbpju.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2pxpzhmab.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qobaflxf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ohfhebnv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tyqxsbae.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ngdhwzmr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ftgqeyxj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fnedcwxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lecsggsl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mkdzyiyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcwxyeaf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zpziamzn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2szcytvfr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2pdcwamqi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2mcqpmvtl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ybwayqhm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eiisbbmu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2evylcuab.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bkkvxymz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2brgcvncn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2aczhykup.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2setrajow.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dgzhwfds.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xognlbbk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2srlsdsjf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2eiffoxvc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qmsoifgm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2oevippku.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vlmybekl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ofvolaha.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jqttmxeq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ohvnhnsz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mjlmgezn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wnoiutpv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lndfycpb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yceiwhdm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ibxebysb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tqixdhjm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ixmlqull.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vabqaqid.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xscbgzia.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tbdpqocn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sorchsxj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uxnticcx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kfwhqjhl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zvjqudwj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2gxartmom.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hchoxxti.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jozcerrn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mmndckbs.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kuzbzqnm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ekqsdhkw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wvlufgoj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pzvpwzqy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tubdmxyb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kaqxranu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ulakklww.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2swdlkype.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tglvwerg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2rvivjsot.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zdkhgcgm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2svdbaagn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2pktcngsm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2aabamppt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngyokrkr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xpadfecg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2aaddenfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdzqwbjc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2mavxvory.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ghrztkzr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2yuuhcqhx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2wskhvkgs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xhnimzmh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2zbqyrhdj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2aigxinda.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2cmgffkyy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2lrmprxrw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lvxxzbnk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jbortyrj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2hmwphtdh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2dvlvzlfk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2newjgdku.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qgcxldrd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mxccxtqm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2yzxjcata.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2hyevnedu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2sjvpjiix.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qtcyfovl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mhqanqtu.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vwvipgkl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rvvitbbh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2oxahgupg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vnisohrk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evfpknqv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2eblmldmi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qqeepfzd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pknnvivy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gzchlvwk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znqyvqyk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axakkmkm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxmqjssz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cktdtfeh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ziwiwjxm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilqwzcfi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nlfksgky.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uehlabyq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ouinbnaj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bcbynmxn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wxlxrgjx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wdgxubsi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2xbhbbwwc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dtcxswuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwaemzvi.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqymxtge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzybtxcg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nrtafhxt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hqgwdhla.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kyyyibfb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2awnkagig.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2eivqtkjq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ktulmjvm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cbuczkvy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kmbmypsl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mvcgnyiw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ewwuawqb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bxgpbhjh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fqmylsca.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zggxccdf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qhxosepp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2swkkozkm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2oupmddhv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ralagvcm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cphrguuj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wuojzzuf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2zhgqssjx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2waikmlip.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zjsbqvpk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wrvpwbeh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fliesvjw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mchmimln.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nnvwuddp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wiqfjezd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ltqtoddz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yaprmsej.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2imbslwwf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eulmzwzb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kwqxunjl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ipadaseq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2auqubpqc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2yhzwuuvv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2txgdclry.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gmymyavo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ljrshkoo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ujnsqeio.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2voauahwh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tixwaewu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2itvyanrz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jpcpygkp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aguomtfh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qmnlncke.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zvzdtwhc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uomljvlf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bhcngmks.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wrpcurwv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zglwiwir.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ccuumfba.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dileeteh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vsgnqphm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fpbibifd.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2lgnywosi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2yzuzlynl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gquwqvir.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tbpesdfg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gnzpilvr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zltssrme.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ejzoevgj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tvfmbbyo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2zfdsdoui.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2igsmdbos.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vwfuzigc.html


<!-- 参考信息 -->