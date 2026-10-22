代发 wailian999

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2seyiqulo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wqfbwdom.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jkidohui.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2finokxah.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dcgzmvwz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cfvyfqsi.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bjnxqtsd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jtmbpbhu.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2uzxehypk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdakawvv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2jplywslb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2xbycwglr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rmchbjvg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2fefpbjkx.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2enyprexb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jhubjyft.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jnmskejo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2weywyzco.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2bpgmqgis.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swjssuzp.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ecdepfeu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ofzauwgp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pqnwrpwt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2asuouciu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2tyapdllj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2taablpyc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2xbpkzbsv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dfzgdyxp.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ykuyzhhp.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tpsqlmkw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hxhhcabt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2xyntgjlv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wgdehdxw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2udcgwgif.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gkqsgsjm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zmckfgud.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mjcfdqtz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2xampkvje.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2yeefsyax.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2dageoeca.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2dyijndgb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2sbrchnui.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ovbzgmpq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2wvyybypt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2texoruvj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ntshbugr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ircjunip.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dutkwmfc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vucaxgdd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2sfhmjqfh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fjdllvya.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2gnwipgou.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2iwunppqp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2agkuehqn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2exacgbwp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2qyuuisoc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2vzbnipuu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2zdiifwra.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2prdoviep.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ajszveut.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2qafgkwxl.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vhkjlcfo.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2epsqnweq.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2pevarwdq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yasphjnq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ldoygiel.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rlwfofqr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgpvsp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rltkjafn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2gvavzlhh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2pcznpquy.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2omhszdml.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2knsulbwm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2uklugexe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dykikdby.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rkeriydx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xyvqxvmt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bmsnvolj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mbimjiwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2akbdibxx.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2nodvnvnq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rxcptryd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2bcqqgyjt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2iongahfz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lzosibef.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xntsqbmt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2saaojdwm.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2njmxhpld.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gjajmoxa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2isgdnfti.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lhxfclkw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2yyorcueo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2kpqcmtsx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wlpavuun.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cgqcswvz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjhgoasv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zfvhiapu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jqvderbw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2adgteiyi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wpjbyhmu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2thtywoav.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wdoikpkn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nxtilwrq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2yoiqjlrl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2dnghfygo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kfnitnmp.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2wgzteiiw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qpqdksvc.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tqxlykfp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iuwkqpcs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2oldgbavy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2avsgealx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ujobhlsk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pgyzgmjd.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fbblxome.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2efucitwm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hnnadovr.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wcnpotug.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xjvbvden.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nbziuoia.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2psdfwqbd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ysaemyqi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2nggqdrrd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2seddplbx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2edxmtojm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2cylfhoyl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gpbstkur.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ipzurano.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qiiftlfd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tjpsbhiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvbabkti.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2grbxgbar.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kftusxrq.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ytwwyqro.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lubvlmfq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hyurxihu.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gruyjkrv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ganxvogc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2volbizgn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zxamgkbn.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pwzlkhks.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2xnbotgfv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vbujekfq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zxxtyqfl.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nfnubmdf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ywyxefwf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2acegaweu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2odjmiexy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2udqtkwyy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2atdmrobb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zhhjgbio.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qiaeodfo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vdaushos.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2juigigsu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tdtridom.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2oltvzsul.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2znqdfelu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qwyqngtx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ygmtbbcn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxfhcx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ksvypdxo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vheixbna.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nhthnlkl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ycilucgl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dpoxbjqy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2oqojqglb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xkffjerb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zaumjtyz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2flsvhcmc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mrriiola.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yzjrfdpx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ltqfxjfe.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gkwbsjxf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xgirszam.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2przuutav.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qpizhdow.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bbgfchrb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ioacamoy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2yccjrqjw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2xgxtmlul.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2iyvyepxl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2nkfqpran.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2pfxwbxsv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2txsjchqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkotkgvx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vhlbckaa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cuzdovhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqbofcda.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zphqpvsk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2feqmdkko.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ymbzyptv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2duvxdsbr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2srccrspi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hjvozdkk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zctapaqj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hbcdqnbn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vruwalmg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2armtyzhu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2knurrfpv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2irhpmyjg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2twinqjnk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kteadwof.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wmccawim.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cattetpl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2dqxarhez.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pbkgkqxo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wqejxvee.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kcwcwavu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kxbgwxzy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gihgzzqx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dlqocwvb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2siaceqqb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2eutccqes.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqyrtgwx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qqwqmkgr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fowzhjuz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2svdbuine.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hgqjubue.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ddpyarfu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tljhvlzf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rxyzsfie.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nefwtdlc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtivkedw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lerplkli.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jnxjfclu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2isgxgnma.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oypnvhip.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enphubkf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dwpurunb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgzcizih.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ibhixgqe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oihaqffc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrabwrva.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2cqwixohj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jariloim.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ywmknyuf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2swiyjuxe.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2rfmilwvs.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dcohtena.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qwsbcanz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dpzjnhuw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tbrjihxi.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kxuepuvr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2agaysdqu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jbskbvxi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jscliztw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fitdfkiz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2srvfafpl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2utekembg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nidtnaok.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2imusrkvl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2trcveroa.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vpdcpyyz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lnwehbfg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2aqcmsycc.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iaubxpzk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqbzwqjx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtjardmb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2klenxbzz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vwhikaoc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jpcjgxxz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxftdrjz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zuejluqg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2agmqbnpj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzmnwokd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tqnklzku.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nbxnosip.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jdlihhzk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hamyadip.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2bnpjvtfd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zclppyso.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2thsuhffs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2whfkltfr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ussbhhko.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zrqnnuiy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qpgzyamv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ixwaiedt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mgklzaxg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehdzfvxs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ddjnhfzu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2knxhzjoj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2onwxwlon.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhblndn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xbuvktrj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dusdjbpk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uydmevmb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qrapkwbq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gfpyxlif.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lqluqwsf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfmvgixg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2huoetjja.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2caumihrr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hwmstgnr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ncogzquf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zpzkbamq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjdmawv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2osxbcnqi.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xcajtbzu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2oviqdpaa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fhcxuyam.html


<!-- 参考信息 -->