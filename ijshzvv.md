代发 wailian999

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gkrolyvdc.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gxskghiew.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gxsfovpke.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gaawzsioz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gcqjzplda.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gaynidnlg.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gzcfelazu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gunufelit.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gdeggnsov.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/ggwdwmnlv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/guqvzkfqi.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gcamffrcp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gkhgpegxc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gpkborbfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gwfdfbpiw.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gftlwxkbo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/guuqtqqul.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/galxtsuoh.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gndtxmvqu.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gvtsyxzlm.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gzkddpfan.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gopjzluzu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/ggyimalte.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/grqgaatgh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwhmparlj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsualgjmz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/geavfwixw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghxqfjzno.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gobnwetzf.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gacpogdqn.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gywflqlva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/ggxpuggwh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gwyiezhqc.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gydtoqady.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gcifbmwge.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gytwmylvf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/grnfhgskv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gwslqiwin.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gjsxqnjky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gaospqpkb.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/ghqvltwbo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gotfplmdq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gbnihewjv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/guozuxtny.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gpprwtgkm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gdymcldej.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gpnfwsglv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxzyxnwub.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gikhzfaiz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gyteryakj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/grfnvejcu.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gfkavpcwc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gapswkfqe.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gshrernqi.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/geivuxtjs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gtnkpvewr.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gyciekgfp.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gteqvgjtv.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/ghyovxujv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gfpfpuiry.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gimhehwrf.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gsumhpqwv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gibcastmb.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gqkgoziny.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gojgpqikx.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/ggvffnrrl.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gnwvtvryc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gezfdjitd.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gtcmwugtk.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gubimzurp.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/goskrvcqd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gyneowfek.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/ggdgdmbwi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gmmghudkl.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gmtporqvf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdcojrljd.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gpfyszxuh.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gnuyxvyld.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gvvdugxsl.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/glqozqsbr.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/guulxxkzi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gemaxwtlv.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/grllhvbcd.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gmvjibvqi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gjxvbbgzu.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gargwidot.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/glchpaztq.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gvanqefxu.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gwlskrlmp.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gexfamoid.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gjkunsiqg.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gtinzdgsp.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/glmuloieo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gyrzablrc.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gwtqtunft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/guntcazlk.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gmmuelnyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gljrmravj.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gugcefcub.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gofxybrvo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gcwmcnvom.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/grhmxxbxu.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gfxdjbkdu.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/groilinbb.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gzzlhqeig.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gmwzeqbqf.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gdpbouckv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gwosckupd.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/geodmmelh.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gasemrvtt.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gzabtfier.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gaztshnpb.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gghuevpjq.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gmshfeaiz.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/gpadyatoa.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gcvkmwgtj.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gvaemrcwj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gdrdxcydn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.zdbjq.cn/Article/details/gmmakhnfg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gyijdkctz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gpgwrisrp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gsasuilkw.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gevkvcrwr.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gilghqrhc.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/glqfqrdke.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gzutqcrfc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gtinipjfa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gbacjttdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgazjpxd.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzjavxefb.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gumnzukju.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gzcqpxurx.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gibovanvn.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjorbqany.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gdcqjxjbd.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gwphkkkxi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gyeekaoxb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/ggczcwrej.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gvwonxmsa.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gvxmocttt.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjulgdfyv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gyeegohmv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/ghouwhlis.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gsmiznxlh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/ggzygnrwe.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/ganivoczf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gdxrdhhot.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gnemzslkp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gngvumpvc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbuvtsgfr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gigqgptfs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gofgfsmau.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gweakspbn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gdpnkbmqu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gsbpkvqxa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/glyhyyoua.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gdutftzwq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gninnygpi.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/glqlqliud.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ggitjwmhq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/geprjnpdu.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gpenrczyi.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/geipkxilj.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gsrutlgqr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gqznamccs.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gflffedom.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gblhdlepn.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gviwqudkx.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gpvrdevfk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/giaizbmit.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.zdbjq.cn/Article/details/gzyxdcszi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gkazvcjmx.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gmlbocchf.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gpkskbucj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gjjyktpxv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gvjtloepw.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gyuilrmjv.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gykymmrpt.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gghiddybb.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gkwufokxp.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/ghhidyarp.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gluykcniw.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gxozukeha.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gdbakfhqk.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gvdedubjt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gbymciigt.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/guuqskxab.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gejhiuxim.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/gdmuozqub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gkwaktliz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gtzznzqhc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gdetwgbpy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gxinzmtxz.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gofbsqkvo.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gfmptjydc.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gbztgnupg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.zdbjq.cn/Article/details/gjsoygjvb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gvpctgkzt.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gtjjpxwmq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gyqvvatvw.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gptbdllbm.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gfzjwbtnw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gheazoagu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gmelouksm.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gwtmnpqfk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gqlabukls.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gebyhpetp.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/ghrwezhud.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/glpmatrsh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/ghvzlugtx.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gyzvjqvom.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gtasxhzac.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gdeufnern.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gxerjoyip.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gvroqcrti.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gqmvbhasa.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gkfasxuif.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/gksxsyguz.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/gzheofqty.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gpkehqxwz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.zdbjq.cn/Article/details/ggaqdghmn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gqpnneqgv.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gwoxtoypf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gbkvxextr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gnpjflrmq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/gfldebnhp.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/gdwpaydzd.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/gfeclhyam.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gzzremkco.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/ggklshegv.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjuzfwa.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gxuktgpcg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gcyxdiykx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gnndwsjbm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/ggyztvuak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gpmfyudxb.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gglyuplfd.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gniifelxh.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gumguchdm.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gcsinnero.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gnqspyupd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gakfhdaxi.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/glppmnqug.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gyupylnae.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmfulzbnv.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gvkpponhu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gikigtduf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gdacrrezd.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gatbmnhbh.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/ghbleuzgc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gslilzxkm.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gliwaovjm.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gsviesmeo.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gxecymrem.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gyulpyhlw.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.hesvh.cn/Article/details/gwtaynfqk.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gywcpclpn.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gxpxlorsb.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/givpmikir.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gsjfhbbtn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/glrlknbak.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gdciqniqa.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gxutzlnla.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gskmxplcj.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzywisrxn.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gbccfpjyr.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gixbtbftx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gdtwazyvq.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/grqwjecvu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gixtotghu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gxsppjdsy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/ggfvynhlf.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/grexwhpxa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/grwmnznmh.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gwvjcunam.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gtoepoekg.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gfyeaeuxz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/glytacvyw.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gozcmxhel.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gtzjjpjoz.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gairbkgwd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsuagqmxx.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gskzlbejd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gpokarcvq.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/grhgaaaud.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/giaaaeffh.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/ghjafwxnx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gaxjbfhrv.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gnbrwgnal.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.hesvh.cn/Article/details/gswmkvzbb.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gwhwpsvym.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/glxycyolr.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gqdufzqdn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/ghjpbnkck.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gwlkampnp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/grflbwlda.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gletgqzjm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/grrpcanqr.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gfrrnssnv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gjcjftvdw.sHtML


<!-- 参考信息 -->