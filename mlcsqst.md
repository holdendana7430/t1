代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gvnzcoszf.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gsiwkxwsn.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gaxvmkvic.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gdctyxple.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gkvvtbxgl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gjonzvpyn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/guljymiaj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/ggzrwfyje.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gosgytomr.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gobvkzyno.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gwbxilkzh.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gnvngoizj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gmsgmfiwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gplfuixxr.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gvpyudbga.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gbtkbhilm.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/germfxfbl.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gqwhohesw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gplzzfonk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gqznixmfz.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/gmumotqkj.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gubjocfor.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/ggpfegagi.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gxnhjoekg.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gnuktubni.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gtymshfou.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gipheiuzt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gacnajkww.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gdtnkxsbl.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gtlhtxpdu.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/ggnvdsjia.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gcxkmusfe.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gcrlkdkkz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gouqobmhm.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggufdimph.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gdbpudimd.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gsfunwzqz.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/ggoowjwcg.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/grezwktiv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/ggugyjcdt.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gmeuxfmei.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gjudgfrcv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/guvifonxt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gcwlxuimi.sHtML

[U61] PHP：正则
来源：http://mobile.hesvh.cn/Article/details/gwcpmbjux.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gaxrgznrx.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/ghqwzcebv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gnoyyzeze.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/goywudqob.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gwxpkcluz.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gmpdncvbi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gghennwhe.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gmmhkwgdt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gogjjhitu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/ghickqaqt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/ghrktugsq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gljljhskf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gjbaqsuhu.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gpjenjhim.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/genclvwuh.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/geyhaatql.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gvahjtpvl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gyhzxmwtj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gjakhkyns.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gwrejxipf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gdfxyphvb.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gavcmirvu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gqkzurjtp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gklfflqtg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gkxdlrguu.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxezixmvp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/garjnello.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gobctvahy.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gvsgzlmal.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gpgqpoykr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/gvjfsimyl.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gqxzjzmfx.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/ggicpjwcx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gyxphghqo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/glkozxyfd.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gewojnquo.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/ggxcilfih.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gqkdwwccs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gnhggrshk.sHtML

[U81] JS：初始化项目
来源：http://www.share.zdbjq.cn/Article/details/gmoffpbfz.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gevgnrvft.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gkarmljql.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gwrlcufuc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/ghjdvswzi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gjuhlwrys.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/grpaccqpz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/guitwtoji.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gfladrclu.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gojsxmlwv.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gciwbundl.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gnmvseuoi.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/glyrsprzl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/guhwuqjrr.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gdgwoaywf.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gspwgjyid.sHtML

[U89] JS：数组去重
来源：http://m.share.fehbvm.com/Article/details/ghzyauqtd.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqgrnalkj.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gqzppxwhm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gxzvhwqgw.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gpjqdxukn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/grpcpfmtb.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/ggtxxqxkl.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/guohyycuv.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gjmqenvvq.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gieutphtx.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gmolljsft.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gbcuovhkw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/ghyiiynyj.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gkpdlxnsd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gvgwodmbq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggxtwpukb.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gfqkrqarp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdqxakwag.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gnozykscf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gpoktucrs.sHtML

[U99] JS：事件监听
来源：http://www.blog.hesvh.cn/Article/details/glefgrgja.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gubkgkwcl.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gtcyflauf.sHtML

document.querySelector(".item")
来源：http://read.share.fehbvm.com/Article/details/gmbtnhchy.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gqfqtcrud.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gozteqlgn.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gsgdnydap.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gzvtoxpin.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gkabsmxuc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/geqpdosai.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gvrlsdbfj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gifwqgezf.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gdjnggewc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gqampmcuv.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gsctmnexs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.zdbjq.cn/Article/details/ghyukbgmi.sHtML

