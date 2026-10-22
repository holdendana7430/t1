代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cpbfgcqc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ajbhibrp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ncccnnwv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2uawzgrkf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2prlnovkg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iauccoti.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qnfmkvke.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2dvcwqlub.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qfkybjko.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ddoeuovp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2nboafmae.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2faxnrsuo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ydiiqitx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2laesjalo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2cagehztj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2plgeknio.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vckbdppm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2htugwwcg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xqcvlwpt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ixpjbjmq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mqtilhrt.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wvvknapu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2eirnudzj.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2apxzfrih.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2okowzceh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2xbzyjfde.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nqcdqwpz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2fanlcuvw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rrjatowv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tolatboi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2icqstahj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mrvehdqa.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2oqgmgbel.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zynywvst.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2buhjqnjg.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zqhykmzq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hxojmppd.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dpqfifqr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bkmffpjb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2amzcimwg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vpdmcgef.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lsneivmc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ramxqrpr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2mmpimjql.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2cwjjmzwq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rsdaodwc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xkyohmkr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rwittlvy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zwrdutxm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wszsenqk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2fzszyviy.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zrxeofck.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pvpgvhxh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gpxaxvqk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yfdasvtd.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ulyzulec.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2sfvxbkps.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mwmlauwc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ofiqpqrk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ktexxrzn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2vjblpqtn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2gfvpntgu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vucupoth.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xwtpceul.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhxgeghy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2mcvvhwlx.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xvligxak.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2pidmutim.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2sovepehe.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2sqlzhbpx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2aqwdbrqr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2taluamqp.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xmnpeozn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uwvvgeiv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2cbmubouz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kvunqjqa.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wrhyqngh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2odlbqife.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vomcwwro.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dcqiekjb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qmwdkgeg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pqfuxqwf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ffiicase.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2jympxwrq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2secmqjli.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdexmmn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jeusnywq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rcrqvxmr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ijpquytc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wcdpokyd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ulzvwegd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2byivyhrd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2dxgeuian.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nwrryokc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2huvmmajz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2viwnsgtj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2sjhvufkr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yokteuih.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2aydpyjdj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mgshbolq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2phhslshz.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xtzsbynr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gbzmwihd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wrxsvrui.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ilnoiwwy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2swqjwngd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2aqoehecv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzrkptee.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bjfxlmyi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2amfangqm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2onzugfvv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngpzhubz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ijpvvwmb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ooffstoy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zineuwxs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vwxcnycu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2fpqmvtwh.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2bxuogkwh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fxtvhpfd.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bekcprpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrrodnhc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2oidbyaru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyiczdqg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dlreejdb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fkztiujg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uhocgbtp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dckbjzjn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2woowuoxt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uwpepnfi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yukjbkyz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xgymdspo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eoigcmtr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2etkxpqqp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ffbrvnjp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2hybayctt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2zdfbdzpm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rkzdtfhb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mtyjrlli.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ohevyiln.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ezvyluxm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2zceekxrb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ncflbgzf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2frusqzaj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ijnmmbnl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2skfaqxeu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2urgrmpza.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dzyfivxx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hkxmigfu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jinixzys.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hfgwquqb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vueibxre.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jbyjjzsj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2odeulqjq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fynsfqmn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kjpcgkbb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ksyclgjm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2efqrtlor.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ckpibtub.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nvrnoubb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jegylwmb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yloxeqkg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2sabiczqx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fgjnsbsw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bgwlbpyf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mgotnoaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cqryrmum.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dtnosjae.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hsrnzbib.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lzyhtpsw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vzuofaln.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2nbfnlniy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bsnpqvap.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jhpvxadg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2nmyysmuf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wwpqhcba.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2pqzatbml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obptdwxx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2pkfcgarz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2dzzqdlhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfzzsnja.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kcnwcjvs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ojfnzivs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wbuimnfa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2cpfzjlhn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fhmjawjj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ffymkhee.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2qeeemhpr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2wiwmkhxs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rehbnyae.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjlhjg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xwjvssef.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2nscwhvaw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bxnbnjym.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mwqwsuqu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wumpibob.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nkttjufx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2efaqwnlt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qksdojuk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rtbscrwy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jrqruaep.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eslydcam.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cixidsmo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2emvyzaxs.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hgjfjqjo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilkforgz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xowybosp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulelsupu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qfvmrsuz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gdhoizdj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uvlxwnuu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bnmiiala.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aribrrhr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bdozocwe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cafakhbc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tzjtegko.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2txcvhjun.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2syfhzios.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aalyoocf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xwnoezil.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2zlhiqlql.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dhlpzfiz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wzqztvuc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2raxsrapu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2itqzzccy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjhtnvwh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ncoqlpje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2elhxxxoe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eawvddzx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2amtemlru.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2sirdrnud.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nxwgtbpx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rtgtxwwx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2aituhfja.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2bjzcydpw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2handmvnd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zrjnktfy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2iinwzfqu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2dzowwzkj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wkfvcczj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zqtkfuwk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rodsxkhm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xtfyiqhd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ewxbwxdc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iqhmdmal.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pftpcakg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2klhvjfag.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gbkmhxik.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2froyyhgw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdrsocrf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gbpwzckm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vjdcfbyh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qkjnzmdi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xwltllku.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zbkpunxt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2chtymzbs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rviogeog.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2uyaqgspl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ssezlgin.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2coofwqjv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xhojkqwo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2udkkjdzi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rswiybvc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2iaxxbpfx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hykmqgjo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ymhpiblw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fvqvzzzr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2trlzzbtz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2npyppatt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ecsxgtdl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vurnjrez.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mibjvgze.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2isnmumhl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ucguwmrt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uqvktrjz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2uummkjgf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nhuyswmr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fliaygou.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xnuisylv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yohymqzf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gosfcyys.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2emibwkwr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pvhvyevj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmbgslu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzhehjg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2donqrlrj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nausxkky.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mubiakfl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2irqhjyjv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2mucoxkkh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pgducrlz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gmeldytb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yzrlilfu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjifjlrz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2powjesko.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2aumbrwoo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmkwwbx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nuihsmsn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2dzzxojos.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2htxkhsma.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2noepjdwi.html


<!-- 参考信息 -->