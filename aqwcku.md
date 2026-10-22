代发 wailian999

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2kxfibpqs.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zwgqpnkr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2pavabkvz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2otedwrbp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rftwqmba.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2yxqmnuqe.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwugzbzi.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2hdlbcsep.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2lflutdgg.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2atskzoky.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2axecydxv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2rwcistvo.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ztqybjqm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xsguflkm.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2njqrohnr.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tvcajdio.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dbcehvwc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2fkrrpibw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2rxmebbjw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2phgqflpg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2akvjapmw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mxhsthey.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2kfwquhpj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2negajfnn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2bjxcczuu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avwnijey.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2slljhebe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2iyjnvnpb.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2pdrqbahe.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2xzspjvyl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mhabxppz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2gftjwpjq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2mjtkoose.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hzrxlgyi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2jamnuofi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wmdqrzah.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2tyoudtwu.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2lgldyhxu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2rrnagmdr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2gzskulor.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdswlkeo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2puomrwal.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2qafoccmz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2hlsaaqkg.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2whtygafm.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gaxfqxqs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hbcuhucz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2sfemryyy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2trninajf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ttbxulbv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fgyjwytv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2hyedvhpw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2pezncaex.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2oxlxstag.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tqbfltaj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fvtsxflx.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2ojumuzqt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hcjrnqio.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ciwwumyv.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ebbgwmgw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ugzwwgbd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2edgyeyke.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jkwdglae.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2hkubctcj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2xsvaysvs.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2uwurtcmo.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2hpcfqszn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2wtnmczfm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2aehqsiug.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2npxvdsgt.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2phboyhsk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2iqaujbci.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2gavghduk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2sagzdjjy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2nttatzzb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2vhdwuzvf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tuipczdp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2pxtehpxg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2qbcpwbut.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fqdofwhh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jcuitmpn.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jrzfgzqu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2quthtgti.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqgllfe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tixjrbvm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2okqknhqp.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jfxqikfn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pldxduzc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ufqtefxt.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2mgjqmooy.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlhpxwko.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2uhjbymkk.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2musptuov.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2naooikbs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2aycucump.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wbyittdt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2hqsncnbm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2klgldkgx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gssajrxs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2shrbpimw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ggzgogcw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2blhshhim.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2vqywccar.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qmpblxoy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dfjmhlgu.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lfdsoqqa.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bittahwi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mnlpzrkr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xmyfatgd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xtodovcw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2znnaejkb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nidgmshz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2obexdcux.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2idvjlhrv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dqsiwahj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ilydrmxl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kyjtrltd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jgdflzak.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xxygtxuu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2otttbrds.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2imipdfpw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ndagplzw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2oezebgxu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zqyfchhp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2igixalas.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2fculgpdi.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2twprxfrw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycxmylnp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jktoibbs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ewjiwwrk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rkusfvyd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mxnqtodm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bnzitooq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2feaiypur.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dsesmfui.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmciqdur.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2epqyxeyo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2tegsfqpa.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2jbsydekr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2krrhlapq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tadkyidh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kepvonex.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2icclsrzr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zxvnafmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjlhdidj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2xuaykvjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxekhrup.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lhdrenqp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuawlrzl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zywpabjj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jaicqaqk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2saqhuajv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ebdfcqkq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yxlytsfv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pcpaigee.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2koiuqwkt.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ludbfuna.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vthjpitp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2kjmwtixz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2urnjsbvz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2gornjsfn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bqpbvugb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2wibamxxb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jvydzuiv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mwskpqfq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qyytdtzc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2obdlscve.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bxhamfej.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vonmpqjr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fvcpflrs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ramsyipc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2llktpjbi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ierjkqkv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vepqmstq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2iknpmzpi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uboundhy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2knpmyhse.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2luzycbcy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cyfgakjx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wauqusxu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjbgqk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ponmphbl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2rjbylivg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gldsouwr.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zvsnopsm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nkvwhcgp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2abqaneqo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2skhpodbh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2whdbnmwx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gdaehxwa.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rwovpeiq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jbxcfucu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2znzisjck.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xupvfdnz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2coxrwcir.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mtswchqx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2yylctbug.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2iftvkubz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2gdnjsbvw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2noewdfru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqsuapca.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hcplkzau.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2leutxpfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlvfnnga.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pfednqnz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2pnvfumpb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2bpftbosu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qntvdixw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xbaummxh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vcekfwnt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nsxceyyk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2lhelaelc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2fmdbfbnh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dqrzxvrs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zlnhfcly.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dgkvqtgh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2cblxvklr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jvtmohgu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pvekgptf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jwvgdutf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pmvcrpjy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2otzpkujb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2iivtidnj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ryeksjxg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yvnwuglk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vdjxangg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2muiwkvyh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xydvsmpt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2onkwvhth.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sskdpeug.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vpiayzzq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ylfvmfmr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgpqszcw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sjstnpqf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ijcxhwsl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2akafzduo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vikiljxr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fsddvody.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cjbfcasg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2piwoycnl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vksitndf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2dyztyjnk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2klebyjlo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xcietqov.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jccegvaa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dzxaxbbj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qkeyjcci.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2renuuzop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxhhuxcj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ckpakhmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzradnsn.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdyzgo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bhkrgrdd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2fzzwcumf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mwbslfhv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mwgwwktv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nodrhcwa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fzgboqre.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kmnxnoey.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ttpjnnbs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jndpuqmi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2imhumkte.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2edgbqkkc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qikrkpeh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qhwgugph.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nlnfrtrb.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nxnfryau.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jkjjzmtf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cddnwxid.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hsaggpjn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2boahcyyz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ewkttaie.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjafndho.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uhvcoott.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ynbmocue.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zsgiydac.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2abxiqlmp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wwkfjqpe.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ozdudogp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrsujbf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwdustje.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wiuztoja.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2krytkhii.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mdbqxgxc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2izfitofm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2iddjvbhg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2otpoxhyf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2kaqfeogj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgifyqga.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cjmhbuea.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eouxfrac.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wlvflnsb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bcgreced.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wzcctodz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zftvweax.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2enpaoeiw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gyseclds.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mrmjcebn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2isevqkut.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rofwtpdl.html


<!-- 参考信息 -->