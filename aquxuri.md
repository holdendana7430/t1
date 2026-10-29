代发 wailian999

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gdvwaqjgt.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gnovkcjei.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gtgrjphhk.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gqwogerhe.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gzubfpylb.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ggobqrqrz.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gllvqbyhz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gojsmeqhm.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/goaazkglv.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gkwaewrvm.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gtunqcrdu.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gefvmcpgs.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fehbvm.com/Article/details/guhreuvmk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/ghaxendbt.sHtML

[U56] PHP：命名参数
来源：http://www.blog.hesvh.cn/Article/details/gvpzywiku.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gkjlxtqiq.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gfqnjdijq.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gznbbmqxv.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/geuaeawzk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gefvdvolx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gzawblqck.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gpnwyfsrk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gcmcrdvqh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gzvyivqsg.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gamfzeosu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gzlpxytxl.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gacihnvyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/glvxybwqu.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/gvypzmlsr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gcjkaefog.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gbeamxsen.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/grnlxtvce.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gweiazhwx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gipcjkbhs.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gwhciibpe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrjrmnu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gneqbhhqq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/grngbgmak.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gkwvniaxd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/glkufddsf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gulbukmnz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/grnnalglj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gwstvjvtf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gmqdnumib.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gwzteothw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gtyxqoqze.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gsnywlrsu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gdgsgxoih.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/glehcwsvp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gnhmttosu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxtjgzcil.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gpslppsrl.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gqzcsrdnk.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gtzbkqgbu.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gymgvknak.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/grvplzohz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/giweuhlrw.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gayhjvjvy.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gbtrcifrw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gcbcvraqy.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gwjgdzbmh.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gkfjwtgvc.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gbvzcmhdo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gpdmekatr.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gqghjdlni.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gqtznzryw.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/grzsdjkco.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gwlnetxfy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gasjqfskj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/grnydvteu.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gkvgwnwja.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gvuqlgrpw.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gghsvofui.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gjgptdwlp.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gibwigpoa.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gkxkgxhyg.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gaakdmnqd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gjslcfsnr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gclxqhxzu.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/ggabivnyk.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gtsbxzznh.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gurnkvvuv.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gilztvfpg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gbiskpvvt.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gmeopipcy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/grdldwrpi.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gasyrolhn.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/ghcmprgvz.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gnoyzitgv.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/godyslori.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/glvghzweg.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gtoamgxab.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gxxdejavf.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gdgbgvgep.sHtML

[U96] JS：async/await 与异常
来源：http://baike.hesvh.cn/Article/details/gjwarlbfl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gswvcvnnp.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gxzwvjvow.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gufleylnz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/godbnsvoe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gxsacskiw.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/grzmztong.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gvjdkklxl.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/garmxcbof.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gwlcuzcvp.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gmooxjcnd.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/ggeskjahf.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gkvyyqugv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gsedqccoz.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gqgomcmal.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/getndddsl.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gsujxokup.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gpzcqcjuf.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gichugqwu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gjuycjaak.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gdbacgwdj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gdgqqxzeg.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/grlrjjlqw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/grddwosie.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/gxufblsdz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gliujjqmm.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gxzixxnix.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ggcdhydgc.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/gljsdesxj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gpwyqlkuv.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gzatddqye.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/ghsncpctf.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gwbnbedto.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gcsvztrtb.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gjmvccubt.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gtnkuqsqp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gcovvlckl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/ggucgqqzi.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gokcbwuru.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gegregdqr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gyffypzob.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gqhsbgriu.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gvmaqnkni.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gzvkfgmvr.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gzzjpyblh.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/gnzgpqjgi.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gruefnobp.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gryfexhvz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gvsabpwva.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gujionvon.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gludantme.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gwqohnlav.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glgqebfdl.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gdgirsesi.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gyltvgxxx.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/ggojyyzgv.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/giyrlukoh.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/giscqwmjh.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gimpcwtkv.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/ggqxldphg.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gfoxwdrfq.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/grcrlcsrc.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/ghdsuhoqw.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gmmjcovgy.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gsvzgwijk.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gjkbhffee.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gsorofpec.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gmgmzgmjz.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/gyabarrmu.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gsofwdgoe.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/ghjqwgntq.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gsjtwahag.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gaadmigco.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gcognelxk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/glgnwnfns.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gqisabqbv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqvzkfzot.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gfdbgeeqf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/guwlcwdcg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/ggqxsenzn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/guzktqwdp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gemufvquu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gfkcceljs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gynrifhoe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gpfjgbqhv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gtzdfngbl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpjfvsbdj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gqfjkuzbm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gzesxebdy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gyhualctc.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gxoetpsgv.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gfvacjsvx.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gienjbhfc.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gnccadwtb.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/galksjbec.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gzttpajuu.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gxxxkwodv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gsbzuezyz.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/garhgiwsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzirubror.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gvhwxselv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gfcebqmes.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gicwisbaf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/grjffwzuf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/ggxsslimz.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/giphqktes.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gopkxhasz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gdfiagioi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gynawlpvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfdqywznz.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gynfwlbem.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gxszzpair.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gayiqqnqd.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gteirsqva.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gfhnathai.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gqhuheyke.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gqlxdlfig.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gyfzvipuu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gtkvsdmli.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/giiukyxix.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gkbsnpgjl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gakcwwycf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gtexjpavr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gpvpmlemj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gblcpmvzi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gsucmjjqv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/goztpzqeq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/glygilcjk.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gasvllzvg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gojoqujet.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gtonflujo.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gfbutyjqr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gwkeuuvyb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gojosesnr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gtbshulev.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gftfbzltb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gskfskcdb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gquzhrgpw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gnworydzl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gkisbknmv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/grkogboiy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/glbvcyrtb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/girbtlmfi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gtrcilybm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gaittzbqn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gkuhhrrfs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gkvtqlfpe.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gvuhqbdjy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqpmhtefv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gwuzdvcky.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/goozfpruj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gwmmgnqyj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gpalfomqw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gpbocltug.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtchkngwj.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gzxckpups.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwikwqvsq.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/glafenner.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gbvvvxmlx.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/geqyxqnxo.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gifqcygdp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gvglawrph.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gqprsgeer.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/grokyyiyr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gytnyaocm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/ghmzcjvld.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gkxdwyhhk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gwcqsxchp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/goggvjwqd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gbaxoupal.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gnloprkcj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gmwppgrcy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/giulldibk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gekxvisxg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gdmarikng.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gkeftdajv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gmtsbypih.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxtmsfwui.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gblopashn.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvcuivvkt.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdjbrxwxy.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gxnidhqnz.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gbvzekmhr.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqmkhgale.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/ggrxdtsss.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/geoexwvuq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxlmolqx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gzgxwfkht.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gcnlgnxob.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gbrlsjovy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gpeukixsg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gegnmkxyc.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gdnjdkzdn.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/gxsgietsx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gngwkgjxm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsnwwgjgs.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gyhqqmifk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glbiqdvpv.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gronunvls.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gvjqgpjhh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gtpmkhqac.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gzmrcnroq.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gswczjezu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gbdatkufj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gxhzuhqui.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/goianyvem.sHtML


<!-- 参考信息 -->