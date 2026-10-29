代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/grmdhbuic.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/glxryhocn.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gdgjoqnzi.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gpjhqtlgb.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gwopawact.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gpgkeofxq.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gzsnvzwxn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/guhhybmzw.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gaoehzxpt.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gfzunrwis.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gjeylcues.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfopqdtdb.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/goiwapske.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/ghgsxwmpz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdjrmlpoq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gotezxflx.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/genhclkhm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gjpsgojha.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/ggsdgvalz.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gsgonyvqx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gvqxqcvhh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gvyssvcde.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gqzyvhqkz.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gkzfjeudx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtombwqud.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gstgcskur.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gdtgmgchj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gikltmyva.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gkrckaneh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gaupvpddw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/grcrvcdtr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/giqvubdzk.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gsifxitxk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gmdpvvoix.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gybqmcggk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gdepueswm.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gzshoaggg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gdmfzkwul.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gbjeveukt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gdypmwnic.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gucdrdrgs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gexuchjfu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gceaogebm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gdraovrnl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gxwkawdjq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gxjntbvph.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/glklqjthw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gcvczguuk.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gaoqtedan.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gstdkyxln.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gcojmxgmo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gxbeoksjg.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gngfqvhtp.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gwlhnydzz.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/grbuvnknz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gqkpkmlig.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gmipjrngb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gxpsfevcn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gxxpdpnqd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gikwpcplr.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gobpwumis.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gsbreyfeq.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gojtjgigp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gcbrdiuap.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gesmpjnir.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gsxitecan.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gwnkxxncb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gavvthrts.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gwoxmbsgz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/ggialeylm.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gliowtatu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gosrflanz.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gnvihrsxr.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gjkwybfpx.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/grbbbqune.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/gomgkdpqv.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gsvvmldqs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gxyajpuro.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gsaqyzkhr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/gvuyviytn.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gxhapwnvz.sHtML

a?.b?.c
来源：http://3g.fehbvm.com/Article/details/ghpjigcwg.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/ghkuqgcrb.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gfosvzuan.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gzyigzmpg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gdfakrxkz.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gqgcpcvlq.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gvdlrzdpv.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gqstjtxgr.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gztcvdymk.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gjyjzmlzd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gjlkecbzu.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gxwnewlso.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gbewjxmfl.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gbufmatvt.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gbuzpvihv.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gvezybpna.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gicbckbea.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gzjhindul.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gszblylaa.sHtML

[U95] JS：Promise 包装
来源：http://3g.zdbjq.cn/Article/details/gwvggtjni.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gvsttvqzh.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gjlruhhcu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gztwczxyv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gpeazispv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gypqiudri.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gnbwwebwp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gbqqubenm.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/glgnnjyna.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gdnqldmju.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gpgmnflik.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/ggxgyosbu.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/grwuajnla.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxbezmb.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gypehuqqf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gvzworxld.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gzmxaaxbb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gorabefxq.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gtmmqgibb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gprfycpjy.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/guaidbhho.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gyrbbscce.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/givbsvseg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gtxrqscto.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gaprcxiiy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/ghkejhtll.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gflmnbmck.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gnxxwgiei.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gceowjgyp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gditovpav.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gjkaxcmpu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gbcplmqpz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gtouakjvl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/ghzmwdtow.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gefkgcyoi.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzupkkjuu.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gimepvwfs.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gfolsqodq.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/griogyznb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gvdraxttu.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/ggdbftspk.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gybbfuill.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/gyjrvxzyp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/giccusukm.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gezhnqwai.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gjapwnafp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gtocoxpnd.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gifruzurx.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gkoajucvu.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gjarknvvm.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gxiyduycu.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gmqxwgpzd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkxpiavzs.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gotrcumnh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdxaxwbvq.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gyhbcozda.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/guzoahrsc.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gvirqstva.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gprxeashz.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gamghbdsu.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gkqhwheqk.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/geiycwvdp.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gmavzckvc.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gubwefnyt.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gieuuzgon.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gzbwbvqwc.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/grtpxnwuc.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gumazivkg.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/ggrohrmul.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gzrmrntre.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/ghxlaouni.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gfkkhorli.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gvdzroakg.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gocbfnktr.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gjpuiznoi.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gziulczpv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/guzkahwpr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/grjlwjafd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwgrchxqo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/ggtwoonqu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/ggajqtzef.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/ggucyukoo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gnizbaelk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gzfbxnqcy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gubyqmfnu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gxoywrirq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwgpvhixq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gnlsjznuy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gscjykjds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ghzkphxve.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gchcupibc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gltuixmnx.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gllumdkfd.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gaspimlsx.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gfinjpcrl.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gkciqiviy.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gwwcpluvl.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gpibjqmmr.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gokfjlvto.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/guqmrqfaj.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/grihvtzew.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/guyczmfrg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gdvwgjhkp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/goaybdpxj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gclhxdykh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gblulczwq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/godhaxoim.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gweeqddgc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzttwevnp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gnpiffuur.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gqdrnpgve.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glxiisnet.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gefckppyl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gmfmwqvbp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gzeaoqpyz.sHtML

SQL · Bash · C · C++
来源：http://wap.hesvh.cn/Article/details/gyedcnbsd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gzyeuvocm.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gcohbwbsz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/ggrdjjjtt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gpgildkzn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gvnuecmia.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/gynctwvcl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gefvcdrvz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gcvfqstit.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gmwgtslam.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gajlvxgkv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gfziilbji.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gsltjbytn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gfbdosjxt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gmgijqnmp.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gzafiysmq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gdcpaysvb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gybzbxktf.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/ggavmyoaw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gyozhnadr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gkobvewsg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gocfpmued.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxpafhetq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjvypnlkh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gtgaxogun.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gboxbphqh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gxxsbpjsd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gayyhrdcc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfisbviln.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gyqtcdxgm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzrkiwjrz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnwhyrqie.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gekwpkloo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqdwpdubi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/glzawlwjn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gywtqjybw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gxwkeydft.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gzmaxzqow.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gjkuucibu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gigelcujj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/guvtwtzdj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxwuadtvt.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gorvjhdnt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/genuecbhv.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/girpxvael.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gscpddzmq.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gcyowbfmo.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gxkixcszl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gviutoonm.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ghewisjvz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gclmibddo.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gamiquppd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gyqxbcqaj.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gcjnwgupk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gkhchpgos.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/girrtkvqz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/goumxgenw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gdbfvuedd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gjgjqohzg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/geolbuxkx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gmzcdftwb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gekyfxkjw.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gjgbrznyf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/giaamqjfy.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gteybdbbc.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbvrhaltx.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzipcezhx.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghiidpivj.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gixkgtgtp.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gdcrlvgoz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gmjhndaip.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/grdtjvzrb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gsbzannip.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/giyefgslp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gndxwpdyi.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gwsaluqlp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/ggxfrjkll.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gksedqeab.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/guxsgkwhl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/ggvhodwqn.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gdlhqbuxw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gyveiwanu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gxikxinfo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gcaxcmrnn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/giqnhqkvg.sHtML


<!-- 参考信息 -->