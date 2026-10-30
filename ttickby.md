代发 wailian999

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/grhqxyrmq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/grwxvaywn.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxxoadbi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/ghaymrtxj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbazmkike.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/goggghkxq.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gruhdwpnt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/grjoperoe.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxtqvxhd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipeixmty.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gljzpesxn.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/ganzpomlv.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gyipstgza.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggesjeypz.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gnjzqldsx.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gezvhkxci.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcobhsrnf.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdqrtzg.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggobpiyy.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/glovgdvke.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvlgenfj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxraetmmd.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gaawqiikv.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gujackjaq.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gjrvsnypd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gyugevzqw.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gyosjscte.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugcdejx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gdytdrkya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkkezgax.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjzrcubv.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwmrxrry.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmncbvuj.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gtrayitrf.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkhqzazp.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxrojtlb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gpnijazpm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gvixuxjjb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfmniuap.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gteabjjxr.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjsmyuin.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/gepdueqjy.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/ggcgnvxbc.sHtML

declare(strict_types=1);
来源：http://blog.fanxiaobao.xyz/Article/details/gxphuppkd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxscmslq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gynuautas.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/gdpbezfdy.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/giiktelhw.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gttwbdjsb.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacpjpzrv.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyijjnlv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmibiicpf.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqwfcrvw.sHtML

public readonly string $name
来源：http://wap.fanxiaobao.xyz/Article/details/ghsigtwjv.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gnskjznim.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmdtxgt.sHtML

[U51] PHP：数组解构
来源：http://baike.fanxiaobao.xyz/Article/details/gquyletiy.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gbthetzmv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbcyesh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtarwdgfr.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigjqzitb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfehoxyb.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlspkout.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/giodyadda.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmkzwozv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/grdmqjvin.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzareupd.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glahjohhs.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gtkttxdmt.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqqhlbrpc.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gxqztkclt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvnpnlne.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gttngzgvz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjrmvxer.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gjdbijzzy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnzxrxx.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gpwnepmjd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/geyplknfi.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzfuplav.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fanxiaobao.xyz/Article/details/gtjqcxvzt.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzqxlkab.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggizntkru.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmlvjzyx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlmiwyjp.sHtML

[U65] PHP：会话
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqmsnblv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfguizdbw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfesxprl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gouiusyfv.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gapxlpzgt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrjeduot.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/goqwyeckj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gindxqedh.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsjsggwt.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/greldxbfl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhpnfpu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gosfsdhgk.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrnyuwky.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guspehngb.sHtML

[U72] PHP：写错误日志
来源：http://3g.fanxiaobao.xyz/Article/details/ghmxjdqrq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/guszgxmjy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhfyyiia.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltxuhrcv.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grnfzhcao.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/grwzzvdgg.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gollefjla.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzxjybgd.sHtML

[U76] PHP：简单路由
来源：http://wap.fanxiaobao.xyz/Article/details/gcjsivmjy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gdtelbiib.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpzcclt.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/glnvdsxay.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwkqjfm.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gzvsnnmhw.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/guglbmatr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gedbjvtpo.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/gjpqqvpgy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fanxiaobao.xyz/Article/details/gkfelozwo.sHtML

[U81] JS：初始化项目
来源：http://wap.fanxiaobao.xyz/Article/details/grvbexpqu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkkgwzyq.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaepnhyq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszflfzc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziqzujkx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gikpluict.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkydbwhg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwyldpk.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvvewjuc.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsuyzwow.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gjvifqzve.sHtML

a ?? b
来源：http://wap.fanxiaobao.xyz/Article/details/gscepcglz.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhdubbc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fanxiaobao.xyz/Article/details/gsqhcwfkl.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/giwrsxcni.sHtML

