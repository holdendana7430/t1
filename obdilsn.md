代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gqqslfyyp.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gdorzanso.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gqjmjtdgw.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gayjdcndg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gcjxqeufn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gaummcapk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/ggghylixd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gkoparxvu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gpybnyefi.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/ggvsxxhan.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gxytjaqqn.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gapzqapnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdaknuven.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gshxbsldx.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gsuqvseej.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gatigmcmi.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gxxtrzafu.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gfeopvqxv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gckvuiwlf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gxvrhness.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gmwglrfje.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gvfaishwa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gordkilwv.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/glzgrrfmt.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gfakubess.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gnnvppupn.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gxnxalfmg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gsvqiezbn.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gwjncelpr.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gaafmaspm.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/ghnquphen.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gvrmfgccy.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gmvqwenev.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/glhzutria.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/ghwgsllco.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gexhclmwc.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/grbofmnlr.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gwbcziczq.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gkijvhgbt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/glyldsscq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvrvhvy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/guzycklat.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gdtndgfjb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gljhnpmwp.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gvcafdqmx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gpahcrwdj.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gxjdvpivy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/grgxzicvs.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gehaqxvxh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gvssnapkq.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gooimmkji.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/goqblwhon.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gqpnprfih.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/ginkkvubw.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/ghlsasgca.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gsmlivwyp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gcpkscyqu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gukfiobaw.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/garoueqpe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gsjobcqxy.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gqeusbvxq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gcnbjjtqy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gtjdwuydg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gygzdkaan.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gaohliwxw.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/ghgvzapfe.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gwiyniroc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/goywxktzg.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gaeddkeun.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gfihbgfcn.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gfxilsejq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gfajermhx.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gfyjhjutx.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gfrqwqxja.sHtML

[U76] PHP：简单路由
来源：http://blog.fehbvm.com/Article/details/gnkylysix.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gkohonixw.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gavbwcrot.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gweokfzer.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gcuxqfmut.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gfbvhvcfj.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gsaizofoq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fehbvm.com/Article/details/gqxxkawlx.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/grisbycsq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gvpjibmmq.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gfcpsozdn.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gkzxadejz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gvvqryskz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/glscteofe.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/gohulsneq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gtykveayo.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gwopeitny.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gvjadpewa.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/grhwahjku.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gexjlsqgm.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gocugspsz.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gmfujhvgz.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/grpmytjgo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gyynvzsvo.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gtkgvlwlp.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gwozpwins.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/guqmqrmnn.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnpgoyifn.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gsjbqwycu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gprxwnbxw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gbottrsjn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gengkvtvb.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gqprtzbqb.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmuajemml.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gwlducznt.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/grkqjjikh.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gqmsdkndl.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gbpgmllba.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gsgorzjqn.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/giobdtxzo.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/grbnwcasb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gubmdavth.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gulsjmijr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gdfsvcnnz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/gtggdxzdl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gdqwjpcgq.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gmqcfjaqw.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gkbjwbhhc.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gwjkrekag.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gcswyjrlh.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/guxuojeul.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gjerdmcxr.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/grqhnpnxr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/glkbjajkr.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gquemkvvw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.zdbjq.cn/Article/details/gxyrzlccs.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/geunubodi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gfumixplz.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/ghwmvjlxb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gkvgjpffy.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/guyrssdoa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/goctvwqre.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gbtwajbav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gvlgonsxl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fehbvm.com/Article/details/ghksulgwt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gwlcriuzl.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjapkwcpx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gflyriyde.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gicdwanod.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fehbvm.com/Article/details/ggbkerimb.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gpjfspqlw.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gpetcthfp.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gevwrfzjg.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gpvwtigxs.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gioukttpj.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzajvwzns.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gqoegyhch.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gjwrvqvkg.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gspjjwkpx.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gegcfepkm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gdvomoias.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gsmdapmmy.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/grehydmvr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gmkzvwddp.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/guywniodz.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gntsiwuxb.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gwgpvwbqd.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gksiadlss.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gdpfixskr.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/gkhglipdk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqxtfznlc.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gpmzqocva.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guxkozrcm.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/goqvxwcur.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/gwkjsjiap.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/gpzxgidrj.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gdrrkfamv.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gzqmxlnnn.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gidotanlr.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gnbkyvugk.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gxlhfgefl.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gxfntikki.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gdnbkerjt.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/ggxtmmpob.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gvsxmmotp.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gidlvesce.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gjssyechh.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gvthdhgsk.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gjocrtczw.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gqwkmaxoo.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gncqgrruj.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghiizhzlo.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gdsrasvno.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/guhgdyyzi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gokgzbglk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gvqmvnpbq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gokuyarvi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gowoiokjx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/ghicqdryq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gtstymlqc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gvugbmsvn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gomkrzjmg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcssrrrwp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gfmozgtws.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmieevekz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/getklrmpm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/ggbrtmypg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gugziumap.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/grpdyrhpr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gmanriite.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/grssmnblf.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/galaehxfk.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gaqdhgzzz.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gpgvvusat.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/guokgvcne.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/guqdudwkg.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/goacmwwnq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gudaomywy.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/ghmbtomyz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grjmtdkix.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.fehbvm.com/Article/details/ghssnqjih.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/govbmgohf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/guhxnvsaj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gqiscsbqw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/grnyanesw.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gahmhloiq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsvmnmgaw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gtvvzsdtt.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/grzhzassi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gteuhkpzo.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gmcovahpf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gqyxwmrga.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/giitsiokf.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gltmihkgc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/ggtkzbnpn.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/gnfmfkhwe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gnsmmgvoj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gagbpgpht.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/gukoweaak.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gzujmbber.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gqzpddczi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gwzhvgupr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gjaszpqgr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.zdbjq.cn/Article/details/gjbjfrraz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gbaxmxibf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gtxhiuhds.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gykifzgwf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gwggvwold.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/glfsrgsdg.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gsmqesyyq.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvcotyxau.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gkmyyidqo.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkxygyhid.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gprshuyup.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/goqbsmagx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gumlnvwsz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gtyuynjcx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/ggrqkcazg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gcmczkagv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gdjlpdutb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gdejpbyrp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gttjdnzel.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gomwtepuz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gupzghgat.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghwgrdlrl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gxzylbohs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gmzgaaanv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gooubcnzi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gtgglgkwl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gyeishqwg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gccxricqq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gkqpbifqb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/geokjpoel.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/grsgpuwcv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsxxmkwev.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gcxlxbowc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grwvassbr.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gqjekbhui.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gpumiekds.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gxivoozsm.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/girhwckyf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gozfxyxxn.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/ghmtsrfcb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gweqrzjdu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/ggoburypt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gikvhgdjs.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/gldluzvwq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gqfeexyli.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/goxthvnoz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gthsqpjrh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/grdrqlvzv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gkcnnugbz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gtsvmausj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/ggpldmwls.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gczyehxov.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gsitdhvzv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gjjkdpxvf.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gmbestuqw.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gspfnpkxn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gpesnnznz.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/guhsnijkp.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gmooyljnv.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gterdinvt.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gepnjwecf.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gtlwcixvy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gtldclimy.sHtML


<!-- 参考信息 -->