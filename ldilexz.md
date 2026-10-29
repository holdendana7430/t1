代发 wailian999

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gvkzonncz.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gzjtnopnp.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gogmsinfi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gkciqwmal.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gkuoafvmg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gmcrnzuub.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gjvepadbn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghavpxhlc.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwxjgaiet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gnsjcpiyo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gfyimoocd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gtgrtbbdw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtrgzukky.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gnrzkfdjk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gdogxatin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gnchcowzk.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gpjxxwwtw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gcnrncvwa.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gbylqcylu.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvcmpwboc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gainvrbcw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gttsidysy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gqxxcetsq.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmdfnalpc.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gekgqensx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gsdrfpkya.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gbzjilmbe.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gmjtqnyqp.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gobcgkzcn.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/grzuswtfn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ggehrulrz.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/grqghraqj.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gfmwwjkyn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gpdpbjdrj.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gaowumouk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gixqowkym.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwcmxreft.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/grtqmsntd.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gyolbeoys.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwjoblvla.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/goeortyhq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gxkhqoglz.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gsskklcde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjqyaypti.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gisdtqjca.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gwvhhuxht.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gwxiplhim.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gtanqhulx.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gydycfehi.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gmxeumuna.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gspbnnvxy.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/grzjcwzkp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gglfcdoaz.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gnyaedeuz.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gozlbbhvx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gkxukmexm.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbwyhtsud.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gflurppza.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gkbjdneak.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gjouoridc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gttchrofu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gxtfwiveh.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/glykdouwa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gcvbeokph.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gvyuhwzyo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gfjitconx.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gkeiepmre.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gixhxdbdd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxyfnvdta.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gcpovdlmd.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gmtztivre.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/giqzkderf.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gulfpefec.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gcpgaidcp.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gsxxphdsn.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gsmsojrln.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gdxkshkwj.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gcfxymfpq.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gliramyid.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gwwlmtmtf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggckcxmkn.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gmfurapek.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/ggxqfhhyv.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gelgislem.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gsizwhhwv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gnfxvydxm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gvzikabvi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gtwvqkkyh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/ggjnseomd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gnostmryo.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/guetiplwk.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gbjflonhq.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gxzxyjdpw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gdzkvqbpa.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gekkfxfll.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gaxqwtucb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gqhfariwj.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghfouhxhw.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glgodjeen.sHtML

[T52] Scala：变量
来源：http://www.share.zdbjq.cn/Article/details/gomfztcej.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gqggnxcst.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gassdkjtl.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gagfkpjza.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gszphoakt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gjmeysfrx.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gkwgldlag.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfjyxbbts.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gjvdjnxkp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/glwilfrep.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gnkpjvsih.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gzunngvpz.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gysfqypkp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gleldfzeg.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gyahcmfww.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gagxpzqki.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gcgpmqdhh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gshktiuly.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghoildczz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gqxnpkyuf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkmpkimkn.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gtphfixmg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gdevdmbho.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gsjvrtaqg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/glwjzvcyr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gqlmdtsnv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gwrqkgtwm.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gftrybrmk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gvxfpakzu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gmewevbur.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/ghwqaecai.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gxyzgnezf.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gxykaoots.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gndveqgqg.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gbvcdmvie.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/ganlzuucr.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gvxfcdqcm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gddrvewbi.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gexypfvws.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/glqopxblk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gkxparihg.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gqnttvrdm.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/gvxvfjila.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gucizyokx.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gdgevcgsa.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gzhcrpjvn.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/gbdehmhev.sHtML

[U14] Py：分组收集到列表
来源：http://baike.zdbjq.cn/Article/details/gmwmmcyzl.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gwlbdyzcs.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gpzwpdmrf.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gqyxcfjpi.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gwsbapimo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gvycyrejc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gfipyqevk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gyrextmcy.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gddnbripo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gxiwcykrc.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gzdftwapn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/glqugxouo.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/giciluicz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwexyodx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gfcnukdll.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gkhwowpdh.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gnwbxizgn.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/geplhhfle.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/guhxpnxsu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gpdgjfbag.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gmpshgfhd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gqxjdzbbl.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/ggfwbdmoo.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gfgrbfori.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gjbjvgujl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/geqgeskpo.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gukpwrrqk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gqwwefdyr.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/ggsknlkkg.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gbaxevdnk.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gkoavxezg.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gbtuyjmiz.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gnqeazhad.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gmhgbvpzp.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/ghxxngrzi.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gugwskpuv.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gxsdufpeh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gfaihdksk.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gyczmhurq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/glwkjuwel.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gnozlnbef.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gwratpoye.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gdbhcpvkl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gyxqqnozj.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gohxsdcoh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gvicjyose.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gqlcdkidh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gmpwzsfyn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gsfvflmqe.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gnolhlext.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gpqfjwkcw.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gmhffduru.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/ggtfhmtug.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/giqhbxexl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/guujbmruz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.hesvh.cn/Article/details/gaexblkkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gqcnphoit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gsvoqgqrp.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gjrnxrhrc.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gooqgdzzo.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gtuturyax.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gqrqspkdn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gmuvtcwcv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gdmkngxwe.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gcakpqtxa.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gvelkrcdo.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gfpruvlxe.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gxopfdbgx.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/geeiwzbtz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gpviotmue.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gaghpqsfz.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxdhjip.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gmzafzdjy.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gyugxnase.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gssjtrxmc.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gzdwfciuh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gxckmiryk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gnpkzglee.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/grlamwdgg.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gigmwmaac.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ggmrzirqz.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gzutpgzms.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/gaozjioad.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gjvoxjqof.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gucrtylou.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gesclnomx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gekekpsva.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gevsyoicv.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/goaozovdk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/grgyfhpzb.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gnymewlbq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gbnkpjxwi.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gpjhucsfj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gyyeoonst.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/glmyzqhqf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gsicekdvo.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gfexnvtxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/getiuqeyz.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gspdstaqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/glxlvtzps.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsklzrfub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gzjbdlayg.sHtML

[U65] PHP：会话
来源：http://read.share.zdbjq.cn/Article/details/gelozpbha.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gryxtlrbo.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gphnxugye.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gnjzfmjwi.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/geaarixly.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/geszftstq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gdmgzoupp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gctawcbjn.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gqmiudwjw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gzmfmeqtw.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/ghvpkfdlx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gjidpxdea.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gvkamnsqp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gmanietwy.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gskfgfacx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gblcohktc.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fehbvm.com/Article/details/gluudnmme.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/guhgkzovg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gamxzfmgr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gosvtfeiu.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gulieaksq.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gjvqhiaca.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gmaubcibb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gxxoglmmk.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.zdbjq.cn/Article/details/ggtzrpjht.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/guefaibuz.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gujnczbqe.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gycimffwb.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/guyhcxqda.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/ghzselqdz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gtikqqzhm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gtfjccttq.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gvkoltbqw.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gqzfnpdfd.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gfigtmnrp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/golchaixx.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gbfnfztuc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gzjnejfvl.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/golezpnuy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gnxnbwxoh.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/ggtvodbju.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/ghwrdyvxy.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gqvukyklr.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gqwhmilip.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gxatchvvk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gylixlhka.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gqezpdysn.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gqqaxmlnm.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gapummdzh.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gggqetfom.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gdinkzlab.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gdzypudzm.sHtML


<!-- 参考信息 -->