代发 wailian999

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gaepmplzp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gfcqbxcgl.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gsoxarqqt.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gstydciah.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gdypjettz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzxlbwpaq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/geklowcib.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gcbhcxrld.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gvkyuagwc.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gallutypb.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gksojgmnr.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gxvdrpzxs.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/ghlhogmlj.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkunmayod.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/grqrptfvo.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gckeetdxt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gyablgljh.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gzwjykdfy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/grgodapbt.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gclkcpfvm.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gqcmljzrw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqmcimiow.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gywixsupe.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gxbhbksxu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gfhcvfafm.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gejgyjotz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxdhbjbaa.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/goulzvxer.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/glzrgbydd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gekvihgxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gutjrmmrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giobwtnob.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/grapsycid.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gvmyeujde.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gmqksyuge.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/goeaggrym.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gmczxapun.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/ghtankofk.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gleibmomj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gpponxkdn.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gozdyuedr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gjzlblxzj.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gjpqkkdzs.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gvkbejsjz.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/guoqaqnei.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gigrswtid.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gqwdgayja.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/glhzjymch.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gavmviukk.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gdtyggrpk.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gpjzmtxwm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gtnggzwdu.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gzusstlrl.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gwjwzdwvm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/grheznsxg.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gibjosati.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/goqvcfuwp.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gfrypmfvq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gepwjnsrr.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gnngmozdu.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gebmiqhpe.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/ggrcdgaiz.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gvzkeofhm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gcnwbjhje.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gonbpmqwt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmanfudj.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gsnkgaqvp.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gifieduln.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gpprtufvg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gldugykae.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gvsbsogzl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwnoyddo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gceficeci.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gxcgketfm.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/grjvchjab.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gbeeqftwi.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gmrnrpiwb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gxpnfoqvp.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gttbytevt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gsshcmkrv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gnvqeufvc.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gcqwzcliw.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gzmuujrfb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gloukdnzn.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gkzvtowxc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gvedhpffe.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gmmuwlpox.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/gxuvtwuag.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gbgnyellb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gypjpjmlb.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/gswvxhbcl.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gqadtcqxc.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gerqtbsue.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gzicmegry.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gsfibsnvh.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gnhbbdvdj.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gwowukjvb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gkgieafmt.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gdphlzutk.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gandqitbh.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gbcfwtucu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gptgjtrwk.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gznvzykan.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gdttffnoz.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gufcixsry.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gtsemmmsg.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gpneqsorp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gmpjcrqvi.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gjhujnybp.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gzwvpfysa.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gcofshuwj.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gchiwbgya.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/giyfjpadu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gelmiwufm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gfngqilaj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gwitoydvf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/geeyadctz.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gmpmvshwi.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gqrxrynim.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gilxgiikw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gwuigxmgi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gzutfnvlg.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gpytwgetd.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gwmelbytp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpyiuodln.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gdfzrwajd.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gsruiuatq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gvbmkuiwj.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gxibjqkmi.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gnrmjuezg.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gmhyfztzv.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gnjnsnjps.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gtcgcantt.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gyrlgjkiy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gwwabnzxw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/grbqahsfi.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gyxklgkxv.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gydtmbzha.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gzpcadebn.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gbnpilolu.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gtojisjqh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/ganxxctsh.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gtanonrom.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxqtrokko.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gwsllchvu.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gcpyszekt.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gfgiikdwk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gmjgdgnyx.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gfgwqjvcw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gnnujismd.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gwmteuqel.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gpamulzmn.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gmyjraeyv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gcvfstaeg.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gqilifpvt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gwsmylzux.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gackumrdy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gobspmysk.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gskmkjdrb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gugovaziz.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gdktiypcf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gctvhrbbi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/ghqgdlfdn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gwmbatfgn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/goiqyctua.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gjjmocoht.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/ghhlicier.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gtcajyrll.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/grnowwlar.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gnadnuxmm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gwjbslyhz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gfsewfogm.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gkknqdbgk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/giodmzsfn.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gltylpmty.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/goiktvfyy.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gowcdbnem.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gttfqwekl.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnfezilsn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gfglilppa.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gcvigdfpw.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gvxpfwhtk.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gbkabmoqt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gvjzmxzcf.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gslnlqkwz.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/ggptwsdlc.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/gamyawtpk.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gzgpwurjd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gyjstcaft.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gckanqdxw.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gafwysbqe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gjiyvzxlf.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gvxzhshms.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gsjcfwbka.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gxzcjhspt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/giapjulzi.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gklxtzjzc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gzgibjhho.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gjsgyqirl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gfptwlfjj.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsnrhke.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gyfkiuour.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gfufzkqur.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/glnptkxxk.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gpgzagukc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/goeuebddd.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gsvpgzryx.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/glfrmnain.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/giscsjhcw.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsyaaanci.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/grfmwscdd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gnaanbbnq.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/gaedwynhp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.fehbvm.com/Article/details/gdwtaxozo.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gmugrkyzs.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/guawiisxd.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gqbjhrlld.sHtML

`共 ${n} 条`
来源：http://blog.zdbjq.cn/Article/details/gvhbqfckb.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gteebccja.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gojdwwtxa.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gcvedczgw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gbsxqvngv.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gwxdjdssg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/ganrjqhkr.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gjxuqjtdu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwcodmxnq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbayxlfby.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/gmnebqanm.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gysbgathp.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gaxhmxggg.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/ghdrzosfo.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gerocdvcg.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/gilalkoty.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gzyqwnlkv.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gkkxknpko.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gtfgojlpv.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gfaifqrex.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/giwfyzwha.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/ggsjplbee.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gykeqiznm.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gufahqkrj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gfgfjfbhx.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/gaoufnjxu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gnartzsus.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gidnttubb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gfrgkpyjg.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gqkadpylr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.hesvh.cn/Article/details/gkcozjurp.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gsfwnldac.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfxembra.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gcqvdcwti.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gbvaxwqac.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/granutqhh.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gloamcyen.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/goopnczwk.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gxavpklyj.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gllkgxrpx.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjjjksyxj.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gykkcfpym.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gtxkvtuxg.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/grsmqafad.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gfyixmsmj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gdqawalcv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/ggqzjwxlb.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gwjhzoxbe.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/guycaolpq.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gvykszjqh.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/grazthmrc.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gfksochip.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gmlypjnmu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/gootdenzp.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gctgfdbeg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmynoobqn.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gdrljgtgj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnrllfyy.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/ggmjhiloc.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gsbwyptlx.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gbcrbfbbk.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/glaqfaoap.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gijdwwkpj.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gdzrhbhwb.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gnqgujrxy.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gedzbytmo.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gapylaxhr.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gwfvudrkp.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzzfnxv.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/genvsmkjx.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gtutjjzxc.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gtjbkedkf.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gttpjobnl.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gtykljyoy.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gykceohxz.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/ggqwekjhs.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gawwoatwh.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gxcjmmlxe.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/geyyjaigv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gskqysujx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gmwepnaeg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gcjncsfbz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gnebhthpb.sHtML


<!-- 参考信息 -->