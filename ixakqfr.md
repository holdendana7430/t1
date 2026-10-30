代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gawoyliso.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gyenhryoe.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhlcnlfx.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftaeppaf.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzqhqzpwt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gdjqvsodw.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqwmjphh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhicatye.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gryeshbpf.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyazpedx.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/glwnxqhhd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyhepfpn.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhocwyoa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuvblers.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyewojvg.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/giuklxsil.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gerbemjbs.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzldgjof.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/glnxzgzbp.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/govzgqqmn.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gmukjlnow.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/glryexssi.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddjktnlw.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpswftuh.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbvxzpa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gjszfyqzq.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gvtglxmbs.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcoapkex.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxyioprn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/giznwacbk.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/ggdkelosg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gxwwnrhfx.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gxkafcoie.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gdiqqwhzu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvkwkkcq.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gklfaonbh.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/ghckbgsrq.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxauqjr.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfbunkgt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsptrhwqh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gkainwasf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/glkzzkgfv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/glxcejpdl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyodlelwe.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ghqsdenno.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrehealq.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ghazakwgi.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjqvfac.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gldyvusvg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswqbniqn.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gaqhzqhqn.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gocaltckb.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtymxewdz.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/gsdqaslcv.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpvawegad.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grzzwbczt.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhianjud.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdqylntj.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhvpdfj.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbmjlzoa.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrnwnra.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/gtqoiuotb.sHtML

[U52] PHP：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsoctqmxg.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvvokhvk.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqbbshtz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftxunzb.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgorwqyt.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfowlpmgu.sHtML

[U55] PHP：match 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfxwbxvmj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlusbwtk.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gapxbmhrf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqtmroav.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/guxgrpvaa.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gehdcpqpb.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gebyntcpi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdvvtvgm.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gojcybghq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxesfnouf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchuzaodd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gquumnerq.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gftkmgvbr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmghvxhae.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuruduwx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/gvdlqlrvw.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfuxcyxm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gweahgcxt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfprgyqg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmqgsymh.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyniaxrs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggslrlqcm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gnlthfmxg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gtfuybxwy.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fanxiaobao.xyz/Article/details/geuhbaxfk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzauvrgx.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gbbavhfgq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gipocttcu.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrselwic.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnsvypzf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxafyubqh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fanxiaobao.xyz/Article/details/gijmkrgqp.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gangarxhv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/glpaionla.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gazhwzyzw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gjucdbnxa.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxbjflrt.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gjiiiuaki.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjepcyjoy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fanxiaobao.xyz/Article/details/grjtrbhdp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gefobdqdq.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gepywlgoc.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcpdxiot.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fanxiaobao.xyz/Article/details/gozzccayq.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhcdzsec.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gvboytkju.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuzjvlza.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gcugglbjr.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyhfwolu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicifsjfl.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgpamrdc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwgtbgz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giicihhoa.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gklnsqizf.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/glznqljns.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdqiwkhr.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/gfjlernlm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/grovaesas.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gioqbozzr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvsrkqs.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlvoxdl.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwcccjvu.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gkeywmvct.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gclgwacun.sHtML

[U87] JS：解构默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gecqxjmmd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkswmlm.sHtML

[U88] JS：对象展开合并
来源：http://blog.fanxiaobao.xyz/Article/details/gxoveuioe.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/glnchqaxz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goofdwosl.sHtML

