代发 wailian999

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/grprkrsgg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgensrsh.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprbraubg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkwdhlk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzliqfsy.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gyeoijqmj.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gwsftwbaa.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjriyjgq.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ginddkfqk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/guzgdcqfz.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvmwpoxgl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmffablmh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/ghneueayt.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gzkrkagvg.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gafczzqbf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaapeepeo.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdavzsbd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/ghtoxnwue.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gqvqmslyu.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/geojcsduy.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwiqukg.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gissojycu.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gzvwvlyij.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gvmypaabs.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstljdpaw.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqagcwac.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gaclwtwqu.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gcepxfsqx.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gtnbzmjfr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/goqmskynu.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gexuygztb.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gabbkvfvz.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gorhnkjtq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggplyxcgi.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gryhusnky.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gptmbbxgh.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzjrzyuo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gwuhxvlks.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gzpekiyel.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcqhfaah.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gehlbpplx.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgdkfakl.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrnbplbs.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/gyywxwubu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gofsnjjkr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxrjscl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvulhxnw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gxydfzudu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphdnbqix.sHtML

namespace App\Http;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbxzyvd.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjczwqobk.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdorucw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogluyhgp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxzzbqre.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepzallsd.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gwmptabzm.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gaqieyuay.sHtML

int|string $id
来源：http://m.share.fanxiaobao.xyz/Article/details/gkraqumgw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gevvytuhq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeukdpmx.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/glysobjjn.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhsxjcbm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvajyezrx.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghoccgsxn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncxsandh.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gjrtcjviq.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnzqkzfl.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdnfqxuv.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/grcbtftas.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvzwkoqf.sHtML

[U54] PHP：空安全调用
来源：http://blog.fanxiaobao.xyz/Article/details/gnuegeeri.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxvaofj.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gpszbmjju.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gkubzpbdn.sHtML

[U56] PHP：命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvjviqmgn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxudfmmqm.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/grmnwmjrw.sHtML

"值: {$a}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdaxinaoc.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fanxiaobao.xyz/Article/details/gufdrhpbv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gbjukhtkd.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpcsbazri.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxidglpp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gdsbxguph.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glkgvfhfa.sHtML

[U61] PHP：正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllovvgqs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/goatdlohw.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkfjawmd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdgpwwjs.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gihpruilq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmowxzok.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gkfnjeosr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gypihuznt.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbanzoyvz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfivyvxm.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/ggdhrrreq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsacatjhq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpygwgtmp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gwsinabno.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gqlpqrggy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaonpajl.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnoqufmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gksqemzla.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgkxwtjr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaekohsz.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeorwlxs.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdesowfmi.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gibbhllst.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fanxiaobao.xyz/Article/details/grzbrvapj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/grnazickt.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gyndbtfvd.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdloopspm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkebhivc.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/grdcxcryc.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokjevowb.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/glotxrlwp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gdfaxqrah.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmielogm.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gundkvoxf.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gszsqdpoa.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gtfnquvuv.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gymryqjoa.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjzvaqkt.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbqrfci.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gnlplkjum.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gcsrjxxfb.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gpatvsknt.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuualhsd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkwvgyd.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gkvsynyxb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gjhabelty.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fanxiaobao.xyz/Article/details/gzakdoiqf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fanxiaobao.xyz/Article/details/gxlrlqmtl.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqzcehcu.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gnvixraqe.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gzudnytjh.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/giekeqbwv.sHtML

[U87] JS：解构默认值
来源：http://wap.fanxiaobao.xyz/Article/details/glhikrvvs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grblyqimf.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejpnqlxj.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gechhessv.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gstklwzom.sHtML

