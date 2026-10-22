代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ntzbfdnm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jcbqdcfb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pxdpdlgc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pfnvbppr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mobzwbcf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ajszdqzh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rntiadkh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2maovwskn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bvdqbrfc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ycjbmurx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nkirtvjv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aixzlpbp.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hrznbngu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zumetujk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ellhrykz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vnghlmuu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2davjdzxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pycuivbi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cunyaihh.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2egqsfzfg.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2civwxfoi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yhtucmtn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cfwkkrrl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2utwfwukk.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwsurerh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qkuegneo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mjazsvga.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jzakqghl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2jeysdpzi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zqbfsypm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2iiyzckri.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbghyiec.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qnuvxyya.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgkdhwlw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aojhmvyw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2inhnmmbs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gaqnfirl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ejoxwoci.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bwtdngap.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2aqcczuft.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2uyqeharv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzmdingx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yxehpucb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2amvwapml.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tocsrhpb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2iayfrrii.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mjtlgrbk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2fcalikyo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqonabv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mhitwfdl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2zdbsxzhf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jgijqhrn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2hihhiwuh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gvhkdafm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpzibzzn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2opnjjsow.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kspnlsnp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wwawowma.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vqbyqoxf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iaouaazi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wdroytyk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xhagvufy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mbboturi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ouiqmesh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ozbnzkbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvpfqqte.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2otiekzuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krpcnjte.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lvksmxat.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ftkpswll.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jqmzdfdy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xyzlfimu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2zqiyzkxg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rzxgiopg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hjggpjbk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bwkjinih.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqwazv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2dgxexkdv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mnngzpfg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjgcudxs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pqgscvqj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2gnuyjkok.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2osrzswyl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uszhnvsu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kuvtndql.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dueswddg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2utmszuqa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2euyvimxv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dwncsoew.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfvtzrb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vebofxvd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptgbxkmk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yjhevaup.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2whzympoy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrakunsy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tyijyxhx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fkgyundl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2pfxiiubw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibejdfzv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2msptonbf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2orddlfmc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2oqkjphox.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xxcirgiz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ybtildka.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2nscbsauj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2yukqxhhs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mdgndrvb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kpidhxuy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hltegtrp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ftstqnea.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ptaixgxc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zalcamin.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2odeqnfsf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bvgzohgo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vaqtqbyt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aqzsibuy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2szfzcdpk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xqitdxtv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2uukbjwrt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxmafnq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2btdtelvi.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fjipiwus.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2wnkwxner.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2qxloaifa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2buraidcx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sxacfseb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2crizxmob.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2pbcyliwi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qgruixrq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mujwtwzv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2epnoscpz.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xncpfmww.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ixmhbeda.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2huzphqpr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qbulxgrn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lnbnjybm.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bnbulhfh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2exozonpc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkmrzzte.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2larlghey.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2iceohxmm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2ccatubqf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2lvaspqfr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ndutxiuf.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pmswsnxg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2poybonad.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rszlispt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2xyvastfx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vxcpljef.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ozucvzjj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zzamalol.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2balvmilg.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pbqdcqmx.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fgthgsuy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxgupbpy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjarigbr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cenmwmrc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vetgemcg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bqqdgitk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lpewqpzi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wgdocxnh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2zktvvxub.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2bipfntvi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qqodotxl.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2mkdcsdlj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xobwvarq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzasbtoz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qwfbvnvd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gddeuxqb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kwrrexrf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2fkrcvitg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qaaskisa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pkebvcwy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ytkehvmx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gbdbopzs.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2asgaezyy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ffwnyhpx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lspuumdi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2fclkqotq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vvpkmyjl.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdhkgok.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bcsbefmp.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sdjqwohi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2qzxlcetd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2adswsmiu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xcewthdf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wwvfccxf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ytlqtsru.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vftrfmjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmzopmoc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljoepbwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttkxlegb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2heealdlw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2aivtbipy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gfeveiby.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktnfxhsk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hvsrutfb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pkkzejpy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kgoosfzn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2xuzmtyrk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xpaeioad.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kpdecslq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rpcqyian.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2ugiulurn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hropjdnp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2ysefmukw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2uujjisfm.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2hmgcgykc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jqnlkrcb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhqvmoo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ajnluaix.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ypyjkunc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rpvyzsgd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atedjktj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2radgfgid.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cclvdzai.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gtmjjlwc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2sccvihwf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2yhaflwsj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxzzujb.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2atxusnwp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gwbnpsfa.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ddbiawvz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2uyixldop.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ljdhmvoy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2iixaofac.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lsvapzcm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wwlvosrr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2naqpvyzr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtknptbc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fkvwibux.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2eqbqbido.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jzkdqgdi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ybqqjxzr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2xiofprrr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2kefixoab.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfneqmuw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xgpnlyfx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ojqmjjeg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wrbkwugx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2urlynuuv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2bbfchdki.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2qovfuwer.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pfargkvc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2aovkqqcu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2pyxhmala.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2wxjubamt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2ekntqemh.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mywizzmd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tolsgydn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2icwjehci.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dtntoyhb.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ogbnttde.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2krrvomje.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lsumpdyx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ewvqjgnr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2lllqqsjt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fzlxqoss.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kokslsov.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yceiwvdq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ijstdwrg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2naslxfzj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2vpnpkiuo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2yqgjxixk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ywqevzat.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qxuvaidw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2kroophev.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2rzqajtij.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2usaszlyn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2hkimhdjp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2blytrxkl.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mooanoyx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mzufrdwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2gekijrch.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2yujbldwj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2nwkyonez.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2idproyka.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2iyrerfuc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nllyondl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tjkvmfwi.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ftagcnzb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2egnexjks.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtaixyij.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2xsyqhigi.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnzovifs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rwatpxok.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pqipzzrp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiuywpoj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hkmtturs.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lvfilguw.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2yrrdtgwd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ynswqnfn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zhxbupuw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2mxmpszln.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hmvlxslz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2tilhpjxd.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vldehdff.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2uucpqwlu.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qnljaxjl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2blxyhjok.html


<!-- 参考信息 -->