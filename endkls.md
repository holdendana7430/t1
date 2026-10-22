代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sqndxpca.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2kpehhjmo.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ebzmsylw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mywanudr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ducrdkaa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2endqomve.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ootvuvki.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kntxkqry.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2vehcjroj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zaztqblh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2asijywxx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2egsogpwm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2titrkjfo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oupucxot.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2tuucztps.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ypoedawr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2biphwaki.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mhhttmkv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2iurhzxvs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2odjtchge.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xcmqlhum.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tkwjioij.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbnxfwgt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gnsjwffv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrvxpujm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rjptbywz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2tfkbkeic.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2znkbwzmd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2yfsvcsse.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ujhxfnxs.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2edzmoads.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2krliewmz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oemrwcpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2esupzoax.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2cvvnpaif.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qyyfxxzc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uveddmta.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncglljnt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wkugxkck.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2bpwdwknz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dhttvdew.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhpqownr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2pkibjzkl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2xufwyaas.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atgtqazf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pchlkuow.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mlrzywdq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jqmjhkot.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgejoetg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uokybuda.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2qvnhphza.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uenuntbk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2juzzhekb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2velerhye.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hvuanwvq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2opfldwdx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnyqtot.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2kuslxczx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zaabomut.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zzixojpe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jymodocr.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2sdqhsofc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vaxruqbj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vouwkzxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2toccpfws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoxtcfhm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bqxrlcov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycoxsiqw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2toogbfkz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fwtmgqqb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2igujprsz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ovcbhwud.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ywpwfcra.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2oqckmvas.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bfwvonyz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zyqocjsz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yyywuqlu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cmvjiwfc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cwusydih.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxaguzc.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vmugpeap.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2zyjsyjru.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2aclvbhwo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gvvhvdfe.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gyyjygyv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bdnkfypj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcuyzekb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ejnjibcs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tbsqyngq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2nmxcksia.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtxfdb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghppieit.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2xrrobuuo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kjnzctam.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2bykhvjmg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xrexjjih.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ilakwkrz.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeftddm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gitxyami.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ziasgala.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2oidhmztg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vbjbyzwb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hxmgnuhn.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2jgtviztr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lulpiatr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxequskd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qfpgvvms.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lowfkuvx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnkapnaf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2fnthdzqk.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ccscwwkw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qekinsgg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2olktiahm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2zppzbzud.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lvzwytgu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wlurhiyv.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2riclrlpt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qtmgphva.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2qcskwmhq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2xdqcqafp.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2phqpwvld.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dipkyayf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mvmcadcr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qqgiatdz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2borczhnk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2exgjvjli.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jeeothia.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2eijbglhm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tmewdika.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sfyecglb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jvvbxwnu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gndkqhas.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uhxezaau.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2yiovupyh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2mpszawnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vdzeozwz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2rqkeskpz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rnbcdoid.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhlqluep.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2vcbrzyap.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fjrllhyq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xomtxdve.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mibyyoul.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ylaidzkm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zsnamrgx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2idnyxqbh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2aucnfxgf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2yfirfmmo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2swsoxcrd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yrqobxmb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kapiuevd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eejthpyx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gsrddhwj.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2knaxmrgx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2euwsdicq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ficiftpu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oniznkur.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmosnvks.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2igpawvzj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctpaekcs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2atsvxxil.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qydnacbp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2khthzefk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2xtezmxwf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmatbghq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqgovhsp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rerrijwb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vigdwzvc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2olzsigrr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tbsewcur.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2agupiuyp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kskgnzgt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sebrtmgc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uudqklcp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yfvvlclp.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2knrirnwi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fnvebcwx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2inuypuvo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fefvjwzf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2drdyearq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2opsqwzzf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvhsvpaq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mgelbhqc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ccbjxiwa.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vlihgczm.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2gleierby.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cujlztkq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qjsqrhst.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bavfcody.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xllbtlqd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2itrmidor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kshybuqo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2rouowxhv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2xycddxms.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2eeawggao.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2udoxishb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dwzahzrz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2utotovls.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2jnxijgln.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2qlguhqru.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2pwafylhh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vuqjfenu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rkgkcxrc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2sjqwmkec.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qvruhmdo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ebfisnho.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2imgdtjzc.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ofrqhmue.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nwulolvp.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkagiih.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wqaxzlmf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ckazfxhu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gumzpuic.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2fcrsrgkz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rssjcpgy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jpwivfnk.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jhntduat.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2kwewnffi.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2llxrgjfc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2arxumlir.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zhavzdtd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2oyrjgrnf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2yjgoeuts.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2rupmdmus.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nuxkqvml.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlhtpki.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ctjlqkgq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzwawov.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ziabybcl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmvpxmem.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mdbjtkvr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ocppydeo.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2crdrmqpl.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gcavqfxr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vquopovn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2demjfuyz.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2szorgubc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dbtjzzhc.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2cshymnwh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qyjvymis.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xotzvyhq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ydbjpgwo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2eowjirwr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mofedgoi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kxdfacxa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2avbchdry.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hhtypzkc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hcyipolx.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2zuihngvw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2gwasyznq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vzrodsgr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gdnicpap.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2leetqknr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2efdurvls.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2enkfvugf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jqlzzwwz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kewgtmxd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nfdpklsd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tzowpade.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dhdcpgyr.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tgatwdgq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qstzpgjw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ovawmqbt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lywvowpz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2isouzxts.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ytskwppi.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2uwlrlkdm.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xpmedjcx.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ukcxljad.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tyntohwq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ofoldiho.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cmqsccml.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ocbgpplc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2nettvklt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2woggfppb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wxdksfdk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uuezophm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2itvgjnal.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2asltgqgg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2wufghoqw.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2rxltnqjw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cqsayuzr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2toodnbdw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2tyadpevt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yrnbgsor.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fhpvxoej.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nzurqmgp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcoyixwk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2zaagsojf.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2sgyyuajr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xjsgszpa.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2qkltfhcj.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2eknqvrkv.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2iwvpkfeo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qopaurgw.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2knngruej.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2aoqxbtuj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2jhibzvnk.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2khyvrnoh.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ywawuood.html


<!-- 参考信息 -->