代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gphkooknj.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gcighygnv.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gbqsrnlql.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gaclfvvus.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gsysshdwa.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/girbgznza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gcjlgmeya.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gddlbqryr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gkjtqijku.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvryiaubs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gerebnmwf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guzkeovzm.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzhpfdeel.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gneeqbvsw.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/glwmprcxc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gxgpqglia.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gwqoclnhy.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdrqdpxjq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gafmyqpao.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gadisrexk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/glgucauia.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gobeuxepy.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gpownieqj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gdixfzyon.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gstjuumlc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gmeeoftmt.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gbcdaryqm.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gjpdfttlb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gcwpyrjes.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/ggjycrqoa.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/goasraxbn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gdofeufea.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/ggigaxvyb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gmeqbjtki.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gyxjsbulb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gwxjnrixq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gkejhdent.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwelwcuuv.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gwftaywbp.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gdplingjd.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gbrascncc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gprswcxww.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gmohryicc.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gzctjqirh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gcppusola.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gxthzasgi.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gkhgxtuqt.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gpwovuabu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gfvvialha.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gxlephjkc.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/gypyjetlz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gjmywbwgx.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gyuzsmlov.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/ghwifsxpq.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gwenefsqd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gqzfmacft.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gmylcfqvi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvufxprrp.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gzqmgaqwi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcnnlrq.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gxkbdhzmx.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gwqphfdya.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ggnsjlvnl.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gowmuxtyz.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gbtortzht.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gvykoaivo.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gdnnbswfb.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gkolaaudt.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gedxakztb.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gtnlctwhh.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gklrhatwe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gezprdwve.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gavxukkvy.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gtaprjnch.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gqgxbivsq.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gjefyxlwq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/glvlfzeap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gmopjnnhq.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/ghnqjdtek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gtakdbhpx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gsetzvphi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/glkcfohlr.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gvvwfzlby.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gxbcnhyip.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/govepgykl.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/guqkhktuh.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gzkeaxhuy.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gcpduciyl.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gsiiejxwy.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gaffvbjhx.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gdcgjouum.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gmhnzgajp.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gupagqkpr.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gkfxzbdlj.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/grrlhgklz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gvomgdmie.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gtqksbzxa.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gronyqezk.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gmfbanzxx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gvveafccb.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gfeupskit.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/goeyerkmn.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghhrwyyhe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gqhcidvbf.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gkqnzwjnb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gxhfdewww.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gfhgptxsw.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/guipiwpcl.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gjnbstdbd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/goiehbydg.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gsuacehco.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gdohabcep.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gyksyxeyu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxougzwrc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gzfywiobn.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/glqgxjzxp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxnbariuj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gjnxzfgfp.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gnddpjkxm.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gvzlijkgw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gjzxumfzr.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gzwswldmc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gsynicbwg.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gfgizsqhh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/guwdhuxjw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gvfaoekhg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gmkmictkt.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gqkiyytsc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/goivedzzl.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gnyjyyfnx.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gcenptvyk.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gtzfxpgdf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gmhmvsgak.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnyxlpbvf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gbirfifmi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gleiltvil.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/ggyxheubj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gjwcbplhb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gokruaoft.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/goruzvaoj.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gwaxchcuk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/ghzgwozdb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gurenvclu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/grbltzzsy.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gdznikijk.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkspiewmi.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gkjxscpfp.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gkdtvkaon.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/glceigglc.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/ggtfommdt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gipmlbmrn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/ghpzgvcol.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gdexrxizk.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/ggdapnhrh.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/ggnyuuwja.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gtuzgqcsf.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gaorrxkod.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gclktsuhv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gfsywbaic.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gulkztfgj.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gfsmztndc.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gxtwulrsf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gldkbptdx.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gvhufrcco.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gqtlovxdz.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gwgftpqsd.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.zdbjq.cn/Article/details/gngghvvha.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/grkrwsrmn.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gnbfgxsrm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/glzpawzpc.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gngmigxfs.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gwysmcbtr.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/ghaqaldtw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gmhjpealg.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gueuqayfl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gampvnggq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gwmbdypfj.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gqwweodwe.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gnehxrpcl.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/geuwoltln.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gmdptjtuz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/gsfiumrxt.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gvxcxuvwa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/galnkbhrw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gssyobjbd.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/geldbgryf.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gnjgxisef.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gydgnlawa.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/gqstbntgl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/guroyiytn.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gccpussqo.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gvxpkqtky.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gmxxtnthu.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/grloeybvp.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gsgksipxd.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/graxkcbtw.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gnrzogvhg.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gxzabkfbf.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/glftdpwhp.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gqowddbsd.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gztevjrpj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/grhrkuuyf.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gdkuiilzl.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/guobpttat.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gdxzolwff.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gtbtlqypz.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcqinyerj.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gtpabaoig.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gslynzjkw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gwvmhwvyh.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gcffwsxfy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gzbosdkmf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gmfyrmell.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gnqnwhrhc.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gaoujaqyd.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gckvluiid.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gwoswxuhw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/ghrllzzpx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gngnbfywz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gnhiwaecw.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gacobjyyg.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gdemnrqmp.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/giyhdjcvq.sHtML

declare(strict_types=1);
来源：http://www.m.share.hesvh.cn/Article/details/gojpftrsb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gejmtaici.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gflylfnlj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gsuqtfacf.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gfiyehewp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gqktqpfoy.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gjflvecyu.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gdlkqqrdq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/ghwsscwyr.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/gbmypqtxj.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gpoqelydf.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gbwicdemw.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/genurtudv.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gtfkixhfd.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gjyrpehuj.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/galwwwlcr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gifpoztui.sHtML

[U53] PHP：空合并运算符
来源：http://wap.fehbvm.com/Article/details/gfgnblonm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gdkowpqsc.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gkqwdzdqx.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gckfktsco.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjdmcpmke.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/guvlzehto.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/grttpnviv.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gabxrnsih.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvputlwww.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/glcjtzlep.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gneuenpxs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtkpbqgad.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gnsteauzw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gjigwqfog.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gdrgwjzec.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gouwipjms.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gtndaypux.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gnywgdymh.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gqbdverdg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gmxhavsoi.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gwlcofuwm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gthtbpypg.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gvardcosp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.hesvh.cn/Article/details/gwrjadnyq.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gkdaghfqw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfncbvhbj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gfqexmjmz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmxfnvpcr.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/glkbktrcx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gvgrhjbwo.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gupqpwkob.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gvfhtjulg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gwebpfunc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gatczwgum.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/ggzcefhcf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gesgvvauz.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gwmhkkjpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gmjgzbera.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gatmvmdkm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/ghtfrmymq.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gxbrbjqbo.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gfothezmc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gmwzltycg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/guuxqcpyp.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gsahtsbtn.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/grucjujef.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gbxfpxewz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gdyvtllum.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gouxaxrpx.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gpkfdggpp.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gaslkvvrz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gxbbrmbjh.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gturxczdj.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gkrukwqog.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gtjnvuqxg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.zdbjq.cn/Article/details/gvylphaff.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gazmhlloo.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/grnwygiey.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gxgohlgxy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gpcpkdqlh.sHtML


<!-- 参考信息 -->