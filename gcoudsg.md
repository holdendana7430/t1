代发 wailian999

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gxejvprvi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeyfzhdl.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ghosvofwb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucensglj.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrvhjht.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/grdsfkflz.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/glxbcyibq.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvndbouzj.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggsogmrlj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/geuxcaizl.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/grijyiswi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrsszoum.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gvnvadakp.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gvayjptaf.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gdmdggpxa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfjusejb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqbzmloi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gycnimwrf.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfwgelro.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gixxydpiq.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gkthhzqhw.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwbetlgb.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggbaermhh.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhjnrubl.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gmxhmvnis.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gktxkyrut.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjnsdzoj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzfgkuz.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gpenhfnil.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gtubybaxy.sHtML

[U34] Py：判断编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggwxhrlx.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdspyvnl.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/gljgaxnna.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchmjznuk.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gemvqpnse.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gissbrnsp.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gclwfuvqa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gijhrsnrq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gmlmuudui.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/guzdapulp.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/gvkkbicva.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gizknfcvg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ggglxjfjl.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gidipqsfw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gwzrswpjn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdsmplfr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvbgpnig.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpkcutwo.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gspkutsfg.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gnknbwxuz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gmxchhmnv.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gluxrquzr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpekecivp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gespueujg.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbhdquzp.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gsqyfkilr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjxztdhq.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gghzwwllq.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geazdvhhp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeqqfgiz.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gdveorykr.sHtML

public readonly string $name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxycucyk.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvntjliq.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgovmlio.sHtML

[U51] PHP：数组解构
来源：http://wap.fanxiaobao.xyz/Article/details/gpjyjzvrr.sHtML

[$a, $b] = $arr;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqjvbkhx.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkctbqboc.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/guvxhitbu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gefaqapgz.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyonzijiq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwkzntab.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gweacnfsf.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/grbeqrnsr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gfjrlgsrk.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdhjmyks.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gntbtfkho.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfatdkeyd.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkktvnafw.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/glkstdvzt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gztuucldc.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/gkgqhdaub.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqapkdgy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gctcnxkpe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gfblnvusw.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/girlvgauq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdctdfms.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxegnqart.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqudsuotk.sHtML

[U63] PHP：文件读写
来源：http://blog.fanxiaobao.xyz/Article/details/gtvqtiepy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohacyzjb.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbsyddfb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/genqgogkc.sHtML

[U65] PHP：会话
来源：http://mobile.fanxiaobao.xyz/Article/details/gzixuxcvy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbjtmnwk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabbzqjwd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fanxiaobao.xyz/Article/details/geleuaylv.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gqrvdtivo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fanxiaobao.xyz/Article/details/gkwraqwel.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwlylodwa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkuvgplo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gowglyjtf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwahawkyy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxtgdicah.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjqitymo.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gtbymjhsx.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gshoehbgs.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnuwzddz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmgwypv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteuaxbqy.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/ghgafevdx.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvciieldd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzryzukqo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkglmopt.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gcdirfvei.sHtML

[U76] PHP：简单路由
来源：http://3g.fanxiaobao.xyz/Article/details/gwhorhzuz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpvzgpln.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fanxiaobao.xyz/Article/details/gbddrpjgs.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhopeyyi.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdfberl.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkmwabja.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gjxgntdna.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/gefpjzpqt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gdxetsftx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrxjuhoy.sHtML

[U81] JS：初始化项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgznhqke.sHtML

npm init -y;  npm i express
来源：http://m.share.fanxiaobao.xyz/Article/details/gencngvtg.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlnlvfl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasiblnym.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/grujydgde.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpgdjozm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gwkhriilm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gfyiantzn.sHtML

[U85] JS：可选链
来源：http://mobile.fanxiaobao.xyz/Article/details/giskevftu.sHtML

a?.b?.c
来源：http://3g.fanxiaobao.xyz/Article/details/ghfqywiyf.sHtML

[U86] JS：空值合并
来源：http://blog.fanxiaobao.xyz/Article/details/gfkhdzyce.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzfxagfx.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaukwneds.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gymicmcgm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gxacjsibn.sHtML

