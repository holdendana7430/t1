代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2daixchyu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2tkaffwoj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2rcgcynyd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vuleaqva.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2snnxijsq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ebfluloi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zopcbqte.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nlktlkre.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2orrtpirt.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2dmhaeumv.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2mvrhiulk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uumggyef.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ixflizmk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2joqksdib.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2rrvqbgsr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xevbhwhq.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2ztruxnqv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mhduthit.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jsposecw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mdvcqxwz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qpxxrelv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lcozxgwo.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2trdlglqj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jcjumdnq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2nhkkwrxf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sdxtwgdr.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2vgikrlnn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2tfjxoyqk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2lbfqynia.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2skvgdbjv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2sdnijhmr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2utrilgmf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdopjggu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2yoodzrii.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2skdvziqt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2qaszukoa.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tbgzqirc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dabihfit.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2sqkrpjqa.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2cwmyvmpx.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gzruxlyr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2eowpslfw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qjhnepjz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2qwvhjawf.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2fqnjsuvy.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2qhpieqlz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2orvrnpat.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fxlsoibt.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2apjjczpv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xbohmzhi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dlpdtxnx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2awabtstu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wfjundlp.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2qgxivqhn.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2jyjstmio.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2awvsmxxu.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2wubtoptr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lhdkvcbf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vcvobacp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qofncykv.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aminznuw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wfhzxncp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nhjsnsaw.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2uvcdizni.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2gebmjzaj.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2plwydlyq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2ezecybko.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mhkzpspx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sedjreqk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2hiqptbvj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rxxsfrbf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2zrlughte.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2yauazrjb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nojymygn.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxccsl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jldafcvg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xomhckfs.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jddwaclv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gmangdon.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txupbcpx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xbepzlnw.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2sfdtgznp.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2njdqoxpe.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ikvipxch.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2kbvpzxgu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2edvhorby.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2khwbtgvu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbogvlbu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2oxsuazez.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rppgwaad.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bljqzvwt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bnwifrpa.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2vqzzvgwx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ytyzezji.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lztlysws.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpasgum.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2uxvzyrhu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uullyanx.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2niyvzddi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wbekbzzm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ivzffyth.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrbqukx.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ofhllzfx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fpnskdwd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qhfxxthz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2murpqlvp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wiqkvkkt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qkyhidgw.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2movtuoml.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mxceuaxy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vaeouzah.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gfcstdqs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2kyrpqprb.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yuegmqvv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2urggtdlq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wwjsdzex.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ioznnuad.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2iflcqqpk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ehlryycm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gysjwgwc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2spwcabfn.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2atynqzdj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhqnbiwu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2djmfurao.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ngceazgg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gdheicao.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2dnawsffq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2nlbreizy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vzouutrf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2fnlgocki.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2buthnqsl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2xgcgzmpj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cosrgevl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nnuqqhnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tgihktnw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yjysycuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfuiezmh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fmgawpvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpxovxnq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2etrzocmf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2dnqslqih.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2sbjdunni.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vhpkakxb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tgeauuzr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mmpseetp.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rztqdnox.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nvvdqfny.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2emndlojv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ocicoims.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2lchkxubk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2maunwdxj.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2nxacldpg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nwzpumkc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2iujehbiw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ilqqyqkr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2obdbteha.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yraziabf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tqnetgwy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2hzhxkwgm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2exuqvyqo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pnmmxmbw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rdwgmgca.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rpccizki.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qoqbmqgd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2hgmxodwl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gjwaqbie.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bgilpsxe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uvtslyjr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sbprcxle.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gdjduloh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ielmamsz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2egcvcnce.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kveqpsrl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jopqbfnh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2bexjxjdx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2muqxngxd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fbfaiszo.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vcfulgix.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rrulqvhh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qkwrbbdy.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ttdqhuph.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mwxiihfl.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bdtitsvs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xtncmile.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wmmmktvv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iiiakhls.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hcksmlbr.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2caluyfxo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2tkzloadt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2arvwqtwd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2codldxzs.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2urfytxqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeglfksm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2iiavpwtq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zupzzkmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfmhlppn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qsrzkiiw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2pmsyuqzp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2rrjpoxoc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2iqhsmmep.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zjpjbpjn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2cunwzroy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rrmhghbx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zkqxjblj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tgeeadww.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jeqnnfli.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zyzfaumu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2rnospslp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rnazcraq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2cclkbcbo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2dsfaxkbk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2iowfezms.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2getapwwj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nlondvsv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rlhtcozo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rbhhvmnn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hyirgtfk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xwbwrblz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bgvolaon.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbieodmv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pnvrncsw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2izjnpshl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2kfhdcbiz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dkglytnk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2raxyrkxn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eporanck.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rupmrhsb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aaqbmhtr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyervflw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evmgksua.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mtfrrzvb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elhdlilk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yhdcebir.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2npqljhbr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkhnhwxe.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jvkdqxnb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nnkbdpbg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tzyzjluw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tnctgfou.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wtrbfjkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivegieyt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2vxgujsqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hldncuyg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2sosafqhs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2mqurbyda.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2uwrxiukq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cvtqjxro.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2sqkdrkfw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zeiwecgp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2djbqytey.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2pkphfpcc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mttgqvlu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lpfdrttd.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2dujbnnac.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rptqzyru.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tcgbbxze.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jynbiaiz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2llsbzzcb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2leemhyuu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wltblgue.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wmelggeq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2adrwmfyq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ojsstifd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2euuibbxw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ugnsxaxe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wusexezl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zwztkeez.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cfdpotpl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jzylxwst.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oyuewexr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ytkildtp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qjpkoeyt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhughuk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vuuaszqd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hatzgtlq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hwufdyqb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ritktdqi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqyudmw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vypcihhx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2onxsgrmj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2egbhwqmx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pijbxsqd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2faldngwx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wsqbxxix.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eyfezymi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrlavdic.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ncfdippl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fluutqme.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bxynwyhj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ywyszcbq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lrordmdm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rhtqoyyd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xiprfcqh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tsjujkjn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2akouxyqd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2owgvypzj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rlpvtszn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvysizpl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ytgkznmv.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbztuok.html


<!-- 参考信息 -->