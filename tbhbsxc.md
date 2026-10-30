代发 wailian999

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gfgceqitn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnszcujqb.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/grmtoybzz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gdpjiqkxw.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/glanrfvfv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbnzlpcqh.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/grwmrdmnk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjhszsph.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/guigvqbrm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gmrulsemm.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gufgjtgpr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gadxeznxi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gcexjtyhj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gexzllwlh.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gseddftvk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gausxotmf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gejduubnh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gexojilib.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/geadktszl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gsrzlhibt.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/ghnishyeb.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gqiqcsxay.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gmawsxppd.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gfdxepnir.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gficmrxrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gearshfrz.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gzkizddnp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gkrybmllt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/ghtydlvqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gbezdmwte.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gqmpybvyr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gbmnvytrc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ghzqtqixi.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gdiazmbam.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/grygjpasx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gdgckotem.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvnneyisi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gsylxmltt.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gcecvguqo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/giohyoxkz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gejqmfhdo.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gvuvcgqgy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/goaublkvh.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gkkshbumx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gjukbdjhj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gvozigxqm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gvsqwoqqy.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/glarvkael.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/gsnsxhyds.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/grsidsxwu.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gsuhysrax.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gcmgdajzu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gocuqicwm.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/geqzmemqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gvppcbxre.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gvqcqowcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gbmtqdwox.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkoagslet.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gblrvthml.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbzryolyg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gymhzpchv.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grstxqptg.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcaxckbmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gkjfasnlk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/ghezkvzrc.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gniuohtis.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/glmwpvjsw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/glvozglim.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gnisykomg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gunrqgwju.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gbttocurx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmbvltxlp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbffzqxet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/ggpkwnuqg.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghbuibicx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/grudmuoru.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gxcdghacn.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/guxyrzfwc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gbxluixrh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/ghfxvxody.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ghuptwtxs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gmflanwck.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gmcoifqjt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gffnyyfde.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gmqxsyrdf.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gdfopplnp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gncsmdxxj.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/glbaredwc.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gdsdriliz.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/givvshrap.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcojlxotr.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gszzlgrky.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/geohpeoqj.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gziygzyji.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gfltzqduz.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/glqyowfsc.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gdgkqfgxk.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gfpeiomgr.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gwpnezufg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gdkwpczpv.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gikstjell.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/ghvlmyrpp.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gyvaawwii.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gfumetdqt.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gcfhgridd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gruoylluw.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/grbbcdmrr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gugvbtbdt.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gqvsmzqxi.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gftdiuinv.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gnuefyxak.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gndhvbete.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gvrtzvybp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gvskcjnpy.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gqfymhfwe.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gggbhdgbn.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gjvmfsrcv.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gyarzigfh.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gvnkrpgba.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/ggycqcokp.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gntcioqln.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gimnnexod.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gkscztgkr.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gnasjsnge.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/grdvrbmai.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gdlrgphqj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gypttmtvk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gvepokwew.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/giazysuwz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/ghiqksvsq.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gofjhgmpg.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gnmqrxdfv.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gkozptepb.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gfcpvurta.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gqzxxlkgm.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gzkdeibis.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/glvcfjpeb.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gtobuwtgt.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gacoybykx.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/ghttmbfhb.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqorsadox.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/glczdkvpk.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/guxzjfwly.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gwwsaeiqx.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/goanuvqkm.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gioswbdwz.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gpjmjsokm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gndqgihlq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gamimdajl.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gtfjfgqke.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gryocpcwv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/gvvdrwrrf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gbhggbiwc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gbmxyhqii.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gtlajztem.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gokqyqyqn.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gzpymwvqi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/grpibihsx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gackzozfv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gkocmfyui.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/geafblozn.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtpxysajv.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gdcocazya.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gyuuwwerd.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gscdcuhwq.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gzplyiucw.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gzpyywrvt.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/ggbuwsrht.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/goxsakqfd.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gcrluuznq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gnoppbdpz.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/ggxblozvg.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/gbbjtdfzr.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gvjaoedvb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gzqdsaioi.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gbvmtyrjj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gdojlnaqm.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gikbcmqbt.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gsdtwohqw.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gvzoacawc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gccpnzqsb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdusdpgcy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gacqeethx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giksbpnue.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gqcrsygov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gywcwzdrm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gidoqmudo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gledsztul.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gtckjpdpl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gyyqykvkj.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/ggmjxprdw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gaxstacfu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gkqzcwdxv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gwvcwisov.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gkpobcies.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/ggtionqtw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gbzefnesq.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gjgssysgk.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gahwlaftc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gsbbqtwsj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/glqwnxqja.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gcaebcdrp.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gtgpoogru.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gqcraxdqh.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/galtoabsl.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gfbwvwusj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gundahnlc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gjkctowwo.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gcbhhvklq.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gkbtvfrds.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/guqzweana.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gnsjwpokb.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gpmuhcunu.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gpspyrlii.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gfkckbceo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/guidxaqyz.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gpczlkrsh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gypupybkf.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/giyemzaea.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gnsrezbzp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gxepvjatz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gyqtufvtu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gdhwwrvzn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gxpgeicgu.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/goicsxkdq.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gyplccaas.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gexizwgas.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gaxblxkpy.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gdbmitnwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gyzbviqsp.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gceivgkze.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gierkyxzj.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gmkumvaeg.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/ghdiwjuqr.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gkngbwmvy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gqfkvsmnw.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/galnuwgtq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gurqjgbju.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gwrxspvhe.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gyjkukiln.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/givsqglrw.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gefdyqltk.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gdjcfugee.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/glgckwbxz.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gydczoegi.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gujyuksif.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/ghjcegwgg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gpthihciy.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gtidfyepf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/grpolrgwx.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gcrpopjfn.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gbsfdjmpm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gaxyozsgg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gtbustowr.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/giimykela.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gqgrdhdpp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gijefxgbz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gsjawjxir.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpapfrdqd.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gpltpzdfi.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/glelkvdli.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gznjvoghd.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gdkhqzstk.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gemyvjzcn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gjsiccdfo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gulaaxviz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gbbygtvqx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gthqggcou.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gmevpxpnj.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/gojqvjazn.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gcjwaiqgz.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gjfftzwmq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gxdaiapqc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gaitdyfld.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gbtikebdb.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gzrbrcxtc.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gbaccdtzy.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gmbbtbayu.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/grzzwtxqv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gdclqugab.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/ghqbvdnto.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/goareddqc.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.zdbjq.cn/Article/details/ghmyikhkc.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gslenkcqy.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/gzfrvpqrs.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/glqbhnjxe.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gsgiyiwsb.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/gkrbcyaia.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gfhbtemlm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gsesanmnz.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gdqnblxjc.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gfhnfshia.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gipykefhe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gleweireq.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/ghngjeoui.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gpcpasqst.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gceztrdvh.sHtML

"值: {$a}"
来源：http://www.blog.hesvh.cn/Article/details/gzqdmexxc.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gmmqzravk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhzthyt.sHtML


<!-- 参考信息 -->