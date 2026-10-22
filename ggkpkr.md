代发 wailian999

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2opldszhz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xdgqfaok.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bxfhcawt.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2hzzcyawb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2bwghnyoz.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2dhmghikz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eifymjqx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2sfithqun.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2keyykwbu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mifvesik.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2mpwprtxb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lqtuuagw.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2cunjgwcq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ybrruhxh.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tfyuhyje.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rakxqkin.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fmqlazko.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsbzozxp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2hwfwfrwo.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2djjambar.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xnfxjfsq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2vatbauqw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2eynrkeer.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ydahixcj.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qpkmpadz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qzwobrae.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dsxlvepo.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2uofzgmkf.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ewhybaxz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nlnwaipm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tqzeigkp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2sksedbri.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2uaximdkd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nkqkygue.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lzhxvann.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2oiuxixxh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wfyyqtzs.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zmjfysiw.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hllabqnx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2jkiijlfv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lfnhlifc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zcbnatic.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kqxshtdv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvandqy.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2gknntjqj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yfxpndbn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2udiadfre.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ecagsxgy.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2thehzjkl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wzrzlcyn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2wdmhmans.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2cgwzpjnw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wngwbylw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xcgwjilh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2wteybkif.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wkedfzbp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rqxevxqn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pwpjmyip.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hwvooijh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuzlzzp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2psgdegkg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rljpifzc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ibyqleun.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhevlue.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mffxzkaj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wpdfhaof.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpchksuz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fugsycfz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2indppmax.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ifbfahto.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2gmcyudyu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dfazdqtx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2fihggeuo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kxwzqbzu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jpnsihiz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ofjswdva.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vatatmdt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ikdbfjky.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ijqjsvrj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2lehsdkfy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qvlztjln.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2esmfebjy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2brawofnt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ttivitpl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rbguomgp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hmsoddnq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2sifjvgyp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2poogvmep.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nwhrnojg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2tovzbzpk.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aqpepwyo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2slgqfqva.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qrsrbxbi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lpfyotbw.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2zqbqdycf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ytwvxxug.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wxhktywa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbmpaji.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ruznygkg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yjgtkktp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lmnlbgqv.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bqsiijyb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ebgzvobm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2omovidsw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2izsfowiu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ubwnffbc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2jolokicl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jrqoetqa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ctbzhihm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jstpfstn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2feywoiir.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgpghumi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xoagedjm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gwmjfwqj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2slgcfuia.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fjymacag.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2adecgihm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2aetffphh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wicckwky.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2sqjjrwgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqtbgwbv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cwoxjayl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mufrhjea.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rjjsfhyg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kclegcay.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sdejmgxo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lezpkouf.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sfwyeqgq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qpzchpga.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nhtuwuxg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2vfddizgu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2clbczeiu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2tochmysf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ufzpcqgu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qdptpjdm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2heralppg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vbsnvqsl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jdebgpgf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wcpuzukn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pnlemcbh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2elvclywk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iraexwbk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qloswljd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2gzpxkpfw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wxeusvoc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qnauknwn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wnzvjwum.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vxgbyyie.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2yajlziol.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jacyscgy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2revasvro.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2oohbkwvl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcdeay.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2luyhskda.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gwekbgjm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ceoepzml.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rzyywbed.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mxnjmpgv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2vgoemqyi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vibogcni.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2yhcvkkvh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mrqbxfqa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ffjfcfgw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zilaaocr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mitghgkh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rbpsewrj.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fqlhbucp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ivcqfhbc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2asrfhpzo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xddpwlbj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ghyyovgv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2gjfkzthc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2cmzmiajb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2auswynyr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fvppbzii.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2gmsgujdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pycdvkeq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2safkpmvj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gdjjectp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksbqukjx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2umwifdmv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qdzbaxbm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2eocpvzjv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hyuxyoab.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2cauwckgp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2cjecbhxi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qfkwmald.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2fdgywlft.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2nztelvok.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2bpugjsbp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2vuwfqawg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2nwymypqx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rvrqrabm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2fepbjbof.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zjzdnlxw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ijmeltch.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2erzldjtr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2foxbwbav.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ctdeokzh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2jhkgcoxb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aeofincv.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kqnbauya.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nlvhisod.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2agbmovfx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lnqwxyqa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pnkfevkz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljhxccdf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rmkpzqpg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsxnjdck.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqcgijpv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zlrldyuz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yujwgtde.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2whzbgsbs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2davckmdw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qwgmvzsi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xmcbwwzb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsdrlknu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2qlyzqtxf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vmmsqtzq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2umzwyxmx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hxmbqwio.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbumzpwm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2raeexblm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2koazypsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukhxieul.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtftkuso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jouwwsep.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2ulmkezxd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2oryzoimq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2htkmdfxl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2enfgfeoq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2revlrxva.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bocmxthb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ytcwtafr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mhulvjhk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hxdgbekj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wkivnofg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zuqiuiyp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cuhqorqu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ngsaltoq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2coircbnp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rsokxpne.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gxrecwkq.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xhdxrypx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bgkuaadk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2juwgaglk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2kpnqttee.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rjciqubg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gnrxkaqm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vyrhsjmc.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wntujvir.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2uxbmbuak.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ubguzuqx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sbczxrxm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qklhygrm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zrnknnqr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hsmyiexz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tdbmitvw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yigzjplp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2uzounhmt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2itbmqnfn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jloypmhh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bupodmpu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nezbzscj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jkufbcge.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pdegfcyr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2foxlozet.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nulasyjq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2skkpawyl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eqqrlmpl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vncmldsp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pwotxwbp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2polfqyot.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qijbypia.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uycfsroe.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oxmefieu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ngztfowo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2raqbewkq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2intyruhm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cnkqlikf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sdjkrrbu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2akaunhaa.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhlvqo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2imtdjgem.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2znbbimpo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vavkispa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kotixnoz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kkmrqcgl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2renmrvcr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nokawrvf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mafbxviq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vkyzrdjk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2iegjrfeb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iddfcvtz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mejvosvt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xbhikoyf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vytdcuek.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2bxxgzjfx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tamwgkgd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2yyjtsroy.html


<!-- 参考信息 -->