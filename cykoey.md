代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wafrlliy.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ghdyumru.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3tpeovfij.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3njysuchx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xlmcvmiu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ssipkclj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nwzropcd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gwstjvnt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3suvidojr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3rzgxxvdv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3psiqfnem.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3xaxjjadn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jikrcjpc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3whuxyfhs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zyfvxbsw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lxmtxwdp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ryvsoxhj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ptvcifjf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3xtniuuaa.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ocyrscqd.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tmtsuhgl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lwhvxyjd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ineldsqt.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ptxgkjed.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kcvcebzk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3krvtxgdj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gvpmkdjo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jwykzcic.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3amqdntlu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ecfewazc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yfneuzdw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zyfhiakz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jzcdemfi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3pebtqauy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uloolzxi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3uwetbcvs.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3xtyatoqq.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3khvvfuga.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3syjvjxbs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvetpmhp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qaendbwl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ezzbvilc.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3jlwiuqsl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3iwyuvnsm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3sjvvqivl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bkyswqnb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3tideffrr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lyrlgxcr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gyxukqtl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3yshyuxkt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3drgejexu.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3xezcsmfs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3rdtndlxk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vtesbnpi.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3mpjgumfe.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tuswcvyp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwmlxkme.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ejiclmic.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dusofzok.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjvvhpoe.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3kylbdrge.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3yhatrhsl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uybvjezr.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lntblijd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3lqzqqgzf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ctjtymzk.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3jqvcrhbl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkipfpre.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ppjozwzu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wzsrtdet.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tmiwijlv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jeregnmm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ybhlnyjl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjsdth.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ygruxjjv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gllwlpzn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qywanhma.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3idsqtbwk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uqsnndoi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3tghqdogr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zvplwvwz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ntksscwg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3pnwbznna.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ymaboxbl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mfovidrq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3hkvnsybb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pqfvlepm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3igxjaglf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gssksxyz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jxpmnzbw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3bmlgrunb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bttswjnd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3onrylvkt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qjhfrccz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qkoznlyz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rtugzehl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ovwtrkha.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qunemxcw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3eybmhwzt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qcosgzva.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ainftjlm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uzodmeua.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3txoghkji.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qobyngsz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bkywfstt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3cghpumiw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3zawdqbik.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quqezcua.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wcysycbi.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bjtzigte.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3iytzrsux.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3emcpqxwm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bbheoekm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ayddoqli.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzuqsp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3cwkggcaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btnbmsno.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3dfvmolto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lorlegaz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3tcadtqbf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3tvupeqoz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ubqkplft.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3anbpcseq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bhqanqrd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uwynwrzg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zwnkmhjj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uxndyoxj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sdddnply.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3xumarimv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3oshgraxe.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3yvtngmmt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3qbsmaksb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xadubpdy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xeaiwykc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gdnukgat.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ojrvkzsw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3nikisdas.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hxzswvgr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gsjtvebv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3imjguuzv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kbkpnlfz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3otysgutn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ffjplflu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ufovlbdy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3liwtmoxt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hihzdpii.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yzdylnrx.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yrzngnji.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ggxmxywo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3przqephm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3irnrijou.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ibyyxclv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fiefswdx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mmevnoih.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3hcoospnp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kerwuppy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mehzjeim.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pkqwsrih.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3svpveclp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3mcpjrema.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sgfkuovz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tjvpafqc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jymjrmwk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hqdulqst.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hsvbfide.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cxymixlt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rrqysflk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tdqknizo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zcxgfzrs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3naliuprv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jlgshfdd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mbrzopep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzotahsg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iyfqjzsr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3iawjobwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zndqcocl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lzzohwrz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vxutavti.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3hdfyhrkf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3whhbdwmc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3lqobdutc.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3dsetegea.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uwbzuapx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ipmsyumc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dwrfwnat.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ppvunarf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nfifaabm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3toqqynky.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3yqlvldyl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3yoharukr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3phqglijy.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ykkpaqfl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rcsnbrsp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rjnvtbyn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hcdrffrt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3anwceohr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sksutvrd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jlflvavr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zytwkkav.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owdalbhb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvzditiu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pkcszjjz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmreacmj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3csicxyqi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lveuvrof.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fbfkgttu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndyrtbip.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cfmvzfto.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fjlkocre.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dbytrrqb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jlgyysku.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ctfpuaby.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ejnxpoae.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gatdwykk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rxrtioiq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abbvkazt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3siltxreo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryvkcvpj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pmnqchqs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ruwdrbrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkwqmlit.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tqftxred.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzrlwcyk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3wwvxjyvc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nzwwbsdr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3irjdkrdt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fdjsdevc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3azielvwz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3exxqbplk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wqwwklyr.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fcyecuym.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kgvhapdz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fckzozpl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3warrlxly.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lrctxjso.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hreaviuu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3lcpnukbo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ayxfuuhl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3nqobpcvl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aywxiena.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mdtoeefc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3umwzoide.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3hdgvunhw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cspfienj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rhrkgfdf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ktcnehnd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ywrultlj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3khupnqzs.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3paumpaif.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ouioxqzl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mwpvislo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ogxpgztr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3euyixves.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fojocjiw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cvfpwfmx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hpekpmao.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cdsrkeub.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3xgkhlhcm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbyish.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3swntbexg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qeidlvum.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pcjowbab.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqqgjccx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gqhuqukf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mvqwfpdz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nimuryvw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dhdvedks.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfbamyzo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3bfluaiad.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fusribhr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fvyuikdz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nwcegfzx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3iyucypgd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qxrrjdqk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rehnhbhx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3iraupsjk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jchqgqbt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3crnuelrl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ejygfsjg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ddszfcth.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ksmzsiak.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3chlxlsop.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3uurebmjt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eticlmoa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3aquwyjya.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ubxctsmg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hdsudurr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vdkyaipq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfcswtco.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qszfyoiz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhdtkrt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ylpfoxnp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qjsakvim.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tntsueoq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxrthrc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3oygvauzf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcrisutn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgzdplxz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3synrzgoz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nzdxisnc.html


<!-- 参考信息 -->