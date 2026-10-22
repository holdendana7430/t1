代发 wailian999

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2kxmdxcfw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uyfthufb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2keadffcj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nebvsqvm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2kwuncgel.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2iihxwvkb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2oscedhth.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2jkuuxvcj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ssfxqhvr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wtdcefts.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2gnnjlqkt.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2zftkzwae.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fsxcrrqj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aemsorzk.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hqvdezyp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxewyshn.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2wwsnofra.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nhvnnuvb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2fkljztuj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pgjkocxa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mfajfupj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvtgjvsk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2aqmfznfb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hvfgfpgy.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2htnznfqw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rsrnpmso.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2fjjwfivd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ieladymp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2anirolvr.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlghsck.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bgqplqpq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gtcnidih.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2opelcjmx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2qxncsowi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nkxujjyu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2zsqoxmbx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2edjofjon.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2dtjkmbgj.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gwojffgw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2lskxgdob.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2gedtbsps.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2zdgnqiiv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zxrkzlxc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ycbijszp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fgowxiws.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2rrjpqlgo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2opdrrayl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ypkwwynr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2dxjdkots.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hkuvwqiu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2gxiqcxam.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2gqxnkdyw.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cewvnvtw.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2gdhcmebe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nazmnlnh.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2asusrqgc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cttqqprp.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hoqxrzsa.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2oflpzzdb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqtyegtu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xqhpxduh.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ieswybia.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2marxuidz.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zimiwssn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bvwqmdui.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cbqpwwau.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2poiddkmb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sglonyos.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlbejgoc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nikzyhef.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2eadbdecb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vsgomvdk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2tihhoxjv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mruuacdj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ktinvvkm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufswswuc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vsxvdcuv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nqedgoak.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bjotutnb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lzvpmedc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bmanjzrt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2lgbmmbty.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2giimshrw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxrnmri.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2krkaoivu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2eadznvyr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2mxcpxlgr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2olvfbpqr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2toiegkek.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tktvbnza.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2mofcxmwv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fkwzhxwr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2nnvehbsq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ddhtymkr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dhfnfrqp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2eunsypex.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2azstlheu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rgofidkb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pgchqkyu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2htkikpac.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2wwzrvdjd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnxvwsq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mxghtheb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qbclvqae.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ttewxsnm.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cphjegtz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kougkkwe.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mmnusrfg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2pjfbbled.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lornuydt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvghmxyz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pshdamrf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2keqkzwbf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qznhqpoy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2govecdxb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rymairxt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hqcetfoh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2dcdjhmgm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rjirymkm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2utjrdecd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gqyrzjur.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vvmvwrzr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2hejijyvl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2brldlpwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byckjmyn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2sqiocitq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eifmymik.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lintjpof.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2omsgczku.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zmwqjasz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pnriwprx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gieovkfy.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2myvsiwpn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cmxtylsu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xrnlfuco.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oyyuqjop.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zodiztff.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xbnkduul.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2fnsnztso.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2miktluro.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2czgqjkrg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2binsxuci.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dbhwttkl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vtoamcsg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jigquqev.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xtbwnekp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rzsfxusd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vlemnsvj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ismnabrg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qcgitzde.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bktdkzuc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2swzywkma.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2msgpzmmf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2cjxejvhp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qkgkxnwy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zmtnyxhc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2prbtzclx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bctvzlfv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nukrtpjm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2phlqjrvv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rxyyurbp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hjuykrgo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ivdnvhyg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ifraxgym.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ydqdlbuk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2odholiqy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ntvdigwb.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qlpgnliw.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2mndwyrur.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nfsghfid.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2nehpbqbh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rkkzlopt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2tdvzjwow.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dyvsefir.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tmcoclps.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ajvqpipp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ivhvkoyh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fqgnezli.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jijhamot.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2erywflcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtufaqzy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vepknilg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2hdvnilan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srmxeolj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cixyhhmp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2oqtpvjiy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2bgkmfkpc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2fapzsoip.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2hpavjbkn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pvrsiylp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2urauusbz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2grrhhhti.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2lktlxbtj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2hhjmxuep.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ejvfcqfx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ijonhalo.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zmgmolgk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2uuyyjflp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2zboetala.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2efwmilsq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2kqfgckxq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2rcgchdyl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2uayflbdw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bazwmwqq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xdwyijlk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2pxfbxymn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ydnjtufe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uykuebdr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xshcpxwm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxtiijfx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pcxvhpuz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2kxmuzetx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvhedapo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wnqkyped.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2brirknkr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tlrpfruw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqzaqocu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gmftxdyr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cchgvhlw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sxcasxmu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnnzaugd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vknqcsip.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ezfvhzzr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hrefadox.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ycilsbyr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jwxrmcrt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2krdqhvma.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cekrgfot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrhbfpln.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2crbjuxnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dslmevjp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gmqznaqw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2muzitkoo.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xpjcuqjf.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dnvkkhcm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2lnqmeked.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mmotgati.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nlxzytyq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2esezdksd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cmahfuxv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kiejhftl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ajgqxdwk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jvohweal.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nmxvkxir.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2omsspazh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eluhvxkw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tuhlsvus.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ykmrrdor.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cvtfjzvq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2irxhirut.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2rnyerjgu.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uluyzrsw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vcjogdmp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tmceygzx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tkqjzmdw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2baweirdj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2znrrgljx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vdawfhpz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2wlnghnti.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxwdrmw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2vtekiccg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jjfcqrks.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fkelacrh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tbicmrcu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2voqwvcgb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rmrazxlo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2sxmgxela.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jawtxduk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hayxbnyt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aijnxsjq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ssyesknj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bnnzhgdt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2omidhqgk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dzimsggz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kclhdioa.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ownqtgcq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vyykozcm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ktehxqxf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dcqmwicq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ijkyriys.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2emokfukq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bmijcidq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wiccupbk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2mbqlkyhh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wuipfrrl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dxyyzwgf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cgwwhqgt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bwzfvgen.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wssocscj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gqonsdhz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dwcqthym.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2feqnwccy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jdojelti.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2zzxrwiqq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dqgcaufv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lustexoi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2svzhygsj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iurgrigv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cjobzfql.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fqfykypy.html


<!-- 参考信息 -->