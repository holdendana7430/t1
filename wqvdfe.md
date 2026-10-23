代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xnpgoqnf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ablanxyi.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3collxaiy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3pvuqzkod.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hzaukwoc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3oujkbkej.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lhqiyhlv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wgqoaznb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bhddrmrm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mbqmehxq.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3zjgkidjs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hymafmht.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zxewgjff.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hnglpprs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3pzkhpskw.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3vqzgfxmb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3upzbaanx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3svnswfhx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ubtmlbup.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3lcimrebk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ldbvvnoe.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dxfnenxg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3cmaegvia.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3isjphiko.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gcbuewfr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3skmnpvtj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vedbkdbi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3topufqus.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3laoseuif.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3otpsqxqm.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3aukuoyjp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3uqlnussa.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3aldrsfsm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xdpakjku.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3zqzjvruw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3vgnoxqgm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3eumfnmem.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mrnkewrm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3koqgsdyt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3piwujkox.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cwprxgxu.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gcpxwlqv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wxqbjlcz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3cdsbuuqp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3glvucbqo.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hppyuals.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3pehznbmp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3njkhwang.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3drayeuxo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ymvbduui.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bajtuoff.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hbcmdswl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aszksozy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qgpsgzqn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3njrlisrw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3jmepmazh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yhxzgvgy.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qrrtcwuj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3njeyfnsj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3egpeqszp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ydcwvieg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tmywzccu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gcaulzzm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awkusxkv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hukfmday.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3piszsunf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mspgccmq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3gxreggef.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3equwfhpi.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qvyjbsxc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ambijiaq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bmfkehmf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aqugfmad.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmlxxfkv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ubwgxtrz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ymwjoxpy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hnmvfwyc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3zjspsiug.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3oprehjam.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3dxzukzqb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3lrefyddz.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3asjuungz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3okutuuiu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3mllqrmcu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3lvvakpky.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pmafmaep.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ydjarjco.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3corvpset.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3dhwgsets.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3indvjnmg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rgvmxzkp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fedlbiwg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cajhzlhd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3namtkbac.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3rzrlqpyr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3sheahsjf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ecnbfhht.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xrbesidy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vcupnjij.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3bvqqpsuf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ftxbzfhq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dyhrucso.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hrqbczht.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fthipqji.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xbujskyj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zojvhrtr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3oeyoaebe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uajmyrgx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3avvfpmtv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3unjsorpy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uwgpfvqe.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ymxajtpl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fnkbgsni.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gqmfcqup.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3qgsajqkv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3iptrvsrd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3egtfvpwh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cikygzfe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3aqovvctm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3coseuikw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyndaozw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ryvgomte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeidciuj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3veqmbqmw.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3grubzvze.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3srdhynij.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wcykunuv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yejjwiqk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jiesmkll.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3iqqnozgc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mhjqspfe.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3luvpcrai.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3dcgwaajs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rtiijvga.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3iodhwafm.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mdhswjme.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3futzmmaz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ujzrjare.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3tmoivgby.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hvbrpqmw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pfgsoufz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gpnlkcyh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ifrcxgmd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jmacbqua.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yhrhzrft.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nsxpepoa.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xitmwszh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vpcwzuwf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3webptcfj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vyucalsm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vrrgldyt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3hdxtcydj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ovkkioic.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ndunlatr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3sagxobnq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fagjzlgx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kgoqinty.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3emzpnwby.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3buohxcmj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yqoxoewt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jivvvffx.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qrezqavm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xsobrzfo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nrgcanzy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hqtppnat.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ysiaatgh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mgqdzsfr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ivsauqkm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zvfyjpco.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hmtywsqn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3tilcxlav.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ymuellsr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3milffzce.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3puuwbabb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3eogeplny.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gwhntbpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtfcrlxq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3awircxjh.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3wbtwluuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mknbssqh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3catnxvkc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3oajoxmjp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3fuauuwpw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xqqdmtch.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3orrbrcxi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3hhctkpjk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3duwxaqbf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3vtesnjps.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sxhvhdat.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dscrpegw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3mfcjwjzm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3twqdffib.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3gqlzvfwz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3lorjupsg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3thofvolb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dgbvabem.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3upmwwizc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3drqgzcpu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lnzrcgvw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3irwxkkki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nucuwdwa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ychczqan.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iygtuznf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3puczelnk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3efqmnnpu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qkiplwvj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3loytrgdd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3yeokoqsz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ggeqdbjh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mpjutjqq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hhigrwxb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ivkzrjsy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qcfhbvlv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jdstnrax.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vvvlddoh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lxfrsrpo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wmcmrytj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pgkuupmv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsbvoewv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rdsmwycb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yospcdqp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kpmbopbl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oovkdvxx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mdjxyuzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdfaodgp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhuygxug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqwgwj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shaqnmgw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3budbdscl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dbhflzxj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rxdgrvpv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3epzmhkmj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pljqkazs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dsopdyki.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3gnishouo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gepddlbl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ixiuitsk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3njdbftmq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qrxdlkhu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xgckyzgf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wzqdzhzl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sokdoamx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3mjffnddt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3hvfghcmt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ffqlbpkj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3lcvhrbtd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3cbwmgrvh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xplsuveg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3alrlnvft.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aypibame.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sjqtchbq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dlpsjxcr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ecywsnnx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lqxifrhf.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zhqkfcth.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3afsjlxaw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gnybheet.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yrpsuiny.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ikxxmjnx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3comztkdi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3nprvkioj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3tqucxtom.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3eppmobxp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fklytgzx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3arqbaxvc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3czwckcok.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xinragps.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nnlqulld.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3inxsgnmk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iyerehmy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbkzzhim.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xwpnuocl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xqnkyzyl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yhqzfwsd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3diyorndr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3afwoefti.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3oscchkhd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oevesfws.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rdctdklf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3skisdyti.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wdtukjhq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gyzihhhw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ylvjbmzn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ucgziqmk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kttsbnia.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nywvroqt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iiwgxjhs.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kspeurnk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mcjugduu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3upyysysg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ojpnydfk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvuwclf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3twlzavxo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpuuqju.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fzpcscpp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3twzldqdi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tykmhatw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3hfmkmepc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pbqcyfoi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dsdbqsel.html


<!-- 参考信息 -->