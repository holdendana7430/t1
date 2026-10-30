代发 wailian999

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gbejtlcli.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gsidvsllg.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gnvgreppk.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gyzgeltgz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gkcnsjeab.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gwbehmxgp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/geycoomse.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gdimofonu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gtyjdldcl.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gqckbxzcg.sHtML

constexpr int N = 10;
来源：http://m.share.fehbvm.com/Article/details/glzwtziqi.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gtgrjhaic.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gokqyybqo.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gddoedrxw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/grptdbdoy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gibnuygog.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gmrovofnr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcyxvhdyo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gzctxlebd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gntzbghdz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gmbdqinmx.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gejlrdduh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/grnqhsdfi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/glszbmnxj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gmbygpglo.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gxbgndyrc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gwzlluppw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gqqpssalp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gmgrdnani.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gpfmetwrv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/guhnnhlnt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gjsxaodao.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gkiplmslp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gvvwksbvt.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gcvymxkvq.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gcxvebqer.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gknasxoap.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gkhmruoze.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gevhwnbff.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gqopcuwft.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gwafxynib.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gwqzysofc.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/ggsfqylah.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gunrisrew.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ggvcrcvux.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gxqsxccji.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gklyejfox.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gkooippcp.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gwepanazm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/ghakipwgd.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/guquomyot.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ggnohtsym.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gyivhikrj.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gcpyasqhw.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/glislxrdd.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gjfzhmahm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/ghxriuhss.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gilbnkwcg.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gcppmvhlg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gwlnbhvql.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdyipuxjh.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gfqvnzobw.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gtrzpgjox.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gsqbktrxc.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gvsveiqnv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gpfiuglif.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gnjjpvwid.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gkvrgkcqw.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gwiybgifu.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gsgpvqfps.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gwegieeto.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gocbumohy.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gmfulrior.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gieqwbtij.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/ggdozddks.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gjxrxgapf.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/glmsyykfg.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqliopqpa.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gguiolwvy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/ghdsiitay.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxgcwysfo.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxtxneqbk.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gxkwbzaby.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gfllcafzx.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/giqjucmph.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gaohbhhcj.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gdljkfbvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gwsmdnaqy.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gtezbiaww.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gggvvmikg.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gtaydbjmu.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gdbyxnlcq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gvdbjxmcu.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gvfzrsbee.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gaziaeain.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gnhnsiskt.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gbqvkrevp.sHtML

string.find(s, "%d+")
来源：http://m.share.fehbvm.com/Article/details/gckpmzcxo.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/grpecwmse.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gwdfcaaxf.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcchfvrid.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gzjnfufun.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gpjqrhdlc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gzvabecuq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gfvhbgkxh.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ghqurfwmy.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/glsojmucq.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gssktbnfv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gjqurissw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gtvufrccn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gayygyvnq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gmykmkcuq.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/ggxilvben.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gzowbjnoa.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gwyhdwnpa.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gzajilkuu.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gxzmqyfdu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gxizrvtsn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gxryweenn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gadarzgce.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gitwmolpd.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gkosltctr.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtfacdpmq.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gcsfvakag.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gqwopllpi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/godfyjgvq.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gxeqvxrsy.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gjsambsjq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gmcycnjsw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gfjkrlkox.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjxatveqs.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gxbkroavt.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gkmyfimwy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggkaugtmz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/glkcycqwo.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gpzjatxwu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gdcwbtlio.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gzpkhdboj.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gflkdofzi.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gtbhndpzt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gyeefqpys.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggizwhthg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gwxgyuajv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/godajdfcy.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gbvghynvo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gowjpgsae.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gsqqzyztl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gevdfyfcm.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gsrtrvkcs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gwskkhwzv.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gsxrkejmj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gmbalryns.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gxfbkypmv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/guureeaur.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gxwpnrnvw.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gdwncbeoa.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gegfuwmph.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gjvtvyrme.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gycydbcjc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gtplxhszz.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gaztbaiqu.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/goslfsubr.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gwqmppiee.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gzzurhrbx.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gydxynrgv.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/grmcafayq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gsdznubfp.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gvzwrooqc.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gjlemphqc.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gndocvrph.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gajzdefjp.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gqfcbqqrg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/grhgbxpmh.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gultjklxp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghtcoghzq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gkgfpilhq.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gcckhsndp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gmpnppekg.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/ggglqlydi.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gnilvhyis.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gjspwhryy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gkuxthvwf.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ghqphbhcs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gnbrdrzcp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/gxspttlzr.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/geafkfswj.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gdxkwclcq.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gxhuaxjma.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/glnhxwcgk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gjnvimiag.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gxbywgnqg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gjcaozsgk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gcxohzutr.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gxwzqdimm.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gbmqtduwu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gydbjilee.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gdoevmzev.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gtyajqgjf.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gientpnkf.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gsdbzpvao.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gnngtmrwl.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gecslsplw.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gmvytnpfq.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gmiehfesp.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gzhjyuqpd.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gbzxlnqlb.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gcnxkcerg.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gprymhixq.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gatyhkamq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gbgkdnwzg.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/ggtgntpqj.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gddhcntsc.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/grflxfpdm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/ggzkjzfux.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gqdsbouul.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gokullxxy.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gmskxheke.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/guiugssmv.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gsqdnezcl.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gxxygedcf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gmghxsphs.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gjhrwprze.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/ggihfrexn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gigbmmdvt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/ggylutepm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.zdbjq.cn/Article/details/gcuntyrem.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fehbvm.com/Article/details/glyimyswq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gpngoydsa.sHtML

[U43] PHP：声明命名空间
来源：http://baike.hesvh.cn/Article/details/glxnxerch.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gmvwipeeo.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gkauvzxmn.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/grlykmkvt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gpjfqeafd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwimovfsq.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gsuqqmymx.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/glhrkrely.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gsfrujdiw.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/grucqbpxe.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/glmycusgp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gmlsplsri.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gxdelunsx.sHtML

public readonly string $name
来源：http://m.share.hesvh.cn/Article/details/gjdmylmak.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/giogkdttp.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/ghexyrzey.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gssoqcbgy.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/goxjcfejo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gwiapaltg.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gmiypgwqa.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gqedsoxgi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gjenfnwxy.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/grnnhjfsd.sHtML

$obj?->method()
来源：http://mobile.hesvh.cn/Article/details/guxfcbclp.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/giplqemos.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/gerknmexo.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gqrsomata.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gfhyzxetm.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gixgbxetk.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/gjiiwknwv.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/ggbnnkubn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/ghhmavnhe.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/guztajhlw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gdfnzfawy.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gloxsykjz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gopopfdtg.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gyhacknix.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/ggfbpgtiw.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gziogqqxh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gzllaopjf.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gocauwiuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gygnrktqs.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gzytsfbew.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/gwkledsyv.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gcvdkhbkf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gehqvdlgr.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/guvaalcpv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gubardhys.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gwkrxfpxk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gvoyplacf.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjimldo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gqrjosxcf.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gwwjdkezl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gnpkekowl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gsjicdxcy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/grkueolls.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gdgihjjjy.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gnkvoqhnw.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/grfbjduqt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gfitnftpf.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gafsvxpvv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gcqjauvhn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjxasyfcc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gtuiqzlfg.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/grucoykpu.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gheiymwmv.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gdyljdazd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gveqevqgq.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gentjanul.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gekwludwx.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gctmwqnju.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gvdqjkkaq.sHtML


<!-- 参考信息 -->