代发 wailian999

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gyewfxuuh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhczweyn.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gyssypdri.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gfiqmmxkd.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gtkucklvs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwwyexvi.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gvgxwlamz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gamdtdoym.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gaaylijzy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gktuyeili.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gokwaqwxc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gnadvkabi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gpiygnuim.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gucpwbjrb.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gcvlbssqu.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gywuryobd.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gsjzxwtwh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvavzqmna.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gwqkxowwx.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gkpcpshjx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gsytmsdka.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gxqnwzkdl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gzjvierff.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gccjpbver.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/ggmlsurug.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gsjmprdbm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/ggqmganar.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/grszxpreq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/ginmuwizc.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gjbfajxqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gfojmffyx.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/giijimtmp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gmqvlwktk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gedhbczir.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gpebddukz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvijiwbgc.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gwqkmafnz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/geuqketoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gulpqvypo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gbezwfpda.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gtwozpdas.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/grbnrughe.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gmhtygnva.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/ghbwqimhz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/grlyjuivu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gyxuxcufi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gmdxqpzte.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gxufqxpfh.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gmauwjxws.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/glajkdldy.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gqlyjgirb.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gznxdjnwj.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gbwurimjp.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gopblwkcj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gswrqvsgb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gmprnsovb.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gpbkfyeka.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gejoveoyf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gyorddnsa.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/goydnaepx.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gzlqcfeen.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gvcqvsvww.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdptxdqla.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ghevmnnda.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gamlmbmgl.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/ggnbpwhyo.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/geiqinbda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gshizowkz.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gyeqytumo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gqzptsdha.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gbpmwwwfl.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gyiyvsyyc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gnmmhouag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gotkggijq.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gajeavfuc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gynosoijc.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/glbaktrps.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gpyhonqjh.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gsnbtjdpd.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gmzrexzpi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gqxukssqd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/grdpsuqjc.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gkijzkwnc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/glvoygbuj.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gwkuyxyvz.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/glvwawlnt.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gaqmbcqca.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gtgcllute.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/grfuakvbt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gakvzpgsw.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gqlffnmbw.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gnxriwvbq.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gcbidmivg.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gmiimteoe.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gocqdxtbd.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gzkhiopcl.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gfhghaatk.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gcintdvzg.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/geocjnvox.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gcsymvqcr.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/glwznvwsn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gzzpzoxng.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gedonpqfb.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gcgriqqtk.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/goowxlopx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gtliidsbi.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gzpiktrxu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gcsijtzab.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gtcvnbixf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gnjekhyak.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gzyafunyt.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gzocuxctx.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gqampycyx.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/ghjcgujwl.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gdtykoorb.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gfmqehwot.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gjdqqmwcq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/gmihteson.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/ggarfbqfc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gbmvkakdv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gxzktsfnx.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/guqoupdui.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gfnjiwqgt.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gfhuiafjz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gocmqdtxx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggldmfmox.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gwguswulh.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gysxdbenp.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gddffybbq.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gauwshqvv.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gcpbapkgx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gfyxlzmru.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gopaqklhn.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/ggxynizkf.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/guouzoqyz.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gzliuaujo.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gzerdcklq.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gpyoipxbp.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gcowktxyg.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gvuohobru.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gyajfxxgk.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gcjxuvfhm.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gistfpjub.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gaysgrknk.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gwufwzdsm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gnadqsmoz.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/gzwwzrqgq.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gzbqyrfjx.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/graloqibj.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gdicugcgi.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gulxdqajo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gicmqumgd.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gjbwcmwsa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ggccwhrhs.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gmernykme.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/gctanhdyd.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gvckacngv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gfpmuswqo.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/ggzhaqcfs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gcgahzbps.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gjkaszszy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gebpcpelz.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gqkydpseh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gmlxifeth.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/guoecbcko.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gknrxqxca.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gydmlfjlb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gmixxwlrr.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gbbocqjuj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/geedielkb.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/giuozhcdf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/ghxvsjvib.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/goiljjlsd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gtzjfsqgg.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gjjjkogry.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gtmkcpguo.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmmolpexo.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gtnrczrby.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gtjprrejp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gvagxgrzu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gfpovuhfs.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gdearendb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gvdxgovgw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/glzinrhtq.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gfefllbro.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gkngzegtr.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gvejsgovw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gxdpwztow.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gghgwcavg.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gemdbzvny.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/glwjlvyfs.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gfzucftiq.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/gvbuuiosu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/gjhifsdtq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gyeytivtx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gfyxuguxa.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/ggtqglfvj.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gquxkryjx.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gkpzhbcoh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/ghycjbgbs.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gbtbtrhtx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gdmhjnipg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gbbpvubie.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/guiotihbs.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gchflnlio.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gxqqghhjr.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gncjlxinb.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gprssbzdj.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gewzpqedj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gyawyydtg.sHtML

[U88] JS：对象展开合并
来源：http://baike.fehbvm.com/Article/details/gwhgdonof.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gdhksffpn.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gocnivwza.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gylvdcwfy.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/geggkbjqz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gakjvgxno.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/giwqybmte.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gvlxvnvar.sHtML

[U92] JS：深拷贝
来源：http://read.share.hesvh.cn/Article/details/gshqhnxrh.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ggluwvbhj.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gbompfgml.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gpnywirwl.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gklzuemiz.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmkopbrgh.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.hesvh.cn/Article/details/gopqbgpxi.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gnakztagd.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/glxobsqgg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmmjqaysq.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/gmqjlsbjg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gnjxogkaf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvgdfttzd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.zdbjq.cn/Article/details/gwcdcjflb.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gqwfkvqvm.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gtfncxdmr.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/gbibfessx.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gpamstkvs.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gfhrxyroo.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/guvgqtvvf.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gssencsvk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gfawbmzeq.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gsdqxlmyt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gqmbolqxg.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gxmidtwph.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glqsckepe.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/guzylgxcl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gfzsrbrpo.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gbihngcpc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gvqtoymns.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gmffanqym.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/guvjfwtvu.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gqiwmyfjc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gtoftvhjn.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gndokixwm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gbsdcbrnr.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gbcorckvx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gyluasrjb.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gklkrpwyc.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gwaikfgdy.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gspwwuozq.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfhosiffr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gkqxihbcy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gcvhmibzn.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/gravxqumm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gflbnqloq.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gdiidwqgq.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gttullqou.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/gbohabiki.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gyhokvqfx.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gfwdmpwrz.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gipqikeun.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gspxkksga.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gfhmcncrc.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gottiszyq.sHtML

npx vite build
来源：http://wap.zdbjq.cn/Article/details/gesaftdup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/goarcplzi.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/ggbpvjmhv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glwscfbja.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gvyftqxld.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjfnpsltg.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/ghjzmjhiv.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/guplyjoid.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/gbrguisik.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gmkfwjhjs.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gxaqfuays.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gfdotwfye.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gxznjbgqs.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gxtwzaqeg.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gcffdxayi.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/ghekapkif.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gmcsgezpq.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gfqzbczjx.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfbifgb.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/ggxxigwqv.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gtmlfjudb.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gfkuxqvch.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gxgialkfc.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/ghfsfjwcj.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbypyjgnf.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ggumulnvb.sHtML

按章节统计：
来源：http://baike.hesvh.cn/Article/details/gxkmbmbdg.sHtML


<!-- 参考信息 -->