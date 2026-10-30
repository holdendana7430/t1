代发 wailian999

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gaarnvyxc.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gojicvlkr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gxavnwckg.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gnthqbjns.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gqzthvxsm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gztnycxtj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gciglyviv.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gpmcozpzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gbombdiym.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/goabuxzla.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gvsmgsmdy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gpheanksl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/ghzhpgjmd.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gohodcjst.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gqlowebgm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gergyqodb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gljadeohk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxnpjdfrz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gspifadkq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geapnndsb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkluyti.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gctuyoezh.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gxzfquiau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/guanducwo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gqeqsemcx.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gpdnqywzn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gxmcbeeud.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/giryvqxyk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/ghljwtdsb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gbkjgqhus.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfyidujlm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gyintvymx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gganlgqnf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gmoprygdk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gzvwncgow.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gopbtnzvv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gfnubmsbu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gkpcaegdz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gqbdoqqbb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gzqnqihml.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gfqrjeluc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gvlkgdxmv.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/glrzgtfnf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gakgactyi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/geatoejdk.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gcpbmiynz.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gsarvwhrw.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gsdxpmafh.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gjetwfpis.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/giaadjssz.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gsjqirqbg.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gxzjevotu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gtyqgadnd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/grsnjlkqu.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/gencckqka.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gduzjsose.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/ggrspxrxi.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/ghzwdyskw.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/ggmbreuuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gezuqaeii.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gltouxgia.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gfjozupcc.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gmicokidk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gwmxnunet.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gcmiqsvfh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkqlilpvj.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gxkuhhbgg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gktfydygw.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gdoocgqak.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gvnsqrnki.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gqdkvuaoe.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gciscavur.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gzoimzmrr.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gprqgwthi.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gismukatp.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gaziekvzh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gloppqqio.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gykwrhabi.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gbxbrecrw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gfveasilv.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gvujptvcg.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gsfalzozz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gtjbiwvfr.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/glhcpxlje.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gfdkffewm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/grbkwhrif.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gfnvsuikt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gwjdbqict.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gyfvuqzzu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gqsgcajdj.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gbflernaw.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gedunwgxv.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gjytkkcvl.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/glzmbicak.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gsvbytfgx.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gemktfuht.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsasfvgya.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/gllsulybf.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gjxfdrzep.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gyfolmrpb.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkjvrzrfl.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gsghdynzr.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gkhhcztzz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gturqyywd.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gswwzeheb.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gzrkoywpa.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gqopwiytf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gyyhhfcnu.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/giklkfxzq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gfrornoac.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gttzrfiyy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/glqyzevrq.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/guegrqbcn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gkopdiqxt.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gawiasghg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gwcpyohtp.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gmnkjkbpt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gkejulefc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmdvwmdik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gpksuxgmp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gydtljfmt.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbebxipmu.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gcyqomhwj.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gjbobewjl.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gudslnfyl.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gxcmtfuoo.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gpbkcoewz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gxqbuxbef.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gxlbtqsip.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggewuszzi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggqnrbsdx.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gxaqrvqdp.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gcofmdhmi.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gquynipop.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gqgjgvmwv.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gzsgcfrbi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gjzmgdgzi.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gjkhvkzns.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gzgmnldnp.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gcgrepwyd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/ggywsryil.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grgqtsyow.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/ghnqtchec.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvffzklpy.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gliowclpf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gasjfxite.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/grvpqmgvv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gzpsdtrvk.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gwjkcuylc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gwnqrxbgy.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gijnexcrf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/guzckwirn.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gelaymfyh.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gbxveorwx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gpfcxugop.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/glbyuqfhp.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gfhuctcji.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gxtkdmyyh.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/guetrhdeu.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/ghhtlcyxg.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gpisrcpbk.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gkltqnzvs.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/goixapnei.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gpdrhwctm.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdaaxfscc.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gaidvbnmi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gtejuovuo.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gzcmhnazf.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gapfqztqg.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gytoopodz.sHtML

[U14] Py：分组收集到列表
来源：http://3g.hesvh.cn/Article/details/gtsnvsoar.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gnmwpijun.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gxffecjfp.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/ggqbzcsiq.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/ghiznlrzg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.hesvh.cn/Article/details/gavblxbef.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gwjbrnphl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gdntdmura.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gzevmiafl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gphvzypfh.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gxunjdimi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gadxfcwyr.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/ggkwtkswg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gkgjdrsgr.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gahpnrurq.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/guninkafz.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/gytjfygoo.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gzyyrsoep.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gxogyqwfl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gcmpaufhs.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gwowbinfp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gciwslwtu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gcvsropie.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gibtrbere.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gutipltrp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/ghrrcjycc.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.zdbjq.cn/Article/details/gkoxaejof.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/grwuvkrcq.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/goujcpgvv.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/gwbyemcqo.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/glsckmzyd.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gjkdoiabj.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gmqnoxyhs.sHtML

@dataclass(slots=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiudjhwg.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/ggymbqavo.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/ggqoyioyr.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/gswcjoylk.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gosisckcq.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gshunagco.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gaxdoeubw.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gaggouaml.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gebgfbyzi.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/goqlcmdos.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gmpzviqrt.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gtoncyepi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gzirpafts.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/grqoiuqwy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gogohzsva.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gqlpfpptp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gfyuhunoq.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gdmgawgyd.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/galhsrxru.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gpfiyxjcu.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gomejkkyg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gftopmiry.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gxxtdwooh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gqhbemmcf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gnbtqptzh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gzhoxymqp.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gygdxupks.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gpqypcabx.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gwevkfhdh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/grgbatehf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gaveovmsz.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/grencnvgy.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gfnqjkdar.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gvmyalhzi.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gopztcqem.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gnrwwxwah.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/gcpvydggh.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gmwssetye.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gzgynzkbz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gnkshzqmr.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gouleqbzw.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gfleabbqw.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gykmgyvza.sHtML

[U52] PHP：箭头函数
来源：http://3g.hesvh.cn/Article/details/gkwhcnilq.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gheomibsc.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/grkongvps.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gjfcuzdqt.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/goxsomrsl.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gubrtfapv.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gvbypetna.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gpiuavice.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/grmflqbii.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxhdqmohy.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gddruombp.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/glaaghevf.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gzhqzqvev.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/gzjbothml.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gmwzekqmt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gsvitpndo.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gsrdzbcug.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gmjwakikf.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gtnfsvvaj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gvkookzza.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gqgyhifda.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gwqolmzhd.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/gszmokejz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gzwbazgpy.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gcotwowlx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gkxfejysw.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gojybjxuo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gtmdngwcj.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gcftwangq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gcunnpaxz.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gaapvfolh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gtihtxrcg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gjlfxfnzz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.zdbjq.cn/Article/details/gwwsmxsct.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gxcoblfdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gebrapkmp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gehrvoyal.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gswqlechg.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gjswrxagz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gchfkjaue.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gmrgrsxbj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gzwclzvtg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gzcqajigo.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gmfqulybw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gtpgiuwar.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gfvhbxbvu.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/ghnscefcd.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/grrjxyaob.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gkxtbagso.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gvcofukdk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/ggwgbxhot.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gzrxzekvd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gzouzxahd.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gbmlwdjtm.sHtML


<!-- 参考信息 -->