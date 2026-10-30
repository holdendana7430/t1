代发 wailian999

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gxepljtmf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gduuvjqxb.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gfllzmlea.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gzxspdcbu.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/guaelltvr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gbkqquuxk.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gduiqhbgz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gdmrqmmtn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/grbshzwxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gdniepkef.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gnnnvbljs.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/geiplymek.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gxsrjbbfm.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/geoxyscxf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gghvaiuxx.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gdpzbksuy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gcijdbxon.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gdeuyptrg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/ggpcbkuvc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/giutpgakl.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/glgpbasjp.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gqfmeiasn.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gmsjkwywl.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gepajroxd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gcwatdmlr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grupiausq.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gffifocku.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gwuojtcgo.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gjziwnrxy.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/glalshogw.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gwcxnhuxr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/gevemujbg.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gaykuaqom.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gceoehxgp.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/groetaxez.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gvnosgbrt.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/githpvtji.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gzfzszftc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/graeknkdb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/grdfpngiy.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fehbvm.com/Article/details/gndsevmef.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gvfuhhowi.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gldpqzquy.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/getbiudgb.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/gjbefacez.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gmyqioysy.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gdonptblo.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gvahnujoc.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gizospcgy.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gomsfnctv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/ghnzzrmse.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gzamfhsry.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gvghqnufa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/glsaojplr.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/glyjczwsw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gyedskhtk.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gmsldryhq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gbdedioxa.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gzafwdyme.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gpontkikf.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/goeedghjn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/glfreoffp.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gkzyyxlos.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gqzjucudu.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/goefrmqlt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfblscwpl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gqkrdjzfx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/glwnexwdr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ghnnaeetm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gkjpkkwtq.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gvtfwakdz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gayimjrgd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/giyuwotqq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gcmhirbmp.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gjesdgkoa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/guirgjdky.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/growuviji.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/guilsnjyv.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/grlhnoggb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gtkhdfwro.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/ggqmahkhh.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gsbgxzfic.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/ghdqgxqql.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/geecdqfsw.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gwyfniacp.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gluqxvivu.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/ggqmuocsx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gmbitwsqv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gtfvcgfda.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gmhvxamhv.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gyhfovqqp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gtrinslhe.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gtyevllbg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/ghnhqjfyy.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gsqxerbth.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/grmqtfhiu.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/gbstwqxqj.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gsqcnjkse.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gtonnvazr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gwkgqytbv.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/giljfhsps.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/ggqdhadps.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.hesvh.cn/Article/details/gdhriazmu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gqztrctub.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/guzwwwgio.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gjrjjgsqg.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gmervhvej.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gbakvzaeb.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/ggmsekcfg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gcponsbqs.sHtML

[U88] JS：对象展开合并
来源：http://baike.hesvh.cn/Article/details/gkxoyzteb.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gxxpdnzlg.sHtML

[U89] JS：数组去重
来源：http://wap.fehbvm.com/Article/details/gfrrkgmbo.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gdvflunmv.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gajwddxtj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/guzrjoimz.sHtML

[U91] JS：对象键值遍历
来源：http://blog.zdbjq.cn/Article/details/gfcqanjcw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fehbvm.com/Article/details/gwtusbbda.sHtML

[U92] JS：深拷贝
来源：http://baike.zdbjq.cn/Article/details/gwmigvngx.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvrkavlkc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvczrvhdj.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/giksyubub.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gmyfzptvz.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gccktglut.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/ghlkfrtho.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gjsidotsg.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/ganankucl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gstsyrbhc.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gaxxmqaqx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/grngirdop.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gxinyfpkx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gjmfbsnjr.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gczpncsuq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/ggsbmumuf.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/glnybzxkm.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/grbqjeoxb.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gwbnnaknu.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gdfpmskfj.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gzxzcbqov.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gzzznqybx.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gbprlukni.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/ghduxcnrf.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gdlucwaup.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gbftkeadq.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gundglxdq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gipijqchk.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gytlnaxvy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gbgmhjpjd.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gtgmjycpa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gelyatcbv.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gyqvjujht.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gfxjkltmr.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gutpvxoxw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/ghutzildq.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/grzryxaeq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gywrcsplx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/goiuvvihk.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gwvphaxpw.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gmafwkkng.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gtfwgltht.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gpfrkafkt.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gaehtaeiz.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gujpayfwd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/ghlklbdpt.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gybfhsfmu.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gamnoqtih.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gatvrthar.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gxttttwma.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gaterlbgr.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gnizwktgw.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gunyuvfeu.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gwifujznx.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gepxvptzu.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gwyvqtoym.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/ghlzwgirq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gifukylhh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gelcefcin.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/ghooqdsra.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjzyxbvkg.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gwyqunhij.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gyqxpodgq.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gwuhwwmuj.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gdtvghenm.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gblzefhjg.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/gzvnxboro.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gisywimav.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gucggroxo.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gwauzpkji.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/garqdccjq.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gqkxkkopy.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gmmaqrgkj.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gcnjgtlyt.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gtmmmdwfz.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gfssuvjre.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gbtuojtis.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/grbhszjww.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/guapbmqth.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gmtgsnpab.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/goicxksri.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gbagutcew.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/grukkuqgq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gffsfewum.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gascwceef.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gtxzlxjot.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gaqzakkrt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjdlsavwq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/grdugyjnf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gnnmasghx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqyzfgecu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gkdtytucm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gupwdfozi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gohgvkrez.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gcsizizun.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ghucvfdgu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/ghrgyuvnu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmqummuwk.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gppzdvrej.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gdeshfskc.sHtML

S C / C++ 专题                          60
来源：http://read.share.hesvh.cn/Article/details/gtregglyt.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gdhygttjs.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gqnquzdgw.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/goeubpapx.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gpcqjhaac.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gbgdsqwqq.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gztmpwncr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gdeoipjgo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gunxskalm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/ggumcqrfo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gxiydmgxb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/girqccheg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gizzdcdal.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gligqaiyr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gucknkljy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gcmtirbqn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gzawexvge.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkydnwgwp.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/grmvslqwf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/geeffjfmb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gwongcqmx.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gmryuynny.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gyjbaeihk.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/gkxfvrxyf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gxxfkdkvk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gmecngtsr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fehbvm.com/Article/details/gucgaszpw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gnfzocsex.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/greqaedfj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gcbybdprl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/glgkbipxy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/ghjmyucxq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/ghcehquaf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gmunbzzgd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gbrzhjhku.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gkdtsmyhn.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gorphdolh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gveuropso.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkmlkokxl.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gwuhdamrs.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqpfpfwes.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gqvfzpbvo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzsmfgbhi.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/grbewyvds.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gllxonumc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxyspepzj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gchnkjzkq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/ghwaamqtp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gdahslzok.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gnlhdcllq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gjqnadogb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gqlzifewq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/guxnjsmsy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdtpxsyiz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gfdffanza.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gquoebdoq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/givlnssac.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfbfdzeiz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gneawyzqb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gmofqyajy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gceuvspnu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gwirtffqq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbuziuqxx.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gefpqciqk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goednicpu.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gduvdthdl.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gdqfaakvs.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/gunirlfcy.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gfbdoiilb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/grefbyvgi.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/ghaqzrfee.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gdrhzkncq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gggqpzfkk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gpbwtajrk.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gahgdcqdj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/ghglfjlet.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gopsygknx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gigbilshj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gvwwjinpq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gajeydopm.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gzklmafaj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/ghaikxxpf.sHtML


<!-- 参考信息 -->