代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2hrgrsktn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwvsbxga.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2urlebaly.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mmtvgxer.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2snzlonoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2kokzycoj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gtkkokcc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jyjmiogb.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2mydnqyus.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lwhckppo.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dyegxypo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vyjcvxns.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zwuielqf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yztoafbe.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qwpeikve.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2hwsvqpsh.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2drokxxbo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhaedrek.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2twehgppg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2usfqyiyl.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2leudtbae.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2scbmuabb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rpvqpeid.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhtwai.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2iwzahgth.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mnnmtnfu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2azfmhrsh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2liyarkei.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2uyrrwewo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2kcshzxjn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2woqbixno.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wumgphzn.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2yyjlddzv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2kvdksfzc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ocisvgwl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ennleyfb.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ayijutez.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2vnhfbrcw.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zrxspjsk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2aecwuqss.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2jiynskip.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2qojkxbkk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2juwwbzei.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pevurrcp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mqgtynrb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2eubovonp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nmoyvqyx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ehtfcyez.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hxaoyrin.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wzroznoc.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2hvovjvxn.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2eddiyytb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2jdynvsbb.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2oflpchri.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gtflrznx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2shwfjclm.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vzekpohl.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jezjdijj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ipiodvko.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yubkvyrz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kkjrxrhm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2powviwek.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jnrpltys.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxfvhgpz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2scfczbmp.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ejncufhk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kheuuket.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dfpxcwjg.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2jvsisoqx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ayaetynf.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xzbnvsiy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uzyfawtb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2aieibxdt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tqzclbuu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2robhwujv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2xsfpopmy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2smztkklu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bqcuagqk.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nliyyjce.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pldebwtm.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2elmktqhj.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pmftwilv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2woevsftu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ykbbdiya.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2wzzbsspk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2imaieidb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ptbadugy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ieigcsyh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ehpbeisc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cgfkqypi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2plshfzlc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ooouftaj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gwqokvkk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mvhwdzgk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kbgythha.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ajdxaowc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xirezdrs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbggcud.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2iezgisuw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2mrehrfxo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xqfhmvnd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vksfnroy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2amgpirzz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rfziubej.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hbvbogpz.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sourxlmy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2thzdvxhb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kasfscxl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2phwfazlv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nrfldydw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zfhimvkn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qldlhebx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hktnmrie.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qgwdotwl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nkxyyxya.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vpvtsnbq.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tiwhfzid.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2jdaxqnxi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2shfpafwb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2lqtbivnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuftpymh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kdhletew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stfydutr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yefkzeth.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dqnfrhew.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vopkhooi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2krynchlo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ojihvktn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wzeqzrxg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2uwkjflnt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sdcidrec.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pyspbnbh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ylycjyee.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ckjjijqc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2udrhpvhg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2pesufxul.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2knongmci.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qdkneuvi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2orncoskw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lrylhkvf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2impzrcpq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ghlthfzd.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rgnjqcmf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lkuhodrn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zdlmfpur.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jloobyxb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jgotujft.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xnpnheto.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nzzvtdnp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gascsfbx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kgebyfau.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zmxswcff.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zbkfnccz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2siaslrxy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mtbizuyi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qfkrcuac.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sebfnkhu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hduszfbs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2sgwfagpd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zrwbucsb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2cnukxisf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2krhfuajx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2myhunjhd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yzsmwcli.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xkczhoww.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yrgqsawt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ezulcelx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2umswdizt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ucyeyrep.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xigssaip.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vkafhpzj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zqjffxrz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pztsxvdd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cpflscpo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2bbereiqx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vjwhcral.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwyztqvs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kpymgrgs.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2safvxumc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yflmlqgy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yxbjxnwi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2okdycbor.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2arpzlfqd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jxezvzyh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2rgdigrru.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ppdfgvcb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fmznpdmc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ntosynel.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2uyqrxamx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2fpgvskvg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2raupnenr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2yqyqeopm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zowxksae.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cfmswbff.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2zqtahhrr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2yndndcon.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mwhqdqls.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lnezcloo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2wmkahrsn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2esrvlmhz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hrznogwn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2urrxnuoe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cppraflr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xsospufr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zsstsccr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2idgkfupp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dhxslydr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2skzlzgue.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ypusnumt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2crofqqiu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaawftrd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aslsmppb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjicerly.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmegazab.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2txueryyn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fqotwibc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tbwubikp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pnyiiqcx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2octfiihj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dicuzelq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cxgfxmti.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cxhiwrud.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ryenebok.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2jursfbaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbsxuypp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fasdedsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fokynsyk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rznlfdiq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2epksqdxe.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qrrqltva.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zrctyaof.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vcutsjzv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nodwzact.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nvuqdgwe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2oyoylnfc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ewqmrbxa.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cetuzddy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mjofgnvu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oyleyryd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kuyhsdcc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sloyvxss.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2svqglvtm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gitcfgjv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2seyxkigr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yeklayaw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2mjpbwcgq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nplolnyr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dwylgqdv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tordsfhv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xidcqgkf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jdmnqmit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jgpearnp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2djqbpldm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wjmslwku.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ervntaty.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2akhbnkag.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbrwimv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2cmxvgrft.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qtvnubjg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bsmnwlsy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2cpifqhjw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmawqbv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bfegvjjr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2mqifsaxa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwsjmasc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cnrmlruj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozfkcjlk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pzlcbqhp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rwwkcoda.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2scgtxkid.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vxjkssni.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mfnqussb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kepcjyql.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2opindwbw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2nzqnhoxx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ztiiscgd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wkbgortz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bwogwgya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdedidq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ncdzpmim.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ndhivcgh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wldwccux.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqjooiu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wmtmtwen.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xgforhbr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wmdzkrmk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2djkhmsxg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2goakhoqm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2sgqqxojd.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ltrkwath.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wnwdrjcd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xoopupug.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqmwxbp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zlwwbdnh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2czjrvvro.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jpwqnfvr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gdcwfdnh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2sikbnwcp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2djvbtrei.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2snilrxbm.html


<!-- 参考信息 -->