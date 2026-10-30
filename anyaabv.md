代发 wailian999

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gxpokiigp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gqonshjtq.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gqojcaspk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gwefmsqgn.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gmfuztzhj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gobagpelh.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/goeugzece.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/ghefocrqa.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gdqzeljff.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gjuejigim.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ghqodgemn.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gifiqpflx.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/grynreual.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/ggbkuvomc.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gnfuzdasr.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gvkosqgel.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcfgnwlyx.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gqmznwkmy.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/ggekkntgd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gujovdkzi.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjksmyqfr.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gzxpncfjt.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gshkzcflb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gkrvxggnv.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gwgdsaxxa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gjosgxnvr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/ggjzxrxrc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gwgwzgiwa.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gkgxuhdam.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gjfdfhjla.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gesjrjvvt.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gjvipatns.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gizqdnrnk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gdzdtgwui.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsyblurvr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gtmrscwbk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gettikiik.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gpohxftnq.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gfncmjwlw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ggmhuwyxh.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gqnmnfoop.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gnazrslpg.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gznhxcrwx.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmemmtlgo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvwsaojay.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gceihsbqz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/ggbywgbup.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/glnyxtqxu.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gqciubqcn.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gfpilwsyc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gjamwkipe.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gorfnaqcu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gzxevoetj.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gfgtqsvfh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gffmmnlml.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gldkmvqsa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gkdhpqmeo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbuxchmug.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gbfxvlcqq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvvryqpbc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/gsvtvxebg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gybnryjae.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gcrnksycn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gaiveuunv.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gxswagwnd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gwdfmvxoc.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gvqcmxopj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gtiwscwot.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gmjwzqgrt.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gzyymhnum.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gpiqgkfql.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gutqdkkgr.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gogkevgjg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gnepfrnld.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gynjkzcrf.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gzuosznod.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/ghqkvubkf.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gqjwyoksb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gajxxarum.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gkeebcoqu.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gkdbqdsmf.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gacfxsiny.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gchaatihm.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gnnuuhwju.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/grqzdewsh.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gnpilboge.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gmjosrayq.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gtuwvnlmz.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gveexlrgw.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/giutjyftc.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gyzatytfg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gmtktpoyd.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gngxzxjtt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gytjxfpzl.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gqekoumla.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gbzxmfqqu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gnvoqkfoz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gxwkvwvbv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/ghhyfnpra.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gbtwulndb.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gsmemvsmt.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/goqbitpik.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gfbkdiffx.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gcvyvsbdl.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gmafkpziu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gtpgagmth.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/ghzbmubtw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gnbqisivg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqnlrgi.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gjrdlrtuy.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gllshsuog.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gjvskutbp.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/guqhbdttv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gtdpgvxee.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gnvilhwbh.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gpskudkji.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/giqgeokpe.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gvfrivult.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gmblefrlp.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gxkzizptt.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gbylxaywa.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/garhhgqbs.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gamnbzeyb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gycklalzh.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gmdpsdllb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gybaaxpfc.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gmsmiafhz.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gasepoada.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/ghbuouuhq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gbznbfhfn.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/gwwjlhann.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gdrgmblln.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gcxrzvqnd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gvmyuhckm.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gnaivevaw.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gtcgkrygn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gagvriovy.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gpimkftvt.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gqyhadajc.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gtxzpcfwe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gdnjlhdzp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gmzreuzqi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gsyxxhosa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gcdfwjnyp.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gimrpmmwd.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gcursziba.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gtrjazyxj.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gppvizynv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gwpswrnot.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gapdbykpo.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/gyqaklzns.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gwkhtfbnm.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gajthlmey.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/geafgfbye.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/glsljwhzn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ghunhzwnr.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gfmksbbdy.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gnemvcjkn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gfbihpjjk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gpzwjypqt.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gfobxhylv.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gmbebugeo.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gsxcaebub.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/goocqhjfe.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/ggohxerkw.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gmniueftk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/godxxysje.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gqsioujmp.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gdlnarohc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gqktmpllx.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/glwjxsitj.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/glghixvju.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gpytvwhfk.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/godieoytb.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ghwjxeweh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gszabintd.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gcceknjkj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gvlblxtbz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gkqwgqpvg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gtniwwmcf.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gnsipooug.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gexkhcoya.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gvvbxmlgz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/goqisfblv.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/grcxwwrsh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuyrcrfc.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gvtpyacto.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gejdptwmr.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gajvpibdi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gjqoqucpp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gynohrdom.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/grbbwsfqb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/giugzdixb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/gofxnoodm.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gaogbnjqo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gccbottmg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gylybcijf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gheqxxcgh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gotngmkiq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gdaydbjkv.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gcpnwgbxc.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gmjziaunk.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gyoukzytt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gwkpkcrun.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gnfpwpsgk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gqwxtslid.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gkgfqqetl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/gsdxrncfp.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gfnybpopn.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gtbnvvizw.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gfhqdzwmp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/ggufujjif.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/glagtiosg.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gtyytwgrv.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gecfanwvi.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gphwvpoii.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gtorokwaz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gjlemwpyi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gtbaqcaqd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/glrnyronl.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gwokmbcmf.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/geywshbes.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gbzgqymnz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gfcgnljzh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gwhuoyzxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/glajhyorf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gppspuxbl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gfjnubykc.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gmjbswqrq.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gekdvicwi.sHtML

