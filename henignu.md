代发 wailian999

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gubpswbkk.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gneqtgvgc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/ghokrqbnu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtuizgeo.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/guetcyanb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gmhsxngco.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxqiidec.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggatwjliy.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gbaexdrae.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gywhbnfam.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqjunry.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gntiehzzx.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkubucro.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/greoxmgya.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/giupignay.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnslvvsio.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggazkehjc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjqvcmrq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewrqoyxl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzvgytcb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gzzkqgldf.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiizgtcj.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonmoidtl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoafoeyd.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrceaec.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gnzszjjiw.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gyupgijjx.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxcyfnpm.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/guzucpwry.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gpkuwctfp.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkalpavtq.sHtML

@dataclass(slots=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gnhicjaex.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtnmawyd.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gmfeiaezu.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzxqpdyp.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gazphsoct.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gaxafgtmu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gezqtkiop.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/grrsbepzq.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gphpcsuoo.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqvououc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbulrnypc.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfxftlxn.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giifnkhkc.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gwmselptw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gwbwqeusn.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbsddtya.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gqfusrsom.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gkksiipua.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunekpzim.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwapfig.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaupjbpy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gadvncwca.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzngptai.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/ghbzeaifp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gkbywvvom.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gsqoqccil.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwucncrwo.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyrqgdpen.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsduwigvv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/glpmzsqzf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdysehfjn.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/geqodjutt.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/glxezxvtx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqfouwon.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gicesaptv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gkrebcejr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fanxiaobao.xyz/Article/details/girqfoqtv.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gbdxifgfg.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhcdxuyc.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gbwjaamam.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvqfmbqwh.sHtML

[U51] PHP：数组解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gscqquleb.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmzjitp.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbabzguhw.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiltqyvd.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gplmgmwty.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fanxiaobao.xyz/Article/details/gdxhflpju.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gspxuzakj.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gizxbrebz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkwvsegz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gwtneatfv.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/grnmygufb.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/grjjqwhml.sHtML

[U57] PHP：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gnkcfgjnt.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzirypew.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxguajkz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamubcodc.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gzmlyitmy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/glaktvdvo.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gviwplqae.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhbowwqv.sHtML

[U61] PHP：正则
来源：http://3g.fanxiaobao.xyz/Article/details/gmelgqbgw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpmxirpd.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gwldymfws.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fanxiaobao.xyz/Article/details/gmksqirpd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhsgrfmn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbijubjr.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgfyraj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojdkifw.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gsxbuyblh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbyhbdcam.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqfbghqb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdrczds.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gboosdwpf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmegirwc.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gocoptqdf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwisxsso.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gastmpxer.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grxhpaayl.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gvnepfujq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkoymgtp.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyuymfwe.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaoebyqb.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmesotrs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhugqzqn.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsillylx.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/gdcbdkvbs.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvenqywcf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gytirzvpz.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gxuilgrgs.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnftvdfu.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrlczbpw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxukgwzdd.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gwmionrqc.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvcygknm.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gozftxuho.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fanxiaobao.xyz/Article/details/gllkrgkku.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfwgfwuk.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfitlcdz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsbdbixu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxzymdhg.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkfbqvag.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/gqslwcvsk.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/ggqvpnkyl.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhhitjlz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktbhnewn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoquhjat.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/ghmakgjhh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtntduoem.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqhqrywf.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnrlfrgj.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/grmwfunne.sHtML

a ?? b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwstwzce.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/grwrdsokd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fanxiaobao.xyz/Article/details/gipjpuekn.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsroeaipg.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwfqadmd.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gloxgsdom.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsegpku.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/geknphbgr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gqjhhgspg.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzawxcxf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fanxiaobao.xyz/Article/details/gugqegcly.sHtML

[U92] JS：深拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gwfuxrduf.sHtML

structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gyswndseu.sHtML

[U93] JS：模板字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkraksdvf.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gnjlybnpt.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghujjfwnn.sHtML

const double = x => x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdaurykt.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fanxiaobao.xyz/Article/details/goeaxixxl.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvvilvlb.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fanxiaobao.xyz/Article/details/gpvheoiuu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdonvmhqq.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gfdwryinq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/giinmuapy.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gdhojzxjr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gdcogioht.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gozjrsvoc.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fanxiaobao.xyz/Article/details/gkcuajyxk.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrrndfbz.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzwmlmxv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtjovyez.sHtML

el.classList.toggle("active")
来源：http://m.share.fanxiaobao.xyz/Article/details/gywzislmx.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvlqnxwd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgrfbblu.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixfvyarn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvxscluo.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqdmcrmp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gblllttgb.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/gjqnhmlmz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gjjkpptiu.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfsfvluj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gntnlwfug.sHtML

[U107] JS：数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gqoqdvoix.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuigfxfs.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/grmzlcezg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyajzvnxt.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gkhhyxirt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/geaupfnwl.sHtML

[U110] JS：数组分块
来源：http://m.share.fanxiaobao.xyz/Article/details/gewmztzon.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fanxiaobao.xyz/Article/details/gjoxofkhb.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gglnpvxsf.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkygorrpi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknxdpacs.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gcrqodehc.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfuaezti.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhtlxzev.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcmxbrkxa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gypuerdbt.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gewdlvium.sHtML

crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/gijntqfhe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/guslkymkk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgwutquo.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gcnhgyqsk.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/ghvlbfhlx.sHtML

[U118] JS：开发服务器
来源：http://m.share.fanxiaobao.xyz/Article/details/gujwllxyn.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/gbraluxdm.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gukiisxme.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gjitaqcxh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfsajqxq.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/gvkuuqrvz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlbmejdk.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcubzcqwn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grulctxro.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnpnufjk.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqqydiqz.sHtML

PHP ............ 252
来源：http://baike.fanxiaobao.xyz/Article/details/gbybkpmjh.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/guusqeqkk.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwihdhfa.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfycomjxw.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/glgseqzap.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvshsroxd.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykwuggbk.sHtML

C .............. 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gztxzooiw.sHtML

C++ ............ 30
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnvqxdoe.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gyakrksqx.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gicywxcqm.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/gggovjtzt.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/grmaigwvk.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuyomvpi.sHtML

Perl ........... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacrztfyt.sHtML

Scala .......... 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuvghwpm.sHtML

------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/glibgcykg.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtwaufep.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gnmhmzcof.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrkgycke.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/glerorqbr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkwiwcmz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllepmmlq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvpacrwb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gklpdcuqn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gxemcstht.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtgtqkc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoacrpcw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gwsbfsusq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwulimifh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gaywnuohg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gpyhiiemo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/ggobowsbn.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsazwaljt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/ghetmdeqq.sHtML

Q SQL 专题                              90
来源：http://wap.fanxiaobao.xyz/Article/details/gbnpospwb.sHtML

R Bash 专题                             80
来源：http://blog.fanxiaobao.xyz/Article/details/gofnpocmn.sHtML

S C / C++ 专题                          60
来源：http://blog.fanxiaobao.xyz/Article/details/gzamexouo.sHtML

T 其他语言补充                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxqsyrc.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gpegudyrr.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/geysdaxtw.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhxtbbrk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmnqgvk.sHtML

使用提醒
来源：http://baike.fanxiaobao.xyz/Article/details/gbxgoerbn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdknniqh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fanxiaobao.xyz/Article/details/gdhnlyhng.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzkzyaci.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fanxiaobao.xyz/Article/details/grrcecigj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbgmyhgy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gvzurpzai.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgdubtzd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guosptame.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfdaribh.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fanxiaobao.xyz/Article/details/gcapeivrx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghdbzqmwu.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gtddfleun.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqnyshya.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/gzenplmir.sHtML

SQL · Bash · C · C++
来源：http://www.share.fanxiaobao.xyz/Article/details/giwxgncdh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gheuyilzd.sHtML

【使用说明】
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfcyxsin.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gubodvmjx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvneawm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/gcefnwrvw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gfopmetul.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/ghjmwqkxt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/goqzothly.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfscyvq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gytldnylf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gxuviylul.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fanxiaobao.xyz/Article/details/gioxfisrf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbkchwel.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gknvmqfgm.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjsgtwr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fanxiaobao.xyz/Article/details/giwtppdgg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/guiumcqhl.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/gwdamwxhf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/ggpqqvcby.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/guivbfkcn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gabmrxktl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcxlhcen.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjyhwgwq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gczywvaip.sHtML


<!-- 参考信息 -->