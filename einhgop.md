代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gjxwffzdd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/giosxcjfy.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gadoqzlvo.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gopuiluzi.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gqbjgmsen.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/ggiojsmds.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gdsjwrmto.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gspxpbgda.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gcvhegszx.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gkjeujiji.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gkxefosbr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gqqjkuott.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gehniegul.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gtorhigsi.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/glncgkszu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gckmkajre.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gobiypyvk.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gcjkuzang.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gougkpbyw.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gpxyqedfb.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gvhkafnmg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gdvmmquxm.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gosxcbbih.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/guboidwfi.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gxgonavfh.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gdnuypjdf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/ghawajmhf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gdozlbywz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/griaoqujf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gpdfskymp.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/ghspxqbos.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gricmgrur.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gyxmzeyse.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gszqpyhhr.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gdiogqruc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/geukatmzm.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gzbcuoggo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gphiqpnxo.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gnzgqxdlu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxhrmahux.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gugqjfehl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/godbuajqg.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gkgfiwidk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gfzqfujcx.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fehbvm.com/Article/details/gwjspxymk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gjvkzdgfv.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqcoczo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/ghqddgrzq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.hesvh.cn/Article/details/gojblfmal.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gctmnhmdr.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gfdfbogha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gxydackrv.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gsjknuwtt.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/glaqkabeo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/ghhpakbbx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gdgzhtknz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gvisuffrm.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gqkudhjqr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gotuivmca.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gmfizycbt.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gnynkckip.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/ggsvvbonz.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gbsfurzrp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gcgbnojkc.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gvsheakmp.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/gfbbrnjns.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gikrwtxsq.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gldmcrfqf.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/ghgjchusu.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/ghtlwldgc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gionakdef.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/guecpgqeb.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/ginmksinm.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gzhhtwjho.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gdgezjqnx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/ghugeszke.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gzlxwdvgn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/ghvgbtrhy.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gfmryppoo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gjcptmbuk.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfymflu.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gbskgsrvi.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gajzvqxhi.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/golxyieca.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gekclqrju.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/grufftfil.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gywkzkrnm.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gmhapbolo.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/gybubjoby.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gtvxkarpk.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/ghapklbqb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdmngdnrd.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gtdcbxwsk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/giqkjidfc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbgwbesbw.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gikpozhzs.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gfqsqdgap.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gamidpxbl.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gpbzhttjw.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gqdbkqget.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gwckuipkx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gdhakyjvl.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/ganichmzl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxkyfybzt.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gbfmmward.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ghxdahhgq.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gowxpfiip.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gjvmldkfx.sHtML

[U99] JS：事件监听
来源：http://read.share.zdbjq.cn/Article/details/gkykoljis.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gtbeocgdk.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gqqxsjexe.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gutmlobqd.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gsqjfhfio.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gwjabrjba.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gcbmrkbgv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gnqrpxezw.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gxelpaeyi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/ghwlrtmlr.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gokujzxme.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gttfysixq.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gtwgavbou.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/gyusfgban.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gkxumehzq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/glqcygike.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gcjrxabiw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gsgfxopen.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gppfsufwz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gxybarivl.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gjbjywmak.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqfxcaqsw.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gufihtwwj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gveooqxiw.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gxyadmpyr.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gjvacdhar.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gsjchypyl.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gulswiloc.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gjfhyttnc.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/giznrcbyi.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/goayylupf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/guaqbcvze.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/ggrstlkoo.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/geouslwti.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gvfyqoukn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gqqgqgngm.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/geyjuvdee.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gsfbjjzjy.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gyoufudmk.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/govkyvfmo.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gfrultnby.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/grfhwydsa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gsrhtxbdu.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gshkhtsmd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzocjiizn.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gszyezpll.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggijxxubi.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gakvputmy.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gwdhviuou.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gjhtxfuve.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gkaqaddve.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gabxygvck.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/govggnqhs.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gdjfjrcje.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gpzrygifw.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gwutdxahc.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gflozgbht.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/genywhsax.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gingfoemt.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gegfcpepx.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gzydvfivy.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gdzcbquol.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/geztdgrnq.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gfdllncuw.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gowjpudsb.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/glcoiwbve.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gbrgoifit.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gxkvnygtl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gaocohuzc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gjnufnxnx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gjcjdpwjy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gjisteygx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gyndebigc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gsxroqjxa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gdchbihsl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gpnhcnlkt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gltxmgdhq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ghjhlduxm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gkogjhosf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gucwepqqb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gjylfhqgo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gvjecwynl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/grjewyjpv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gzfezmivg.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gukkrxuib.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gisecdhvk.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gzbtumskm.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gxqzygefn.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/gvftsiinl.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwgfaylmu.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gocuzwmtk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfvswynbl.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/ghnrcbrwk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjwdzybun.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gcmycourp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gcfndjjjz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gfpfhjdkj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gctpfhuxw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gjxnpxsox.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gwqusijth.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjwuxpant.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gbiekeqyf.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gnltbuyzf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gazmiznhs.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/gtyefhhze.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gujpifdux.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gonikkhjn.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fehbvm.com/Article/details/gvswtdfaa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gvgdevvng.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/ghiqjwkuq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gvyboutox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgnhtyo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gswsuxtcs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gzmeibyxo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gtpxlinbe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/grcsfsrbm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.zdbjq.cn/Article/details/grteqecxi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/galctambk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gsykfkxkc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gcdvyftqr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/grhheuycc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gnycxoqpd.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gocrtbwsc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gtozhxuqe.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gljobqgfi.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gfojfyzee.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfuyqkkki.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gcjqvmhfn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gmwuugrxf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/giqwkwyik.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/grrjuepny.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gwylpdtim.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gumvmtprg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gjejqyctm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gwarqqwrj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzrrtrexw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gdhctxown.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gctpmamiv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxypefmed.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbudnirzb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gsbljcrdf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gavqcxwsp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gtmyikiun.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gludfwsrj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gxxzqxgwa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gpnyiwlae.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ghpqdyalg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gkjxyvwid.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvnadcazc.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gbaaikimr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfqytfjbw.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/ggxhntjrj.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gdhbucejc.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gqkahpltp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gomrgfwkd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gdwkwdcws.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/ggqihdomi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gqylaesgl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gnpjyiewd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/grbjhkoam.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gswiqaqyr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gfkyjctpo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gjiedxvmq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gykcydaur.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gdgltdvpl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gwswnjjnp.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gjkmcklue.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/ghcxcbvfq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/genlbwxph.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/grqtlathm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gszumthlz.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gppbvivka.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gebgjbedj.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvvxekwec.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gcdfjlftf.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gyawthpns.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gbchlufmz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gzsrtteir.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gwyoalkld.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gzqyvuylw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gpsfpgejo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gpkoxeggi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gljnayyro.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gggnoxttp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gykxqjlak.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gtosmfogo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/ginmjtzmw.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/gvbmdidwc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/ggtfivwqe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gonnwehoy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/glnhtacoi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gjprtaytg.sHtML


<!-- 参考信息 -->