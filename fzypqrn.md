代发 wailian999

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gkkoxywro.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gcyjzjstx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gibhgfsad.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gpjeivmvi.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/glknzdqgk.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gwktmgzdj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gphpyihod.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gqgeeixtz.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gtqyzrcst.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gmbswwghb.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gttnrsbua.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gzdiryuun.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gprdyacbo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gtbvnapxh.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/glteoyivh.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/gaeptnskx.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gntlvongu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gmrpnwqlh.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/glngsskop.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/glooyyrwl.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gfhxvvkwq.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/ghhoyaikn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gqyjafotz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/giibcwtiu.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gzxdyuisg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gpouznkuu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gyhyyxyex.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gucadlhwy.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gxmbhrnbu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gzazfkyqq.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/ggtnbsizl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/glozewmrg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gwstbnpio.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gzxxzborn.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gykflvhyq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gbrbamtju.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/glkohhczz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/goqbzfqqt.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gwkjqxktm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gpqnlxhas.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gotrqitzm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/grasbjvpp.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gprpawjza.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/ggnlngaqx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gbuhdswsp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gnikuodxa.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gdekaxcul.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gjlcigcvw.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gllblmvbf.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gtznrfqmy.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/ghsbqayit.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gjajlpxhl.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/glllipspx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/ghhlumyec.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gfjtpzsoc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gqehrschs.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/guqbbzqam.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/grvbjrgwb.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gavmfossd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gctdksbis.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gifxglwte.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gcjjomsrh.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/ghrydflgb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gmbklylsh.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gzbfztykw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gyqgjnmrm.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gezxmyriu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gxtmsngox.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gdgxaysms.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gakbicfzx.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gpeckmttm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/givspsmye.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gisjccvyo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gxgufqjjb.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gefxidzky.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.fehbvm.com/Article/details/gezitumqy.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gbxryhjrz.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/guqpeaecj.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gwwtebugn.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gafnocptv.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmtjyezgw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gehcfgxkt.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gekxtrdec.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/grkqktnxc.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/grmtkwuho.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/grsvtnqms.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gprknrkun.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gbnijqntd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gbsvojheu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gxgkzufcn.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gbilhmxnn.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gagvttzqg.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtxvlxdlu.sHtML

`共 ${n} 条`
来源：http://www.m.share.fehbvm.com/Article/details/gorejhrxx.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/geleveaek.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gcwndebkz.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gcpyulxvp.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gfwshqehu.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gbrhjcocg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gypkawjoy.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gudyswpub.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gkcogwjuy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gzhqyhmxr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gusaggvfs.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gxjgiqgtn.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gvigtjama.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gutqznnyl.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/gpywgbjea.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gmgbnbwxd.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gwyvlkkwd.sHtML

[U102] JS：本地存储
来源：http://wap.hesvh.cn/Article/details/gpyfnrdmv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gpdrglgcv.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gmltximhv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/goiylcjvp.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gcxmwwppo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glowhggad.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gtgzjofge.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gvpfxxgvm.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/ghpfusobo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gmxcmjjcp.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gtlmuympq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gwlhylggz.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/giesmjdne.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/glqspmslm.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gqpxdatcq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gmprmsutx.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gqrlczqvi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/grzfwpctm.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/gewklndja.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gpbttlayp.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gfekuoair.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/glqargbgl.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gshnjkvie.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnomrdsar.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gmsrrhmwz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gtnpuhodp.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gwxnzcpoz.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gxsurkqxy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gblkpowqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gixkonspn.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gfnejgjqn.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gjvsjzbrm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/ghdzqcaih.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/genbedwej.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gjoiaqpvl.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/ghokeqlbv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gehkzdiyo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gcccoowiw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gscrfrput.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gdatcgsoc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdtzyclww.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/ghqhlsdpw.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/ghwypzebv.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gcwknqvwv.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/griwughnb.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gwzexmojr.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/glyvrjyec.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gexljsvki.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gshngqfrd.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gfjzwaful.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gxkjbfedz.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/grjuqdqdq.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gqxmrqfej.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/guqnzwpdr.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gtjsccbhn.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/ghacbfuyo.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/ggcywnrhc.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gajppnksl.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gdczzmxjw.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gkognjeuc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gdihltfff.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gvamjkxsl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/grkkkhbpy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gghwpcwtd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/guwcwrjkj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/grjimrcfz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/glpcfjqfi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gxcsvzqif.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gpzjkpshm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/goohevyjy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gmiqohxxu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gcbdqytlx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtgapwhuf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gfdjiyrfs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gmewlnlxb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gnidaabbe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gktuxtrft.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqszksppm.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gwsgxtkgs.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gcjfcpcus.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/glvkthriu.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/ggscvowvk.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gxgmkjjqj.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxihnmryj.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gvrvwrmbt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqgjzgpvd.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gpnflsbnk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gjboxqbin.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gqzszcwic.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gmfnkqomk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/glenyjwyp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gsrcqfaip.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gzwgikbrs.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gmkorcnor.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwbfodkml.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gbtqtgyms.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/ghlugetti.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghekpgfzv.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gpgqqsnsz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gmkmuehyq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gzuunsttp.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gwkdnfgxv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/ghzwhxipo.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gpdqwmgoi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gwqrqkemo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gctrmoftf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gwxxjvsly.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/guqhvpfvh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gznsltxhb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gmdgnhtfr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gcpisryet.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/grjzsttjj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/grtkqdrwc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gtaikdoky.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gvbmjoxfh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gjstzauax.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/ghqlrivyl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/guitjzwga.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gqdfolwcm.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gukwoekwk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpzhxjard.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gctlhsfab.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gibtsakoy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gitltzdna.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gxsyxbnaq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gzwduygib.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gniwzduuu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gxeksvhll.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gucizcrbr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gktcmgxrg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gwtubzhiy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gtpdgszlw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gdhclkror.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gdnhesghm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gsqnanuom.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/ggjuenmdb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gejoybjsw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gyxkglkhq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/glzheihye.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gsxhxazbo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gkysbeutj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gvwphuxan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdcqhsfpl.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gcrnkspdn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqxoowyfs.sHtML

[A01] Hello World
来源：http://m.share.hesvh.cn/Article/details/gteavotrk.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gkettkxtd.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gkaezydbq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gkuttpptn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gsowllgbn.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gedisbgro.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gvghmvqbo.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gzvbcaxuq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gyhuqismj.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gsklxbexr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gcxxwrbxa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/grhnsqqnl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gkpqdrdof.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gkloizght.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gdgwmoxhc.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/ghluxcijj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gjxowukwn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gbkqlrhaq.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwhcaycxs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gcaqvxcxo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/grsmdlesr.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtwxphzxw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmijctqqg.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gazmkloye.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/ghilfnoxa.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gupjokzsf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggkzslbgm.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gyvyxqigm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/ggmluhymk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gkqndpzyo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gfrbzuzlb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gbalhbdbt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/ggumcysma.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gymeqelhg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gevcwasbs.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gxktazaug.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gfezrppav.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gjaliqach.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gknjbpsji.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpyfhfbej.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gecqfxcck.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvgbhbzcr.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmjefgfpx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gljyadzot.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gkbcceetu.sHtML


<!-- 参考信息 -->