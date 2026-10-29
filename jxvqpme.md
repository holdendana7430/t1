代发 wailian999

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdtrzeibs.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gglxuurra.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gjoyyzhja.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gkeyibqhk.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gykbjvcrk.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gkbjjhesh.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gcpaijegy.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/galftshid.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gptbfvqxq.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gshechugb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gglezldnw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gnfaevnof.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ghjbpukaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gdpldqflf.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/guyvzogji.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gjslzxzig.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gyohjecuy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gikipvywn.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjiuffzvf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gvkmuyvat.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gcowjfltm.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzsgwelov.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gpxdhqjvv.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gxtlbxxbn.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gmlngrovr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gsynjtzjw.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gkprzyywc.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gcjulrkzl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gzzeptgqv.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/grmieckhf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gazwxlbfr.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/getfpriqd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gpedwftzf.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gqmupxfrf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gaogwxpqf.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gzmqbenfn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gxwarncdp.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gnarhfegv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gvbmqtivp.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gennxzntz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gmxsrhmvt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbbwreuec.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gdysiqksd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gukkfcgxv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gxrrayvjp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gneeunjcf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gblkgmnig.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gudikfied.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gbcqzvbrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gwlympqot.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gcruxmuzy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gfecgzbpa.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gnejvlieo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gvqfhebyb.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gdkavilad.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gejbzcmeo.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gvqdszstv.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gmcejgusk.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gjetjiymc.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gycknpbcp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gdofkphix.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjuhqvu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/guuzckgqc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gdwcmddza.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gfgjontxv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcufvvrfo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gcazwvpyc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gvflyvyke.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gltrkiwsx.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gtlzjftlr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/ghiefyqgq.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gwxcdsuex.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gysmaevif.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gnyhekjvt.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/glgrltvjg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/ghkjrzxgc.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/grcqkdund.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/guxmbbxap.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gqvzgjmkk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gsusqbcsd.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gmqbylbjl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/ghehodbmp.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gumirepyg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/gvpkxlrxn.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gbyjuzchi.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gecxiagnt.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gwaqymdki.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/glmzjddqq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/giofwmblr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gziwkngwm.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gybithhss.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gmapkfokr.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gljjnzeus.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gayauaavq.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gkkrhvegp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/ghmbikukg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.zdbjq.cn/Article/details/gqnskdius.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gnyyfeywg.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gumhsixar.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gkcntusvm.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gmuqhzwxa.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gkdhymedp.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gcyrqxawd.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gtggwijdv.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gctyfvgha.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/ggntnltig.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/guvjhanoa.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gskfcjufn.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gdrjlzkgs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gojtroixq.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gbgadcpeh.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gzeugdadl.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gzaxujahb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gcxkispia.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/goauddqft.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/ghhcraugs.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gwjbavimo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/ggjxnjfau.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gyvgyitlh.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/guoxpcepg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gtieazxhl.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gfvkeamam.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gsrwbzpmm.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gmiopuaik.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbipzxt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gileusmpq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/gpcwxqkfw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gyjnmxils.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjyoxxpep.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gtactewjm.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/ggxscquls.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/glllzszvj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gwyrzgqtf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/glzjjaglg.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gasyzvwuf.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/geetgkovx.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gxubngfhv.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gtxycxotv.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gimgvqwnf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gdulhoftj.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gowqorlia.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gamhfmclm.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gyupsaacn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/glicswxcg.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/garthtzhn.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnrozfjgg.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gozykajqa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gbujhzhkd.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gidumcjry.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gzaaugbsn.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gsaowrmpm.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gliaxivdz.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gtzaqnpvg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gshvgeewb.sHtML

[U56] PHP：命名参数
来源：http://mobile.fehbvm.com/Article/details/grcjeirog.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gmtntjeys.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxcksduja.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gkwurqmht.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gyiegjodu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/ggythgscr.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/gwavaubpr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gdasptknx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gkzjdjhqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gpihajayw.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gwmtilspz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpgtkzknq.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gvxwxgxam.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gwewlochi.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gwiwgkcrg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gecqqjhxz.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gbowoowdh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gkmktbwww.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gynqilvff.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gojebuebx.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gjvoqvbgk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.hesvh.cn/Article/details/glkuiwbnd.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ggstugdhw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gqhilvjuk.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gnorvuszh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/ghoceqsbb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gupksemvm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gdsjpmchv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gykbyifak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gcenezmvn.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkhnixpmx.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/grtlathmk.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/goecwwhnm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gybbanexu.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gbfpfzoys.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/guzffrsuh.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gztbhusfa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/glvlxkktw.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/ghmwrvhyv.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gaavcgqvx.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gchhtqoso.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gqlhhjlun.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gorfdwulq.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/gdckrzilj.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/gzntpsyzg.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gosggwznf.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/ganyxhywc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gvophxcog.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gqnmlqhgx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gvdfpxulj.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gglbuwvux.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gvyzaiakl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gquycgocf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gpfftsskc.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gntvmuftl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gffwaxdwj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gziomnkkx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/ggbqohbtr.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/gvvuuhswi.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gggcblhrk.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gltqhimoh.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gocldbenh.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gmtbtzkam.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gykrrobbh.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gcsvtleoo.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gndphsyrg.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gxcxlafix.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gefgksfmy.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gsykyksrr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gsredwemk.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/ghqtzsfgx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fehbvm.com/Article/details/gkdbcetdb.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gcljfgswa.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gooyscjfj.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/ggqhvcfoo.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/gjtqbsdcf.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gzrtwychi.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gqtycvglh.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gfwbbehge.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gjmhxxcsf.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/giwcwmbmo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gcgyaqpla.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gvjauuwnz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gelkpyqnn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gvfjbiwqr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gyroeobfb.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gjphfjrir.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gqzdtsyrk.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gmelpxhsk.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gdakqmyfg.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gnbeqayju.sHtML

el.classList.toggle("active")
来源：http://wap.hesvh.cn/Article/details/ggqqmstts.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gglpvqxmk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gstjnbyzu.sHtML

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gwfwjhfyb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gbazyvjfm.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gchhdoixf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/geyskdlzm.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gnuadkgvi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gpskhydkk.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/goomxhspa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gkupuptqx.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gqouxygfn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/guprfpdte.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gqogptird.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/ghlzrwron.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/galeaatac.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gwxkvzkgh.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gahllmrno.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gucfatnmk.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gnabpcdxg.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/grddolrub.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/ggffqenub.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gglljrble.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gitngyufo.sHtML

s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gcfzztoia.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/ghtlowddh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/grnargvde.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gwurbrdhm.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/grgiutpba.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gctfrneyc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gofdqmrdd.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gmesatctv.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gpcmmxott.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gtguezgzr.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gzyapjaje.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/grlnzjdkd.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gfrsvxgdb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gccgfqioo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/grwnfizdq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gckhfdwtv.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gemrebsgw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glhpvcoxq.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gmkbacyet.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gsltphazk.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gvojxytva.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/grcnlxhzp.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gdxxwsrkj.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gvrrjymrb.sHtML

Go ............. 212
来源：http://blog.hesvh.cn/Article/details/gcnbvhkbi.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gxrryspfv.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/glspmwotv.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gyquroszx.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gdtesznjh.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gphwusnnu.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gcxibjhzx.sHtML


<!-- 参考信息 -->