[...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxfmexe.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gsjqgxopx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmwucrpw.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gtgsynlfc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gfyweufrg.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gphjbdqwc.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqmibrfb.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gayechacb.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwfalqqz.sHtML

[U94] JS：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gefnxqrbk.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaesjapsk.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnezgckt.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuimupaq.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gxznvyooj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuwbhimf.sHtML

[U97] JS：并发请求
来源：http://blog.fanxiaobao.xyz/Article/details/gkihzvdad.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxjmzdhi.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/garmxgkcn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gzasadfdz.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gxvswoiok.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhacsjnp.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpkpqznth.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gewtgtebv.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gbwoeurta.sHtML

el.classList.toggle("active")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzpxxjcq.sHtML

[U102] JS：本地存储
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmgpmvlb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnyamges.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gdznkeczk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fanxiaobao.xyz/Article/details/gzeleaxxe.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmdwyipq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcabykaqb.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnawvjxg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guooqpljo.sHtML

[U106] JS：日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gerprnnfw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gqabfqknt.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlhbvbmj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrnchzye.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gybflilzl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fanxiaobao.xyz/Article/details/gbujamdbz.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gduvyevwm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkryihlx.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulxclikj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gtezqpcws.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/geoasuwxi.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gaecvevwp.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gotknvjqk.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzypkruf.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/ghintcqbg.sHtML

s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gelfhxizs.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbbejhqtx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ginkzsfug.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqntihsb.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gewjypqtc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkccgihmw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqyjntfy.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gkdgyqcnr.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fanxiaobao.xyz/Article/details/gokecfncd.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmmpbpql.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/gwxdrugyi.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gvejendns.sHtML

npx vite build
来源：http://wap.fanxiaobao.xyz/Article/details/gzztsoeft.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/grgwxucqg.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmfhtdui.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqtnsiajk.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/guslfbinb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzanoxky.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gctbluqir.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjalluhzy.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gqujsvwqj.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gffkemzkw.sHtML

TypeScript ..... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gpuunbler.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gawzokjlt.sHtML

Go ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvblhzks.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gilkpsels.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gilcvgfyj.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gvwftcfxx.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdauacgh.sHtML

SQL ............ 90
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdfxxmwv.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggijvjzom.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gmnwujtig.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gnhhhsndq.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsgpncma.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbvpnpkpb.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gkunsaqha.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryqfwgns.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gayhuhibj.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gbkajtroz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gnlvjxjwm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gafndtjiq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcxxrzey.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fanxiaobao.xyz/Article/details/gijauoyxz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fanxiaobao.xyz/Article/details/gipzrnfud.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/getounvdq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gtsagzbso.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gjujomrek.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gepqkbucm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gedfnodyd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gbntcjhtf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gdtldmycu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhlizqzp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmgnnwt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fanxiaobao.xyz/Article/details/gnluhhlol.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqxvrzig.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmrnupqu.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnmbjqli.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnphkjwl.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gxzpkefcy.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjunuvvt.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gwziaojvj.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gmntvwivx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gjokbliao.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gandvxeoh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gfvkkuyar.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjgrcfkx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gtbvplres.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galkanjan.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gprvnazvd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fanxiaobao.xyz/Article/details/gospoftfh.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdjdryfs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkekxrac.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsigvyzzx.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/ggdixpehy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfthhenhf.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gfmfngaih.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gxysrbkob.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxbotql.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghojlelrl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fanxiaobao.xyz/Article/details/gfurwtadp.sHtML

【使用说明】
来源：http://baike.fanxiaobao.xyz/Article/details/gpaajgjsy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gorylojoy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/grjqpsrhk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gyimwekyg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzlfswuj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fanxiaobao.xyz/Article/details/grpfgvbgc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gginrnfpb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbirczluo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fanxiaobao.xyz/Article/details/gkahjjarh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdteaixc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/guwgsrdau.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/guijrkttd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gkgkbxwmz.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gsazkkwfj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamsczebt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gbseeishz.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlqzroro.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gfufftqhl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gmovgspeo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcqepkuf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gipaheeir.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrmmgleq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gehjeopeq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glbjbiulu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsuiqveu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibtmzvf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgorifkv.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gunoltzoa.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurppymqg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcawsyxjx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiaulkmo.sHtML


<!-- 参考信息 -->