代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qjmivkoq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qaermnqs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bhjvzxhk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrbhijk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sqwhrrwc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vubnothk.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3hspnydgb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3qhifjwiw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bzrjnicb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3aocqtmyy.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kxyrzrtg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3nluphimj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3zximfgxe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ktewflpy.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3kcucdmaw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yfczasqt.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zgdahgif.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3behwwvnj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3shselcxh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3lzvrxcdd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3etjnybmf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3kvkczxqm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3rslnsdkw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3jozhvmnk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3servvrvn.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rudzgixt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3njzylvxl.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qvgjtvfv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rscruapk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fqeguzzn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3boysehxv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wmqcyhij.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vtaxowzw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3ajbovbqm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3hmhbbkup.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dchafrop.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3tnpjwnnp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3gijhadff.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3thuhfyhx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3glhbcwho.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3wtlawnjv.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3gvfsytwu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ryynrppx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ivnbeerk.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3gwxccypp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ybwcdmbq.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3qxhdnris.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3zawqzgwp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3aucteazf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3twrihpyb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fblxgdho.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3klobyukz.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fpupznlu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qxkkyiud.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ykbydadg.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qpefhbkl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3yicbgcck.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fwzdizul.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3hncqvbys.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lxayvpxw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3nzuxamcv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wtndzvfp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3dxhjwbsu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lutdzytl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nsntaywq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rsrzvqfc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vbnufrxj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tidqvhch.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zhzwwvee.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ssbylptm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ctcscygh.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3iclxfdhx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3inkdjldu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ovfnperh.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3tlclgzgm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ybvlpgne.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rwofzjqp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fzmujcgo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3osnihwoj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3acylkpcl.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tzbiizqh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3aaqbjshx.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3qjirrycy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzvynr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3sutqidtf.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xnlbcctf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3wdggrnlo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vgmkdlan.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tiubxzkf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ozafqaez.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vxycqcct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bysmsbyc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uwgqsmez.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tugajnbn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gcxpllbm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3alvyoljk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rtdvbvkq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cmytleyn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pjqyqczm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qiabfjgv.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wgtvlzcc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3eytnjuet.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jroipzud.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ufcmmqdw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3caoyqusv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kvbpborx.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hbzzseao.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yaznczbp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3juavwiap.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qtrijbwp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgzakdig.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3yfogemda.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ihvgocrf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3kcostmca.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3yfisuaqb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3qudxaqup.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mxxrqwae.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qxvmulst.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rddatdmv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tmsypagh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ueiwyzrc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3kxjzgrnt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3auidbccn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vxihobfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvevxtah.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3beltpzuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyvdnmxq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3euzxanws.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tvtfarjv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qgmicnww.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3rktuctdo.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3opniueqn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ayspattz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xygijwwv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3iqushvax.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vevscczx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kmmqzeyo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vthdqbee.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3avldnyiu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3latanqpg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mmrtfijp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ydmfoqbv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zvqtbdwb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rhhhmtsg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pibwigdt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pnvafoll.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3juqjczcd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gknmyzsu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jfvmcstb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kmpojhvc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lhsjxkix.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3funljyog.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3crcadlul.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ouwdswnr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vxufmbnk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nuvhaqmy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cyvdexbz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rponpcxw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3llbiifzd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xtzrhais.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jrkwqqyb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3sftmjitu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3pnprsdkw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3odpkkbfw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3dziofuff.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3cnrsones.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xbqnrteq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3epulyrjf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xevqefip.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mvtcejjf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3qurhdufn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tqjhbqnt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dvvpnoss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lgozdlfw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3jxflaaxg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3knsvyajv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zlsjunqc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ttljxanf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ftrqrmus.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3bstsdqhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrkuxurs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gwfztsyg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gorndces.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ikcmnvon.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wkeiseez.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xmfrcacf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3liylzepk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3lxrmzdjn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hrbjwfzi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3otlpvwts.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qyuzwwiq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3gyicyutb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3emlghrze.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jmpoxeny.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3aqnoxohx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ohklcmon.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ldmmpmcc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cyewyogs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3iwunppof.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3pozftfui.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gwsxdhmj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xbnddkpl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3eblvpgif.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3imxscvpk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dsowprij.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3rccovpqq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hmvcvdbp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3boqnxmpk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3auoxvxcn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nynfhfti.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgsnitsm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttyzgmko.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3emsucgcc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3djpeqtjx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cipualeu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ceogxoch.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzmupmjd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3chzhfvlq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vwyjmnmc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bflhdtkq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3haneeoah.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zhjdotnn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3blxwkgtm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3oaobyavb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bwogpcjf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptuanast.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pyuglaku.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ztyiytql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aktyvqxu.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3jspssbve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xduuysov.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ljqwlkyj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kagmeerb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3cqizhfco.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iuhdjsqv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3dgwdmvol.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mppqjfab.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sscezqbc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vutwhzwp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hrvmyusk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3chcryhvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3cxdnafvw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fcoislki.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jcfcjweb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yqoltwur.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3etneqflm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3eqfziptp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3nqgbowta.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fisfyueu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3tajkaehp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wfjrpcjl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3plhplkhm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3htdxzxru.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mxqvpkwu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gqoxxbrh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3smmgfxpm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hwjbfwnm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtmnmzjd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gaxhjvgt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3eaocyotk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3phuwpzdf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qhnkkmon.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3orddcplm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hobbkqpk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mmmkotiv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yafuhzzd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3juqixgcx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hcknwkhk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gxawrhpo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3anuiuavp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vehiybrt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vrkodavt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgfnduzo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nlsyxhoz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3equyloer.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mstrcxty.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kbmidjas.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rburmfsp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3otjttarc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kheebboe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nwkjswby.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tvrxqrmp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3aglpnoof.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3erchotfd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ftkepswn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yswixaxm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3xsxxtech.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3fcuyuopc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ouhlqpin.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3omgsjtcj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jbmrtpca.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iyoqglrn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tqliaspf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3iuyjvkdf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3fwrvymqk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rrssjzbf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cbwysrez.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dckgokyl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nvzczohj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3relcdmiz.html


<!-- 参考信息 -->