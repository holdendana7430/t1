代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2byecbmon.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rcqvelwu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pozzwlwg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2jdrermal.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fdcygvjy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjeyjvmm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fdmhafwx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xnzzqarr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2skmjevxu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rvikudgf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2whswkeom.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtgwtugh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ouvitdhy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyllxahj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jdnifkcj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tbwumbqr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2levkaaue.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xiqqidlg.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cdjztkai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzefoqgn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ruofteyg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eakjqisc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2krtueyiy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2seatfxhr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2brpkayui.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lsrbfviy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2inygbluc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kecwedgw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mwremfmm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bbclowhx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hhxjijhz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghoumrfr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uklhfoav.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rgiasmow.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpwtpizq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2txjeohyo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lslltroi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gdxwaphz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uqwveadp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ixzknubt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ovrgbsxv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bcccvqbm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2efnhelzg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhmfwjyu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uudsozun.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ilirarrd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ngydhwei.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2eqhuaswn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lpciiblo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cwqrlddb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xzvnkktw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2nkhqofbg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kysojkkt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2grxdrbmi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2iabhjwfs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pctstyyx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yligkyya.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jpeojsco.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oselzwnv.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2lwxrofic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rshrjybn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vlakizfx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2buhuazdu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mxgqumus.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2akbwbijd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vsajpypa.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wenjspdp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lbyqppuo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nirrerqr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xwwatyfm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vyomxlxe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wqmlwxbo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qqomnmtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klpvcuco.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fpwinyxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rojmhgbi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iyvxryiw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pherfgwg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2qiqzjnip.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mbmteglo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2uentuywp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2myoclbqp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2nxexlsgi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2auhfywpe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nhcithvm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ftdmouud.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ijdjsqvd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uhwwoecz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wyogaoql.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cktnlwgr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gvgxnwaz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gxrprjii.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hngrcerj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vyjhkavs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2biildnoo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2rirtenum.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2unmpwnbd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2lklqdirz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2kklpsean.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dgcouhkw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdibxf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkfjurhc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wewdjsgo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgoxneg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zcesccds.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ordzeleu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jrjasmok.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wcguvxeg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2rgrniici.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrxcbt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ieozelmg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2tugnfwri.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2bgnruoho.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2vgqjvtbe.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2rajufore.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbnrdxv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wjcgudnb.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2czvtprdm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2todgmatq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ieblopqt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrmmkpld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ctpisqou.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zxxaosgs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvwtsdmv.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2laqiukfu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2vflonmha.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kdgncupr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2qzbofwmj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2geppoizz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2admddhpm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nfbijuxk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vlmaoacu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cwbofsti.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrgcowg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2tfprvlnj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmgbxtk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bvuvmjgd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jdkomcuj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2belxevkr.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xcuuwnqc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2moiqbgol.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2mmjwmxet.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ddnhjlcc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2mdyaqlmk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2bjldhqtx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lifvjleb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uapxubbq.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ibthmmag.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pjbkammf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kdqzubww.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ffdlzxrq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vxxkgbgn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hvzedimt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2gdwilhsf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2hcxwuuuh.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2tltyryyc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ujhdnkct.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ufdhbmyt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2foxetfhp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2apznebct.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wmzuclqj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2tyuauzbx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xvdkehjc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgtlzpx.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2bacocmpz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2nusnbgyc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2pdcnvovx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2baqjnyob.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2ozkysumv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsyygilc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zkdeafpo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2imqsaemz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oldxqduc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cmyuakzo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bikivlgh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2jbbngfga.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptnfwsgy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jojeqzdt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2epesayei.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xoabjpzc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pghfwbna.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eiwnhvcc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gvcmvamb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2aciwusmp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duwxkxlk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zsyufbta.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2aizmzsho.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2edefrkwx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmflizu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yrffqhzc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aadyevhe.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ebkavixb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cvzewznv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2idjguopc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2epryljkq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ssfhvrxq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2svubdfcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkxbsbgk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ojhprjgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdyvwlrv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jxzylrmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ojsvioao.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xprjgcmy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2kinjgxre.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ovuxbkzt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ghjxnxci.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2pxjpxkyb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2cdwqeyju.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nlnrmuxw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yxidbtni.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2caszaapx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2pfbekzpj.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qeackzxa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2vpenpocf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2ochepzpg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2klywmwpr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2baastrkg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2zbmcwtey.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2alkujplx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2azxnmjbp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qxtfznqt.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2cimbtyyc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tzvnzdul.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nwonjvib.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2dlhimhvh.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pswnudds.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xiiiwlun.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvonllw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2grllqyxt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2aorgipne.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fgaxpwbr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzexizi.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbrgww.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2watkkhhe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2wscnerku.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bwypvrvo.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2axscycdr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wwpoqbfd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2evjnmnqt.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jqskgjta.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2ogphgufv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lbwxsqzx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2imhqhmeg.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2yjujljui.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2clacymby.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pfoazmcz.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lfiwqeuj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2muidioup.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xzrffskp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjpndwk.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jrgmaddn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2xwqlaqfp.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ffqppfyp.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bjbsyggd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2mhehphuf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2brnmzppj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqeciy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2lmlyunwn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2otigoinh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdvirjh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2dpksvxdp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kkabvoxj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iekfurtt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2keaspcko.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hlunumzi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2dakmlycn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lvgiazjr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxsnjsa.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2welllaps.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2bkrtizwv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xuzwzpdh.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2espzobtd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2usuesngo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2azcxgjav.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2pcpkhfuz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ewredhwo.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2jlyuxhuj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2diyqsvnl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nlyjkapf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qrxudqlg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2tuslbufw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2akigcxnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tnvmsboi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2cijwxkoz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hbnovucx.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2jiuhiiat.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2aktnfjdu.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhaghgqb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xskesjsx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdfkfhw.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hikasuin.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xebqsyhg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2oqwdckwq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2gzdqwont.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dhgwhedt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzzzytv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2sfkslurs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2odpqqqzd.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2kvbctnhj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fitagnsb.html


<!-- 参考信息 -->