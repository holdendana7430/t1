代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gdhmmqeyi.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gkrciiuif.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/grwbuzyss.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gacznihap.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gutxfyjaw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gqogwlbjd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gxemgybei.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gvfkvrdla.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gtdyfkdzs.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/grcpmmncm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gjfopkfzu.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gdylvcnug.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gzauepxda.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gybitirjo.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gqefignod.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/ghjntbgwh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gkurwprez.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/garwxhnod.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gwkfpyaqi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gzapshtuw.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/ghgfrfpnw.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/grdosvjzw.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gpxwxmpyf.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gihewseuc.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gtqjjrcou.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gwxhmmssl.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/glpqalvmh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gxtzjwgif.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gdhamajno.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gvemnwswi.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gqzshbgzt.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/ghdcwjkvi.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gnvqkxhlc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/ghhgbuood.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gktipxlux.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gytqyqwho.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gtrixdqgd.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/ggqijodwu.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gmmoaugnw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/giekrvvaq.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gdmbkhvie.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gdoglaxbd.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gorswaetk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gjcnlaiws.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gilymgxtn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gomrbkwvm.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gzkshgtsy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gzcyogije.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gymokigkr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gfkeiehmf.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gcxsxekhh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzjypdq.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gxsyqdcts.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gsbbtjzpm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/glqsesogo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gqekdmzyv.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gwrpmmpwn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/guagwdyju.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gzkyxflut.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gwttqltad.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gixpyzzck.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.hesvh.cn/Article/details/ghjlbrpaw.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gzoeqmugl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gajncfssj.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/genaaksyj.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gsbrbatyj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gnjuusfgr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gjmvzucil.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/grwindkze.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/gokcgyovu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gypevqsfl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gikgzosny.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/guxvjduyh.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gxhuacubg.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gykbubmkw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gkwrgmipl.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/gdcsxntug.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gksouftwc.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gogndtkgt.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/ghqobwibs.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gztgiuckq.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/grcjkhgew.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/greienxna.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/guyddyzma.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gxmuodhcv.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/glnzdctxb.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gxbilaucl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gloktkiqq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gdirnieyc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gxkeavhxs.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gxairwtxu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gktmeuvbb.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gtlszyqhp.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gijhkhylz.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gwgsqzqgp.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gzeyhnbgr.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gievowqjv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/gpylpjyit.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/grplqtycw.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gpppocckw.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/goyrafvqi.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gqatyomqm.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gkhicmqys.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gisgxmtgr.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gxarkfefb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gklhfrxzq.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gmzoqkcyy.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfrtmzfzg.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gfljmddcr.sHtML

`共 ${n} 条`
来源：http://baike.fehbvm.com/Article/details/gsakyutif.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gadomblyw.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gxglkuidg.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gwsjhathc.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gjqgzkrey.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/gutbpefkf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gmrosvdih.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gchvyavae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/ghsopmexa.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gadywpmwt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/glgqjtqay.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gpgfwoofv.sHtML

el.addEventListener("click", e => {})
来源：http://3g.zdbjq.cn/Article/details/gnhffyrep.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gvriksjer.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gjbrvlzjg.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/geiapsjhu.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gbkapoyqe.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gdrjkpgql.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/grsenvcok.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gqmiywbfq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gxymmomas.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/geetahpef.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gezqkkroe.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/glondqxzb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggdssyqna.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gfardalsc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/ghaqrntuh.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gtzuakdhf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gvtxcrpnx.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/goeokquxp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/guwhgjgsc.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gpqohiyhd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gpbtcmczj.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gpychdqbt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/ghzychgou.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/ghgyuilvi.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gccywlvme.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/guuzcyiwg.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjthtddeq.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/gwpmkecav.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/goserxrll.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gqhfrdgjo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gkiififqt.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gxcvtljyy.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gkfzchdbc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gyxiunuwl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gegcgzkih.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/ghmqjoshh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gaqdldibp.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gerjwqzlg.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gperrazta.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gpoehegqk.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gdzswubpj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gquclejje.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gflrfpojx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmsmoodcu.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gkzykjmcf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grboiogcx.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gawwbmrgr.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gerqzqayx.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/ggsauoopm.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gxcojdang.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gavtrelkl.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gofchcegr.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gkpgqfwid.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gpewncjie.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/ghlunbunb.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gmhyflhfc.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/gghwobpau.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gxzklmdcq.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gkcywbwfb.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gprlanino.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/goznutnbi.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/guhqjgsnh.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gfzchdggh.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/ghdwtjnxa.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnezvbfvu.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gfvddzilr.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gjbpaopng.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gxwzlfjjr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gacywryxn.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gpxwyinuh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gfeudgqxk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/gupivpvxu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gumywisvk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/ghiugbrjt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gzagyhgwb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjffdzypf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gemwgikpn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gjucdmtwt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gitwozwit.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gbivittub.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/giuaqlxyq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gozonbzpy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcurocvbh.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gjjcqnaee.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gyqwglgqi.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gsbqhotxy.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gmiisfimu.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gihkqgitz.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmaxtpuuj.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/giijbmeek.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqcmojigb.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/ghdtumqlu.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gbdhjgzot.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gmckewidk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gbpwjmjpz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gxwypness.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/gpfztsqyn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gxyqiytwb.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gikugijkw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvquehqrw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fehbvm.com/Article/details/gjopzsbme.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gqsoivhxq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ganxtngxr.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gkqffujqg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/grkdcyxwr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/goyacvhlr.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gbmsungmh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/giifpogpo.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/ggptsduje.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gvjjbekbr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gztpxntji.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gdpvgxifd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/geumcftin.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gfpnawagm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/geqrklnat.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gczhmaotp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gkllkkizz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gsflhzutm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gvornqqrv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gftxxugbn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gibugptdi.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/grbfxlciu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/ghlnmuzpz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gkuyvspnz.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gkmoinrii.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwbtekvlf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gmothavqo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/goivylafm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/ghgmzvfas.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gbxkdtfat.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfgfzovqr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gzbslyhks.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvyedhryu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gpjqyrejp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/grkrgipff.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gqscwihyu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ggzryfdpr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gsrxpljsq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gzgsdgtud.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gsnwgjdxk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gsmvzdwqx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gbpbcuaxp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gcrcomjwh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gjxulajyc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gzcnzjaps.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/ganlcjzdm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gklglypru.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbixoteql.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/grnqwpfii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gikkplkmw.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gstmmhaos.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gsztjwvsj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gdkjtgiqk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gwdapkawx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gcrlgnzxd.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gepnktxza.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gjwpymfcz.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gomisgovr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gtvcgdrbf.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gzdokkstd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gvujecbmg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gfucnikmg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gfovsmzqm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gvrdrvxzm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gkxtnrpol.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gzrgbitbt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gxraxhazr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gohynubnq.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/gduxuoqny.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gydddxicd.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gobuvapxo.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grfsphaop.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gzwaskxfk.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/giicsrufa.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gnymwuqph.sHtML

Ruby: PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/giobpllly.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfixjvgqz.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gcpdfropr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/grslqlgxo.sHtML


<!-- 参考信息 -->