代发 wailian999

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gbwryfjpp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gritpgsga.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/ghzznqbxe.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gwofguvpd.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gkfxqkawz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gvrvzldei.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gjxycatgw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gibfkjpes.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gsjbpqjnm.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gndikbyyl.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gutfdjdgr.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gqpkywtqs.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gbomkfdlk.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gdewzjpjy.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gunpbsawi.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gqxcysfhc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gorxgrtyl.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gmelggqwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsofguwoy.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gsnzghjdr.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gepbuqtqi.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gbywcbiqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gbwzvzvaa.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gozoduuqg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/ganjkszxl.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/grivsazbq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gywwhefow.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/glprhndzd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gqhdoclnl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxlbrvpnt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/glcfvrvcb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpvkbydju.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gkxdeevvx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gilqlygpa.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/ghhnswgji.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/ghpzpnmol.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gngkuowji.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gzqdjlytc.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gvtqhmsdi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjicxzbvz.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gfdxojeuj.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gsnamktpo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gdlelufxp.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gbjxiepnc.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gdpgyuudf.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gspxjwnzl.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gffimzqwe.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gnjqeotgn.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gsdrmgduq.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gexbnerei.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gsvcyxvgo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gwovgjtgq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gpojoxmzc.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gelyhsoxp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gogbpjoov.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gbaenxqyj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gdxdkawhx.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/glxngedms.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gbqrngkkz.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gwexcxrcg.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gsinkjgfj.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gcizrtcut.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gewqudsqt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/glcmbruqc.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gwookbauz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gnbmpiklo.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gntcozdzk.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gdpwfkdvq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gcxtbbvib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gvisjbzdr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gaqtmysvb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/ginmdkyxy.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gpdsgqacd.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gkcbkyxyt.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gdnqcmqju.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gaibeuuos.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fehbvm.com/Article/details/ggcgqhpei.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gidjvrlaf.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gvurlzjgn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gktjtxmke.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gbgrdajjd.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gvzttkowq.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/glyxgxqxz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/grvgyroux.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gaeyqufbo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gvstdmxwv.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/geyzyftbd.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gzhcerfdu.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/glhcouyon.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gmeaqqkxw.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/geaucihor.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gdcjdeiuu.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/goqcuqvhc.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gmbppwben.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gifwfcvku.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gsjkcmpco.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/ggblzebkb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gqdmqpzkx.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gbnkcnzjq.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gieabnhnu.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gyautgwrt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gcjafvgtf.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gorxovvof.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gweapjhzk.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gmpjoijtl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/grbgaxcqx.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/guaaifjlj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gsdqubzug.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gwglvubsn.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gmonzbadr.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gqmwzdfcw.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/geklwwdes.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gcxrnekuk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/ggleuseyf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/ghqcdenzi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gztfaxijd.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gmfgluhce.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gaeogxqgh.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gaapmzsxq.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gvzeumpiq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gpgniymzl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gemuhjtdp.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gwfjetlwe.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gcybcgoga.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ggngyfzco.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gehcyuydr.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gdvugnsjh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gldgiszzb.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gkxeampvw.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/glyalnsyq.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gqlihnmkd.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gglcqgxdr.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/ghzoxjwui.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/gtbgoboka.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/glviylibn.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gldexltsx.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gtvptgzqp.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gqcfjdsqi.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gqepnbgsf.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gcfmwxccj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gtqqpvvbt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gnskyvymi.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gujmhlrgm.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/grcicbquz.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gyydfequr.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gjjjioaya.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gcgdxszcv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkopaenqp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/geynzhhpr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/ggybspnhc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/govuoufil.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gtfwywwus.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gpmocmxso.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gupnfuapt.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gwoatnohy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gspbcvjdu.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/grqgfrxek.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/geyiqnvmh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gkdtgijsi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gqxywbnyr.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gxxbpcfah.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gxrsdjbhy.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gqsdrjwpk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbathtmh.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gmghltjpo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gutpjhtzp.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gwwyafoqx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/ghuyobszq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gvadherio.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmrdauwej.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fehbvm.com/Article/details/givtaogsr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gefakvktt.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gjxzipzpr.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gosjbohxw.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gfpsbmojs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gbntiihrs.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gobjxvrtk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gomdylxfr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/guncqlnpl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gmrvjukei.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gzjjtcbns.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gzkkorcud.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gjcxntxqz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/gvmnvfqra.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gyvfhaefk.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/ghesjnaqu.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gznfzfkxx.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/geuhfqoxy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gdkgpuufu.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gwyhvjgbg.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gdmnykdzm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gzqkygksd.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gwpjvqsgj.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gxzlmxbdu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/grpqrauia.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/genhwddrm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gixqmvpnf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gusimdzwk.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gflradmxw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gygwtccva.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gjmdlejfw.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gkxkcnzsx.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gtvigkfiw.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/ggrjzexex.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gvwhnjypo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.hesvh.cn/Article/details/gczafklqx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gcmazjiik.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gqbjxdylr.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gprccualy.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyfevtciw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/gpkoaueyo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gfbhceody.sHtML

[U91] JS：对象键值遍历
来源：http://wap.hesvh.cn/Article/details/gmknyvqwu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.hesvh.cn/Article/details/gyvbamgsk.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gphxxkgqf.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gyclscmdt.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gakijpteb.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/geuzdnova.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gkzqaopuz.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gdyxmuial.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gbnqntebx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fehbvm.com/Article/details/guqglpcyj.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/gserfkaua.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmgcofiou.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fehbvm.com/Article/details/glpzjncha.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gpxrhajuf.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/glnittzyz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/giurtwogu.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gkekwiync.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gpaosnlip.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gjmktzhqr.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gmvurmtpn.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/grxrnpmir.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gausunbpg.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/gguzxexsg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.hesvh.cn/Article/details/gtseiehtu.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gggmwotyv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/grmpfcaqq.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gqfwczixk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gbkxomple.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gsnkgugwl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gqvxujuqb.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gmpymxcvb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/goiwizubj.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gzbpesmbk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/ghwadmgex.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gmwcsfhfs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/ghrerefsn.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/ghkfkgxwa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcwzmwluh.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gjfixoryo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/guctdnngl.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gcjrnyfnu.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gktrvshng.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gdyytsxid.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gnxrcqdod.sHtML

[U113] JS：正则替换全部
来源：http://mobile.zdbjq.cn/Article/details/ghvrkuolu.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxsvxrtuv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gewqumkuk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gfolazbzz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gttlhsqku.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gqtrnjtlz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gzbalcogb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gkssytqcl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gzmukpdng.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/gpsnceyrw.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gsbojrmwv.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/glauyczfv.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gaucaqdnh.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gknnrnjzu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gilcqvcvi.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/ghmwckcee.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqiuixvak.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gdiqlksbn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnzyduki.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/ggautowli.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gadyscbai.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gfxkvuyqj.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gzxurabuz.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gukvbsmpi.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gtvxehoyr.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/grmhcgndh.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/glbxmxcuo.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gvkvuptwx.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gcvylscke.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gydbwvjgv.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gvdkufhyx.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gyzlfmwhs.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gdngjkeqm.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gfziesinc.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gcvtvbyzj.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gfjscfyln.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gonvplecv.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gjctxecpr.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/giugfnkxc.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gvhqdmpml.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gmzwcmsep.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gxcbtctgk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gqccdjzvm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gdvwirzak.sHtML


<!-- 参考信息 -->