{ ...a, ...b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gymffhify.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gomnwnrpl.sHtML

[...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gghpmkqnx.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/glrsibxpn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gczziwcjo.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzooyxyb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gprfrboae.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtsjrotyz.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gznvlkdew.sHtML

[U93] JS：模板字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gkjabufaw.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapoiyzjx.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqvedktmo.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsyzrsek.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fanxiaobao.xyz/Article/details/gxllbywqw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gemcvgbsh.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gzuhjdavi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guspdbvlm.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchzxwcqs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gzusrytsk.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpdlnpye.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gfoxlgwzr.sHtML

[U99] JS：事件监听
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmylsmz.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnwkeyp.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxgtyroc.sHtML

document.querySelector(".item")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgegsqvi.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/gcxvdkkou.sHtML

el.classList.toggle("active")
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbecqre.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpnohlxn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhjkief.sHtML

[U103] JS：定时器
来源：http://3g.fanxiaobao.xyz/Article/details/gwfcuwdkf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkptfbwj.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/glslrbqdk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvyhwhona.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwkcwgwd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gaohiayba.sHtML

[U106] JS：日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdbqrpogo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmiljavi.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gwakgnoty.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gisigtcpm.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpwryvlh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/golhenysh.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gioempqlf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gxyvxijlf.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gqgsdpurg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgxyeguk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjwuffor.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoqyuqsn.sHtML

[U112] JS：字符串补位
来源：http://wap.fanxiaobao.xyz/Article/details/gxewiebxa.sHtML

"7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gidmluwiw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gsezzgpbw.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoybhyor.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gwaizrvee.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgulrlib.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gcsfknddg.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlifgbdn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/guqiliwmo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gziitmcvi.sHtML

[U117] JS：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/gogdyzezs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsusssxd.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gdppmiaid.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/guwtehgeu.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/glryvkhih.sHtML

npx vite build
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwmvlkew.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbclusvqv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gufwhzaft.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtrwdnqh.sHtML

统计汇总
来源：http://read.share.fanxiaobao.xyz/Article/details/gurfmfmog.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfswztgq.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gjytmbbww.sHtML

Python ......... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/glnzhdwuu.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhormcaa.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gkesjkozg.sHtML

TypeScript ..... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuotnoau.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gotzinuzi.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gcparmbxb.sHtML

Ruby ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gsmmstwlq.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gfynzyodg.sHtML

C .............. 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gonpwcbar.sHtML

C++ ............ 30
来源：http://blog.fanxiaobao.xyz/Article/details/gvsxrybct.sHtML

SQL ............ 90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyatywvix.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gjrqlhtkk.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gbmakyjyo.sHtML

Swift .......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/gxjrzltaf.sHtML

Lua ............ 10
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfsayefa.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrwqcovj.sHtML

Scala .......... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaormhaps.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gvxffntef.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gcntgrmcl.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gkcgzqenl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmpiybc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfudmsgm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gctnuninf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gbngdeodr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fanxiaobao.xyz/Article/details/ginunuhcv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gcftaiejo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gojnwcbfb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpcgixf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/ggosdrjir.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gvybkdsvy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgsdfwcp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxhtidrs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/grgdwjhjk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbylants.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fanxiaobao.xyz/Article/details/gbgjsdalg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcdgjjfy.sHtML

Q SQL 专题                              90
来源：http://baike.fanxiaobao.xyz/Article/details/gghmmkcac.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gumfdzxsb.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/glmjjstmf.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gtfaztrxl.sHtML

U 高频实用片段                         120
来源：http://baike.fanxiaobao.xyz/Article/details/ghquhfocd.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gwittmvxh.sHtML

合计                                  2106 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvernmefv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gxzcpwapj.sHtML

使用提醒
来源：http://3g.fanxiaobao.xyz/Article/details/gfjlmorcq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gqihjykdd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gwlzcufku.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqvyrgcx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gagtkkmvs.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gfrkxzuer.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyibpmfgm.sHtML

—— 文件结束 ——
来源：http://3g.fanxiaobao.xyz/Article/details/gqdijqulr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfzluaftn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhsuskfc.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gueqttfdd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjkfydayk.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/guxhemupm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhybdcgy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgsymueo.sHtML

SQL · Bash · C · C++
来源：http://baike.fanxiaobao.xyz/Article/details/gjcvjpwiz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbkyuykh.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gjfxytwfq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzupifng.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fanxiaobao.xyz/Article/details/galohcvis.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/gtrqcyszq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuwrvsuu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiagrxvh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fanxiaobao.xyz/Article/details/gxuhvvskl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gozunikms.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwuheane.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpklsqnrj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gkgioqwyg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gumdgnpao.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqcbotjt.sHtML

【文件统计】
来源：http://baike.fanxiaobao.xyz/Article/details/gzduxovoz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/gocmxizuy.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gdkgdmwjx.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/gpbbdpaih.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycgjjhzr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhfxpqei.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtfldtcdl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwdxckcs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqddrcik.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhxqutpi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnahhify.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/ggpalndyi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gapnefbox.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvuewtpj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjoarat.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gnpozuqqd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gttkdbccx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkvcixsqm.sHtML


<!-- 参考信息 -->