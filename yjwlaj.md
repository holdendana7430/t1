代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vqgtkpif.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ddygfafw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wdrszjbe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lniqueda.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3idzdwvwt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3akoikmex.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wvjtawvt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tugxwhvu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3erqezyeo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3poinukix.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tumfikbo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ulkkntem.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3umuwsbng.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gaykauhx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3fsaxeczo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrgzcsl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3dwckzkwt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrtuuesh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hygecgjj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mhttnnfn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3enmdhydf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hdcmstud.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pvzshfsh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjyxftxg.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zhstrdbe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ebwbeuwz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3brjewqrt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3eqcvotxo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mmtkubhd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xdvxwlgt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3msoedfic.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3shhfnnts.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3snsfrjyo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3wtzzromg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rzmmlquf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jauspyss.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ktazlljn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rrrngjeg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3klvtqvym.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tuqbavmg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ljisnutq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbjdmjny.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3frgafxgs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qdndjydv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3trreytcn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hpczkjvu.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3blvnneji.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3jxebwnmf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rbsxqpae.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3crlolneu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3edtxrkys.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qbkcaudn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fjrmtktk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lckrobkr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xeymkqps.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3djdfgfas.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxsqbgpz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3nyllldnl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uuokbxhr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ozghuxsw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nsulesfi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3araibnes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3enpzjrcs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vgcgvqky.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qusqydff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3echariqj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3soixirlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oclwisrl.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhbxdnxu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kcetrxgb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dnsrzaat.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cvaiwhup.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3adjptljr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wisjanoy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sfhofczl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cmrgyska.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ejvowhek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cnsbthyd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3iqfwymqy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvjdldq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ehnfiqjn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mhrentxg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fzkwqnmi.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mogotbfe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3oitutdne.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3zbmhiyje.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zlggkkwh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gsomsnvs.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lglqbuwl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3viysgbke.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tbdrqkpi.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vgwjklmo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3iezikbhe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3burmijpi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ifpxpagb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3paotosbh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3tstcchnw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iywqguxq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qmnfqzbb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bhomgtew.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ggbqyklu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qcrwusfj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mrqabdhu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ntkalaqm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3exjlhzqq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xfjchine.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3viqshesg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bscolpsl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qummhtbm.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3qfsczkyo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zxqhdtjb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jlyezvjp.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxjqlyfj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmyoobu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eqvjzsdd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3egsdkjcc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qlpfhniv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ljcipxzh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tiakabfx.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmuqdpt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dfryrwsw.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fvhdtbud.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmskdu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvshnwy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ngfpojqt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3jjykhgfn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ixealkjx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3elgnaxaw.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kegrjrjy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cvtdyyip.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ionvprsu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ehwtiajj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rfndjyql.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zeznmhln.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bvqglezu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3eobbqfka.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3iwgndqou.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qahcahgq.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3edbzecfb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3hcjrjtue.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kusweimn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3gyoeawqs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3liadvqub.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3feykhddq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3azvxamwa.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hzwyttpx.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3owupvxrz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ngenzaab.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dfkefrax.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3edybwtob.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwommqvd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3vbwomdlq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yntpreic.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kgzlhdbm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhpaxrub.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qujwpiki.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jljaqyjp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3salhtetb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3kaxwyrse.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3donzacps.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3wffwgbts.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xmudwumo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xvgwulcw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3iaralhcm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3aobvgnep.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmpeldld.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dcexaoby.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3gtdoinrk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxsuzqrg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvoecsmr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fxmkgyrv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3tkwyyifn.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xioybtte.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3guhjsazh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xqvundjd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3dbuvzqkq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lujrifck.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3slqjavsc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mtbiedhm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nxzlnnnw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ywmosgmn.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3uhhuqvke.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cbaxugng.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wzdgvmvd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wdhymxkp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wcgklghs.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3brooecxg.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3crqfxjbj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3bzoehdoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzojvies.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhmgixon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyfuqcuv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gnvkxqnl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3iyrucpzs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3broahzis.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3kksromdl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ziflurbd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3epmxjzbz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3bluqprtb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3pifcehta.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qoysjtcl.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rdyecgqt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rtveatlq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ugqkfptb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ikxwmrwv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nbqggcbr.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wuozcxkr.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cvmkosyh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jtmvnupf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3sepzfslv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dstxkkme.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qbejlyrq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ydkcznkm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3qvikjwmk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwslcljo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eowxcadi.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3frcamagt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlnnqvy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3eedjysza.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pjzvaxxi.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ashobihr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eiyjvhzy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lyznvphr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nshkvkyy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yprznbbr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkavwtp.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hbahlmwn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnwayzh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zvkmentj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ufehtzbm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3gblqimcy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mgzjciam.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ctvqzitf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3cjhpxcbh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kskxoyry.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3rqoergfw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3izcmnfgf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tkicyymu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3owybgqbr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tssuydok.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3obdeepak.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zutznqmv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lcqcmdof.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jertknab.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3aixqmqic.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3akyicrcp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uenbgtfm.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3btqthuvi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3nqaybqts.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3wrmfaiqo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3smpnemsj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwzyxwh.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ijqjtxnk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ldhepqhq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hryuzxug.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3anjexoil.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xjotwlrp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mjfdrkbw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3giwgcigt.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3sflfflpn.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pfyfddov.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3akwfefhy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zdehrzme.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkuczwz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kumsdzxb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3pyratkxc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3axprmvgh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jmvlkzbs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zwlzcswu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bxmkpwci.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zsfsqyfb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3izhdzlte.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3aggegrgc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nlzphrwy.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3syprsyae.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jxwwfesk.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3xmiesykb.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3yodgdmjw.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ecbryyjx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lhormjsp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3ojrnesnx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3veuszybr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3gnffwvef.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ltwmdwmy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3umwcrktf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rufdzdqi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yswupuhx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kydtvsfc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3euqosdgb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jvjlhupl.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3ulrxfnjn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3spccdsxg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3uxprcefh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3rjqvifvl.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3fvtdqgqs.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qfvswnmh.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ywqvyffs.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wsffdubd.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3fxrzwnbh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3izcsxdmz.html


<!-- 参考信息 -->