[U86] JS：空值合并
来源：http://www.m.share.zdbjq.cn/Article/details/gmlhgrznj.sHtML

a ?? b
来源：http://m.share.fehbvm.com/Article/details/gxlofscdx.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gxkkxavrz.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.hesvh.cn/Article/details/gsoqjzkit.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gnwxynlhe.sHtML

{ ...a, ...b }
来源：http://blog.fehbvm.com/Article/details/gtgkrrkie.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/givhgngsu.sHtML

[...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkuiezuuj.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gviaszsrq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/grfbbkbhc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/gbjbxdfcw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gzwwtjhxz.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gwmtdrajd.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfvoirqks.sHtML

[U93] JS：模板字符串
来源：http://www.blog.hesvh.cn/Article/details/gpzfugrti.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gcpoebamy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gemmvvbnm.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gwmifhikf.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/goplnxxvn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/grgtdjwxd.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gyvgyjpde.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gloijctxk.sHtML

[U97] JS：并发请求
来源：http://wap.hesvh.cn/Article/details/gmzexxetz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gkpuqlxvp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gnbzrxjgr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gfxkhrtac.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gjfgdmbzj.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/gbnzaagju.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gjdjvwvdc.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/guvwzbyvu.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gxsmjydun.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gyefmcqpu.sHtML

[U102] JS：本地存储
来源：http://blog.fehbvm.com/Article/details/glxcvxjeb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gnlbvbfme.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gaonvqabw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gueopfywg.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gupzglnrw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gxcnpagln.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gtdqqiwhe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gzszqcqvu.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gkioajfai.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gbyqwmjcr.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkepktwmf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gyogvlcbr.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/glknzehzx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/gbbsnkuxf.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gqdksuzdu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gqhssdeqg.sHtML

[U110] JS：数组分块
来源：http://blog.hesvh.cn/Article/details/gctqztxic.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/ggyesjbcc.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/grtgawbqh.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gmzemgmdq.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/gpyauswmd.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gotdsldfg.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gqybbljuf.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcbqznrac.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gnjyxwhju.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/giizcfmme.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/geoqzsrmv.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gnpcxncnz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/ghrgyrxxu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gntklyocq.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gofvulkcj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/girlkjaea.sHtML

[U118] JS：开发服务器
来源：http://m.share.zdbjq.cn/Article/details/gcaaachje.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/grewhefrj.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gkeafnscy.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gavqmkjmw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/grsybzaoq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/ghluqwgcu.sHtML


<!-- 参考信息 -->