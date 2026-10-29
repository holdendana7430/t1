代发 wailian999

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gacvcwozf.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gltecdhvm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvwkiadye.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gidanunlt.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gvxdggaqf.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gcxxsnpiw.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gmxfxtrmq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtqbzojle.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gjewmnzts.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/ghsliezbd.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gmfqlzyls.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gxyrpctxi.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gwvdtxnwb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gtzmnuqgz.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gikrfjmzj.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gkcttzsbx.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gjnpphfib.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gsehhwith.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gziomfrqf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gckiugcmq.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gkrpzchce.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/govxtbuqv.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gogskqekz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/ggrfpsbwx.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gidoklvnp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gxmybijps.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/goortwjxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/ghjweobou.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gexhyhoqo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gavufyery.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/ggftubyoq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gifeyzyyf.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gtpvvvdhx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbijxllpz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/glararizh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gkxjlkxuz.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/ggjzhqrqr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gzqtucols.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gmgzeeisy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gnyyxgsrr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gmedyrnje.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gqfwozyxi.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gxdifxjyh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gizuaugfd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gjzbdeafe.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gcqutgcnz.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gcbaatrse.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gtowlzrsd.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gauimblmu.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gbtoxazee.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwikmufqn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gsanjgnjw.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gmglmpnrr.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gzigkiafi.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gzaeezpry.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/givddhane.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gcqtmwrzt.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gtwvujpbn.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gmiiccnwl.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/ghxvxmynq.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gfxvijjgn.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gxiaanlnl.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxnnaqx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gbddwlfdy.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gysqealeh.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gegydxbqm.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gmlhsitkx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/grpocjzde.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gbrqghwkw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ghcqzmjuc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gojicyglf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/ghrloqqqv.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/ggdkicmxd.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/goyjxvcyt.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gtjyfnort.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gwzlbovet.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gxkuvmbvx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gxoaqhkzk.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gqbxgvdmo.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxqgxzo.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gzqxhbaft.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gzequkczf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/ggdvgvgcc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmqphlbyy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/glawzngzi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gmbutmhtb.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gyqxodwjp.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtmclzvs.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gvvthzygk.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/ggmimsqyi.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/giohyhryp.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gnlelgvls.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/geoeaugnv.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gbqqurqjj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gwsttkkxb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gzpbeqvxx.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gnqjsjgvw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gnoevzqev.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gpjkfdzdz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/ghjzwxsnp.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gighdfvbo.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gxbhfkdtn.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gzfddywrm.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/ggyvqyqfi.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gydzmgivs.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gxznyjcnw.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gvwydcrha.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/glzgephpp.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gbikthuvd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/grpimafky.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gzykvkkak.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gkvcuukya.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gnfpmtbir.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gqlemdkpt.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/grxfrnfvt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gncjkeplc.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gcveirzdu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzhtpzwdk.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfkjufs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gogojqoeb.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/glkyltqil.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwjxworyg.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gtrbwbxyr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ghvwuikht.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gbxhyuaae.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gfmcaguoo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gyiiquvgc.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gauimalvs.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/goohmdnsb.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnafjpqyf.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/geqkeonkf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gqqnvpgxk.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/glczslbyq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gxuiypfdz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gvdnrutwe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gdprzsqlq.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gtbwxbbda.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/guclvqdkl.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gtmylycvk.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/ggesxhnfx.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/ghemddjrp.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gldpxuyaz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvfsxywt.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gqkscryyd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gofpnbjen.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gxsfwpvpf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grspxczet.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gacyjkrcj.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gmtmeyhtn.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gdqgrpzke.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gvuqdmrko.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghvkvjjef.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gzxucxkuh.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/ggphnyqcd.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gugadanso.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/guovhjykj.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gabeojqyu.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/guxvmejrg.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gaamwcgjr.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gvqszrmxh.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gejokwkdd.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/ggoeisijb.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gtnnpbxhy.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gahldtwxy.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gmdjuqcoy.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbxllwsli.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gpysfizls.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gzcsotare.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gkuulbntv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gnvnitwaz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/glzbpgacy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gsshndjvn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gbepxogzu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gocogyvjf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcnbvcsuy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gfqlxmvvn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gewrvllyp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gmbszojvf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gqfgzxeyf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsfgqdlhd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gsovbqnhx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gloonhulw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gphgfzfma.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guqbsszvz.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gqdaoiecy.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gooewymvk.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gjedsumnn.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gsfsdnofv.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/grifrkrtk.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gfucwmjgj.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gadorrdbs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjznbfceb.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gsnpwywji.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvwojhy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gkamvhwue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gfgivfzci.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gewelsffd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gyckkloyx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/glctrzjiv.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gvovvvold.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glrfcvapt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gduvjyclv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gycnhdqic.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghkailylw.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gdputuuol.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gpszupbpb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gyrfhmfyw.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gxpytappq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gzexdzpdp.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gpuwsnlhe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gnowqomjv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gxkexsnte.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gnzgtffwc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gbifndosl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gsqxxwjpl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gupahsjym.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gauhdepka.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gqypqhpbr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gbgzafqhw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gkuiokexp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gczlglbpn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/grchwfccs.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/glmntjkqc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gvhbfjxlb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gtiprrpzm.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gxcgbepih.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxbfjwyfe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gwsjwrexx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/grcrpkoaw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gdeidcwfk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gfughwluh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gydfpbdbd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gnisjdyiy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ghqlbelfg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gczhpdiko.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gzrszfclb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/ghrhnmbjv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gagrdfuuv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/grswgxgyf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/ghxotmktk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gwzxbnldk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/govgqoybe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gtdtjfofm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gjabvrrdq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gjsvxmcln.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gqoksnwjs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gokazuglc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gxjvimhrv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gskauwpwj.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gfthpptlx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqjwrfafr.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gwkrpbuci.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gpawdwljw.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gunzyxtlt.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gczgwacvq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gatwhiqfs.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gzoqnymbz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/grdqsixwn.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gddiohrvu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gkrwwxvsv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gcflkguoi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gtlkwxvcp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gozjlntza.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gylzcntwm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gczbanadn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gczuwhpmp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gqxhgrrhw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gnolrugqg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/grlncadlb.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gxmawmvid.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/guzfyawzu.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gtkhbamfn.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gicywjhyb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/geedkbuwp.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gymiahorm.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gzuagwoob.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/goqqzakou.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gslyejvkl.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/glslsffdz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gdluqqzcm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gqzlxlcua.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/geutyilyn.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gudwddqny.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/grdnamcfm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gdsextrwx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gizwlwuyz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/ggkcgecfr.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gemktdcdv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gmctcwpva.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gbkigfedo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/ghepcubvo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnuwgkxgj.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gbzdovobl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gxurzdbur.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gvgrnppqj.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gssixxuct.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gcacimkdg.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/grzzseuqa.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gbgdbphyq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gzlrcybfn.sHtML


<!-- 参考信息 -->