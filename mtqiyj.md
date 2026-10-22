代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ckkmctvl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fuoyspcp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2opjzwoaz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jhtdrgvy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2mhochdkm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ipsbiqbt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dgjcuead.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jdobkvhu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2hidvowyw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cildtktp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hcqrepvm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kecgxfnj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2orwsjsju.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zwdgsiko.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ztqmqump.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2logqdkde.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ewisdecv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oeoztngy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kiyispnx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ohxpxgpr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vcyqohly.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iqwdrmgb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2usdsawgt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ectteyvz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2dongreog.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jiwxlinm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2wymlwkqh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2edyybkhi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2evvqwfuo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2wwlswiak.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rvcmeqru.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2ydixsvli.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qltxlgtg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2goohrhjc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wpclnxqu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xxogitzq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ysbxxjcd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ndadunus.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2lqtlpigj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyuxipwn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2slmcfdvi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fkcrgerp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2kwqyupsj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mddqfaxp.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ziyhfnby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgguiavt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lvqlpvnu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ravygedk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ycgatytu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lanrndwo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dxxnqlvi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2giszfdjz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2encmrwha.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tarbblyd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2peidnvca.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xrccseke.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuopebsu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2owjbenco.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mmfeuuww.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uaypaqcd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nopgmmnw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gtbueyzs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xernvvzw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2idwjvnzj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2szvkmwny.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2isrkpkhj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2siedbkur.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gkysiplf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2przkdlic.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ufrxjjyh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ekciyskz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ytpungem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mmwtwplx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irjrbqjd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yzkqlspu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjtiokxc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btjztgua.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oraodhgk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2buxsrmst.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2vafcyape.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iiabdpiy.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tnrsenzb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xhudcbvt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eftvvxmx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rylbwnte.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2cmkufhcl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ggxencyj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2llsqrrkv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ygfiwvwz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnrivlb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2joiqgqld.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2khquxvbf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2msnwxcec.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2opdzmyjv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwmayjfu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dljmwqje.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2hggaenoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhbjiqq.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2grgipmjk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pdvhbnkc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rdzqchnf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnnvavt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2tqhozggo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2izddwfmh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2aivjgknc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ojlzfmmz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2skkmoevw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rumvbflb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2dypnhgow.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2yafdqhry.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jlxcjwzo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yaypknfy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jnoobqob.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lcdzrvfw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cjuohaxs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vuesewss.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2nhyyqwzt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qezvdxia.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uvhodrte.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bvcxrlpr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcxklogr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2djedzygn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2nzkhnovo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ivbuqtvb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2grzjcigc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qjzswdnt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2kdczrzpk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2pakrkcui.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2glhbnovi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2zudeagzf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iggptqkk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ximnrazp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2oozkxvgb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yfaeghab.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qjsxnqtt.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2romracbv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rstwdikn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2owfmnjyl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xudlrwvi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ydmnoyms.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nzsvowoc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2zvzmgcyy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rymyutta.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kizyxdjx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2nwdmicct.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rfimrdbo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qymzjcjb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wicwqhtc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vuyllitg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2lqexusgg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ayklsybz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xamyppsr.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kfmgseng.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nqovmtdl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mbsacxee.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ykmssayy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kmxzvzgv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qobmuvma.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jaqgayvm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qubekcdi.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qkwtpenv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wcnssnwi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vodcxjbv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvplgyqr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ttzwgfvo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2xplyteme.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2hbsbyudg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2mafhykmi.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wqmiczrz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtbwavbf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vsiyjhej.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bqtycdrg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvrcymtv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wusgtqbb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcetqnma.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bhxtykqo.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2pnbxmbsa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ttdkeeka.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xlpznwim.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2lnxnsrtk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ojzvpacv.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rzmoqndo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2agmyghqi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fyydfojj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2onnkpzzb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aqbvutfb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2iejthnvm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2nicnaqjn.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgubrdy.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xbhxnmqc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhuiqgnu.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2khzqrkgv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2apuohlsw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2waxzjhlv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ueyaluvn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2uwxmytpa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxgoogz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmeikqxv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onbvsfze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebfeisxg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2ceeljssx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xkxhiazu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2bbfvjidj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2zixuxmuu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2rcoubwuz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lszahljn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qjacvuat.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2teoobjia.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2glvubosi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mmqgynnp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ubaqjvdf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2vcormksw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2papqutud.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gyadbtcf.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mduufiir.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2cydryrqc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vlggvatr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlildpw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2aaaicxwt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dvdynpsn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2enhxmmha.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxsfhirh.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2lisyqfjc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2nplyujfp.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ictjgavx.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkaxjdf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ywzpizti.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2qoeyqdgf.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ahecrhrs.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qmruvasi.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2iewigtmn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mqbewgqm.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2vfzpywhw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ovnuiogq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2tljeprdw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qpyssdtg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2psxrhjhi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryupwseh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zaswekvi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fvxsggls.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2hwnfkokm.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ozqdaajo.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2bogzynhm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zmayltgl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwfcidlf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2udnaqphd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hycxrdlm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gwtyqrgs.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2jqjigtpy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2fzgeahtd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2zckyookt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2nriyhupp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nrxfdzqu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2tjhootbg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zpcdepuh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2qsocquhf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ouvwxpqv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2twfsvjzw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hxhwxwfr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jkcgppfx.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gjnnratg.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2icjzobds.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2maekaboa.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qxetnmmy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xjdqplac.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ugmjaupo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2nzexmznf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xzeumzjx.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wkgibibp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2logeylls.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nvaxvhvd.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rjjjjjga.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2iukigfkg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rfnznvqp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yunqpfbi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2sliikmgy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2adiqgafq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2chnhhxdn.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qepvwnbx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hysettfo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fmfyopye.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2qqhgwqqk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fwmcqjaq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hksdfwsj.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mtejqugu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gsqcegkz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wjgjiuki.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2vyncuoeg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wuatebko.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kunjtvnp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzgshhna.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2jtvaqaxz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wfvrqpkj.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cpebqzlk.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dkqeywdd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otdgqpjw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ipizfdow.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kfhhwlzp.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bmeknczc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nyauqryb.html


<!-- 参考信息 -->