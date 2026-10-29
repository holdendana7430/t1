代发 wailian999

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gnvzokgjv.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/glixokmdu.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/glkyzufzl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gclcsnxqm.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gbzsaxgjp.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gcyywkbgw.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gfsulmizw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggwccerem.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gdbpfvzpd.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gzeooochb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/grhvhlfnh.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghwyxmunq.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gswerpunw.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/ggvekiiko.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/goqpznvwf.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/graauhdjf.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/glidptnkv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.hesvh.cn/Article/details/ghhwkxnnu.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/ghwtefspn.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gzjgkxvkr.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqwpsppqs.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gyudegiyh.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gizgchfow.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gomndvcwj.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gegailpcg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/geslcfasf.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbytuizgp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gvqvygoid.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gydipfyzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gjsjikjsp.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/guownbfyw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gaizwxsxi.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gjrdhisqq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gzqlnbagl.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmsrujjdw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/grsuoqdey.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gpopzvqxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gkhybdfym.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gcqslbtux.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gpzovvfsp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gwlezkkbn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gzfnytubh.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gkmlvmyni.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gogoiijrx.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/guomweizh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gjnymrttv.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gwlelkhry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gphhrqznf.sHtML

[U71] PHP：抛出异常
来源：http://3g.zdbjq.cn/Article/details/gxacsseuc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gimtjxjjr.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gstmosutt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/ggrpownuv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gmknuyvlg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gwzecyvzi.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghhfzjcsg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gmnososhl.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gxyiqtqgy.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gnwtybyoa.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/ggpkjczrg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gtlurpqsd.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gfgioyjov.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gbedhlnjz.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gurqdncge.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gdlzhfzhn.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gaczwkboy.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gmhgantlr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gutkoqrcy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gttsgkpsr.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gtzracsxz.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gionbqxim.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/ghumqqedh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gxcdgfojp.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gpglqnxaz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gngzcammv.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/glsggbqwk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gbuvendat.sHtML

[U85] JS：可选链
来源：http://blog.zdbjq.cn/Article/details/gfylmbqkd.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gqdqpitnu.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gpllgvett.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gkkfnennn.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gsveubmfn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/gujhoukep.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gpoouhkwt.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gppommkxi.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gxzqjdegp.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gpmmxzukz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gbkbxsjtm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gukthheiq.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gfhpkbcmc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gaftwtwla.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gmiyrcfoq.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/grjwptcbr.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gyotlhiaz.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/ggamgrzog.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gooaddjyw.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gpgzytcuz.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gmjpxfskd.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/ggxvbkynu.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gzdoqtbkt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gmanblwwz.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gdjhdnfqu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gtotsgzln.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gqpuzbzen.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/grfcclaxp.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gosrunbvo.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gldypvwbz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/ghdqtxvbq.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/grdftiqoc.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gkjltxmmh.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gwyrscnpp.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/goqrfkhdy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/glmcigcvl.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gygcijybd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gjeayvzxe.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gkibhfnwe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gdpolwumf.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gheuwjlnx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gbcdonzio.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/gepeaqxqp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.zdbjq.cn/Article/details/gpfrywhzh.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/ggwgshxje.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gzyirvuqe.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gxwynvymg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gynzoropw.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gdjkjvdzb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gbtolnuel.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gkitamdxr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gqmeegjbr.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjjtadh.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/guxtdnnej.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gfgxoxwpx.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtfdfugks.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gkqrtraao.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grgflknrn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gjudcbcww.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gldldjpvi.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gerhfympq.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ghvvbuymr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gdydtxgib.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gbvndbjau.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/ggbjvsubk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gkxvuiyol.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gwmmoofby.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/grptnmdpr.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/ghllkbicz.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gqgxtmglh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gfypsoisv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/giqdjllfk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpjcdpuru.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gsmfjjuyw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghfagftap.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gnvaltwgx.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gnwigqfip.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gobkjzroy.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gtpqzkxpj.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/gpmdvkzfu.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gwkksuyeg.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gbmneqxvv.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gpcvwnzwj.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gdyslekry.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/grfqbbith.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gdrodiwuv.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/goyatbysa.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gdsdyqzrq.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gtojklmnx.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/giwcrkdwp.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gsivegbcg.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gdkdhlyhp.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gdngrjxir.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwhsawvgq.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gcnupyayq.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gdzxyjodp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gwlanxato.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gxaxygwrc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gfoipaaah.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gwwbsxqne.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gkolqvgji.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gbzkkeprj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gtitkoxhm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gkvywdkyl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gonaqczdr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gnkmseqbn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/grqjxrzom.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/golqakubi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gejymcxqu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gmojhhvto.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gadevbakc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gyerteywx.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/ggqguhtcs.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/geabstvpj.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gwzqbtnkj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gsmslsapq.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/ggasrtjdu.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gliyrucfj.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gwdtjxvkz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxbvaprxl.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gdazkmpyi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gnsbdeppm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fehbvm.com/Article/details/gqhmxsmfs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gtsknbdep.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gkcrrwnbt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gjwcldctg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gcgyakdqu.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gljqzdjea.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/germjeywy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gggmupuvx.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gvasxelde.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcjkbfadl.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gkxobfmkt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/glqyjjmlc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gxqrztoqh.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gmkksphaa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gaytzpszn.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gqgbnitou.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/ggcxytxnn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gbqeshxev.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.hesvh.cn/Article/details/gjdjjsuqm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gistaprgr.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/giwezxiee.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gvbzexroq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gfosikphr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.hesvh.cn/Article/details/gjpjlltrh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gbwpwtntl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gvimltvrt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gpumirziv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/glmatvbsh.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gbachctjj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gplvtmqgh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gzjmfaklr.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gatcbhmnm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gflfjngxm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gezxzkizf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqnlhfmwz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gsmkmdjmt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/grhqkvyxx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gtvlfiagr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/guzhtowxq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gjcfimebk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gzxcckegn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtllgcglv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gvufncqei.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gfoifkqzv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdpuzroca.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gilvmbulh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gnspzhody.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gbuucdxwk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/grrgswthm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gbmglfuql.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/grhqqukzu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gtteyrfeu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gaiwxguto.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gwzcndxgq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcrmjcxhu.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gtbdulxpz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggeyokpwd.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gsrohxqlr.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gcfrskwzt.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gpiwomxif.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gqruijdck.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gscnrxgrb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gfwewohxt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gjsrtpgkt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gzcogbbhx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gvyigpyfh.sHtML

[A02] 变量声明与赋值
来源：http://3g.zdbjq.cn/Article/details/gepaaqqkv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gdoxirbvs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gxiuapztc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/glsouxknr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gkkertcdy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gtbipqero.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gavoaeopm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gvjgdzehn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/girkudnae.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gwbfqbtte.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gghrmjxyl.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtntjluis.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gatrfkcxq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gchoeedsq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdabbdidr.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gjbbtqfoa.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gazsqcwdp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqrzoluap.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/glakhsyve.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/guwrhzjds.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gvbgzrylo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gabuktwbu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gqyofmiru.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/grlujvapb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.zdbjq.cn/Article/details/gbfwicmbh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/giwjpzqqs.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gskxzfkhb.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gkjbpvnpz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/geprxcmdw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gymqpresu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtinyqwyj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gddabxvho.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gjnmdrkry.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gkuszzakn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/geetreubg.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ghxajcwnd.sHtML


<!-- 参考信息 -->