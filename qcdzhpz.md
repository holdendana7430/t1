代发 wailian999

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcjixrnbo.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwczkble.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gqaaurqoq.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglgmlhrn.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbpndbtl.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/guujseqgm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvojwmtwo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxdzsvbh.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gydcmidsn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakvuabgw.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/grnjhywfh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/glttpetpv.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gehydzdaf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gllfjbdeh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gpqutavsh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqgtbqkj.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejaghsb.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbttcvo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/ghywxazxt.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmirgyfhy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlnwtmjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gjqzqapgo.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslfidmkv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqzsblap.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gmqyasayj.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/ghabktqqt.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsrcwblm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gnuuxxaah.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gtzreqvai.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gkgoiselr.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gogqlcdvj.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpmxxjha.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocdahno.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gpwoxltef.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gfjprdqhd.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyucofsq.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/ginobdrcc.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/glzwflmpx.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfucolsn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gvgxqvfly.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzwhbkif.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxpwqbzg.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gjsexxnmd.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeqgncuu.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggptrovxe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gomkbrhjs.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gggnndbxi.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/grspcyhit.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gcqylrpxh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gildoarya.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gjtkdrzem.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gitnskfhz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/giwxhwasg.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/ghfqwsnon.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/garfcwmir.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnokdpye.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhaxqvbk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fanxiaobao.xyz/Article/details/gbtvxrgrt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/gtatwyqch.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/givvroyqy.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govpgyprt.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozvqiigp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvzyjzh.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmrkntzc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gegsktiuv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdscuiwsv.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gygzsklgi.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/gwlkxqrqg.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnantcmzh.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurlsutgd.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gtkibvwpp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdvrdxyh.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/grpgskpws.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gvmjtszrc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/goknxvvlr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeumhfyf.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykjngool.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpagzoiyw.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndxhmbbo.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/geshrxhel.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gdiirrmaa.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzfdaylp.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gwfwmrtjr.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gynaxppyo.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gspuztotw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fanxiaobao.xyz/Article/details/ghuajddwb.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnofdjqm.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkpkmecb.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gfycevffr.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gicgngeab.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkoiphoi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gipsjmuit.sHtML

[U59] PHP：自定义排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyvxgusze.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhkhrvap.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwossziu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijyxtpsz.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gxscoiept.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnwuhswl.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghpfmhd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyxluzjy.sHtML

[U63] PHP：文件读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gipfeqxhq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fanxiaobao.xyz/Article/details/gisobfndh.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoxopuzd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmmboubh.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/guhkufjwt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/getixomnh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtcxfhwf.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gladmnzab.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gubsqeyjd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkdyxlt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/givtlopia.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.fanxiaobao.xyz/Article/details/gcvauxymx.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gduwjmivq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgrnntvx.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gudskobol.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkokfjmvw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gdcevhxxi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gozwynlov.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gekgowrpc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gphzqsdds.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkxcuksq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhwdrwde.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzlzvbfl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gazzcebty.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupkimkcp.sHtML

composer require psr/container
来源：http://wap.fanxiaobao.xyz/Article/details/gxvbycasa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxjiudjf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fanxiaobao.xyz/Article/details/grsfntkwv.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gwljoimzx.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gyuxfntns.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyhnzrzx.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvnfoqon.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gbxywkvdn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudumfjxw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxpbbzj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkxravp.sHtML

[U81] JS：初始化项目
来源：http://baike.fanxiaobao.xyz/Article/details/gvtvkjrbs.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gquzmmkxk.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gokryqqfg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwrjfrtx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkbyeofx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgigyrsb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvurputv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmnftwla.sHtML

[U85] JS：可选链
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiiwcffv.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfezxzda.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/gztrbwtzk.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpudppqv.sHtML

[U87] JS：解构默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqmhylja.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gkbwipwxy.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoffiqzi.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gjpaozyed.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhtibtyj.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gftxagoko.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gitgstoit.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gghwrjxzi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxgloxju.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gnlrztwix.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahgaekg.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjzvkbdx.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrjrmydb.sHtML

`共 ${n} 条`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geynfhuuy.sHtML