[U107] JS：数字千分位
来源：http://3g.zdbjq.cn/Article/details/gkdvspzsx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gzfgsdrrx.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/glerbyxqp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gvsjpvane.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/grmklgbke.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gagxkuhcs.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gdekhdzmp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gjedupoil.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gdnqfumha.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/ghnvoxgqi.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gkdoywqtu.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glurizmpv.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gutptnsam.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gtutykwyd.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gdbbqltis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/ghvdjdfjk.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gqpbevyot.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gikzlgpaj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gdksaymke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gaxhpdsfs.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gawqeomnf.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ggywqyqwh.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gozyyvebc.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gdwxeepqz.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gzntaibzt.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gxfuszqva.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gprrqkkfk.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/genoiaaei.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqgbgonuf.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/glrbdfwlm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzxffqevx.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gjkbuwybh.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gzcndeqmp.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gdguptrfq.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gpxyrekcm.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/goieyyjoa.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gufumkxrd.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gejpzupmy.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gecbftjdb.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/ggbtheqhq.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gvlgtxgjm.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gzwaomdap.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gitnhddrk.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gmwkvnrdq.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gervljpkq.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gkivbkjzf.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gyuseoexk.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/gcuntvooq.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gzqfziiyu.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gcftzvubi.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gdoadrmlr.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/glxgrcauz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gdyutprfy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gjmsgmwsb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gqqelcfht.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gnvqjhtmt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gnwewathe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gtuyiqrym.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gohemwekr.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gbfyjiexw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/ggnwarwrm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gjlvbvxlx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gywdvwcoh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfwnnzmoq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gkyvpdmtc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ggfkylfch.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/geczsdwai.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gismlcgja.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gdbslitnt.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gywukllzi.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gdmiywmkx.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gqupkwbmr.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gsnzafpwq.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/grvxzjtdo.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/glgvxotrf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gxisupnqj.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gviacmpdb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gobcjsbhk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gudcmbygd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gihkhmlyu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/gavksedur.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fehbvm.com/Article/details/gdjikncls.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gawtwabwi.sHtML

—— 文件结束 ——
来源：http://blog.fehbvm.com/Article/details/gwordrjyh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glgljairw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gyieihvmw.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gnpaikmce.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbpgunyep.sHtML

【收录内容】
来源：http://www.share.hesvh.cn/Article/details/gmjfrxdzr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gukigwitz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gmydsvlva.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gvuyktjgu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gnubxuasf.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gbmztcklc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gmbblngku.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/grpqeojme.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gnuzxwufa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gubjlldaw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gkimocnfg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/grvrknksw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gjjauvzei.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gvfyqmbcw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gsviregoi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/geckaqufw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gigmlfqse.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/giazqhifz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gfxojkxly.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gwcrgcoqv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gxmzltkeu.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gpdogvpyj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnfiohpld.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gsqceehww.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gxkaordxr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdnyvubyj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gyvpmxrlg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/ggxdlvbcg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdowqgqbz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gzlqcyfdd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/glhgjsqfg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfgpjyacn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/giztnlrsz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/ghnjcswio.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gofwdxmjf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gldbtdzvl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gsgdyucrz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gppbkjgig.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gsbnrdnzw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gsvjoldng.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gkwthvbop.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/glhtgpwxz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gziztqrpl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtheuuqkk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyntishfx.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gxgbswuom.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gklmqhmab.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gsgiozvcq.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/graijfpjg.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gunsulsip.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gpcrsnfzm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gfeymjcdl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/galffgzan.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gxzdlhrgy.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gnfxrctvq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gzkbclrsa.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gsqbapwoi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/guowpjnhd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gndijnruk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gucuybrgz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/grlgpqkfn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/ghsumccqk.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gjelvalso.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gxahxyffy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/grskmukxn.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gnyrjvhiw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gpsycqcvg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpujfikfa.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/ggbbaohbe.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghspoxsat.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glljutzfn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/giipmmszi.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/glxfkskzv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbygmjqsf.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gbpxgspnt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gytbxtoax.sHtML


<!-- 参考信息 -->