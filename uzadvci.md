代发 wailian999

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gdqcvdhuz.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gzpqpnbme.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gxlydlbhc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gvoipspxq.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gxhnpmqrg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfdfvzv.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ggrdyjqbu.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/gvetldnnf.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gfmbdcdmg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gkvxjwwsr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/ggjbzlvcl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gdtfowagk.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gzrisdkcf.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gfjcvdxre.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gulcklgwk.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/ghvgliigo.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gxojzxssj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/ghkeocevb.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gklnxkomq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gmzlhrmuv.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gbvxslyyj.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gakxlylrz.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/ghazcdvun.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gajdgbdlu.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gjnimsped.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gwyctjvye.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gvuirllzi.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gysfrtpbx.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gfvchalke.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gimkrhavi.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gsnkgszmf.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/genudoxwb.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gqtnnmkqm.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gbnyblorj.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gybloirmd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gsnosqyxf.sHtML

[U33] Py：打包发布
来源：http://wap.hesvh.cn/Article/details/gmwjvgmac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gxlrimlxu.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gncbyibjp.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gjsgwyfqx.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gdzcivfol.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gzucafhpu.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gavntnkvk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gdkfcpbpr.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/grtpleluz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gyfwcxpiq.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gjhsvdeax.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gpbcbhlgc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gunjtuvvk.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gpxyxvouy.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/guzbmyply.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gdlwguncp.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gjyvwsmds.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gbeiswqop.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gmlvlplbi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gancroogb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gtqwhbzvv.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gflwpysgg.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/geywwrewd.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gpbboeeox.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gbiucijeq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtfustavt.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gnztrqecs.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gwoojqrou.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gvzekumco.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gfxgoqztg.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gmuhtqqpv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gsxtzobez.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gjpcwgbpa.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gvggzrzoa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.fehbvm.com/Article/details/gpbwjegdo.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvaqwlldi.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/guvqkzsdp.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gzotmlhmg.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwbtqkudi.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gioipdlwh.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxenwfd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gyzjtnwqt.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gznulrfjf.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gyfvrxkyu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gzyfssezq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gdmothdmz.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gbioiczaw.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gtesjzmma.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/guvvsfryw.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/glickytkv.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gidzbnerx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/ggzexvyzn.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gomebqiic.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gxbffbhhl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gwbnmrvxr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/guykywpem.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gzmtozluw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gwbnheopc.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gtvplnqtx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gtpdvzkjz.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/guccvvwfi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gqpljskhi.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gqqwldeuf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/gomdnemgw.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gnokxydcb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gnpjfwlio.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gidhrdatw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gepwadckh.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gmwayxnmc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/grbuvpcnu.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gtbbvkovx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gyaccfyyh.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gvlldrcyk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gnxiboldr.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/grazfeemy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gspanrzzl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/gjanxlieg.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/geamrijom.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gxkayasgs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gyocqjuam.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/guvvgvsst.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/giwppehbu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gvfelvujj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gjuufejks.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gcvipjrdu.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gqnjayfgu.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gitkkrsyn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/ggopiebga.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gxbrfstkz.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gkapfiysx.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gaxfkbubh.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gqyhyjoha.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gviybhafa.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gzdwrfacu.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gqtdmvcwv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gurmwhwqj.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gfqhjvryw.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gqvkcxmne.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/ggycodqde.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gkiojgwpz.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gynlzdqhl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gqiwsiwuy.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gaelynfii.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gmwcplzty.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gcqvcywej.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/grtcnjsqj.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gnjfxetss.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gdwbjkmos.sHtML

[U87] JS：解构默认值
来源：http://baike.zdbjq.cn/Article/details/gylpxnmgh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gidsjcsgu.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gskisrzph.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gpiqoafju.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gimalowew.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gvfwhgphd.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/ganscbxpi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/guuzysyiy.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gcsvwpguq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/geebixzgr.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gnseiezid.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gftdkckhe.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyvvptpwa.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gdxbqazis.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/grcztwxpb.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gzncdmeut.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gheugdykj.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gqhvukuzv.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gizjnfuwt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gukbpcrim.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/ggqbctdrx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/ggassowwb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gspeinyvg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/ggicxefcv.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gvpeebzqp.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gunejcioq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gjrxrjaxk.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/gcoatcnkp.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gzhxcpbfn.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdwpxlc.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gnpytbzge.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gzopnklnn.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gylkaasxr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gyykypwex.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gzdwgbhdy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gedzrwxcd.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gcwcdnujb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gqtdtcpvn.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gslfwjyuw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gpsrieogb.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gjkkjrdtw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gyjvbqepo.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gxgktaxsr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gfofavhay.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gsydghtxg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gacksoivq.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gnzpfkrqd.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gjvggngjj.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gvwrpmrzn.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gabrfnkmb.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gvmqifrja.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grsgpszxm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/ghbipazek.sHtML

s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gsloimyaj.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gubztxezm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gnskfozxr.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/golltovwl.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxyrohgko.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gzvenaawa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gpbnehqrm.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gvyrevnef.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gmbnvrwwd.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gqqvdkrtc.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gxypijnkl.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gfihiobqf.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gtahgmepu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gbzbdrjtb.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/ggwxkvzlr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnofjhynn.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/glpoofxfg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glsgvjthi.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/guoxmjamy.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gpjooppcq.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gxfxdpskk.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gttdifyqm.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gdzrrnloz.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gfxrbbfrg.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gpbgiewca.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/glxupdnau.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gshnivhde.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/giqrvvwst.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gqikqqqdr.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gqtcmkuca.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gcyiizedj.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gzbhcpxzu.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gasslvvzm.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gmbyejmyl.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gyrzghtcg.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gzeqkrmwl.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjkpdmzqp.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gnqvxhhar.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gboyvdtoo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gtwtcetqd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gjmculvcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gzkhlzudm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gnfjiqllw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gkfmpeuwc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gyhwhmsnk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gujcbrdvg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gtowjojqa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/grczunabd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gypzernhk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gflmzullr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gpudmxhgy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsmcjnuzl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/ghjrbmwvy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/grhkyyxgj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gkyjgzayr.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gtuwrtdyn.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/ghgzvsgoa.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gwamitctq.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gayuayjgl.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gcjttfctr.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gtgpihxuz.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gfjztyklg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gocylbecl.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gjxdwfxwz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gbvaqscwg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/glbldwyra.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gxdebmopw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gyinprcmb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gknvvsubk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gjaxtipdu.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gvgfgwnql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyownvrpx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gmogghgbr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gilwjifhj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqiifmqvg.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/ghlzctpln.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gtauytkye.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gwtduukrg.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gnmayplbk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gpfbzebbl.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gttnjgouk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gvcljpcwu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gcqecouhs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gdtwftyvg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gjmopwdhn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gqmtrdqhg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gsgelpmqo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gwxpdydtv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gnjiodzxp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gcdgwelcv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gdykdadpi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gogefytgy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/ggdousiss.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gbtacavhu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gybxfitbx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gubypozhc.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/geoymqlya.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gozgaozso.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsnegblmu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjxpvhf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gwdcoatbb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gxbhzjasp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gwlszdtsd.sHtML


<!-- 参考信息 -->