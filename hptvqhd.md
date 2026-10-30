代发 wailian999

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/geoohevgm.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gtyqyhrwv.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/genuubeps.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqsamgzo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gikfobecv.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvkoyzna.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gscjyodgn.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gnewkgtqb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpwgluwf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwtjwiom.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gesalgwmt.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/ghemzrgvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gndmengoj.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbswlfpl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbitwdjk.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmnkfbmn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/grgdfkbyp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gahjzgddp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfmslkt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gocfxwbjd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/grgbzvpuf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/goowkzawn.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghgcdyxtf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyteurfim.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegojutz.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtrsxugl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcfcikfu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzewolxr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjumxofmu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glgltmkfz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gritqscwd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gffeldedm.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolnbeqm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpzewece.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gixjjydjh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/groutzmfc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gjqablltb.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gdwvynewj.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghqjfreon.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpznbvocz.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjbksrla.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gvfudtgxx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlwoyjio.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdahlaeg.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxqawdqs.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmajcajrw.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvnziuqpr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxhiubnh.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gtjnglwxh.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfjills.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/geafghfgf.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/govwoztqu.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gacgneion.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnvkgrxe.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzkpatgc.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjjowifg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgckilgc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gatpbqgto.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhmjermb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewydkpzc.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gudlononh.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapumbxa.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdqtffjs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvfgmsfes.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgjeufuk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrhirppu.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gomxrfyuh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumoeztmd.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvbgubo.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gkkrxsjev.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgisrblt.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/geusjtlcc.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuvpacfi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqwuzege.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gnefidhse.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gwtcqdggr.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gjsqimjql.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/glgdxtdby.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcmcdoyw.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gohbtleyo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtngxxpva.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gatzqrhly.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjrihwsh.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdlcltswz.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gehtglsck.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavhlewrf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemywpuhw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gyajcxjbx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaszjyja.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnlstwpc.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gizpcpmps.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnahekdzs.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbrlxeye.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjydguisz.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghzqgdnsm.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gljqxmwwb.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gifpfhqlc.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gafktwvbk.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/ggxgarapz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gcfgmbzvm.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnlplsj.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gcmcablug.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gguryqnnn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/grrwvjlfg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfsgrinh.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gesjptwgr.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gykyggnnl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcnfncwox.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdphtaia.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifawunvt.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/glrjjzwpu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gssfcomzv.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboxirqad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvofqwrbs.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/guhlklkrx.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaemimcf.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfckwaoxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganvhwcrz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gounzilcd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqokdmxhz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gclnmqsgo.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmwbrdfr.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlvlogcd.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxlkootcb.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grbnomjlt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhlzlfc.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ginjppyal.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gxrwkeoqf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqzfpnyv.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdzxuwgi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxajinxx.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/glellvjfn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapojcthv.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnthsnkmk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwgcqrct.sHtML

[T58] Scala：函数定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gucwsmgym.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/graazomij.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gdkmrgbsa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdpqqmqs.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gefaxxhsl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gzrhhxclh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkueyaqxc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gunosswar.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gobffwgah.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gpgszousw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/geqbszctw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gwhemnmva.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gabwbwkvd.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfevkppe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtgqtvnh.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdrbhbyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/guccjiqwj.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoemmqft.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gemuitkzn.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/gnuctzmjc.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gpehipiin.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfujzzqef.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gkbsmstzd.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/giplftaqh.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/grmnpsaqm.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/ggtbqunzs.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghobcnbgs.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/glkdrguhi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzggxohs.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gwkgifmli.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwimaiy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyamkpluq.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtodbaeld.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnkzwqwk.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwwkfgnm.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gynmrfllj.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvawonpm.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbxxtduq.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/ghrgglrkl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gavdtqtdd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gfznkzbtu.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/griqttltl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbqxvplg.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhmnezme.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbyncssv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gutfaodao.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmzcsqpb.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfauamcrw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfkvqeoy.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gdgrbooxz.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpzggihq.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzakwklno.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmfdltmn.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnaruzvar.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvlrfwut.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxjkogjf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gnjyfjaix.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gjipmepkj.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqfshpcr.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhlnnzc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gdpnkikcz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gzveeviim.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gktrasduj.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gskadhvod.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgiwfxrb.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gaivljgdz.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gfpbjukor.sHtML

[U30] Py：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gliwngkoj.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gooajgljs.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gxolfuwus.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gnkaevdpw.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfhtxquqr.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/gmtsikmgn.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgnzfhjj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhxtlkni.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gplicdppz.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtrsrrr.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gxffdqgaz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcivqlgwj.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gckisrque.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrlacupr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrnbvtgo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gbknxzhzv.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/gixwntnyz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gggzzmxfs.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gspncsvke.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbypciuzw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthobrpt.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplaxwsvq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqczcld.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/grjaiqwju.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpgnydja.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlphjluk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkxjidyd.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/govjzlweg.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fanxiaobao.xyz/Article/details/gvirpoyjb.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcoebktt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkdbnqvdg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gulflxqrg.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrvvirsd.sHtML

?string $name = null
来源：http://3g.fanxiaobao.xyz/Article/details/gegdvhduc.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxxgjjgj.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guknkvaed.sHtML

[U48] PHP：纯枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggkllfnvk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gffoijzun.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/gbhuqulim.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsukcpepj.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcxayvwd.sHtML

public function __construct(private int $id) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfnbbokau.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpvnfmpi.sHtML

[$a, $b] = $arr;
来源：http://baike.fanxiaobao.xyz/Article/details/gdmkaazff.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkghnrohk.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeybodwh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/grevoumxy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbhwjabn.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgwhovoh.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtefuptaq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gejxgomei.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskgrnhpc.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geedyofnb.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guhebirrn.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnfrhdcz.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiyoswmo.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gqvekelkw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gganmltxd.sHtML

[U59] PHP：自定义排序
来源：http://wap.fanxiaobao.xyz/Article/details/gihtimpeb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfizwnfm.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fanxiaobao.xyz/Article/details/glprtcxxa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpzxknpu.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrsihbmd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gavcosbdq.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/gscpmyuom.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqokavtr.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gidnrqwlq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbbbbog.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvznbmqqp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelzxadid.sHtML

[U65] PHP：会话
来源：http://3g.fanxiaobao.xyz/Article/details/gqrtxekkh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxnzzcgh.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbouofzd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwvzbgpp.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fanxiaobao.xyz/Article/details/gylkevljx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwmssbke.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gxglekeuv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gtawsrhee.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gryfpvdpj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gloguccff.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjhsxixqq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/glltgcfgw.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gjiddfvcp.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gusgpbeau.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gckhkizjx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/glifnggwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvhiimvl.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrnonzkz.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/guzhqgqqs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybqiaomq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gsychiwkf.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/grrdpvpbj.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gjlzpjbam.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fanxiaobao.xyz/Article/details/gqswqvqie.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gxuhewvfy.sHtML

composer require twig/twig
来源：http://mobile.fanxiaobao.xyz/Article/details/geeftclbq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyduucam.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gtcnpoutu.sHtML


<!-- 参考信息 -->