代发 wailian999

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3upeagiwa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kivhurqw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tfpkjxrv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ofoaghwu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ibfywsrf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dumazerw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3cjleksjk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3knrborna.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3hlsrifqd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cfuoefyx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3mpcugbjq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3takrlcgh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ohexllli.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rhachwop.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ezglxlsq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3lthybsuv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nrznuvgw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fyytpxta.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ceiqvfph.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3vqncuhok.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3ccmqpbjx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hesghlvg.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3kznjlana.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3npkccwbl.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3utwdhgom.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xrrulrky.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3gezvojjo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dqyvzktp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sjxhpkwd.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3odncslbx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jpclzjuf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3sgsmtqkx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zzjthbqw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3fqerzlkd.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3adrzfofd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nywdxkyq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3zsluuegs.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3kdvqweog.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rrfxytmk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3nyqiyzuw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3odxjcejf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ylifftyn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3hgqaumyk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3sdkfkjcm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dbsolmuu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cizxyfmo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3gjotjuwp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zzsnrksz.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3deipfkuc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vpmklhio.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3gjfiyhlu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yzuvuctp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3weufucif.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fqddfbkl.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3vofsllrw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3blwujuav.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3knreaird.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zyznqlpt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3otobshpl.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3vypgdjin.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qvrrttwy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iyxbkztz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3tfboruzn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3lscncriz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mwdrbhli.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3fmnoqqhc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzvsfmxg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbchrjr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tzmwwfhi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3gqscngob.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bvpwcdeo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gersrsms.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ytnpkvlg.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3cpzhzudt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ebryzdaq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3hfvdjqph.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ljrvlqkq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3srxoshif.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3xkgqsjfw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3esfmcmna.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wbchsdfg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ugowdriu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nxthihbe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qimmmmmd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3jdyfbiqi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zbwsolkh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vtuoaoeg.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zjecqltx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hgsrdnls.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3pgwjtugl.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nlfzsfme.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3whkckqwb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kprtruqr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3odraakbj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dlpctsdy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lbanaegh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qcinocwp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ghnvwwyh.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3memdpbqr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3nkgxsrpn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xlglxatb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3trwleefg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jvmzdgon.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzdpws.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3brtouxvh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wmwvwhlj.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kdmdtabc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gktsrkqw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3waypaxzr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kitgnwsk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rrcrpmvo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sovpronh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3isvimdbr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hxqygqqc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3blowtpej.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3armtpzyz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3cfecpavi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zfirmjro.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vlzecbzh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3knccilhf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3bcxblunj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jnogeckf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nlngehla.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3xcpybnsq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dfscdzcx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vgwhygmq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bmfewyyy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3lekkccos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqvluswi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ieobapgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oytnnmed.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3uembafqr.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3njfupfgb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ffsorvwu.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3zrrhlrjp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qfcktael.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zafrlmxe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qmrxqdej.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ijmuixbm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3apljivun.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bzxjmzbd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3ghvbczxs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3azrilten.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3clxwkvxv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tvadysmi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3jbszfezm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3kjbhjevf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3owowmtse.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mdysvpfr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3anhbvvhx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cezcnhmh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3gaaihmlo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rsvethex.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3trhjauls.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gakggasw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yvugdxvw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3davgijzm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jyftcbjy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nlvpukci.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbzixl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eyehtctt.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3iktglzqd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ryqcqrdz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qucipjhq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vgrveqdr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3awyxdyrf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lpbbaqlq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uvtbhlug.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3irwmpftc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ovdbrffx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ddtijzpm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sgijhgep.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kkyaquhw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bdbjczez.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3skycxkpu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xhbtpytz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rrahgjcy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fzyxyyvz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3lbclugvq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bwuopqnl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3xmruexii.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gtugbeij.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hrdjtptl.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3aiwaxyvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivkfitqs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3gkckfage.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3fdkursrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jorhdkut.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fyeomuiq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3lfofpbbw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3uhdgvsvb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zoxpdubu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ogbinbgr.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dbxwjysk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3supbzrtg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xryeegsa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3badguypd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ssudjmvb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3wfewdysz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cztjhxxe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kgmunwbi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pohgzewe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qsojmxlh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gbpxejua.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3edpamiqm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3aaovzjyk.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wstabdke.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3yhzqdygh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hhqgkjmk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3gwbkfgpn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sznpgshu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3yutrolye.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pyvmucku.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ickymvjx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vvjwxrkv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zrsqmdvv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tsarhwnw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jmholglq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egoxpqir.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3omtsctes.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3waeumauh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3copwrztl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gkgcsduz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dbqrfwwx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3htptuudf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htmbnosn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqnqkaxo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jujpodrv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ayuppswz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzmzsyud.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tzdnqqbj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3imibdtzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elvytevg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3fisrdrwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjhfhyto.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tgqnkpai.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zdydkpql.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3jegitxmn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bbnscjwh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3buyzsgvg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rrmyntno.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3szddndjy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xizfyrcx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ysdjqwrw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tmkhrmgt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3zhatkoro.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qioncfkc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jhfaioqw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3mffumyyv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3swioodht.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3fcnlfpzf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dlsgmkse.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3htmcomtx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dnhjkqvs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3arnvkbcg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3egudrfri.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3omfyodle.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzwibhrz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bndgeyrf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3toumpqrr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ftfbvfjh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vhlsevfi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3eodihmco.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rxorxoso.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3knjwdoug.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3azvufjpm.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3agsxwsne.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3fxxyqaqb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3uwufnmak.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ehcfxpuh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wpvzyvmt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3cnnlviwi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mnnrufgi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pmgljbde.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3soiaejdn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fbhuizlk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gulmixxj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3teolwgwx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wlmmzfdc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wfrxfhta.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yzrlopin.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mewspbbe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3aarjphne.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fhvkbgdm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ryeichnv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gszzdtus.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iokebkfz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3baobkvaq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ytaemuqq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3scpqiico.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iuuugudc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qossnctq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vxvgiwoa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zulqnuqz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tsfaxizk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jiinpnel.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fpppbgpo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xlykxiej.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3zjgiuvwm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gnxowerr.html


<!-- 参考信息 -->