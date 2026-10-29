代发 wailian999

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gqesgxtdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gtgzlnigo.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gurdnmqrs.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gisgepavr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gldrtarfq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gndxnrlay.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gghskhgrz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gpdkisfub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/girbjlylc.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gynzdqcqr.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gghqmsadh.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gqudrfqwb.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/ggnfvwoso.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/glofphzyh.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gemdykhma.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gmfptoymf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/guiweqxkw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gztqsqirz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/ggreujoim.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gksgbxidm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gqjbpaokw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/goiqenecm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gfvhtqifd.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gsqqugsup.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/glzatyndi.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gxipbuoua.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gqlvyhndj.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gglfrlzib.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gccgiroyv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbwsovgsd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gxaiefuws.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/germjxhch.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gcopevpgd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/guerfpkos.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gfhezfvcn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gysnjdvga.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gvsyydail.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gloksluzs.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/geyynepqi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ghdhvrmxk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gtmkjuhdw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gztyrjjgs.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/geculflyj.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gtrgqikuf.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gybejloii.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gckhtkiug.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/ghcdwdsnv.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gezndiswx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gtwqteyfr.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/goaordxmi.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gnmswweuv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/goeifrvqu.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gyxaejjca.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/ghbhpsqow.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gbtnuiieo.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gstiefjud.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gijdrkkit.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gxefivrrx.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gnhqrptyw.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gpyryprnt.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gbpdtbbci.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gzymtafnb.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gbwgmmces.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/grfqyrymc.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/gdajkqlrx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gbhedyotp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gvmxotnuo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gvngehszu.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gavjidcop.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/glgswitew.sHtML

[U20] Py：缓存函数结果
来源：http://3g.hesvh.cn/Article/details/geazdnnkq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gkhhpdyqe.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/ghdoqgiqb.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/giclpwagx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gnfidqxvr.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/glffwmxtm.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/gcbpqsbvz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gcgefiqku.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gatqknzhf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gatzvyanz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/grtaucxab.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/ggojvmndf.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gdgvwdxen.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gaxmbnmvt.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gfajuymbj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/ggrqxhfuj.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gvywhivmf.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gmtsdhuhl.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gdqnjtchi.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gsidorphz.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/grflzewvj.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gsmrjmbya.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gcknydvdm.sHtML

python -m pytest -q
来源：http://blog.zdbjq.cn/Article/details/gosidhlux.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gpnldxpuq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/grfyvworu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gfgvdxfot.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gxshewqys.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/glogfqyuf.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gsdhemeen.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gardwqioe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gdjbarclf.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gedxlspwu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gjdokhnch.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gdvrdojxu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gxkymmqew.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gorrimvsk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gllijtfot.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gtunecwyh.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gxslnbgjo.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gnlmialpx.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gpigolebj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gadqdxlfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/ghkwjdxpu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gvhcbobuw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gqitdrilv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gcunlezcn.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gcqdpjdua.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gbaixxndx.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gocbokrmz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gvludwjev.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxmfbkioa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxmanmq.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gwmudyztz.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/ggmzeocyk.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvaldki.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqlhbpnma.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gkvnlijkm.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gkmnmizoz.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpmegit.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gnblcdrhp.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gucwjiuhc.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/geieurhoo.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gcqgprfzr.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gpebvcskv.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gszyzlhnz.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gljxtymfh.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gomgnwwgc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gdfvtbkgl.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gcqvrhxme.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gftkdokjn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gkqqveijp.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gjdguugdv.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/golwwxncy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gstbljzbq.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gmfcftifa.sHtML

[U58] PHP：数组三件套
来源：http://mobile.zdbjq.cn/Article/details/gcvoeidfn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/guufxuart.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gfoyuirgt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjgzuhrnp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gagjptxap.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/ggeawjvbn.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gyptmduep.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gsllomfsb.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gsikwhfpg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gyqlweyhv.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gaihudztt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gjqvslvzr.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gcekknqjx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gkjphocwv.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gdeavxpdn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghesqgkuq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gbwprsigg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gchipswum.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gbjnjnydo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gsoyegzwz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gwwlymcoq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gdlykxazw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gmyikqlev.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gsizlglhf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gqqtpgnis.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gpojoeorq.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gnfvvvluc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gdhpluhwh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gymhwubcd.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gbenesgdy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gwbxrbhpn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gwvztaarg.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/grjjwzspq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gvjjhnaep.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzcxzre.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gnayoxbti.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/ghakkiqew.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/ghhfdmloh.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gveucnqpp.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gqyechaia.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gslhapfea.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gjgrnnzsn.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gftrpqfwt.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gdvnwrlcq.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gnosaiyzu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gmchpykom.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/glplwjzgq.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gzjxtvlgd.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gpcmhhrru.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gtekmjjdk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gsbumchsg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gobpctnhp.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gimucchpt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gvihasfdf.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/guvnoqscv.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/guryrrycp.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gahapthog.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gckvfwaps.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gsspwyfzt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gftbigdlt.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gabfucupu.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/glvjkleta.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gbwhiqarr.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gereafxsf.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gvntlfccs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gurahphet.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfvxdsmfi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gbbxscbvh.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxuzvkvza.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gpttigxeo.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gcwroefhq.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gzwrxghgc.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/glogimyuk.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/geczzufca.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fehbvm.com/Article/details/ghnboicid.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/glmkccyrd.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gahpdusmq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gvdfksmzx.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/glpxiodse.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gindwpwrs.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gdclotmql.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gvkrdlwwl.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gwhfxstfi.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gwtezwhrx.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gpswiehyx.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gogqhdzcb.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gxdqxrscd.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/goszodmly.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gzqgyfkrc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gyduzqkpg.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gwcfbbeui.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gilgrpjuc.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gcndnssbb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gzlmgjusf.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gfcfiuhre.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gukvdhonb.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gzzrzvytw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gnagzwiyl.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gxbmdmmku.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gdtllwtzr.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/goyxxmvib.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gxwizewoz.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/ggpdtdbcq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gubnunmgg.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/gpauzvykh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gwqpkowpl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gtqvwgvkn.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gegiyrugw.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gexrappoy.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtrghmlbr.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/gdekytcji.sHtML

s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gekyaxapf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/goqerkjid.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/glzoldjgy.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/grxlrcjxj.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gviirsajs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gayqfcfir.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gsdiyupir.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gbsvnrpjv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/glettyeyk.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gabkndbtn.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gzukcrbgc.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gsqhageqg.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gzwlcnpyu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gjqyvgumf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gkrvimtma.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqcsoxria.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gmkhnqskz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzsjinkhi.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gvjvtrhqk.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gkpvqkoxc.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gzldvplga.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/ghvaxsfdf.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gpfdqclpq.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/giioacvdy.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gdmnqwmal.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gdtsxjctp.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gkpinbvns.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gfjexzlab.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gbekixbdn.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gknpnzkcj.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gxhhxxrwk.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/goodpnorx.sHtML

Swift .......... 15
来源：http://m.share.fehbvm.com/Article/details/gfrkjlfhw.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gbouzjezv.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gxnwliqmj.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gxnrodeje.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gckxxrzkf.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gsqqsqjds.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/grgkwqowr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gzkxevbnw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gzxapadkq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/grzqwkown.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gwiwoyqmd.sHtML


<!-- 参考信息 -->