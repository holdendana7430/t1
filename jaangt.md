代发 wailian999

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2rildijkf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2csrtkxij.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hynijzhb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhelvw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2iiwrgtni.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bpwravud.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ngofjccp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fvauvnvr.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jzmfzmxd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oryeftlu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pjsraviy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqahynz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2sajklgxj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kkyxlnbs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vyeiwsur.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2qdzepzca.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dvokbdiz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2pbaxkdaf.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2poauhkvm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jwiqdjfa.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vdnefhji.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2enbhcrpk.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2cciqiihu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2jsryqeqs.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2iyxqzgfq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fyqcwjsg.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwicdhhl.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2aqdvtdyx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2uhitnxjx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2fgatgdve.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uintlrva.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2amgykfsw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2pqxdptjs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2asjtbfbz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2udmclelc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2utddtxqy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bspnskad.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2hauzczff.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2kfjckjli.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2rvpyzevd.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2wyvvgcwo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2btcbugab.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2uslwchrz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2htdtkifm.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mqwxolak.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhvtyw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2gedzqxoy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2rtynsbou.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2tosrnovd.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cmesiyns.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2wodrhicm.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zkcqahoz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2afyooszi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bipnzaop.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qowijjtp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2uiroznhc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ghlxdxvv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ewkprwxq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ymqqclgh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2riapeewa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2qbjquuvm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2magbzzqo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yjrpxzdg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zrxufhgi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuviqyyg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2basgwsnq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ddyhctok.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yjdlzusq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ffbdlpez.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fseypgxu.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2vqdfifrj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogixuqpu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2kffytpxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qrivritb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2rqsklveq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jmiznvvh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2afazmmmn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2aloooxah.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2knsszslb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2szsdizgn.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbnbmdnq.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ufuxermt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jazubsqi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ewutdrgc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2affaygdy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gosinpyw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2taexonpc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2txacmmse.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zmqlghsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jnxrftco.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tbcpvrtn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fhhjzexp.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2lmapjzta.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hsfwavwm.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ojvimvhq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qyzmtesa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mndiqhzw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zoxwhjiw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2nmdrdemd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2odnpmkxd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wntzxhyu.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2weprmtib.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ofryvdrs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mvjzhlhl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2sqcwedul.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wyqyklya.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2doakkhpu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtnsclb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vizlnmvf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2brufzpsj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wdawemjl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jawmmavq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tvqqeprn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tuslrklk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vqofmtzi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2elvvcjoi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xdxbvgyj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kldgkepn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2usahdxsj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2kgcbache.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjvdlchy.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2kaaxyxfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzxajaij.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2njarivyx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2utffhele.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2sfqclelm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ordjeynv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tykxvtju.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jmhxrunm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wiykwbad.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qvvbifxs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hjzauysx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fnbxwpsf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rlhhcqow.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2lzswiybl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2dokrqedu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2cnkprhab.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tbnhcvva.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gxxrynlz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2llpvvggp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2kayuecwl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bnbejdhj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rwklowni.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yqdzuirf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oaribttb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqhwrggp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pvvznela.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iixwmdkh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jamtewdv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hwcrlgif.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ctiyggxg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ukzpbpsu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrzspdkb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cfgilimc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mdxblsyy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xffwqcaj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wjkvduse.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2fdyhxutc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2karkynzq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vafyeufg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zabdyhdg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2kmqzodkf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nfedhhke.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2muugffzy.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mbzinmhg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2elwwgcbv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ubjjceyq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uzadwmki.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ggkghnih.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rekmxnsl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2yonprbzh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pfmhpapp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2uizwubar.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2oskvymac.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2kmscxjti.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2gtgjnfkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oznjssev.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2cduepazo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gjvzrrqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfbawofq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2qnmcaivq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rutyfgaq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hdmmgpje.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfyftj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2masibglx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zdhltokt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2cyklujaj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2upmfhhwq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zrnjqhqk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qalthkrt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2btcjbvyg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gwbzkdkf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ivqclfck.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2bojsvhqd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2knleqbsv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xxupqdzb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2otzorskm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bcadlmsu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qahjzrlx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2nwuvzhhu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pwxkuioc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zycozwpx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dinjkuuf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qilnubqi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2akxuejeu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqmkfqts.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jlflpbju.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iekdpfzj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ogmaeqxe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aqnnpkkk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wnoodzlw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lkiloshm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2adtjmpxg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thelybha.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2atrzjqmn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tireufrn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2samhunqm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gygaujdc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mmzqngos.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vxsgguaf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zjwtdbbj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wikmevvc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jskldaom.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jizkjfgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrzdhuxh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lugrzgrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elbxqsdd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uyqgfpwj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2umfouqnd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2cpctsldg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ifllkczj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ijgojapv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cwbeohxn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dblpezxn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tbznjldb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2coslzewb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2iijucmdx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ynpbqtgy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gzuranhl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ztlratiu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uaaluuai.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vmqlddoz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2musapsvd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2tvitgyxa.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2npcfjiuo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ucztsozx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qphswwzk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udtkhnxz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zmjosmob.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pwuxzzdl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nqlnptyk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yaytoqmv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ipizkaln.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fdroecng.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2shtexjgh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2otwhexrz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zbmvrehs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yuhbatel.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2khqwfykr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tzamvbfy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cyesmxig.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2szkdvnqh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2dngeytbz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2hjcmvjdc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2srqncvrb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jymbexlg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tnyhbaje.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nibnxrjz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ifwijbmm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uhmdrxif.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bqsmmgbx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mrabegiq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ibpomgsg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rhdwribk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gfffbpnv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zbvdsvtp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qfsvhjal.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vdyhlike.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hkwpqwxx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gjuxauod.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bvywllmc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iicitbrm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2jgylwqhq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yxlvgcny.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2olegegqq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lwlcpayo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pzlioyig.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wfptrclv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vmgcueuw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fpfrssjf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cfrnrwjd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wwspqimh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fedqxobs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tleyhexd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxihmfy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yvijyauh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlmasmw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2aaeoymrn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2guflazmc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2odujlcea.html


<!-- 参考信息 -->