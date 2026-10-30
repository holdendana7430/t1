代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/giyusfppv.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gewpzyhdb.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxbcwkz.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjdcomtx.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaojjsnk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkydcgikt.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjoldndn.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/grsklvaex.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzpehclh.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/ggboavbym.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guaaqxsnh.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gkxywimgw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmplhypf.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggncotata.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnzxctxkp.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuvkwlrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gngpzeipx.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokabuyc.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/giujlhtzq.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gikvpezdq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnscxsqa.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxizgfseo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvebggkfp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggjnxreoq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpvnhcyv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlunuuxn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvxicsu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxitmwfzg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/grazcufrv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnmcpuuv.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/goskkiazb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwgwixgn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gidfzmfmn.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmglldxs.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgfbkici.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdsczqnk.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzzejikt.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gudcthtos.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilifzoqb.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gljtrkrga.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhytqlbp.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghtzvivg.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/guqepyjhi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqysasrti.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqxccfus.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gigcnvbzf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gicobxfbh.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbsptnud.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgtdkdcm.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gtytzjlic.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejndqga.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gznvvmcvt.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/grtyjutcx.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvyqpdix.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/glpxhxrze.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gwdmcybuh.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/geloxgerc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzixnocp.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyrxynth.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/glajbyqof.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkqfnjqa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjsodhgo.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjyfbjwz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gpyktsmbl.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gezcrbbbs.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gooscghuc.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/ghamfnjov.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnkgenbr.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvpjyotlo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmritmpo.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxxpixe.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gppkseytl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/glzlgcvqs.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhfvknay.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/grepbketb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gavjtvqxh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdeqhyep.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpcrkayc.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykecdcei.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrpnbdsy.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glugvycdq.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/geowrokgk.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsfeujwr.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmyqrkpt.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubzdkupx.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gyctajovb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvnduhrt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrknzjpe.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gsokxznws.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbthqmpet.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxngtdke.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdteaypq.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gnthtucwe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gsyjuihaz.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gahvdjcof.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gutsulfmh.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gxuawkxkq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gvjsseepi.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkoxmbc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiylrxqa.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gdxjdoogi.sHtML

sys.stdout.isatty()
来源：http://3g.fanxiaobao.xyz/Article/details/gueqhedya.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwevqizt.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gfohxfixh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/ghedtnxgr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvdztvc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrirjsln.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqxykeqi.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/guhtfyxbm.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzprkhcw.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpbjlgg.sHtML

