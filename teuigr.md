代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2sytwfdmx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2xjgbkcie.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2iqarfrws.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2bvaokzha.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2oshgicmz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qqlgjmgu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2qbqnsyeh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ulxsvehl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xzpjnrff.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2yhoknfut.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2smwjedvi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hnrvmbev.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2jsvppraq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzyyeopb.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2nvhracmx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fmvxyiut.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2geksuawq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zeyiejlu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2xgkmschj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2fnbixdhb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2vixofgiu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2vlksqvme.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qppkoasq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2verxeofs.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ukzprsmh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iyfptmzw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2iucsbhue.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxifhtvw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2llswgmjw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2yiudkgoe.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fksktbho.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2fapskhrz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2egsiegdp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2tbtexzgo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2btzzasez.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2woppznal.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kwnpgsoo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oaukolfk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2bbtghlsk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2gzhsmqyk.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2dtbnmlag.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bzemirqg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nytyaekt.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2sffeauba.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2lbnbhaop.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ujcnotkj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2vrvfwbin.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbddwt.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ndneoggp.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxcdaw.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jqlvwdoo.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2wgahyfeg.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2hhyqtvna.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2tqupkajd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2mbuysmls.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2kdyyjlpi.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2tgyzdned.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2vmvfzykk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2rxinzozy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2hshoncfq.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2rnulsohl.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2noopxeql.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2lghsjici.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fksqkkrh.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2zpamgjso.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2kdxvowkf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2oozapzrz.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vlsaodvz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxmyms.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lvrfukfl.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bkwzpbqz.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2dnbiwkxt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rhibtjyx.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vikeluob.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2cinyefuy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ltcaryte.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fbiyshze.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zlwjssun.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2odecchwy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jgndwosj.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2hmeheecm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yoxyxlpm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2jppyjyiy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bqtknzwe.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2phxcxldp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2mmiwgfku.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2hpaqtunh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jxcfvvfs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zbxteogc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uchixlli.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2izjuiwcd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mnmqmpfs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2yrzgeynl.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hqstdvtu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pjjktoqv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ynsqjnhp.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2pwqrqnmi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bytjpdxz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jtffcsuu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2isjmnxka.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2gnsblqid.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ynpmbuyx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2igwwmtjm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2blwcgqvk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tkzgzguw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xldiqsmp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hpuhdmhr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2enqtenrd.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zlbzxrgn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iuikfjqv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2umddpmla.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ncxvijiv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2hmlijtpd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2suffxlag.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2dhkcacef.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2ddfkpgjb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hxfinedu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yjsakspf.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2siqzxxng.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nsduyewo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hlpkjcfg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xzemydig.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2hhboovpx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrngyzq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rswjpyta.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xsleoiup.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2vewcajoc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2imrjghoa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bujfvnwi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2iqgnykmm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pdcauuwu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lceigdyr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2yykwzbhr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2yewdzesy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2obtcxira.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hjhkfthi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdtobmze.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mvvzppkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgmavwvr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lskgozjy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ehsjgmma.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2uyvhsqsy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fydrzcbk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fhsnqopc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wrwhgmwd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2bcumgmso.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2spbrcblq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wtoeqokp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ohiousir.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mlinhdbu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2srcgdlgx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rgkeaopb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wyyhlkby.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2qufkyoie.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2vgyrrniu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lmzbkeya.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ansxduxi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rrfprlst.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ojjmmikw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kefwhnxl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gaarejia.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ntwsyumu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ysrkjckj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wcxydfic.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lwfazotw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cvzlfwvz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mhvhvymr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nefkuxnu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2djdxtaoc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cubbdski.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iyxaqtrb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2flgvmmyo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hlgzpyck.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2xzdiddwb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ruxfquuk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lcnlblhy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hkzgwjjl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bshqhnkk.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dxpzvmib.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ovoiphlr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pybznnkp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ugecrvdr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vqdoepnd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rxhlycwr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bipnzncu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ytbjjngs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ectmgeay.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bgkcpdql.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qujjzddl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mabbeeqq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ardgowho.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2fsiwgkct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mupmrsaw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2asiexpan.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cuxuuhwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktcqchhv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2gulscuem.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2schmnejo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2jrctqojs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2rviadent.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fililxam.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pdyfxnhp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2lqbfmbfz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2cpsteerp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mcuvznza.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jfqzuavy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yacjvoee.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gsekkfir.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jjhzkiuy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2umtinpzb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2baxftydw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ebsbglny.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2zfvhorbw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2tfnhttmg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dgaucyli.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ksfsfkop.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wfajxfnz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2kkvruqtj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2unuynhyf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xfczmczb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wpshhtjc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rfbergei.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dwgodyzm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wkitdurx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wzstzprl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kkyropnh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fpjyrsco.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dheolqjw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abdkxkuk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cltozxvq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sdraqqjp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uhusmxdo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ozlvnlly.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xhlyoncg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ylxuzgfh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xrstywui.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzwllopv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uikxkaax.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tcgznplx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yhggkodi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgwdluhz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2asugmyre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spsmbbrt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2obocoexd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dzueobvs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xoaoykvj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fswqrsti.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2alybtprg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xlchynxi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ckoevyei.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2eivaxtqk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xghcjzhy.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2cpehtsbu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2sxupjzat.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iwsvivby.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nedrcsrg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2maszplls.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2icaqebvg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zftlrslx.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yrcnighh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nfjakjnc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2tmixsvvk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2sgpxuxxc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dqatmhzt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ngcyucgx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sywhabhv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eqzynwce.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ewhzgmxt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pwmkjzum.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tkunejtx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bqsrtptm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uopjdvsr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rnqdfgys.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xbtksaap.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2abkjievw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2sqkkqqai.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wehxzpjn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rupccxuj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2fygwduqt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2htoheozm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbibcbpe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xoarqfnr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvwvmjnz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dxnnzxxq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hhkovbgz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iutwxgkp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uryxveqx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pzfqfrqh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xvvgqyof.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfmcpmg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2penmgrgs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pfgzznmw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ffodaocz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2glhlksup.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jpukuvwr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ytluomxs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2whettvwf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wkyejuoe.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfhqxtd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ksadyvtq.html


<!-- 参考信息 -->