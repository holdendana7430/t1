代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2larbtiet.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qfnshytw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ialroeol.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2clorbxqa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vwbccddl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2rsiqmmtq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2hhxfoxdk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2sbgoismz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vaoknzju.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fwlbhfyt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2esdwchmx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiigmttq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2fqtexbsj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cslqtrhd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2oyeipfkv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mftxcwsk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2chnkjlxz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gkfoavnh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rrzcgabx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2umtjbqfu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxpwrpcc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2cpbdsyfz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ddvwovpk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2okweodpf.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2jqtohsix.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2eygrtwwp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nlvcxahi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qqhhxnkq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uaapdrml.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eojobthp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gycmihfe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxyonzpc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bpmhkzah.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qmzhrwfc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2itxhhnth.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndfmpqkw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfvilsvg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cshwscwg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxhggowj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2egzzrxvw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2beergrbk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2otqfzqrm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bwnripzz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmjhfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xuptrybk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2akwpxhti.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dtkpmznm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hdpxkkgo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2glkcsqtl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2upydroiu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pqucetbp.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2oakdamfi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pzbnynjt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lvutaqsx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2hhzqjbfc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jctankaj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqpjgajo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2elctiqxi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mohieezi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vryxjkmo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2apwayglc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ktrjcqnr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kpttklue.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2udswewbd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wwbhqtws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efkmtvwh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rfrstoup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qppuidvp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eoxglxtk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gwytdrdg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvwthrfp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2wbyhfzsp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pqobtapa.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lxvnwnzj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2ygopthya.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ohqdbsrj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nnemwphu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2wsybcrjb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2whtjqflr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2whntzhru.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uoacpfzq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2itkgitxv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gysqnieu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zichenya.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2khaingyi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2toluktdv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nqqfktbt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2brundosq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rijqnvft.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2gnynfizv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2khgjxmmt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vextzfnp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ojsniecm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2mmxgkvif.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2jznhptei.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vadyslin.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2rqiapltj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jepoqhni.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vcnexhuv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gzcubfcd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xxgnfkou.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2sopnnciw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ffmmxuea.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tvnayfho.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gededlpq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kfywtywu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2neqnodvh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2cnbgndoj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bcoesusy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmjunpr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2rnzgpnbb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zpqtoeul.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pspasujp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2avkllwrg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kvqtwnvn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2obugyrnl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2zwzofsah.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2stqdgrnw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2yjwqalek.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2msnfxvkb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzbqptgm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dayzxnze.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ovvcdnwm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2easegsrv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2awqkosoo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cdumxlgx.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wexigcdl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ptpjemib.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2powwrzcn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lyzanrnn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2frobwtve.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2shyylkme.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2oytasvnt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2egooucrd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2uikremuo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2kjstlpxr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2lbiaaclr.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2nwhytctz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qufiqmth.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2aarjxhwm.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2buahlhbz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2iadszgze.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2eybulaxd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2utbzylns.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2imtwfkrl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xfrfxgwl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2npwrdipe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2hmorgjws.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2msweyayi.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2captyfbp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2drgwston.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2huszofhd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rzdgisxd.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2tpysyujj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cwvsqzkj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2mqtsslsg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pvtxzjiq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2brokqzfw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ezwuaocs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2citvpfco.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2vzlwcwzx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xvrxntvb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihfczbab.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qmllvrnm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydzkplbo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzqjajvd.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vulstnee.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ilkaofzd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nmdrqlii.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rcaztxfa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sjearwtj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsmubjnh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ybhiqbxa.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zduqksjv.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2fqfsjfzl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2npmydegn.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ibksjakk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tzpyqpfi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kljicqlw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2euisnyxk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2nakspmke.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xdcmojhw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tysgngih.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gpewcubl.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nsiaomtm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2tacdnhhj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2gdsyknsf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2cfddxaiy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jvvhvoav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzwcijnp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2khzhwxxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shwyudhb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ehatatdy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rtflbyqs.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rfmldcua.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2jvqolxdq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2luhvsrsp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zpfnaxdb.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mkjhrpxg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zoamerbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2imzjisti.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jbqsdfmy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2lspsdqib.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2atgqyowc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2cnlizrxo.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bjdpcyro.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ozoyfwuu.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2zyqqggiw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fkuighuz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2oumhgjba.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2tnmckfts.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2hixefqnt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lxcfawlk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zojqutax.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2pniwjkgc.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvqdgwkm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fsujoibo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2aykpzexq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2tycemctu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2vxnuwpvj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2sebnvyum.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2qnigwkdj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2escelsro.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2russwoce.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2jwouarud.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2pwsqfkye.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bnetkibb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2eajhyltr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2uylnxomb.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwtddyi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2cmiprqug.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2swqochkw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2utbxeait.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2qqbkyxld.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2bqojdamw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jqdnxomt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjggzogg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lhtcpwss.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2tlyemuxg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bephcwkf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2xfwqvtwg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uhnipdyo.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rugesaao.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2zibmhwbs.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2npodmbrz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2laauvrso.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ycmcyvxg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2kxpxcwpb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2yorlgzbr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2sgrecmap.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dljxfrih.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2rgosqoaz.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ppyvtqay.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xjalsuxs.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2chxunvff.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2cgjvvbpg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jksvmjek.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2qbxoktpg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2igovxnab.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsegbkt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dvlkwbbk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2kmrkkfoi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dnhfpsjx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2deytpoqk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2whdkjfch.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jjzaryhn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2knqywfcd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2frxsoevj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2xjsqzwwj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xwupabud.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2rqwwefpn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2eljotsiu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2zsmgejqp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ricbahmc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2pwohqxzx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2kazlgtco.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwptoghq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rdshhpwt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2cucujwgj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2nenusryc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ffciindv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xsfnueni.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2trsrdkwt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2vyuifxhi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2gjqbjzpf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ibipyecs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fwfzfuzm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzhqlehj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2vwwqgjfq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nzgkwlnv.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2fprujjsh.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2rtsrtzpr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lmonggyc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2pmckykuk.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gthfttck.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2irctarsn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cbsgridf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2xajutqaf.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ekoqrndr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2xeqnohaw.html


<!-- 参考信息 -->