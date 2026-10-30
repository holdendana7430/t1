代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkshdujjh.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfdvrqvjn.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnsanpwdq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gcguroeyx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiitbnas.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gvofemxmx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzbkcfs.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdbpnyige.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/ghqkjqtcz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvjlrqme.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqudanbo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcijajmg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvejgbakt.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/genmkusjb.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjsaveksz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gswtjfzts.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkmyykxkm.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gguclpnrt.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gdluqohsj.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbubhhdw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjgexstlx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfqqqhpg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/govsavukk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gezlhwlug.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpghodn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdozrbdf.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/ghchoomjf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gezfodtdn.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giaigsfcl.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gavrtscsl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgccqlgq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlmgood.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdvdzubx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gdyozawqx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gjbyvlefu.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeirsyzx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpolwamk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/glrpxfdjs.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnybniz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmlefvrf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guexaufdc.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvayhoqyl.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtvaquizy.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/glorlnddr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuwrzuej.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggceboyrx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpttjhvc.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/grwvcjaym.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnstbagzc.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvqjdew.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfyobntp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gbhkipupf.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gzowyifdc.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdszopgs.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/glcwuuckp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnkmypmyv.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpwducvd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvffstlae.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gzvrkyyil.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxkimws.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gdejnumfp.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbskdqfz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnibhhuj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkdwguke.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/galpzarpl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrixrvrs.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/guyrxafuo.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmmtzfxk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdomjgvl.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gtvdwicba.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzbwziha.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gkqlwzzjs.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdxqpggx.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gracsfypo.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gahbrjwpr.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gyullqzzz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldzfppnp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsbdjuwk.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gvqqilvrc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrqpmcwb.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gfnmnimuo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gamtdldgk.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfarvhegk.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gsmiyukwo.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gtykihowf.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtriccoc.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfenkwsm.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gtvvgmmgv.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsbfpivxb.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/glkiwclvc.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/golnadyuq.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/goljrcgei.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifknzzgk.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gstdgqraz.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdazrlpuk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrqtvqub.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqxkfzmq.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyewdinzc.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grnlygohx.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmwjqsnow.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geikcyrzw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftbxwket.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/gzvmkhiee.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxvnxjgl.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxketnhs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gokawuzcd.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/giledrlhm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaregfdg.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgpxwxny.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfxgnwcw.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfewkcdp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gugthqzok.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzfxflmm.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtrrjwiu.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gukizhyxa.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcazpkmtb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glsbxgprn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/grjivkkdc.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gsbrngona.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnwshnvt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaxicasr.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/giwnozjwk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gvygvumnb.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gumuazydi.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gpyaayqhb.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnoiscfsf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdbyemta.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/grribzply.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheypqjks.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzancmnpl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqndmqcf.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gubquizrw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqalipods.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvffobsjz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxvflnue.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqhoeowy.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/glkiudhtk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gdycrnabl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/grfzxpmbh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqdfbblu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gthakdicn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrjbfsjp.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gigopxokc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/grxkxmdin.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gljqbgibi.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gumhrlyan.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gonnmxgrb.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvvypyk.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/goifdskvd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfkgwcxo.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwkuykau.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjuuvke.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/guryniwlq.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gmatdwiak.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gwatmgzmf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcvsrkpc.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gnqumwadi.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcipxdmln.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqsqzepy.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gfyzabznz.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqglqgiiy.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmlhdyvw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgnrkjja.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzngnore.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/grhwfhvhc.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genuxqzkl.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyakkwan.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbxfzgnl.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gazkpewrd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gulaknajd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/goxzjgebq.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gamlbboaw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqhhlsln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gujmzdceh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/glmxkyllh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gblfqbbqd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzefbcco.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhqptpnc.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpubosplo.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gntpetyub.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwyeiaats.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/glmazmpuy.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/grvioyanp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjnaffde.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjdbpknn.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnaatytv.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxafrycy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbbxfzvl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwubfvgz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqihwnbzs.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopxjqxmk.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gaaomvcox.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqoawwnx.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/grazgojjt.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtnxgpoe.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gsltkjjoq.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gcqxipuqj.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/goybpmpqq.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuuseitt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gihaicepn.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbzmvrwz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gymvqabvf.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoihxvof.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcgfzrpb.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvernfgq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyhknyoy.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbwgjvyb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktaslhxz.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnhpvend.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqphwnzt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/ggggptydh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyxuzocf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihprkbhu.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gfztgxsio.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gufylqwxi.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/grpneasuc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnwgxig.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gasjqqohu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fanxiaobao.xyz/Article/details/ggswwoanw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grenxfnyv.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwdmvyhb.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/ghlmkupwt.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghorpzhze.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gttcplvhe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gebuchrct.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipzmbtli.sHtML

[U46] PHP：可空类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxuhooibt.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gghrspwhc.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/guipesyde.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/gkjmxiutu.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqsrkefhx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltqmhtdx.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxdsawjl.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gqrntaavp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gzycivwah.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gszdrhuua.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/gxwvxmyud.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gremolele.sHtML

[U52] PHP：箭头函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvocwht.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkghhtykd.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcncrceu.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/glnlaawoe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmneirpar.sHtML

$obj?->method()
来源：http://blog.fanxiaobao.xyz/Article/details/gvbkrybhx.sHtML

[U55] PHP：match 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwzkvtcmm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcojmnss.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gbnmmrzet.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfveupksg.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gqxygnooy.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjehfayi.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/godxaoeek.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ggajqtgoz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwvfrmbr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gcfhxumbb.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fanxiaobao.xyz/Article/details/gvbtjicsb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gshdazooz.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/gjrbezbbb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gyjbgziqi.sHtML

[U62] PHP：日期对象
来源：http://wap.fanxiaobao.xyz/Article/details/gkmwvzhkr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcpwepjo.sHtML

[U63] PHP：文件读写
来源：http://baike.fanxiaobao.xyz/Article/details/gtogjjarq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgaryeks.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbekqxbm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigcvekkj.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gtwxqbxqv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gztlhvsag.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdavdoomy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gdktvsqkt.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fanxiaobao.xyz/Article/details/gumshyeay.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fanxiaobao.xyz/Article/details/garrrsqfg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxxpswfs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjfdkfce.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfkzmnw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmeuodztq.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmpoiwvdf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvopkoyz.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/guibtfyyv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdqebqmn.sHtML

[U72] PHP：写错误日志
来源：http://blog.fanxiaobao.xyz/Article/details/gmccclptz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqxsqug.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gvxaqrwkw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxntuwqud.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbmocllhd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fanxiaobao.xyz/Article/details/gnmjqqdic.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gcvselnbi.sHtML

composer require psr/container
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadyewwux.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gilqfvtcd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gdpprxcgw.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/glewtgpnc.sHtML

composer require twig/twig
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxndxcou.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgjbaygc.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiuullci.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gpslgoigm.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fanxiaobao.xyz/Article/details/gqludwidw.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/ghitalswa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gklpxhbis.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gcdwwknhv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzinqczx.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gmlqezyvo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaabeibm.sHtML


<!-- 参考信息 -->