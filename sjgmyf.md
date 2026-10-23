代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rhddcwue.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3etpysnjg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jmtmvspk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yuhnltfy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mgbyoonw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmceinw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjcmsxvb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vxsrkzon.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3eyukaoxq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bylwpurj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xvagoctm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfyxvzy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cffdpkxu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3snprsnxb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3etmmijrm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ecwsuanu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lisshuvt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3akrgzlrm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3xwxtivup.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fsjhgnyx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3izyfvxnq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3johdgpyx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3cnhpjjsd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wbnlrxea.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hdgxlvdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ykpqmhti.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3uilmijwi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pxrseztk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3thebclqo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kasmdarw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hccxhjhb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3inisilfs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aqpamkhs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rohhxmyl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xcxbaqkk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3igflmcrh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3chqgkmen.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wdfqehbl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gbbswvxm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fbgljhnj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgqvouq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uebvepnd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zabnixne.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3isgvezbv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztngfrhl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pwajvhew.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ycjxdimy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qjvouqzz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vkknmgrj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3falnechk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3joddknog.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3siiwftzt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3khgfolfx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qtzazecu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xzpziqps.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3fqjedpwt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3izvabluw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ylmeytyf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ezfevndo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pqptdzpc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3opvjnfmu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uqzscrnv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fduvmorf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hxbjqbww.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hajetsgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbncxhqb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qbbmjgtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjwhllpi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dxfdczpl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ctqtqybh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qywcexgz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wngfmcib.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3aranbqdz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yfyftlel.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hqimgiaa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3glajcano.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zztgzdwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cicqlcxh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3asvtopzl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zzrudwct.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dqxhulmw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3goyrhnyu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gzabethj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ndxkfxht.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3otfboqre.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3xxgmcvfl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eweesnxr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3xndzaxmp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3myygysrq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xyhzpgyq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xfcvfcxu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpwpsdkv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tskmdicq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pabdudjd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fpgvywoj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3trzdbwlc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3whpklfsd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3oumjracu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xphskpww.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tparsjbi.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3vdlypsfd.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lgdfstlh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wixeblfc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xugndhya.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3brbpipop.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xmnazxsk.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vxlzdfif.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3gtrymwct.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3tzxjmdfj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cmrqwlun.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uhrgicol.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgvzzxxq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3mzabxqql.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jhsjgnth.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3chbdsqgf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tarycvpb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3lwygjibc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmjgwmn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tkjqwqgh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tzufnscs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dehvaeem.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ncteigbe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kddozyqy.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3wczmgxzs.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bynpxxdj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3cjpzfpzb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pbvwwsia.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ghecesct.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zydpmdph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xkrqiesu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3neglywiw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcsjfmvm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zlgdnqbv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fwwngeeo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wgazjegp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3oxlkepku.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3aicrihmc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mjhylmlp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3secywkpg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cirzfold.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gecgaozj.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3foojvxfa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aocjtgml.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3okazubya.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vnhqgbhw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3veuueeeo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ryqphoxh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bogxexjx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tdrrcbpt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pwcpfmwa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3inqqvtqa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ykronleo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vzikunxf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3irogeqqs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3punvzcnw.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkndtfyd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3noazbdqb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ytokxkii.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ithjcsml.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3nscjlnxi.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3zemdhdtt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkgwmcdf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vesqtroz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tfhcisst.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3prtnkdox.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zykehxtb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3odxgvuzx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ozovptfc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhzallkp.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oiwdnlov.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zecuhjmo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ukjnfyng.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eycjuoyr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ygwvmvql.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mvaojzmt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cqyvisez.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3csqvfgmb.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lorzkhij.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpgvjyej.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3itqbvhhj.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nklpwfns.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bfncnkxo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dstaiufr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vkcjjppg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bikdpgxz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywxfnfug.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nwuzfkov.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bjfjised.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3daopbcqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgledtez.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gziphphz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihpzlxqr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3wynjdtqp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3fzelmovr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rleygwtf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvtqzljk.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hyajzzsm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3xiskmdlm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ienhdgcd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3dwaxgfkn.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3sjltkgto.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3psicsmzg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3npxlcaji.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xhhgskoe.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ezlclbme.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ocffumnu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qncdoshk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3wcpxliwm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hloemngr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ygcsrwin.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3udplsnko.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xixebgck.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3xuzsligv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsweqvbc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nddhniyf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3awovlxmy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3enyvqyzu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3phwzudko.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3vifkjugu.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yhrfbytv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ppmvqlcn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3juakcyky.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3pfvhcseo.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nxdyszzn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ogsulcvs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdxffuj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tisokhen.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3idpicbyt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mmxmmcnq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xmmklvfx.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dwakbpao.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hhrozmpe.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3syjqehsd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3mqmunexy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wihejjee.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3hbaiekbt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ftiknyzk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3httjgtbe.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bfwbckxq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lcnnjojs.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3jxxhekur.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqnkned.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xtddxyly.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ysmbbavj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3cmfhnykg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3astjsfcj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kzqxszla.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3fcqgeyor.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3gsufsepy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ogbeeuxg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mdufwsav.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cdupqbcu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3shsxzmmf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3admdctpv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hghwgati.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3fwjnssnh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3uhrbwttm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ozrdnbuk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3yhfuceve.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kipkzjvx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vtzzkahg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sskwphad.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3fruzsday.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3paehvayo.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3itpqsagz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rstbuiot.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gwrmbgxf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3psxpkduf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3fjrnjirs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3tyvbzmir.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3roekuvse.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lweazzma.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tdvpvwqq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dqvowuip.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zncvuryo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gzumxcxg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wmipdypt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pnjeebes.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmpkeprf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jvhebxpp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3psbknfiw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cerdyhby.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3aampjfnd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rcovfxef.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3yghakbpy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ohkxlvdb.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ncioatxr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotmlgkx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mqsenrxd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ocqdlfix.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tgsjeuuu.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xbadqcut.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vdbldxfn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3snefixmo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3iiugyfuf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3maxbjxqc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3edpujzgn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3suiycuko.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3vlomyshh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3yedybwck.html


<!-- 参考信息 -->