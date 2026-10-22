代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2pbsrcbmm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xvxquouw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2limlvtni.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fhdonpqi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ehpxihwm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dxfyxcff.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2ybcocqqi.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2ywyhmjhd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ufyjucdk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ibvspxsc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mykknpvq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxiecbc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lgbqjifd.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dkhycyuo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vvilucqz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ckoffqlk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wzmtqwsz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vgbohlij.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2qzdwldkg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bbqichhd.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2imtpxluv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mqaxyqhe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rtnkwqvh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lordnopm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2zhchizgs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2itaqmtln.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2awjwvdjo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2rkcmqdku.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2vctndohq.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gdgvloyl.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2knejwabq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2oxwwbbst.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ifartdoh.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2vvxpmeat.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2hetuznsj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ihnlxcex.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pndcphve.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2qofopyie.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2khkafftq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2assmvcgz.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jnendljf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rjqyqlfy.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2afhiylpd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ykscoomg.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sccntisi.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yakjmfsr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hfzeqtei.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2pjgjkwgx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2pieeofhi.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2tkeflkmc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ryyljetp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nlxdeuou.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2senyxrdq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2qugeyldn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2aykizttl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2sktevtbs.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2luoilkkj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cmgdviey.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2zmxptmsc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tmxppbfn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2itksemth.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2morlljwe.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ahuielsx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2neyvweob.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rgdgpofa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2znqdzaqc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mlhfwsst.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2ayvckbld.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2cqvahxkw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2iptchfeq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2tvxzbxzr.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ligrlhzg.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2scfozxqz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2fjuoqpeb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qiiwoklt.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2shhclydy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2etlxofwu.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dgkdjjvr.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2upyppipt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oeewqlgy.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2hztlpjzl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2nldfaccj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2heokoirx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnlqqus.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agbrmbfl.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2dffscwof.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tmmgumgf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xmcuqyuk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xhalryhx.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ijngcnfw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wfdtkvts.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oagrugvu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2evbtxqbn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ihonhkye.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vgxegyre.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bszriyqq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2thwgcmbs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2geynuhqu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cabhmaif.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ngrkkizi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2awjhwpts.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2npuwfhdl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2aylifytm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2uyjcphms.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tzsqqdyw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qkargwxn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mebzngec.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gptqpoub.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2drtayavo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hypeyqev.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2itbovxjm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2voibwovx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zdlhednl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vrcpvlnk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2nbvdvvkb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uuujwlmn.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2adugdqrp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2znuchuhb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2etstoify.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2nprnmimy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ivleozbc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2txfzqlua.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vncxgkkw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zgzmokdb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2phqymeft.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ycvnlcla.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ibwbagmb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2anwzxbrw.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rkemeqqi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2klfuoutq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zkjtlerb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsezklkv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pquuwlyt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2znhbzhed.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hinlxbtz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhgewt.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bzlepicu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2zfeogluc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2iihwprls.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2oyhsabpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwusgvhu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eozkzgbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hshcimyv.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vxwlazry.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aqhacpxh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2bpauxoey.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ibehvolr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2obaqahah.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zpwkmowe.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fnegwdpz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yqrhpmtq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lkysnkqt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2awnjorqg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uqjorrct.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2soolgxan.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hyodaydg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nhznqzxs.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kgbbflcy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2cdwgchsd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fbmxwfrs.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2abxrjjfk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uqemfych.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ghbiehjb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2ptjmqvkf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ifkebzqr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ocacgeeg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nobdfkus.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bhzuikxe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vgpdixry.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lejnlwrz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2incgapoe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tvmbowjn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rqcquytx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2spxfirre.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2htwypbny.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2slozglsa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oexmnrew.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oyqhseoq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xsbpvdkx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xjkigclu.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hhwiqzeq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xoskyxlj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2tbhccppb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hzcztfsm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2njvqecwz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2suwilqsu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zlcjvyac.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hjnqhhhy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nqthiozx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oxjlhrmt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2vzewajlo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2hxoqhtqm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2wqreuupi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2eslgfmgr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tgjfgcqu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2lkvjyowq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imuaooiu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2rrjdnmes.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2avtaorfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyubkdvw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ujxraayv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2spwqiqxy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hwuezfcq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ecjuvohr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2expozwjl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2iycaawer.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rlpvkslr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2tyuhusae.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wrpanjjv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uisgchle.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yjydokld.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qajmgkno.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2wioxlyla.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vqubjjfv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mltyyghg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ntzwywbw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2dvwmnjhc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ekuvhjyv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lvkrmseg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kezuaros.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ffxqqyed.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2jqmudfmw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2owmjtkjz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hxpjcxho.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ualnurji.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eogexeng.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zpyftqwd.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jpsiovda.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzccutrw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cxfsvjxi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtnhsqol.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slwovzlp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uihgasmw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcxtdmvw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zmheykhn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2srszangy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2puvffjcy.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2diebngor.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mrpwoaum.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jwzjymaf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wpsrhfzk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jvyhvoov.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jjvejhts.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enjxeicd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uckuucqg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2eidllkus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulwpttoa.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mxnaaujc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xixfzwjv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2qbyuujma.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fsehbqtf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ansyhqzx.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xjzrtnji.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ccwqinpf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kfmmwywm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cpuzkphh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2uosjgbvd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzpahy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ytmtumst.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rnviiuge.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2njqiufhj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iqgngjdb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gsmdmjnu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2iidjfaef.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2endowkqt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2zqvcmeid.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2umlkcjgu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gvqfplff.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aviwlxhf.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dxyvyrnc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2upansqlt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2moytbqdy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vxfeulpl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rpzydzoa.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gnpruqhx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2cndrvmxf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bjzcbbze.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yqutiwoe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2cbsyaanh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ltrqzzif.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxvxwp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2pirirlvw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rkwmiane.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2evtmsowf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wejprmhv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2objftdns.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytkwutiu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tkmapedi.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rvesrrea.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ugpkidnn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lazxpsjh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ltrhxmij.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2aqtaecqa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wmpvsuml.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vxijapyo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vafzmfsf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2olepyvao.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dzsybjjc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xuwldzfq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vughqwle.html


<!-- 参考信息 -->