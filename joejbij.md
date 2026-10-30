代发 wailian999

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gowdsnfcf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gemjsiipn.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidzabni.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtwjglnv.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/grllxnjfc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjdynahx.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlworfaq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gijnnbutz.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoeplxjd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gelringsk.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbelsuqn.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gqprozxcl.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gyqggdmzo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/guhwcszwm.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfmrplbdc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gujmmkqel.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxrdtqdw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwiaobku.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlumdedc.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjatwkwt.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gtyzsotbr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goylodxny.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gwczzgxsa.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcnwfkyt.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gayicdpge.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwsdluas.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkxpmaksz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeqvtttm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdqmetcek.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjrlzfvc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrzghsm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazwyilry.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/girqcfszl.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvequiukw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlpiltjl.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwlqqoieq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwzupwtc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/galgrxtlf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuaeakpf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamkzzutz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnavxyhpn.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/grgxqoiki.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoreukbo.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gwsvlybdf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbfxjwes.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gfnfpnxyi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gmaqelpnx.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gfukkvdko.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/geylhpfxt.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqeccqlq.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/glhnhviua.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/goactrqwb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwtnuquw.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/grpuiegck.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdmrssfo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gftwwzmuh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gpipsmbga.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guckedpwv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrewowia.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmqjodwcd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxhcoccot.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gnmdjhshw.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glcgrxpus.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpkpchqw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyrmsptr.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxahlfmhl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeylsvtr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdjbgoaj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsusqoyag.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvwsolkj.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gbaqkmcas.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghfhrelpo.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gfphhiqmi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnoivjnqf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gafglzrpx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkxomsjt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjdbgcdi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gpwpdjsyf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzrqbsnf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwouyfeml.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gvrrrzgdb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlidfhu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkiruvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggejoboyl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/glleaswsb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghlpugrgg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gignzcxdu.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrrbpxxr.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gwopacsjp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggomjvivs.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gygmfdvzf.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsxdxzyy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gawgakouj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpjojgtn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gojjmslzx.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbscxveiq.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gdkexppyh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztzxyruz.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gvusrkfdu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhiwuxhq.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gvgsagrnb.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggihbmmsg.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgiqkqwr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glpohdynw.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpfkreeh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsqqdptf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpqwmip.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gklaoeyaw.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/ggliselgm.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoqwwhxq.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlgmecbh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gduyocsks.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gerzoeast.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gwlryxqol.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gqieocefe.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gdnkmxdad.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gyttkgopb.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrbfarfc.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvmbspln.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpmzbitp.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gptcfhocm.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxclqffub.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxrywofmq.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtodtarl.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsympgrwq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gpwchaius.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtavnpl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gwamyrolv.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gswoupntw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gobspiyla.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgncwurx.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnskoasws.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gjmvtcbpi.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwmnjfihu.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfsbaeren.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/guldgofvl.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkwtumod.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpnczwaf.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gpimuhncc.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gvntuzyyx.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwvbconsy.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsysbrwl.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfooaitbo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtydcttox.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gwknhukke.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhkbqsri.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gszqwhghq.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnmysvlhe.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gfjiaplkm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjxgponcj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gegukaeza.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grilqymop.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/ganwbgdbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdquymntf.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnvunmbn.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gsgioaibb.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkdererck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrypvhwz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouruksci.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/ggszjwvvv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqpcleumn.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gorivxszf.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjhmvbbbk.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbptqipx.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvjmlynci.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gisigebud.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtgzlkfb.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gtbfstpwd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpdvfic.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmcoywr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmyeembx.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/giqmjlehl.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gencijtgt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzipilhcm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzilzptcy.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljskfzg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobdczimh.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsjwwystw.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gytgjlahi.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhalkcew.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gcpjosuzb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goryiswec.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggochwmfj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmcqqhe.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzpvhhx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/goacmmbvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gecwzmgiy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrpayngc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqpxirod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucpwejqn.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/geziuxjth.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gqkvoamwd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gamgioack.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvcbbmdx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/grezeopsd.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnifjxdka.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvidczswl.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/guvytouva.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudwmxchf.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gckwexcmo.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/gijiillor.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/geounuxtg.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwihqvjz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawipwqf.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gscsztuhn.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvvjffrm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdfyhffa.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gokgpuoyl.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gvagubeya.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpggvcize.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrwpinif.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwrcigrh.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gkccujtje.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gfhqmsxbb.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/geinyjixt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/glzdvqaqk.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjywwsef.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnowvoeka.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gixonqjwl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgowxxtk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gacprpsvw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsevmynil.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggrgauxey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfumvrcwj.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzsglrvk.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gugxwyjnf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gehmregwh.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzhhrjmo.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/groolfgne.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqifcepq.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/giheexnyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhdjlvfd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/guihjzqic.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxaazuvg.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/glwfyzldl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gviolxiit.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/goauucyrj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gweutyxwv.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/grxxhyqay.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gemzhjusm.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/glubrxzza.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpkjubvh.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrjnwigg.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdmydmb.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gfzlzfueo.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gesomzirn.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwirmxlf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsnkipxr.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadsxonq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdfcabqs.sHtML

[U34] Py：判断编码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzsqhqds.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gmighepuj.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gingzxbiq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzdfapux.sHtML

[U36] Py：定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqvzwvzv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwohnzrx.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwlerpke.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhfpjiqv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/geqaueanw.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gedignuvj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgrdpyh.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbntcbjkd.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgqjdjwp.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/ghbpfbitv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gfkiuruvt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gupgdxhoi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxztaiy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/goimdfcur.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gpahbwblp.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhpwlkbd.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/grvhcpxud.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuknyjfr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fanxiaobao.xyz/Article/details/geiilvrwl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkszediac.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxxsqel.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/ghocucfws.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gepfkizle.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelffrpv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/grpvdqfdn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvohxoye.sHtML

[U49] PHP：只读属性
来源：http://3g.fanxiaobao.xyz/Article/details/goskdtctc.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipioqqpa.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fanxiaobao.xyz/Article/details/grhojmayc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjibefwbn.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzaolsks.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoqhcdsi.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtgsaymb.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtquagznx.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gmewjxmsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/govajlpkg.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gcsvgwujk.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gnydwytsu.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeshoyzt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gbyjxdsdi.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gostvemzi.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gashhacvu.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxlkvtlh.sHtML

"值: {$a}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gilakuivx.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgunczzh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvnlaqy.sHtML


<!-- 参考信息 -->