declare(strict_types=1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsupqfen.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/gulwhqcqz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixlewbiz.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gofuxqqcd.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gtfjpltaf.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbetqufsi.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gyyrogthr.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctiqxiag.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxztxxyb.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/grfupxnyq.sHtML

public readonly string $name
来源：http://www.share.fanxiaobao.xyz/Article/details/garllrynk.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gybdbxohg.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewzqzxxh.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvnrmtra.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakayknnc.sHtML

[U52] PHP：箭头函数
来源：http://3g.fanxiaobao.xyz/Article/details/guayljqtf.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjcuosta.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoklecno.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guykzfqsi.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvdqqyzm.sHtML

$obj?->method()
来源：http://3g.fanxiaobao.xyz/Article/details/gzdakopqc.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqsyrod.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gsyievnsh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqijkszc.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gibwvsrhs.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxqimlry.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gztvjdgyd.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gzpkbfswd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gkaihcpec.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gasjzudyh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gemwcxfts.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gxqvjchwc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwiuuvef.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gsugedlhy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gngpluwjh.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxjemqrp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdbkoasf.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gxwypbeio.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/goehungdv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gemtgqjoy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxblsqqz.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gpatokuyx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmuzqfei.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fanxiaobao.xyz/Article/details/gpknqybhj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjkrwsdp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fanxiaobao.xyz/Article/details/gufneegfb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gewvmvfim.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcrosgvu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkkoedjm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gshekynsb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyykrhry.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/grviodyme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gdefcezuy.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golpwkyaa.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/grnxpbsxp.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzxagxpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gxhdunckp.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gtjknenec.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fanxiaobao.xyz/Article/details/glrxytdrf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkgtbraxu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkqldlbi.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexavjhr.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygorkodb.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzpypbho.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhjlauux.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/grqdleysx.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gbrqoejvr.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzutsrnh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafhbvukq.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpdrxva.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbmuqzzt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gxpjhsjlp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxrwyavq.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gwernyhzk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzagavl.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fanxiaobao.xyz/Article/details/gtchfjfdi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gezxiagyr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fanxiaobao.xyz/Article/details/gfqzisktk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyykbfbzc.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gspjgmcch.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gmfzzjbai.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gtqgrnibk.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedfuclhn.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxdbfxwg.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gqxrfreww.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaqknsce.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrmqnyqa.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fanxiaobao.xyz/Article/details/glplgzgox.sHtML

{ ...a, ...b }
来源：http://wap.fanxiaobao.xyz/Article/details/gocroxykg.sHtML

[U89] JS：数组去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gopyckowl.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbwcalru.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fanxiaobao.xyz/Article/details/glqhqkfkn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrsntfmj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvgjyuq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fanxiaobao.xyz/Article/details/gfsjbpipv.sHtML

[U92] JS：深拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzrpujqqp.sHtML

structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnketlrpx.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqopvgacs.sHtML

`共 ${n} 条`
来源：http://wap.fanxiaobao.xyz/Article/details/gppiahvix.sHtML

[U94] JS：箭头函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeshfwje.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoqcsauf.sHtML

[U95] JS：Promise 包装
来源：http://3g.fanxiaobao.xyz/Article/details/gmynpjqmp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpsyfzdl.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fanxiaobao.xyz/Article/details/grrmpbpqn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/giidwvszj.sHtML

[U97] JS：并发请求
来源：http://baike.fanxiaobao.xyz/Article/details/gqadjyine.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaqeqpki.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gjzhxsijn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gepzsfcdh.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjurunwml.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gsgpmytxq.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhbdzvve.sHtML

document.querySelector(".item")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxmmfdkc.sHtML

[U101] JS：classList 操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmzdlgtx.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/gqwfotusl.sHtML

[U102] JS：本地存储
来源：http://blog.fanxiaobao.xyz/Article/details/gkgudwewl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhjsprwv.sHtML

[U103] JS：定时器
来源：http://baike.fanxiaobao.xyz/Article/details/gbphickto.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbftnwezl.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuwyqlue.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/govmlupoz.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/gqvycqaet.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gywjeqppg.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gkdaoxydi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fanxiaobao.xyz/Article/details/gejijkodf.sHtML

[U107] JS：数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/gylbliqfh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/ghwowajah.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gydffbgkf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwhybhdx.sHtML

[U109] JS：数组分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyodfrgr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmfxztkn.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gxlfzunzk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/glxzywhhf.sHtML

[U111] JS：对象转 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gceslttlv.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzpdzcvx.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/giymkkjhz.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzhtuqqo.sHtML

[U113] JS：正则替换全部
来源：http://blog.fanxiaobao.xyz/Article/details/gppxydqng.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjkvayph.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqieyirmp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gpzmfgrwk.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gguktvgel.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufttesxk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbgjifp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvedxfnrb.sHtML

[U117] JS：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqpaapev.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzgfkijq.sHtML

[U118] JS：开发服务器
来源：http://wap.fanxiaobao.xyz/Article/details/gyvthlhxb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/geeksubzl.sHtML

[U119] JS：生产构建
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmgwdjqt.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gvnjgfofe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gqdwncror.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fanxiaobao.xyz/Article/details/gwgeqwawt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwnqiaiy.sHtML

统计汇总
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpenurpi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhuasfyu.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gipthtmjf.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gumjxpnwi.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunzzesuh.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/gggkcjrbq.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gbzuufugf.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/goerieegg.sHtML

Go ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyhtguyf.sHtML

Ruby ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gxpmoblsv.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmurnmj.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/guztjfyqu.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryrwwanh.sHtML

SQL ............ 90
来源：http://read.share.fanxiaobao.xyz/Article/details/gppyzuhuz.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbaqutkv.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gfmuynufl.sHtML

Swift .......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvhmmhsx.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohspdzd.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/guvudwxkp.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gkdvudylh.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gmvwraqdf.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/grrigmosg.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gtcnkixij.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykxnjaqd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gxysduzee.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvwdoelw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdydtngaz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/geitpxyfm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqebipi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/glfmakdeq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gjvusufud.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gesstubtp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlrzvypm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gsbxqdgmm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gzetkqxor.sHtML


<!-- 参考信息 -->