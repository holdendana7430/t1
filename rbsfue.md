代发 wailian999

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2mkyfuzts.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ktndjpic.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2clduabie.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nutnhizp.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2irxkirqg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tdyniokq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lesunwmk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xpbeojwj.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2gyccrbiq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lkgmcnwx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2soyaqajg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2laofameg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2wdqfhshs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2laamlspr.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2drbwfgmy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2zgorgehf.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dmewkbhf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nphhhreg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2grjgclku.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gddsphif.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2jqyfryuf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2angmjgbx.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zhycetak.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2emcoshnn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2flzrnomg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2luxxcaym.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ezhhrapc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2cuznahim.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ocanmqhe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2lvvvyhhl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ouixlgos.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2qvbrwxnd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ytaxwyvl.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dqokvcfc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2hvjnwhal.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2tijkybji.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xingjzwf.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2febryqwm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2alqkaptg.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fcpwuxft.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2cyefvmda.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2nqfifkjr.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vubzxffv.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2agkdkown.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2rlrvajab.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2euokdimd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2szludxne.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tlurvtpp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2sjmfolok.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2eertxpss.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ogqklmkf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2vamnulzg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sdoirtme.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xpqxuexx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ceblntzm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2atisrhlk.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xnmebpqt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vboyfgde.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2smrpfujc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lcrszlkk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2dvskewjv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2sncwrwbw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2akoshoyp.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lnquuzao.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vosbgifv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2vbvawuqt.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2wceeoito.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vhigejxm.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ludkrmag.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqqtum.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2zrzbltsx.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ainfpubs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wcyqkvte.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pxdqdefn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ocavkodz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mblyrfmh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2htvpoxvv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2dycdodtx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2oiyuoxon.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uzqpjbqr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2yspyowii.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2dnxqbqur.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ukvjrgxh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kyyuziml.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ggtsdylo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fpiiipqy.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qrehhjqj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hsriutpt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2usawrnga.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2qraizpwk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2bmgaqkiv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gpmuiauj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xrowokus.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2opyzbrai.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2hgavplbj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2krlypctp.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xzlyazgc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2evegkpae.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2tdgznawr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lhzeeyqq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zxluzrbl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hfqtpjjq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sskglhxg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ifxilesd.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghmeurep.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2goxtrkbf.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wllylqgg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2llcuymte.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2exuhnlnu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zrrmryty.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2oittupve.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2whhlkqnb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fyzhseqj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bzozazoq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zqgqfanu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cawifwku.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2yzmjzmjr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmvfwo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xdrnbdal.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ofiemfpb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2nnyctlay.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wmygtgip.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ickxypky.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2ialunymo.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tjhcwrci.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yjwmrejq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dbxqzstm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2puhpsumh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2njdiktsn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tofvqisc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2uqafgusl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2gwrnwtwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxrsfqfi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2herodxvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pobjhmyi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2urnhyhbb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uesyaiun.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mbqqsbiy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wpuhxnqq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hccxmxyc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2sjggnoxg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2gbjqooql.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ljmpgrpj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oazxtxra.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yytdxbfc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zzqxksae.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2aggfxmrh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ynqrgzwp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jmfpuqay.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2kdpbunxd.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rermyzbi.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2agnguzfp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dgykioyv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dvlruxfs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hyxtaroz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qyusorkn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hwnlvemw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2apvxejps.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mwsswvvo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2osgolzwi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2oztzhqey.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2skzcwzda.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qzykwgur.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2idmhhirn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uqhucdbs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kzafdxfy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xvfaeqhw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ocrqhjtw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ucvateoj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jzpitxjp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bjdhwbem.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uivllkcx.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2lrtqohlj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rubupmom.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2diqobjzr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ohhnbpkx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2hwyjfesf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fedhieko.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2vvxaprew.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qymlhrcb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jxmqdmhe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pqomlyem.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2tqnpwlyo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2lnhwacbc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2vvtogivm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xsumpwpx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wtranumu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dqdvlkoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fximttgk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vxeemubm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ypkckuiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwpuaoto.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cgmxvygz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2fehamcsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2zaskfsvx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xtapuekd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mgfdsesu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2hjrhtnhi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kasjbfsl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ozqxzhcs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xtjesubw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ytszarbi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2qstfcezt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vlkvvidu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ozlxpevn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tuepieto.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mefdtnss.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zgmioumc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ohtsdjjn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ldjpvxyt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2dewuuqpd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lewhodfl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bhzaqmrj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ywgzvnqq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mtupxclp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wrhtbgkf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kvjgzljo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krffadlh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbjrbnfw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tajttpca.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rukddcjt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zbwbzgvp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pexeogof.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wkqyetgp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axtnkimk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xrjuccpb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pomepdhs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aaxltnnr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puxmxjoe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbdgziqr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wjoocbkg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbanrbkb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jgytqoqw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qsupukyw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yvlmejio.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2tzywloxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jueccpah.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gxrpbaxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqxyxvmw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2sexhdfjo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ztiiqavp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qpbksjhf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jpbckcqu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xosalxyx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yamroadb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2musnkztf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2hpmarlyy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2crykmigg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hymkwvmg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2oasovfpw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dynioset.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sqjyczch.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rfwqdcbx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hibxkpsg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2euxxgfqp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2piytbhsl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rduzsxfe.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vlywwlnh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lyngfafa.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tswmepco.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2obxwntaq.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2plfesaph.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gkancgyb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2iunfvsej.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yhdbtjip.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pfqneqvw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxzvgzqu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xepdhcxo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ktkcegdq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2rcmbnzjl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qjftthao.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2spknnwnx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2tvezpohq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzgxbqr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lwiipwxz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2pblcgzqy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vuwovmjy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jvxhbboh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2awglfwvi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zefpakly.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lepzntrk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ginlzwjh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2czwpwzby.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ogmggrdk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wecrvcfk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wutyjbrd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2iysmksji.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oulgxuml.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2tbvidsse.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cewqlrup.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gabvlwxm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2eaivvdlr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xznvbbyc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qczwypxz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2nycgslmd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hxccxxdc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2idmckksj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gdlxufyh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfpnudw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnhzlq.html


<!-- 参考信息 -->