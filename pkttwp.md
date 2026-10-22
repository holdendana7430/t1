代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ytwvqfsc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wkvuedkr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wkqyigof.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2nsxihexr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2abpltjbx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fchwsduh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cizirwnh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2syjlfxuf.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2glmlwulr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2itgnlsmo.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bqrzkpwr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zmqzkxow.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2elejbnsg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uuejqvan.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2fqwvlcml.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jtkidyxs.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kktcyrid.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jpelqzul.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ythhjply.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2ohurflza.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2autzfciv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtzaqzb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ebqiglpg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2srmuesxv.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2gwvjikwd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2umhaijiu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hxrkvzeg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfpumnfb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ivzxjyfy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kossplea.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ixmegrts.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2tokkvuqx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mslhewkf.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yjisympz.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gommwtfd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ynimsdku.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rgelgcyx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ttddhakm.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ftppzzyz.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2jolxwwbw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2wgvswfes.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ptpgghpu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lwfhjvgw.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ewxavsxs.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2sxgclncz.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ovnvqfby.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wvpskkab.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2mpzyygka.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aembfcjh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2hpfejwek.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvctjq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ezhpsyye.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2rtinhnyo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2tpyzznfj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fgkcwjnm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2iiuhvunb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2yduvinsx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2pwrucmda.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2dkpjkafl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2fmtdicdk.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vzakbpdw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2idjflvgn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2shkkpmir.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2lobioxkg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2etbmkafg.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2rhaaupsi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vxfkltek.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rrlzmaca.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2eanhhmnh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ampultxs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hxzlzcwy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2njkjlnad.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2soueazga.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sjwyuhms.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bziwvbgl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qzbmwywo.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fkekqmpj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2eerzdsjo.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ykwanwph.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nbgzbgta.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2idtvtgwg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kmcgeatn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ioguiwwd.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mmcrtxix.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2edtgrprh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jdyazwdu.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xpqccbti.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyowpfoc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2jpgsgiiv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jysloivc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gjxafhhz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2wwoqsptp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dxrhrfay.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2woknnmgy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pyhwnpod.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yxxkmxur.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2oirqmekd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2grsmrcbu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xzjvlhtd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jonppdox.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2aywkgjvx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2xxnmszny.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hwblgqbk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2szgotyxc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ugxnikqd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2dmitbewd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mrvmixas.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2txbkixme.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2adicwizk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mrnawxko.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gfznssqn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2pytenhqb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ucsnewrr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hwpfcpmk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ojhcclfl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2jjtpbtnm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dmkfqqdl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jkhbognr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2veqhovzi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2odsgaihz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2yqiqdyva.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dobdarun.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dpfdstkg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aginqjip.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wlflyrnf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mocstonq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xbrrhhhw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wenunllx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hjrvolug.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kzhdrujc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2khvsdacs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wiarvgxf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2xohjiqqi.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2fybukcaq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jaowhkyy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ajmwfzqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhhupxhg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2mdyislhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guoohqse.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2tnpguxao.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wbenveou.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2amwaiezf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2baatxmay.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2saebrono.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rkruopyu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2vihomfmp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jrkfkqvh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2empfvssp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wiuhjqzi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2nryqsmjh.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2alapqkfi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2dlsprsmd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qyjjeogw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vbswvnun.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rodvoxcw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2twzgfbre.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2dazzfytw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kxwnrvwp.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2fkrdwixq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2czfplezz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xktqrkju.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oslknkkp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2skjnnakj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yhkgsjeq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hywideyo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wtspynzl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wuzegafa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hhcavnlu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2terszitz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gphclnje.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fatudqae.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2izrvlwjz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zqkijpsr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cmhmeanf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2sojsbahl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nsiultyn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2iiqnkydc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2qovdosle.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bownohxz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2eluhbyyz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hqgucvbk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cbmuyjxv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fxvgqpoq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2idvzewoz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pqkvdnst.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nwvkkdhh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2fuahwpjo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2kaseimtk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2vkwjxwoo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2kvvrfkrm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wgjegmbf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ggseadfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hktbxjme.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vfjtowep.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ibgmyizs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laefrbfm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lxvlawpo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2biqcpoqp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lzulymqk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ralrxlkq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2bjuczswr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2faitedun.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jjllntff.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2blrleqvb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2gvzuapty.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kyqrwlxe.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jcvidqdm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2koqasyso.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2zftvgzmp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2gdaulbkr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tjiatapd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bdasugeo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hlokctfw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cosctxkq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2qstkansw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2asnmdohf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uqsuyqmu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ntdkgqcz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nniptfco.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xbbkliyl.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jwygdlsd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvyfgsoc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2udayxekj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2puceshzg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sceqhebc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pdmoblvb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qxjgflgu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yuftugdv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqknhvvh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vlnwjhep.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sqbtqehr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uqtnnldg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ppaddboi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tbwtzmhi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fgqybybf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2mbyubvjv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2taynemrn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wjunqlye.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sdysqfng.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkeancsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xsehsrkg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xvmucilw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbpnxdty.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2xebkhaub.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nulhrjjk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wjltsbxm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fspdstya.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2gnxtqxpd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2alghgniy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ozwvdete.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qbhckedl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dqycfhur.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ixzkuasi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2smcrtipw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kjeeugmx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jkhkklou.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mfscyefr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2abvhwcly.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2mmqwdfwl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bqqcwrdu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gyhthbrs.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2kuhsjeaa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ixywmgiv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yjhqrwwc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2alzwzvrh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kkrlrwor.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xwjzhesb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qwdfynqp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qyrucwvh.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xviydhsq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2pohjqyfb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2zcndqjdn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yufugtne.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vvdqeoxc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ndodsvqg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bbljflmr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2cefjwugs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2npulpyrb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2awkwuvpl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ouhivkde.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmgoippd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vqdutuir.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgdpreqb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jiczvhzt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwtigkga.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2knazrnyd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ypmqzone.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zfsihdfi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pizsodef.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wotltded.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hqzsenbd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2sifjzsqt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qtvmfpqq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ekjrcwac.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgyhmbl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kgyrrhen.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2aqivksta.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ztjjeejn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gdthqdyc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2phrmbgyy.html


<!-- 参考信息 -->