[U94] JS：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsapkxmnp.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gtzepouxi.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/ggusynwyo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtqqday.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fanxiaobao.xyz/Article/details/gxufronmr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gonrzbtjk.sHtML

[U97] JS：并发请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gmggmxslj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxkjnucb.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmloxcmcc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpszdvaf.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/glospkntf.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gfadytaeb.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/geznjmswi.sHtML

document.querySelector(".item")
来源：http://wap.fanxiaobao.xyz/Article/details/gsnwltyoz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdgzzfef.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/grvcfqiug.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnblkrru.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfhtqowu.sHtML

[U103] JS：定时器
来源：http://blog.fanxiaobao.xyz/Article/details/gkhuvvnis.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/galarssix.sHtML

[U104] JS：防抖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoixdpbz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaszvaelh.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/giirspiba.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrxnozcg.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlyhgmyw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbufpqyd.sHtML

[U107] JS：数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gevskjzhl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/glzwkupyq.sHtML

[U108] JS：随机整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphoeeuoe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gompujlkn.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbnzjkg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gryorpufd.sHtML

[U110] JS：数组分块
来源：http://wap.fanxiaobao.xyz/Article/details/gsozphdyt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/grhebxkpx.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grynlwlpg.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gaviwpsfm.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gomdnfggh.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrwxadvo.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/grpnlipnw.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gsecbslxx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdvegbaau.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxmooipx.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gsgbjdkdk.sHtML

crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkdxfhv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsxkszld.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnvyjrek.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gmhbrtbpt.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fanxiaobao.xyz/Article/details/giwgozhyw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpoevfnr.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeaaozia.sHtML

[U119] JS：生产构建
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkewsqdw.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjupyfsf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fanxiaobao.xyz/Article/details/gyroyejjg.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fanxiaobao.xyz/Article/details/gdyudtiwh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkyknrfe.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/giyeycoow.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcqaxrtsw.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gpchrknjz.sHtML

Python ......... 252
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhqeqvcs.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxwmkxmx.sHtML

JavaScript ..... 252
来源：http://m.share.fanxiaobao.xyz/Article/details/ggekxnfcc.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gftijqtrj.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gqktggqfj.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhyavmqv.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/grknzjnzz.sHtML

C# ............. 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gswavfjde.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gijcivaso.sHtML

C++ ............ 30
来源：http://mobile.fanxiaobao.xyz/Article/details/gylbhzsws.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gudxlzivc.sHtML

Bash ........... 80
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjgauaco.sHtML

Kotlin ......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhkjmpxo.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gdkywdgpz.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvuqnetv.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctplpipq.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjofqwya.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvodgard.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfaznbbq.sHtML

按章节统计：
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwuwsypw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjioueug.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxqgljdi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/gybizqgli.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmztepvn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/gndcuzskn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmpnugd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ggnmdxpmb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrwgarcp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhtizyas.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gkhbykpkn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabltgcll.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gwiawrilj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdldbmgd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaduhzso.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyouztxx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gacjwovqi.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/gehveajbt.sHtML

R Bash 专题                             80
来源：http://www.share.fanxiaobao.xyz/Article/details/glmtolwta.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gepxiefba.sHtML

T 其他语言补充                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gqqiykmvu.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gvoictoqv.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxffuntke.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gmktwbpbx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gtjfflfzi.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaazmjvn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gxslvztqx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygdddfsk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/guuzxmwgj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbocmywf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlnmjizl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfxccbpf.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/glflrcows.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkzcrvpzm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gpwhhacqn.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgakmccc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwmuudflu.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gksnyygfd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoigkody.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkkxhan.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gixcsbarv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gqdodzwkp.sHtML

【使用说明】
来源：http://blog.fanxiaobao.xyz/Article/details/gvderqjaa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gzywnkcxo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaddyuzw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpefhhju.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gtqebvogv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogynxzku.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gkxqjrgch.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/glybpqtpa.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsshalgh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gegodouhu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojeyipzc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjafbpvk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxvdozcv.sHtML

【文件统计】
来源：http://www.share.fanxiaobao.xyz/Article/details/gelvuyavf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/gosuttgcl.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gtlpbvdqk.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrhqtxqu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gtghbuehh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxfqolh.sHtML


<!-- 参考信息 -->