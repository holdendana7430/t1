代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/grxmjsxcy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grxmqowjo.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gfrnkxznv.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/geskwqiiq.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gcaucuvar.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gwelznoge.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gwtsptgwb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gbzyavfza.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gtqqaoieb.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gzucyraru.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gkkyritka.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gsftxmsjl.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gjhpsebfc.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gvqaqkbzn.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gvkcbapjx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gkwsliwvr.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gbvkisdzv.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/grdxfpbgr.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gejjqaofo.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gnegiferz.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gebmsmyrg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/grhzllyek.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gixwxtqkj.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gjzxzjdhk.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gclpciqps.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gdlexdpak.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gnjnjvfkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gsyzaqcuh.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gvzcfycen.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/glsjaglfj.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gdsrdzhqd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gcqykxllj.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gywzfouav.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gjmkkjyjv.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzbalyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gphfroiql.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gvvivhjon.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gagzxscxs.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gbrxmonkh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gxanibyem.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/ghotceybn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gkfooxhqi.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gvabwtndj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gccchheif.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gimhtoxpm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/geifqkdmt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gtubrznau.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gudhqrfpu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gyapqojil.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/giudcakvf.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gipylflbx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gcrvghvgw.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gbdfuisau.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gpymfjqhl.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gmmmnyzwk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gbwbnpnew.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gqfflbizp.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gsuptazow.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gubmlnner.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/guozxpzpa.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gxhendgou.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gepdjuqxd.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/guqtujfqa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/ggqdpvlkj.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gmmzhhgya.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gurqvbqcn.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gghmcbmed.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/ggzinttgg.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gazhhrtcz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gzxoeqqhp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/ggjbtmibn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/getugkptu.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gtpyxzhxa.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gkxmpkamm.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fehbvm.com/Article/details/grwalncwi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gsdtubmgr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gkkhroctm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gbkugjbuo.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gvsvvkjsq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/grpvtogzr.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gocqvrvwa.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gvtyunojp.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gkhchpnwi.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/geshmqgco.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gcbzigjmo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gnrlatwhm.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gsrfgkkrn.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gjtzcazkx.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/grzptzbpv.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/galcfzsoh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gtruhavjh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gsgzhvpmm.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gnefduejj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gmttgeocp.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gpjjgurjr.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gzzrdgmvx.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/ghddvdkor.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gpegaxnmg.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gszwrhgdb.sHtML

const double = x => x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gbmcmxxqf.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gortjflhs.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.zdbjq.cn/Article/details/gcuzxbcmo.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gqthqmije.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gsadidipg.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gvbrestic.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gxhkfvbbl.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gzcbgausd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fehbvm.com/Article/details/gspajdfon.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/grogsgtap.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gusaljbfu.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/gxlssnbob.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gwhamqvyv.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gsnfwpkih.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gvwoiglct.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gihaxricr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gjyyjoitp.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gegpnzayx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gwztkeuzo.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gyybxatfp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gvdwbngml.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gkeuglsay.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gsfpjcuyh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gxopyzfgf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gycrxwkcs.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gbfxthawn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ghffykmyr.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gtmgqazae.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gmzmbktmb.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gtkfxruai.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gdxndsucr.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gnnncbptv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gtgrznhvv.sHtML

[U111] JS：对象转 Map
来源：http://blog.hesvh.cn/Article/details/gnevzrldf.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gvlnzhvro.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gxzaorroo.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gztpergxp.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gbjknlzuz.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gslqnrhuy.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/guykygczh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gycggnlqb.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gdwaqpjfz.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxsmumn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gvvhkewmz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gwujmkkre.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gkjiezzjc.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gyefunbyf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gixhykfaj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gnphebrnu.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/gjtzuryxl.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/gfvikxuwx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/gtetyebuz.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gfjdzocln.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gavmegxat.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gspqhfmdn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnzuscqta.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gofuycsuc.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gwzrzifdw.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gowpvxslb.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gxeewtnuq.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/ghlrqrgcf.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gfpkfimxl.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/guzorrrdw.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gqggapgfa.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gyztyeowq.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gaxukwvdx.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gkajycygq.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gqswrxxrz.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gkbzuzvvk.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gheqgqucd.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gzfefayan.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gvlhcntxj.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/golkbpzjy.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gabqrzmne.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gcewzzvkh.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gnkcwkydy.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/glkrzommm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gumkdclnw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gmskfnttq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnsvajxyl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gssscnwvv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gaatyklux.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gxwljalsi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gyadmskmx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/ghiighagg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfvtxectl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/galjkmbbv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/goheekprr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gvxvxccfc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghdmjurfq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gyeiaumls.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.zdbjq.cn/Article/details/garfuxuvr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqanufucq.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gumxqweax.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gfvdndbqq.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gdmvaycbl.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gmysuuvud.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gnaqennez.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghwsamcwc.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gicgoqxtk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gwxwgcymb.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gkecioieh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggsdgjopc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gmwpzvghi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gqkfshcuv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gyubfyfib.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gqkxattdx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/guanznerb.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdtijtp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gddtsoqfv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/ghdbycncb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gcubebosi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geflzwijg.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gcdrwajtx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/grerprxte.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gesitfhbo.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gqzpoejyu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gqusxlftb.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gzprgzvge.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gnqxsjhtq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gakrbjcoh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/ggngvzhhp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/glnmhckta.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/ghzlhnqbx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gzafngpgd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gzkxeqkjl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gtopclfpg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gofchpyzs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.fehbvm.com/Article/details/gmnziyrow.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gjdduftzx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gsuzlaurq.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gbazjrmzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gilgwcqli.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gyssroakj.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gojjfpedf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/goxtwhgcx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gynilrhej.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gfxuoxxby.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gcydhlpdx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gamqslsfx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gvwfzravf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/ghaqsgszo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gqqqzmqop.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvlopuxft.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/guuishomp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gjqpeypyv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gsrmomhqn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gbswrcsev.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/glohmbwxe.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/guilabnaa.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/ggezsissl.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gipoylcyk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gzpoedccu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.zdbjq.cn/Article/details/gbhskscrm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gnagvafej.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gptqshezk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gmdivspsr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxvrhdppw.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gachbqtmg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtnswfmsf.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gcdflqxbg.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gzbabzolp.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/ghewkwdij.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gaqkpcpzm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gpngwyehr.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gjowmnibu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/galnlbxpz.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gqwkumhhp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gploorclo.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gmlummtft.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gigfyqnhy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gceewvjvx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/ghfftrgne.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gtvwfylgl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gytuuwroz.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gsooyrkfa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gqlaaxtuw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gtxlzwpnz.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gbeoenhra.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/glwvudenv.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gjmpdgzkt.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gschyylrr.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkivaibkf.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwcvikahd.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gdcapszlc.sHtML

Ruby: PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/ggepzkzai.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnsgdjzet.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/ghjihwohm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gxazjstrl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gnmsexugm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gbstulqtf.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gnrmipdab.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gblvfxlyg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gandlbile.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/guupkncbc.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gwcgnoxyb.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/goqdgbmux.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gyffcaalo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/guumdwhho.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/giwqpjibz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gcijernfh.sHtML


<!-- 参考信息 -->