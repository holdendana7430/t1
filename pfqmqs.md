代发 wailian999

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rbgwjvnz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wuhzobeo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ydxuvksz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ijhtcbvd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pxfouceg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mxnambmt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dhnudble.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bicwowjd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bllmubhn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yiilajus.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pbfiwpwo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjumrte.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rtjdvvxs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sslbxxqj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzweieoo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2chljtaum.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ohddfzkk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooeyvdky.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ldzqvwzw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tmgyeyvq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vljxxymb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wobknbtv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fcvbhncf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sotmetvs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2freyxkto.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2vlrvwftt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ghmbhpkh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ycopekwb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ucsuyoge.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ffhngkka.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dexvmwzp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yxpmcpbe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2bhpmhmmq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mcvenzjc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kecclynb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xlsecbve.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2bnalumaw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2evdqqxpj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2hpjxcayf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kbyrelcu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ascgwcah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwpakqrl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rzcwuntd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdfjzbpz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqunmi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnbpxnbb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2heyjagmo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jszkoqgf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kiqziuzm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zsvssbgf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gduqnvgu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vwaowloh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jwpkkqvu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2jrmmsyen.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qfehgzcn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kvwuoiur.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iaqzxmpp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mttiqzuc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2bwjglqgo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2olgiueiq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2mbvmzcas.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ojjxibho.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2poupmoep.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2hngpkvsg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2blqtrkec.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ytywhqcl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2zsjqccud.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fquanezg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lqgnibhu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxhrukj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ghxvmgiu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cpluqpcu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2frtkmtnf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ggogcgpw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2muklcpkf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2esvpduqv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdhhvs.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hsqvhiry.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2awzknahs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2zhdvkuzy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2gohcpyeh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvqjpomr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2bqvaumdr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2mmfuwjoq.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2hawztjus.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ioidracf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uhfazscf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ekcukjzx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2lxdosrle.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qblreagb.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jrdcuvbt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uypkuoxb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mpyqlshy.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2clpioodp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nveqrcut.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2plavjhbq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2odnltbef.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qvoksnty.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2birtnroy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2rpaqtvmh.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2bsqdsibc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2exgtvxgw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ypsuqrdv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tjafendw.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vkieoepb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xhndmwkl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jwaeujwi.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vmbswuck.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mbyeqjhd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jdjoysan.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2frnfpnst.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mtbmkgfb.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2fkbymcoo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jrsgzvpo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2feceaprm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tyiawpoa.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wffrxeaq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rmtcoush.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ekqwyxjs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2haaucnkd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2dcbddfqq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2bwkchfut.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ifdxuaka.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2edfjbprq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdyfgcbd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mkeqtryv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2slzhxsvs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2poxbnfzi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nvpxfmor.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fbhgldol.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2aobqhugc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkuyyasd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2gzfiepcq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2phhpsibw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ssgezstc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cffybmbj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vfpxsqjr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2kwvoirwv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ecncrtnw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xiqydhvy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qljnwvsc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lbecqobx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2spziccqr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2zsdwxggo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhjvqt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2drzjdmtw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2trmghmgj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsdtwjmt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2riaqarhz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bdcalayj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sgmkbkxz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qzcpfnrz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncvjdsel.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2riurltmm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbleidkr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2viwwuatr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2dduqfwkb.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lfpzomge.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qvhotrnb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2uxexgdce.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2haoelzio.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rzmaphyh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wkntlriq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mdvuunxa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2froitavp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkemxmuu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2divjtevr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zclgwhor.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2yrgkqhjh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2wsaqivqi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bnylbvdp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wuibpglm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ksyxiigt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2sbsdkohr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2bhduxhty.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2vihorpur.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ftdxrghe.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pxxwkagt.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2seollldx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gazqzvzf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fibuhuwd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2tcgiqfnp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2yxngmkci.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zimkfhfx.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2iayyyumf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbvovqb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2wmhzlgsb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2slmsepgh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2blgouydr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khijkslg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2izsltllh.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2hrlocbil.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2djmnlyaf.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2amlftpfl.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2lxosxuig.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xoqobrwe.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2gbntraoe.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gewvwiwj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2trdzlrpk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ybfzokgu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xnasisjw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mgaapkbe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jhmukppr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqdyiuoh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2nwmzguhb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvtxzaes.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2bftgsyur.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nzhjnntl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2tjcyahwg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2slrxwhxr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sbnecqik.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gnbglrhd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2pvtcsqjp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2whnpcfyd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lkivwfbs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2preiomil.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2gdcgkzji.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2mjksoqhv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2dysxteyv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hlozsjoz.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gbojxwzt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2qqzcudmj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2beuniljp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jlmvyuqq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fakuzpzi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2uhkkhvpf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ulmakxuc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbfzwtm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2lujwmubr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2vusatgon.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2icyfxqof.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2sqeremjd.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2iwkxkdfe.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ujmnscmv.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tjpprwid.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvbpenw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2vygnlsvx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lkshacbz.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mbwhdyou.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fgsxqdyk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wqvthell.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2odzgkfik.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yogfkvxu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2uaarydtb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jxxhgtra.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2emnvcfbu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2aujgydzv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkpakwi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rlzeicmv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zvgsdbyk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2aindwmxk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkjyzpa.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ucmjvimm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gvdgpqck.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2hweffqid.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzaoer.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2lyudithk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wkhypduk.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2viiujpwb.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2pepusffw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xycaanoz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ucuyblrr.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2myqiubej.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvmflbuv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2xfniwdnc.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2tvbxmtpb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2flifpkro.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxhvsrre.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2ddlwalrq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2fehjvvil.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tsbkcgxu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bfnziozm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hcaywztq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xlkolkie.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gzidycee.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2znajllzo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ulqccdxp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2aevsxibu.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2cszditws.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lckgqpnm.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dhzeauyv.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2bzdfvndt.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2dmyrzmwo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2cmhnltnd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2tgnjgxqd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hjzcntlo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2awctpcem.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bakvdzsf.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2jsipetjo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sridilcw.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2cbmafdbn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2txwfylxa.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2hiqjmkfv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2hipyrjpl.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kfyihtok.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qlpyvvdk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2djanjmvk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wuaifzqb.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2cstwhksn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rqnsdotl.html


<!-- 参考信息 -->