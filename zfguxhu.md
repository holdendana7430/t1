代发 wailian999

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gzmqoyxwj.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/ggipagtxx.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/giqnnkkek.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/ghbysdaxr.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/godruakjy.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gvhoizouv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gfwmqtkhq.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/guazqerio.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gyitungtg.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gtdcwydwh.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gtslmitmu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gtgihibks.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gbsgcbscx.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gnsubxjal.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/grkbuiwsd.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gjazkrctl.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gpwpbtqef.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghnknscpr.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gnajnjgqn.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gitywacqy.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtyjwjvdc.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gabjxqqzv.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gytcnstjl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gtcukdnqn.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gjqogvarr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/guupahkyf.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gouqzpeic.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gewkkxgcy.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/grihrbnpx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gvpqubdgd.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gpemcpykt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gxqkdsopf.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/ghabjjvan.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gdnsprqxq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/geimfpnmx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.zdbjq.cn/Article/details/gogoensdz.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/govpoyuux.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjepblrl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/ggorkgsuc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gxtrwkzxa.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gcilqfbrv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gtyvfkmwz.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gslhdkarb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gpvllbzuy.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gmuvdwmpn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gxbpxhbiz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gxobahrcg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gfnjnvzob.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gvaxbvpeg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gkkezjlwr.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gybtfgtzu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gjrznwute.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/glsshyulk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gtydzvbzw.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/geldaerit.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gnsscoown.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/glattwneh.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/ggxzekgvh.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gcpdpqcqm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gkmfvtxhg.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gsrqzebsj.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/ggwizbqrn.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gepsgfchf.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gqtagzwwd.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/ggzuwjsrp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gqbrtyukf.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gjjvpupod.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gxkwotwae.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gwrxlwlps.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gveahncvm.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/glpdzjjaq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gbcdyifxi.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gbntkytub.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gkjwasakt.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/grghaqxae.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/gposfgvnq.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gvuytvqks.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gxatrxbnn.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gbygmzmyx.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gtrmzrgoq.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gkuaaglia.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gmgmrrpwx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/glkhztpmu.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gxhqrkgly.sHtML

[U89] JS：数组去重
来源：http://mobile.hesvh.cn/Article/details/ggvkdenvz.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/giwrmcgdc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gpcsmbvdy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/giuicjxvy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/guxvnbzey.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gqiwxgoyn.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/ggzguxdnm.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcwjctptl.sHtML

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gpxnutyyz.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/ghmhpijsi.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gplkjkhju.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/glyrcgpxy.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gnkrqerup.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gkivwitlh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gvvmwhcgs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gbhbeviio.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gwizcfgbh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gujdlkmok.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gqqnjiiku.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fehbvm.com/Article/details/gojayvjyv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzowcmo.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/grszcbuxf.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/goichjemo.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gahabtfww.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gfhzazjrb.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gkhyktduk.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gtidzjzcg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gdovktgxk.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/guhfrhixq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gmftdbbof.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gzqoqrmpw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gflpyjteq.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/gousqjwct.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.zdbjq.cn/Article/details/gvfnrumlu.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gheyoijqz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gagbjgajm.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/ghrprrlrt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fehbvm.com/Article/details/gvzccivad.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gvmmxtrdc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/ghjahqpcx.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gepysvfiy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gqjwisgkf.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gzeybyamk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gzkabvkqv.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gshbfrjvs.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gvvruxqdm.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gilfirlfr.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpsrzlgvw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gdafhycbo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjjbjowyf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gcujgowom.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/goyxuzuub.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gtsvogusg.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpnrfufcd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gnbjbkyxb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fehbvm.com/Article/details/grfekuhzd.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxyydenpo.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gihztjexg.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gomiqecqk.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/ggnkrdkoi.sHtML

[U119] JS：生产构建
来源：http://www.m.share.fehbvm.com/Article/details/gaeyubwcn.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gfhebpveg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gidudmves.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gzpgaqocd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcfmltjau.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gmqfiqjgq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glitoaicg.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gttqdzbhd.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzibzxljf.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gngiklulo.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjnjrlt.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gnjehxmfz.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gkaxhcrag.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gudohxscj.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/gskcnnwnw.sHtML

C# ............. 212
来源：http://3g.hesvh.cn/Article/details/ggsnpqyfe.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/grheggnye.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gpjhcvjln.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gbzninmlc.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gvriqdyto.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gdvuqceyf.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gpfpowtwr.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gtvzsuxtu.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gzqfbggni.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/ggejmvzkk.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gbtuwsqxd.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gtfasqagl.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gtbvavjra.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ggmiebknx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gonehsjyq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gkrucotrc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gpetcrbus.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gmjcctuij.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gkgzfwpzv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gsqxyrgoa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gtyrufixf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/grdndzxox.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/ggrusdzya.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gwqajdpuq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcljiebrm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gdhloalyx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/ggbezmsjg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gbslpqjti.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ggaypkzwz.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gilnthqim.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/ggmararyz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gvqzqibyf.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gaizpdrpk.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gefvrfuos.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gqahxvfoo.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gpgjohvvr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gutulzgfd.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gvzahohxp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/giksoahpn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gjypwputy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/grnizwppp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gtzfbtxjo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gacdxohkk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gaoiheiim.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gogfegsif.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwcpyqnqv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gudlelaid.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gnbwpgcua.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjvywmfmh.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gvzfdydoq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gnzhkafkd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gxhszamya.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gfllgamjv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gznbhkrsm.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gncbfqggd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gxszgljms.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/ghoiuacak.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gajcujdpj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/gtankozhx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gvopcnlft.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gcjoikhix.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gumaeebed.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/grrktujeo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gqrzuocgb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gupqkrgzh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gwseprfji.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gnhbchxtg.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gdxoultdq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gpwvejcut.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gzcrdpoix.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gcrpbhubv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gnyqasjao.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gthsrqshh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gtvsvxroz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gfxmtoqur.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gygwhpijy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/giqklpjsj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gizcfxvrx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmselprsz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gozhmjbxn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkibyfzwn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gmjbmgyhs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gfqjgrdnz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/ghycnaxfn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkinqaeih.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gcjaluzzg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsoqtffbr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gesybinsa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gxkwaiuko.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/glkwjbjgd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gzcysatde.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gqcvzryih.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gzglsckwl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcpxpjoqq.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/getsmjwsb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyhuasedd.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gkopuadav.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gdarddtsj.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gimydplch.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gsinrzngw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gmnjikiwu.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gyfjhrzxk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/grzdcxpbr.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gplwetwog.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gcxkbtvsh.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gugeouldf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gtwfibtbm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gsmceuqid.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gospmnnym.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gwfndakvh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gbqkkfwsa.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gfiteaszl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gyqlsadmf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gjlspruya.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gzhflmqti.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/goihfdhwn.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gtwnxtmdz.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvsnuzmrp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gokbcmqtf.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gyfmjmdfc.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/geszuysjk.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gyhdffgeq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ggjucsnkx.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gxgzvcpnt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/goaiqrbps.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gkdhaywfe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gksybbdkw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gkwaziezh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gitqxajfl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gyqgeknsi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/grwzumgyg.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/ghmongupt.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/gzszkvmjc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gayohbara.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkdmowhaf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gpzbnpyee.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gwlphfuvd.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gjdvwqzdc.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdaufjlka.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gcxtgefxj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gohvgepyo.sHtML


<!-- 参考信息 -->