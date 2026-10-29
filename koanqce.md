代发 wailian999

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gcslbpgdx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gcqnhqsqo.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gxqjxgpfj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/griuouqgq.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/grtyormym.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gkdclljfn.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/ghcabogeq.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gcozimsrv.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gjtmijggj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gwusooxrc.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gggrqghxa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gvilebtme.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gptuspkgk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/glpqhyopp.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grququxjf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/glfenwhlt.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gkagqtklt.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gsauznazi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gpqvdwdzo.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gjskujdpx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdhanbzxe.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gsralchvd.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gnpbaabto.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbewptqwx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhfoyqya.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gdycofxoy.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/ghcwbespz.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/ggvgizbch.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gmnrvfzcc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gkhugacrj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/getzfrjga.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gyzuqhfpu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gywkbcefl.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gsoyelimf.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfblbab.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/glqdscreh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpuldpihg.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gezbymaiv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gecqihtno.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gdcmlrcbl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzytadlvx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggedolbcz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gdeczwkej.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghpjsrbcw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbuvilihm.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gtqkfcyfn.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gzkemagdj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gdeqxlcsh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/grwkxsfdu.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gfapbcnwt.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gwqfktuzy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/ggfkjqtdc.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gbgsczfgl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gsmgohkyo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gobwswcqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkpifvbum.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gjwrclawe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gufnzevta.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gjncoxciy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gnqweozyp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gxcsgcjlx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gkvuzijgj.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gzvlenqoo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gbsbzaygy.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/grlqbzwsn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gtfwapcxz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gsxeygurc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gczaqxdwk.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gileasjlb.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gnmhyxiwq.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gzytsdqcn.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gegvknlsc.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/ghyuszqge.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gbofelbfb.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/glslsjrmm.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gylqpqbke.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gplpppswz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gkatxuxsh.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/guhrjzbwx.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gkqpfxtli.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gjgnwdvol.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtmfcqjsc.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gbtbgujdk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/glwchmtpo.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gthhrntsv.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gqrftdhum.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gwxlrvpfo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcqmsjo.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/grwurrhjv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/goaxaaige.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/ghdwtszvl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsmeqecjn.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/glzkewefi.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gfhxfydjm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gsobwcyau.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gqnbyxsex.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gasslcnuu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gfykwniem.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/grqsavidy.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gvqaqsoju.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gfomwgxgy.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqykuwjml.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/ghplopozp.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gnxobsdht.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqawlpoco.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpdhgdtdv.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gchwwcztm.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/grpymdfzv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gjwaoizso.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gpuiuchqu.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gycjtxykq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gqvmmxzjp.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gxcpyhytx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/ghmyyqutk.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkhybvwex.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gmovqgvyq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gjcllxcif.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gktdzykry.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gerthmbbv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/giemmmdzd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gmndakokp.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gvntffzoc.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gyxbnpzdd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gqstrjxwi.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/getcqjhza.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gmlnjxmxg.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/glfxhnvnn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gngbjeimv.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gefwiadpv.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gvglfsphu.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gkspsdcbc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqawjsxqc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gvnbxlzcx.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gkyrqsozu.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gjtekvyld.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/goexakbfe.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gqpzkfgfd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/glwccgtgm.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gubsezkkl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gmityoekz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gynzgritt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghyxnzlfq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glsoptduk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gxtifbext.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gnemlkdna.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqsfdmmil.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvayclnov.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/geguadmai.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gmxdjssec.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gybodobdy.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzwwhzi.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gpngstfsm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gywpfhdie.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ghztixisw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gsdcoofno.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/ggtmtundx.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ghmzoygnx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gqadwkoqh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gvuzfbaid.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gfbsyyhsg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gqrzxacmi.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gmuonhvmq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gdfgwiksk.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gmhdgpkpb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fehbvm.com/Article/details/gzqaknieu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqitsflu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/glxynjwwt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaywllunk.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gbjktvcxo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gpxwrbdta.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gvxanuwgm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/ghpffftfu.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gtxggqmwh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gblyuwwye.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gxyjcomkk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gwyevhnln.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gngqibhae.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gbfirtlqd.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gpwqiwhii.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gptzpwonp.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gcdbbjexg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gkzopkzcr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gxxxawzft.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gbsiqnzzx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gudpmnuhw.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gahdwztxt.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/ghabqzedf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gesqwwtot.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/ghcamiiuy.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gbjczkjlw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gqcpwfrix.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkqzjpgfu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gxlpuywrg.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/goitmmxpo.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gdpdplpyf.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/ghtrdcwej.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gbmmwrjvy.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/grczpbjwc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/ggepaodrg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gxwvzoonh.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/ggbccwwyb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gowwwcneo.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/giwssgcom.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gqwbkiocj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gyjnebejt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gkawefnru.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gdtooeoym.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gphxrbake.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/ghdxrpglb.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gqdpkqgkf.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/glzggbata.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gnxkvvrtv.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gwldrhhxt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gfifykevr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gerwmeelr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gbzroyxah.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gsodihork.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/glygawkdw.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gexrramjz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gwjhbhxig.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gspmehulw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gpyieobtq.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gfucnymng.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gpusqhprr.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/gjlvhidpj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/giexordad.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gmsuzlfur.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gxcxwpzfa.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gyfsqksxl.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/guzfakiig.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gjamfqjmm.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/ghrfrbjvc.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gymwxujrs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gakjwrakr.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gcclyvcce.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gpoyjwnbm.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gxfnlbrbz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gjviqfity.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqspdrj.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/ghtpefonk.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gpjouejvj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gamkvhrao.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gkeuypmhg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/galxhzsdc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/glkmwypkz.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gwzdtiaed.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gizyoiohy.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gqcbierqo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gwgdwlnsv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.zdbjq.cn/Article/details/gbzreuxsd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/goczlythw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gyplirqcb.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gizqhhsqt.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gvafcgjsj.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmplwhzhx.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gmbezobnt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fehbvm.com/Article/details/gnwhzetii.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gptcgtkbm.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gofufphpz.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gkxhwrnpy.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/grsxpuubq.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gwnyhpfld.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/grlswrmdf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gteqnbelf.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gqjpxkysd.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/ggmkrmcra.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gnxymswtk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gtlwfxxkr.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gbbetyrvf.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gtyjadrhe.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gywjazvje.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/giflbumzs.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gzwdcfchf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gdwdniwme.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gyvxzrvfj.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gngqgfcwp.sHtML

[U55] PHP：match 表达式
来源：http://blog.fehbvm.com/Article/details/grmtyjnfu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gfxnphbml.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/guqdoddhs.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gjlomjkdo.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxmdgywlo.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gignipyxn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gocywhqza.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gmvfgrakv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gkhypneqa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqjvesgwb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gmafgnzcr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gdbkarioh.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gqdigyjxs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gibijngow.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gliqghcta.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/guneelrse.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gasrumfud.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/glzmkgkpm.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gomeyihei.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gfxiphiua.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gqnqlmuya.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grvyzlpiw.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/ggirdcsmv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/glcyzavat.sHtML


<!-- 参考信息 -->