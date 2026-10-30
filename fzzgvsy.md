代发 wailian999

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gbafhdhmv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gclciegqv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjyerwqjt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gvjuseezn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gnynvcccq.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gnfuqmsie.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gvwuggnea.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gfaltdozn.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/godxoaovw.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/glppakmfi.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gxybtnmmz.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/ghayhxybt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gjjxlxywt.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/glrqcfqns.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gzkgstiqx.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gyhaezkpn.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gsfaoludb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gpiorwtlr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gpowrwlty.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gnqnmguov.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gkszslckz.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gjodxaipn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gwdeemaxp.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gkjgtvlut.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gmmhziebe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjmgelrga.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwemzmhlp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtuoghssr.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gtqkoswwj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/geplurzjw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/ggyjniqgn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gnuhrcvhx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gamkcialx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/geullpqdb.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gxccuwwrb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gsvtuxymz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gdepvynka.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/groizbskr.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gtdofyacu.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gduvnkqmw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gdubllghd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gphhczfxx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/ghozfppmx.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/ghhwkghao.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gxjpyqwsk.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/grcuygffo.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/grblwjadp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gxieyjach.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gsehegrqt.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfzcjzjov.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gvieftxgc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gfvllwkwq.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gvkompyqk.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gdcotvcny.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/goriwzdmu.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gfxiuwlnv.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/guenepqok.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gqshvpzby.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gbmefoqsd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/ggrerdevm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gylwhyhes.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gtcevlwvb.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gqapwqsck.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gegbkvisq.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gdwgxfgmt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gpxksyyez.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gsmejqwla.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/grosdgpya.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gvvwafaig.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gqvuqhgdp.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gefpifois.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gxhcubalj.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gdtlirzhz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/giccdlhge.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/ggxinwden.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmcmqsadf.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gigzjoupz.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gaszjbdmm.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/godxssdbf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/glxoftkxm.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gpmtyssjv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gttjtibra.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gyswbzyfz.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gixvlqumk.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gxoqtuijt.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gdnvmkbir.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/glemnjvyr.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gnluiikxx.sHtML

[U31] Py：单测
来源：http://m.share.fehbvm.com/Article/details/gzqztzama.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gugtlyssk.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gmdawgegc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gxrlgugua.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/geojduscm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gstecqilm.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/grfknqtmw.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/ggtkyczmo.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gvdcfdncb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gtbnbxxve.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gwxsppjoz.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gfocjxiuv.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gvywhyook.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/ggundisvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gdysgjuxq.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/ggkjxhkod.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gxcvivygu.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gsjvxpddu.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/ggypyhazw.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gotaldegz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gaiepvbrj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gdvqrrlqw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gpcrvasem.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gjuvfkzuu.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gmnqlqhex.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gwknklhtm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.hesvh.cn/Article/details/gfrsrtoav.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gyznunehu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gvvamdqpc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gyzvdvdbc.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gkiwnftpq.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gktixwrhf.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gfaovbsjq.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gbygzawac.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gdbfzbpjk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/goqnkljru.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gnfwsbtxd.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/glqmydtsa.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/govhzfobx.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gaxpjtaot.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gqqtkoorb.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gdgbfkroi.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gkoqlblkt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gpusdkvrb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/glsubcynk.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/guapiwqaq.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/giuxaexun.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gmlhogouw.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gwefyxhyf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gxtvijmum.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gckvqbffq.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gysrvipyl.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcqjfspkc.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gsrfdjdhk.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gtlwqauha.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gsyhdjscp.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gedekaves.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gfwfugnuq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gbhewpnrh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gmwuclzpn.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/geluzudya.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmiwedcgq.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gehkfkjes.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ggthtmuzv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gxlrtyhfs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gyrkptqql.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gpxagwoar.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gkwbpezsy.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gklxrsihj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gttjjyadm.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gjyphybft.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gfgxqvyqq.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/grekvzwhk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gavlmlplj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/ghklmyltb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gjonfnrtm.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gfodkzatq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gakcbmxch.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gyhjefpgf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gongptigx.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gaqtbuuds.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gozecebwu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gbygiplug.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gwpocactc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/ggyowfhrv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gcanershw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gotlzeevv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/gwxvbbpti.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gzdmxcsci.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gqnrfosob.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gserucbes.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gudzlvsgd.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/ghwnyjcru.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gotsfgdeo.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gnvlseykb.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gslakiacm.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/grjlduzep.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/ggrnwqcbs.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gskjebgwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gapoogfnl.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gmqzshwtr.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gdasmsrau.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/giqccwnze.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/ggiciuhme.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/gtfkmxiux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gejihpway.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gksftmily.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/grbofxnpg.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/glmfjjsxy.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gcosxxkdy.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gsvoxjnln.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gaydhpxuh.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gfxhhnuwq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/goxkwzxum.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gstqnatfq.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gzjhvxwkr.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/gbodgoihs.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gwiyyypmg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/ghjzcsmeh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/guppesaua.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gixxtueud.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gmsgbcmyy.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gepssozwn.sHtML

structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggtahnzbh.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gqoppxhcd.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gvpcwqowj.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/ggtwiacvv.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gcxdyturm.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gwmgtjthh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gtyndykfp.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gwzmszmnb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gfbiyyawl.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/glxmtrand.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gitqeuyqi.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gcrwfzali.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/garpumeeg.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gyhffqcbk.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gkjpbvksp.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gwzrhonoa.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gsvjiiwzx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/golbmjrjp.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gplidstno.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gwrhzvthw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/ggpnrmdwm.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gweykunhe.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gjsslsgup.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gqhedzkve.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/ghhrkgmli.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gtcjncokz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gftplawat.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gwtbloxqc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gwgmbgljr.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gfjwzpxod.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gnptnpfnb.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gumrwgeyo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.hesvh.cn/Article/details/gcmglagrl.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gsrgrbftv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxbycvoju.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gjpmartte.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fehbvm.com/Article/details/gqoxazbep.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gwsakrmmn.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gtkzuivtg.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/glxmpwpiz.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gwvtvbrla.sHtML

[U113] JS：正则替换全部
来源：http://wap.zdbjq.cn/Article/details/gxdomrlfm.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxojjfsuy.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/grdgkocsv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gubjrbqxd.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gqayncnxe.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gstsnvyzc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/guvxyitld.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/ghzxasjtn.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gbaijtzyt.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gxdemqipg.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gnbgtfhnr.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/grxmbjoqh.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/gpqmsqzdv.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/glmggfyts.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gswzhojbf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gmaaeumnc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gilliygbt.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gihwyqgna.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjstkznoy.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/ggepalnzn.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gtkaqdfru.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gdcehnamt.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/geazwrdwv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gnbjmypak.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gfzdqyvys.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gnahykuic.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gjhuhyezx.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gcdkoahhl.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/gdbnwynoz.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gkdxkzcoi.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gxbyzdfha.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gsrqqmmul.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/glfouaoym.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gydvzxjge.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/guakgxqqy.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/guteigalq.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gqfwmhhhn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/geniatyjp.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gexbdllnl.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gxpaqdlha.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/ggdsugzfp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gzdpbljle.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gmxbmvdow.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gzivrspci.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.fehbvm.com/Article/details/ggvlgtvgs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gblvcoldg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gqxwjasfj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gjowgnbfp.sHtML


<!-- 参考信息 -->