[...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gmnqdmcll.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmnxwxcp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfbnlvit.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldpgmfjf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmopcyvm.sHtML

[U92] JS：深拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gweajjwav.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwojsjbhl.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbngprrsl.sHtML

`共 ${n} 条`
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzixkcs.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garbphgfo.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gluemsohq.sHtML

[U95] JS：Promise 包装
来源：http://blog.fanxiaobao.xyz/Article/details/glyctsoad.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gitysjxno.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gffbokqhj.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfpgkepl.sHtML

[U97] JS：并发请求
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjpfezvh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlotbrw.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gkufrvkgx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fanxiaobao.xyz/Article/details/gnjwztqmr.sHtML

[U99] JS：事件监听
来源：http://wap.fanxiaobao.xyz/Article/details/gznyahnez.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegiplmxt.sHtML

[U100] JS：DOM 查询
来源：http://baike.fanxiaobao.xyz/Article/details/glmwptvpa.sHtML

document.querySelector(".item")
来源：http://3g.fanxiaobao.xyz/Article/details/griatyvya.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdirlcqlg.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/gdegmstpe.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gunwupgrg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gaouyntmj.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxpvjfgx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtuqghri.sHtML

[U104] JS：防抖
来源：http://blog.fanxiaobao.xyz/Article/details/gbteqlovs.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmosoycpn.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtzcyxtb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzckrtzh.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gadnmhpyt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfbgpfmy.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjcfkdx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gldwnbijt.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gylyupart.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/grehwolhc.sHtML

[U109] JS：数组分组
来源：http://baike.fanxiaobao.xyz/Article/details/gowlagokl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/giearixxy.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gxzuwpcxl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzlwiifv.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknmomoxa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqpxaid.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/giszzxiwg.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gpberngzd.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gguzlqyrv.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gcqougcra.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupxpknvj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbdjjadf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzdgghnc.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gayszkgsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gjrbgxabp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiirmixl.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gykgluayi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/genluvztl.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlwjmmc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudsaytrd.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gkexgnees.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gjckjrvja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwetitzqx.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gavscacna.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginnyuyrf.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gztbccvck.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmepkhok.sHtML

按语言统计（条）：
来源：http://baike.fanxiaobao.xyz/Article/details/gciiyaygh.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/ggnshulpv.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gofrjwlem.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxtjjwvb.sHtML

TypeScript ..... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gktesklbs.sHtML

Java ........... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gupgvvgal.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfmdmbgi.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/govykgtri.sHtML

C# ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhvzmqrz.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gpbhfegov.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrljiijm.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gyczfbzhw.sHtML

Bash ........... 80
来源：http://blog.fanxiaobao.xyz/Article/details/gknlygmql.sHtML

Kotlin ......... 15
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpejlwwib.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gnilryuyd.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gzuqntuhh.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gamrfxpxf.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzregpil.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgqwkkbz.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/glsapzisz.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyixkcvg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gfnfmrptx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssxasalf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/ghmrlkfjw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gpviwxxdz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/gpkyiyuoq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gaihtoazu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gjgtjowgp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gqxfxeaqe.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gcupxgley.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmfaqkkr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gphjdpaow.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gyffulxyg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gabmtoopd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/goizpqaoo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/ghfomynmc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqyfgwdx.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gikkershw.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/guccdrhlw.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudhajll.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gmzjmijiw.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/goasucdqf.sHtML

------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gqqaanzqa.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrkkxwpn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfqkcslk.sHtML

使用提醒
来源：http://mobile.fanxiaobao.xyz/Article/details/gtidbwgqw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gphfeftvg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/ggxtbelij.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvjzdrq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpsclaks.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fanxiaobao.xyz/Article/details/gtbptbhhi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaipsfvi.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gjycuohgk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gldubhuvw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/giaoviute.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/ghczdtwxs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmuxatfhw.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gkxrlgtra.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamrjwybg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxnqnoh.sHtML

SQL · Bash · C · C++
来源：http://3g.fanxiaobao.xyz/Article/details/gmsccyzjz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqmnklpv.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgdxgtx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/giiabrzzk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/gdxmrtcro.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fanxiaobao.xyz/Article/details/gdhexdkhr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsyzmlfx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fanxiaobao.xyz/Article/details/gomgipvlm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gxskjdyzl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fanxiaobao.xyz/Article/details/gddqblzab.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfematlx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnpsantd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsmdvleg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/ghktqhqap.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gpetmdcla.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gaglsjqbk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gaeokgmon.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gagzdtthk.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gbxitfxnm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gvxlxzxfm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guurrixno.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkschkuqx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqtahuvdg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gknrphlkv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxcenfm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshcdleiu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmebnzrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisxifef.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gbhnkgtnc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqpqykapk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gtbogdfxk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbqybtf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnbohrdz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftnocdvh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgeowert.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwhmfzpx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpeyeiqd.sHtML


<!-- 参考信息 -->