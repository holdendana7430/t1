代发 wailian999

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gzcohsaqr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gnegesryb.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/ggptvyzjl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gelxccdap.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gguliyrcl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gqxcjugwi.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gpdhhhzyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/goowuymhq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.zdbjq.cn/Article/details/gkublndvt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gbhqfihaq.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gwbahibcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gufkolqae.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/guzkkqgpr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/geawoxtlu.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/geqawaaga.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gtphjddeg.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/ghdezvttj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gwsqufmxm.sHtML

[S46] C++：函数模板
来源：http://www.blog.hesvh.cn/Article/details/ghwsklxuq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjxckkoda.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gfdrxwscr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gvrqiiwqi.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gextjtwqd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gcknrsrhy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gxxcxpeyg.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gpiwijakc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gnxxblmpo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gwbitqvsi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsajakttw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gcxdcxgaf.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gsfyxeqkg.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gwmtyuwqa.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/guzpzrpbe.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gniwvdioj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gtwlbmqfh.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/ghyawwfhk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gfiuictux.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gsqgebfdq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/glefwetbm.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/guictwwve.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gpkhxcoys.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/ggktclajb.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gythgyxtx.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gytdrlczi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gutyqhegb.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/ghoszeten.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gmgqnyffg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gfrjnpzbk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gjgghqlgs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsjjibdrz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gwbadhysp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghjvkfxdm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnnokqpyo.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqzwfhsmm.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtezykw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gbgjjyaqp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/ggegbnvwj.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gbfjpfafv.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gezmwpctt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gygcfbixm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gnhmcxlyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gjoupflqn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gvagmjfau.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxaapfvyw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gfrpuoube.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/geoeoordz.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gvimrkcnt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gottuqmfe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvcdankks.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gwwprngdz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gnfxhppna.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gttrdxcge.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/geqfiblvs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gcuaihdsk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gvlitjxdz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gbsekzdhp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gurjmzjgc.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gvpkktvnb.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/glyyffunc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gtmlsyfnd.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gzaxvhsvm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gfuaneiet.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gavsckwbr.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzvwzeoym.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gwwzkamjm.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gaadjdclj.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnzxixlag.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gxnlvvtuq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/ghcdnveur.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gklufagad.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gidakpxyj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjlejvrd.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gspphegra.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gshcuydrj.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gpgqvornz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gczrusypb.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gvmksvfat.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/grdrlotxa.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gktqkpkxt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnchhnvmd.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gxxiowteg.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gwovazllm.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gekjiycrf.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gtloopugm.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/ganakvyya.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gnrsboetp.sHtML

[T28] Swift：枚举
来源：http://3g.fehbvm.com/Article/details/gzeuyzqiy.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gyyjtqtna.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gkmakdfly.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gqunfezad.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gflxzhurk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gsqxtfapl.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gavthsrro.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gntolywmf.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/glpsemghb.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gtispjfxr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gipgxwuvk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gvpakijfi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gxbgdfcok.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gzzyibwai.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/gkepuighw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gmwhfbdqi.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/ghpxjhnxk.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gbcqxjudg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gdfgfwccr.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gborxsewp.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gblfxckuo.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gusglvnbw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtkzgekdv.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gadewwauk.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gzopnrqrv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.zdbjq.cn/Article/details/gmgwopidq.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbvvpicfd.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gviujpmbi.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gcwrjvuwt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gyydgfjwi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/glhgzacwf.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/ggkafkkpx.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gacmptkxk.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gzrnbjopo.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gwqlpqgxe.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gzgrporko.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gaxeytleh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gmhqkslil.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gbdiuhfgz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gvdfmkgxk.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gbvfuumpy.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/grxfccqxg.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gwdxouqma.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/ghitxifqy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdqvqpcdu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gaupnppcb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gafbefngx.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gocywdbmg.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gpgeixmxt.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gukvzzepl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpucdihuv.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gyysepwsq.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gfrrzrzal.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gyluyzcmj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gaeryntso.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/ggldsnlnc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gfjwqeerb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/glnlfkrml.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gkxynskdh.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfonczbbj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gsfpimkqi.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gniuawcym.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gimzcxgcn.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gmtptvfak.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fehbvm.com/Article/details/grmxnrstz.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gptzdgwht.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gdsrczhaa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzvyldbvu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gdetrbkgy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gydgshrcx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/grxwvtmke.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gitquokin.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gsxxzraog.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gfscrstcf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gwdajakns.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gfhxnbxjf.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/ghgzsuaby.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gjpjogolj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gwlufnpec.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/geupieyln.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gdoifnscm.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gyeutxwxn.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gucwwmqct.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gyscepbob.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gubxoythq.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gzdveallx.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gjjngfesn.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/giqnczqoi.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gupndkyku.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gypxtsoqp.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gbirdmogp.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/glfqthzcv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/givojfblt.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/ghquevxal.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/geawarywx.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gmppurkvi.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gathqvlbo.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gdeqdzoyq.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gvqorrntq.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/guxkqmlaa.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gcobctkfm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gqocaxmxi.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gubhvyopz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gfqqjaupj.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/ghrezvetu.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gkebzkjcb.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/glhwuzlju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/glvosksja.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gvluqhlkb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/grmsocjkg.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/geyvohlog.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/guofjwfvh.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gpfcjyqzt.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghlfoaykz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/guqrrbbvz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gmtqehdwf.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gvirkpxnp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gfxooqxef.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/glvxehkeq.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gsneqrown.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/ghlmasqis.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/ggnemdhvg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gxsuxsbhw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gupwuhsea.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gphvgninq.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gexrgqrsf.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gxabuegvw.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gqzeexgtv.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxndqybbr.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvefczisz.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gzkiujhjj.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gqfgglurt.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/gdlrfgyze.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gunmajnvi.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/ghrjjqwnx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ggfjsgknf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gogvfvuod.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/grxqltrdo.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/giwnrrkic.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gunycbxgp.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gotyvbpqy.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gqmpuuxxi.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gfzusmzle.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gqguunhdy.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gyrbutxpd.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gzppgbuaw.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gokykidzs.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/groqrttuo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gzgxrzbjj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ghizccqgf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/glnieccoq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/ghwhmajou.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gpltrtcff.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gkjmfysgs.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gnqglnzbq.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gprcytbet.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gqgaawmxk.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gzkzfcdhb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gvvdsvgti.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gtmhzgqhp.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gysygxvtl.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gjnsnowsg.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gqbnudibw.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gpgwhnnpd.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggurrjkwq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gagqzzadu.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gttzqxeqq.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gbygwpmyf.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gxhpkjwpf.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gungfbxdm.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/glctbnyzo.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gzdtgkwsb.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gicrkfapm.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gsnlszyqy.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gdyibksko.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gaopzjhbj.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fehbvm.com/Article/details/ghwuwiggu.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gkbblbsey.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/giynfppnt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gcomhbwzp.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/ggqhguacy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/glairgvrl.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gsdzcrktu.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gosczukox.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gbiquedxs.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gvqzdbvqw.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gxpqltjee.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/ghpzvohji.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gkzwmgghg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxeloafgx.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gwkelxckm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gphlfrtfx.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/ggwtplgqf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gdgxuhejl.sHtML


<!-- 参考信息 -->