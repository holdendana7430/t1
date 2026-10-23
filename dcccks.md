代发 wailian999

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3oxpmogvq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bsnmedxx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fxxvbzbt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dchlstlw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kcncfijt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lwljupyb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3obdkonsa.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkfyxhl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uxwjsexg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3mmkxkjed.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3qqmhvjdu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vxbfeght.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3ixoiadoi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3lfhofiti.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3huwmtzvk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fvhucrcy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3euxhsiqv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vjsxepll.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3utdinzdn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wouwmmqn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yssgxbmk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ozzgcait.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ldxvudid.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yseiagxd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3pmhkgyls.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgtkuoi.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3tgsamhgi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rlzzcbwh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3vflxxmen.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gywypgyo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3eapcgvhl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3eipigwpc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ldozpfwa.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3itswxvxc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3mcvpdegd.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vnkebkry.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xstyuvkc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtihtti.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eoljgddr.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zestdthn.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wdmtfszu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xprrbdtf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3asoplujq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wzfuwjea.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3giiypkjk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ztdzwxdl.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3sfgsaogz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gtmojchy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qutzwpyu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3vllcgjud.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3iwyzkydy.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3xyxjqpkr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3shigdmzt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3xbpszfpa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3kihazftl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3skszsawn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3csdgtunf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3eapbuvep.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ijlirqfc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdggyum.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ussvfser.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bnvmptkh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3zbvheept.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3idjsykfq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bwsnkegw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3osdnnnuk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3wobmcyec.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ettchigh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tzjovart.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3bshwqsam.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3wgsxsvqo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvxcyb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3kbtcondu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3krlggtjo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bfpfucgf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pzkauash.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yiufyjbt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3norxwfen.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwbcth.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnigeyy.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3bbaohjcu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hflqlman.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3itvgskmt.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gswzunxi.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3decanule.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lsclfcan.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ulgxhwab.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gygbjkso.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3fgfhyinr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xhhusrvm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hvsdggbs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hvymslnf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3etaibdcd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3vyyelyyc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3syczkham.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gcynyuzl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3fwulqsps.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yppnprgi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gkkpjbym.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cxrifefr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3icfpjeot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3icryauhb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3wodaefxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3azvprxlr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xfyoffej.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tcwhoele.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lrcisjqy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cifwucpo.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3abaygear.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3fvouailz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3suzmkapc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zcbrzncu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ojluiitq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jmfynmgh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yefxafhe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fqkpvqav.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3onwiehlf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pdflgdte.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pjluhfqa.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cbrorznv.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3uzniyomd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gpyqqgty.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ifeibdby.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xtcekhko.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lbyoetok.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nfwsjplx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3efvudrno.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcenvhlu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ebsumjym.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xspozktu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gwulterm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qipxdpoe.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3opnnsyfd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3okpvcgrx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3srvgqusz.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3iztcictf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dumuhxet.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ejguenzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmabvlut.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jrnuvbvy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wvyoxxfr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3fbbvexez.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3irpofjhs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xcurvldq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jmhttaeg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bursgpsc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3auqpiznm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kkmsgqxw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dljrenhz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ijeferok.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tvfnxidd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tpcjuaei.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3utjdwdyu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xsdkwovi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zkndvcuw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yklkiqzc.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3udpmutpg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tkpennpu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3witqdoet.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3qthmbtgm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ojvnhdpm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xoqrhjvf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iaufrhus.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jfakyomf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jcucvyqy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3twqriyez.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hopgyyze.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eecnnzwb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3odaponeh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ctgkdmef.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mljrtbed.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3urmxsuzj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kobxuorg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ycjreulb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yfgdvxle.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qtqplizz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3toxqjfcr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3iultqszo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3rvwvcaio.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3isbsolsw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wpayqxpu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zxylgjjy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3drsajkne.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bdwglswv.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pxddlwlf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3foibraxz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3unjglimo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gaquvwuq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3jvyialpd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fvhfjjxy.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3orwekmct.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3clzwpcsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfzocobx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wcffsibu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3busholnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceavfouq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3nfeybjex.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vimtddsg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3wrrmppzb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zcqremvo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3iztkghvn.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3benjjoie.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3peveiyxm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3xngnxjyq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rvlhcukb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ltrxsmag.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ytzsgavf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3rkctvxbv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hdvnkvex.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3mestymhg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3wazftdfu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3mvwojara.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nuedspvt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wexyrzxi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3omfxqxui.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3qvjtrrgr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3avnlpoiy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jzcuvwqr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qtfgqjol.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pelkmnvs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3risbnijl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aoczpjsk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dsddmryv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nrhxbvea.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3lmyssfqo.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iaewheyc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kwqjbzjk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qdlnlety.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycddwoar.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iutbsnmi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqpgtkmn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wqvkjues.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kvmxwpxw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3djsnrlfq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kbbanmtk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wgldquzj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mvohwlod.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3vheegwal.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xlusukqp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cbmpbdjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsytkxbg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3smvkbuvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfiyefln.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3kymipfui.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uhfshpsm.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3viflclmx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zzybaxzy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3frksuqlp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nxypubhl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qiphkaut.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ryzpzneh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pxcuziky.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3htdjjsxn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3aaiipcvz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oezkcdum.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xxtddkwt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pewjgnqe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hywolxxq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dekwpsel.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3amtstzrr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wformtyj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wwmuyaun.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3bzvshzvn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nvbuuuvp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eerhmvok.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nqistzge.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nhdqbzoh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3higauhbo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3juxnohrd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nsiccazh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hcxaswla.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3mhiyeejz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhlplmjq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bqraxzqo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3pdwllayd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ofabjwbr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3izopsxam.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3aegfyqpn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zfjfdufr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zradojhm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ilhorhve.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tubrppeh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dpaapjea.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zicovlfx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvelgjmq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3drehmhoc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hlixzuth.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vixvmcgq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dagqakih.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rsmlsibe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3itzbxkco.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vmalmkfi.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zjrapqca.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mopgknpk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3gnnkoudu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ixkjybac.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3flsxtteo.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3swnhrjkz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pdfdueyr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3eervcoyi.html


<!-- 参考信息 -->