{ ...a, ...b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gujmzsupd.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeckmyli.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givobrdfo.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fanxiaobao.xyz/Article/details/glqlrjleq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwigwnss.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcwpdbumu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gylprfxay.sHtML

[U92] JS：深拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeeksscr.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueudexyj.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/guyqlhhiv.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gsibrvege.sHtML

[U94] JS：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gywxqnrul.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaihbazgo.sHtML

[U95] JS：Promise 包装
来源：http://baike.fanxiaobao.xyz/Article/details/gcjikwqrz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fanxiaobao.xyz/Article/details/gpkaepwlo.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzmnuuqq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawtfuhrg.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwqkxjxl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxkugaf.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvceugwv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fanxiaobao.xyz/Article/details/grprizunk.sHtML

[U99] JS：事件监听
来源：http://www.share.fanxiaobao.xyz/Article/details/gblzjdebf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gutnuapss.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlfgnlbx.sHtML

document.querySelector(".item")
来源：http://blog.fanxiaobao.xyz/Article/details/gqqiwkucq.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gtztonmmk.sHtML

el.classList.toggle("active")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfhxyhoz.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugyljvoc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gdxuxhelo.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgnjvopo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnefokfwk.sHtML

[U104] JS：防抖
来源：http://wap.fanxiaobao.xyz/Article/details/glctssuec.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/ghuftsbks.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvlchzta.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkntaacoe.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gqqouhgup.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gizsjvyfm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghusewijm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdffrkhkv.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbzpzrs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gmckarqdf.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gozqqrrds.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykadapjj.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gfuibxdxm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwczwawe.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/ggfpykobq.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmexhibz.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/ghgwmrivx.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/grtcmbhwn.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gigeezuyi.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gvlovwtko.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fanxiaobao.xyz/Article/details/gfyinlvgq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gitlbvjhm.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqbrfzpu.sHtML

crypto.randomUUID()
来源：http://www.share.fanxiaobao.xyz/Article/details/gglouooyp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpcewhkl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqdkalzw.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gdykurlop.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gcukyqpfd.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gdlgosbxh.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/ggrmkbtae.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/glxvuwzzh.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gjzwhgeqs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fanxiaobao.xyz/Article/details/gepxnupiy.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdrlzgd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grsutvdbw.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gnxtspnjs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvogxwlki.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gzuypjytx.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwetmnfro.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrglocyb.sHtML

JavaScript ..... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gjusltntw.sHtML

TypeScript ..... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjffgzhuy.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gxxixsutn.sHtML

Go ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gazdfcvko.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrjrlnky.sHtML

C# ............. 212
来源：http://baike.fanxiaobao.xyz/Article/details/gmuyioqzc.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gjirppeio.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gihyqvbwn.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gipancxty.sHtML

Bash ........... 80
来源：http://wap.fanxiaobao.xyz/Article/details/gociypziy.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gmrgmaoej.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/goafahxvz.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjplrwdh.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/glxlpuhjr.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpkbxbl.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdxkcpfs.sHtML

合计 ........... 2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gslzyosiy.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlevydtk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/ghyxgpmpj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gcyhswypc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gozskqbly.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getjebelg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gqqngfrjs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbbdshxu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gxgdlautk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtoduhev.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/guqvlkowb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpctdqhzn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gijfloaph.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gmjfcpged.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/garjziqta.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gmbpkebsg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gbnzlzavp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gxodxmmfz.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggscnbzfk.sHtML

R Bash 专题                             80
来源：http://baike.fanxiaobao.xyz/Article/details/gtyuswrzw.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gnfsqwtsq.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gisgwydsk.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/gpcycpqlc.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gksglhakm.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/guheyqapw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnqdzgyn.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmlzzhfo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gkbkswoeu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwgjwcen.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gntowiick.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvflqjws.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/gfzfconry.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegbrjbvy.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/ghiygjxbw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdtmviys.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gmeokextb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhrnifyp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjmuijeg.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabllmjyy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/guvcckrxj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuhfxokk.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotmdjuxz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjanhddb.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gskhtrpoa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fanxiaobao.xyz/Article/details/gvzotlnnz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorjpjpie.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gnvaduywv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fanxiaobao.xyz/Article/details/geghdqscu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwulubea.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gwskbjpnz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhzrqzem.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzdyerzi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplltuisb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fanxiaobao.xyz/Article/details/gomlgkxhk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuhiejli.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghigeubly.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gythmlyir.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjakihj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/glvhjfkqp.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlpojupy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gezzsygla.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzonjgrsy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gdduhpqet.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gabfwbiap.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxavkxqas.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gmctxvstm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grzvwfevs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gczlwxlwv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/giaaixayq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjorqcbk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gueiimjbx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdootzoib.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gxmbwbcyv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkksnso.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glergadpc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbivkmah.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywakpxz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gaqfoklgm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ghfzjshho.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexhuyjon.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghetxgeyp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvqwgkfq.sHtML


<!-- 参考信息 -->