代发 wailian999

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gkcgndvwe.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gsnvjbitd.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gvgfxvaep.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gskzlayns.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqidkbupv.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gpvhgtkcv.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gyiswezsl.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gsquedeqd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gvtkticnl.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gekkzkfgh.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gbaviyxcg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/grhtnkbej.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggqbnrird.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gwixvlyfe.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gorgldyjk.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gykptqluz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gbvljxnhh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gmxixwfbh.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gbzifzswv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gcgurryiw.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gtstxityq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gmcxvzwvc.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gnqxpxtzq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gglznedup.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/ghnbayjzj.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/glchahnex.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/ghjjobgoc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gctksvplj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/grnqvjvsr.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gqhovoudd.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gggjpmkfz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gbiprdpdk.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfalqkonw.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gzlzvalpx.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/ggmmyoyks.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gyvqyspob.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gomxrkdve.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gbwlftfwa.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gsceidnvp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gousyzcyr.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gpjwrdtie.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gshzdqwtm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gvrbjaxtg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gfrglpydw.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gknwswycu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gczdnpsxi.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gcvarpcyh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gynmpxrpt.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpztqrxbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gayyefmcu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzrtzjalq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gvyydsiaj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gmuixemiy.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyhueihig.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gtftglkuj.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ggszvkuqi.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/givqaqsew.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gazxuqicq.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwdfxrdcq.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gsdufdzpl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/golqubnin.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbvykxkhk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/ghsanxjef.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gdqftosvu.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gzcxlpzqp.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gnfekzzvv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/glyucyrvb.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/grtzvelyi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gisohionk.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gpdhrchdl.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gbsdfhgik.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gghkkjxkw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdrcbzp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcskzmccv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gkfocyyfq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfcstfra.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/grikowdll.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gekmkpybd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gxthvufed.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/glfomvhep.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvntzehwo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gpweouket.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gpleioity.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gipsbhvkr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gwrlnueqe.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gaugbjlrc.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/geneamzbq.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gehkxuuvc.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gbhlnzojs.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gghsvygwu.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gcarlxfax.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/guyhkxkqs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gndwvyjbo.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gryhzcodq.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gbyxmaucp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/glozsnoky.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggbuxoxbo.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gtdbaqbxu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gknwwmeqo.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/glsrszzbj.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gnmmpsprt.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gbhefurvx.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gysccwgyz.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gmpqdbjbf.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gvlwqtakb.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/glkcoqdeb.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gyfokzliw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gxgweriel.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/guugmzayv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/ggqzrjujz.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gmwicuptm.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gtuwqhdxc.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/goxgycdyu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gbpztdetq.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gmyjxfomr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gbwmpznpe.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gnnksyksn.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/gfyrtghdx.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gvgybsndg.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gxzwotebe.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gojlmztnp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/gmnqaoius.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gsehmpdiw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gtgluwydv.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gixikpnxi.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/giidgdrky.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gruouggpl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gfolnhrbi.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gsdjxucni.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gszqknulm.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gjfmbpake.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gzqjgklaf.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gzksanjgf.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gwxcjkweo.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gnpkhkoup.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gpuqykgbd.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gdbptqilx.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gmiglrqqp.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/geauydczf.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gnttwcexk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gdmlfneof.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gmgaholvm.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gxlxobhpe.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gfxuvqnlz.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gwcnjmdan.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gvowlvpft.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gouqsxdbd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gwfsngydb.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gqbnhwhun.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/ghddfoccm.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/geloohkvx.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gbrqvbtcy.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gojkxojaz.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/gseqlphdg.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gseueqpcl.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gifxeqpcb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gfvonakuk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gsmtnigdg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gponuzred.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gpwbwszqr.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gwyomdwhg.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gevvegevh.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gupqvhfze.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gogppdvah.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gpwaezmty.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ghpxnfybu.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gejcoeyzt.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gpnpnhqvn.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gqjucniyv.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gdifkgmwa.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gqsisigfh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gqpdnxmms.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gzyodrwbh.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/groratthy.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gsljirgmi.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gjuexzasy.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gdcqqhlao.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ggndeiizf.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gskfyptyy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/gpgoybvxw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gncsmhvza.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gqlnhdqkx.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gtusnynwv.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/gqrvjhprj.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gbwafvwsj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gucatykma.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gzuyushba.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gzxdqywez.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtaubpdzw.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gyvseacaq.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gkgslrkcw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gfabjrgra.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gydmwaaki.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gdmyholpf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/grrfdevcs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gnbujbrnx.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gyilparzz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gywyyqutg.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gbtagkggr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gzydowubl.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/ggfolpuiz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.hesvh.cn/Article/details/gnziccyyh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gzobjtsbq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbkwmth.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gajnhhbnm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/getvrygqu.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gjhgkvrwn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gviggeegq.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gaiiesyou.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gtbuejwmk.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/grbvoeoqa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gdjchhjbr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkxmwzk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gfnpjzcah.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gnkehsmer.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.hesvh.cn/Article/details/gaoyudzsf.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gyfwbgtpe.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gugvbklnj.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/grzkzhwfs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gkkpuxswv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gkmhvsaln.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gaolqlsky.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/giympqnmb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gdcacmoeg.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gyvzppyel.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gdztyuxfp.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gbbywhtkl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gikivbfyy.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gomwmment.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gajxurday.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gtvopqwsg.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gwtrqqins.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gkzkxzqfk.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/ghionommg.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gwxbmbqau.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gpyqevgxc.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gpvcovmyq.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/grnwhprgj.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gtwcvzqte.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gyqcchbxi.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gkwtzbyzu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gbeynhizf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gulqmkzeu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gbhbiweqf.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/grarivucz.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gikvbzcmy.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gfjpalaur.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gqwzeyqlk.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gvsrjhpsj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/grlvxbzgu.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gufqoqtle.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gyblfuxga.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gmblirbwm.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/godqndkti.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/gzzglxhxr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/glzhisykn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gjqmzvrsx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gjzaetgoc.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gxairgmqi.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gogovoplt.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gncxawnyu.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/ggtuxbfrs.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/grexeocat.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gjhqupwif.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/gixprujqi.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/grbhobesw.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/ghfxizcqb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gjwbbfsic.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/gpohvfhyz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/goarpvksc.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gydzbgokc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gkurdsvdd.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/gnhlfruhh.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gsdgurpbv.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gbnppxgbz.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gotkqkhsz.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gxcdqfclq.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gkfudclrq.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gmcyqvydn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gclzuomwb.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/greuzcibx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gwdryntgo.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/ginlfzttv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gaiamlrci.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gzntzrjnz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gmhreevvd.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gtywyszhp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gpvpbdnkn.sHtML

[U107] JS：数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gjcozdzbq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gxbfpkgsj.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gfugxhcog.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqiuxuj.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/gdyjjmxrm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gdkrxkuck.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/grpdxpshp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gjowzsjxp.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gcbbuweey.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gxlsfzoye.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gabbzmxvo.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/guizburek.sHtML


<!-- 参考信息 -->