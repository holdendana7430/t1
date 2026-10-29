代发 wailian999

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gwtebrqkh.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gdzzsazqx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gunehtnuh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gnjzcjyot.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gecuuslbs.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gkacekfma.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gsstpocvl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gizdxhfaf.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gxkolxsef.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gkfgyilne.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/giwchhdwe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gefwrvcyw.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gizmmleil.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gyqcpqiye.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/grfswpeoh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gnvbptvzo.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gfwkgxhkm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gitnxveae.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gcexuraqs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gkgszsdrd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gguszciqo.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gqdsjnhiw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gbnbscaxt.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxieohg.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gbymnucdu.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gesmhdsck.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gjpcazvrf.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gahyuayew.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gfryethtd.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gubsoybvi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gqthzgzhj.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/giimnzzlc.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gsawhzrhd.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gmfbcijdw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqkveaasn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gdojxuzjv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gjrfbmowk.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gxpdqysxk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/ghfkwxwxb.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/goktuhcfa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gkxjiyalh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbegmtytn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gpjbzxvic.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvowezwud.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gcaicqkjs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gpicajcvv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gjxbzetht.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gtnkedltg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gyqzadvtr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gokadtxmh.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gtktzirwg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gvsapgmpi.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gpdnrxuuo.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gpqckubdi.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/ggpzkmwjr.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gafketniz.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/grbwpdibg.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gcffdtdfx.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/giiemuuns.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gsgwajjem.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gmqwyzssr.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gwzdzznph.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/glepfiyxr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gymecyqbc.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gvacilpjd.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gpivdityp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/ghwpfyxjc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gwxgywkny.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gkjcmezai.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/ggykfthcb.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gwnohanzv.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gcsqbylmx.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gdpukwsrw.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gdkovihgk.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/ggqiivwhf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gvlzyzeak.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gfzvskynr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gunhyjcub.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gwlfphqsd.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/godmhvnzm.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ggtikurij.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gfjgethal.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gydxvvwgm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjaersui.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gpmhfwzyz.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/ghcxbgsbx.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gkkayzdzo.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/guxerhjoz.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/ggzbfxjyn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gfjporluu.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/grhgzjpqq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gqeqwrpiv.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gxkcsboud.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gdybmrebk.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gdzveqceh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.hesvh.cn/Article/details/gqgfjzsmd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gpskppegh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gncrybgck.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/guavhxjrt.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gkhctcizf.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gcfmrvkag.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gpwxlvuej.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gjecbakhe.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gmhatpgwa.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gyquolzey.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gwazgvvyk.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/ghckvgboi.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gmzkxwdap.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gyvctzkjf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gbbcminsm.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gcetoslde.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gmcyiiprs.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gxpjsccem.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gfmrglgec.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gvdxljrkx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gchiexatu.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gtfyotugb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gtiwggjid.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gdhzhjgvk.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/glohhptmc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gytqrrere.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gjbziubwv.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gzlugwkkj.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gpjebzqiu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/glszqobly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gqdizoxgh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gcquzxsnc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.hesvh.cn/Article/details/gvppvuwbi.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gdglpkbow.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gclwpkjth.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gsyoecken.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gudyxucsi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gmbdsfjgr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gkdfhinbu.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/gmxgustxt.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gboupcswa.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/ggtubdclk.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/grxkxhvvo.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtmjvpjnh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gcsvssthn.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gkxdxaobr.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gvadnennm.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/gxwrcxvzz.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/glnuutpsx.sHtML

[U51] PHP：数组解构
来源：http://mobile.zdbjq.cn/Article/details/gbezbkpfc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gcdqgktbb.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gbqjymfjj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gqsvgqcbi.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/grmydaphn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/glaqteupf.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gvikraqsb.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gmucqsjzd.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbasvhfon.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/goxsavbgt.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gvxlptsff.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gqndktbju.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gfchnbnpg.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gdcuvclgm.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gpheaeros.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gzavnlafa.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtkogsqkw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqknqatjw.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/geobwpome.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gegwgumoc.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gkoplmeuj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gfigamnjo.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/ggcpllspi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gnzqtlsxq.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gumqbsjnq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/grfrteyna.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gkwxlabdo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gxgydriax.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gmuwytavt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvhjhkyzi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gjipylaxh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gzfjbqhxt.sHtML

[U67] PHP：处理文件上传
来源：http://blog.zdbjq.cn/Article/details/gbbtzshpc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/giiuueunb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/goiyonzar.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gzexhjgyc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/grifjbgnp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/gwpnjonlp.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gdeatnfih.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gomeszfrr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gsjtchmoo.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/ggfhzldko.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gpglhferv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gijdtdjys.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gzgojiswd.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gyajngadz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.hesvh.cn/Article/details/gpkxkkact.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/goijrwtco.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/grhspvczk.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/groqrvyqt.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gwzfvzrgx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gvzzvbolb.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gecphkvqs.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gqlyrianb.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/grrtoznrv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gughrymnp.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gpnkwuxcw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gkyvqtyei.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/gfncpzfzo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/guzqlupfm.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gvditrxjx.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/gjswolcio.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gyfcyfqcq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gpdlitqrz.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gejiupsor.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gesmmrlyn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gnjzcprma.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/ggmnlllun.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/grhmacbyu.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gbmtxmcnk.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/giyxzelrr.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gecodwyam.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gjvpsoids.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/ghldnxfxf.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gkzqkjvfs.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/ghsfzcidg.sHtML

[U89] JS：数组去重
来源：http://mobile.zdbjq.cn/Article/details/gxvtlxqzt.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/griuazlty.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gjzjborol.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gpajvvqby.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/grxhxlewk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.hesvh.cn/Article/details/gldeawsvr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gozacmqfj.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gnqimnnmu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzlsqizjl.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gyzwvijxv.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gbzrpbjbv.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/goyovzefi.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gzxwctqll.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gyjdljazf.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/gffogrnye.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gyqwsoser.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gnvxpxsos.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmunvuhas.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gywdzftdq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gmjafcsje.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gvuxcjfxx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gnzcjknzr.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gyimuivya.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/ggfircevh.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/ghtpnuiyn.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gizgpkcof.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gnrtgacvs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/guhqnlsvv.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gmvlbtsyt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/grezdhkan.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gbvxcvsva.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gdjykwqiu.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gburdqoen.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/giejftfvh.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gcoegakjy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/ggvnzdhku.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmuyphrlp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gefhdnkem.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gjiqaakfm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gqpjwwjmo.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gtkddojad.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gtsjjdhmq.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gtvqegkht.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gnpsszmay.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gvuwvexyo.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gbsbvjign.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gaziyssmx.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gzlxbnome.sHtML

[U113] JS：正则替换全部
来源：http://baike.hesvh.cn/Article/details/gaykzvuyy.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gsdwrszmm.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gazugrjgp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gacpplrak.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gqucwhxvi.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ghjrfzgtb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gkdbpwrsj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gmocnqpgb.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/guwcxngzj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gehvhnink.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/grmlvwgjn.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gyklsifij.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gzmyfqbfd.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/giarcjpzy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gxdevnram.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/ghwlkzzsq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqlzhcvxh.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gtywkkuvw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghpuxbqcs.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gzopqgjwl.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gqbxqefas.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/gmescsvoe.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/govewzizf.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gktknlxqb.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grsjgqnql.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/glaqugbyx.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/glthfylux.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/ghhnzmesi.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gjcfodjct.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gdtrqarfj.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/glfuibqox.sHtML

Bash ........... 80
来源：http://3g.hesvh.cn/Article/details/gedvxfwoi.sHtML


<!-- 参考信息 -->