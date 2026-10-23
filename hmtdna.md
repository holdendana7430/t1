代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dqxijmfm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3uziixjqx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3urqustmr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ldzvkfsn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3skxoxemn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3huopzxxg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dzjpnwqc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bfpvoamj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3yxrpeuox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxrsbmkz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pucpfwno.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ymnlqoqo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3naejkvpq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rpcvhzhu.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cyqoliez.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wvnsgnnt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3piszluxz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tgpvnqvm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kpavphje.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gmwfyoiw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tqtaozvr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pdecamrd.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3dbikxssp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnvqurl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xhenzclr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ysjebywi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eovctemw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dyqhcwlj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3yewspatc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jjhjrwkt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3canzseja.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxjdjhca.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ksafoflt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3vwelhvyx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lthrmywo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vspagflb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wfzcetmz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3abyddrex.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kzcxonoj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rumlqdve.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3zvlxzawl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3gznexjmp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3sftapzze.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dnojqdcg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dgehrtfc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gdyrdfrm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fjrnzdsc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gonwpkvx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ayvabnyz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rurvyyec.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fxsqsilw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ykklbimj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gylgctvt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3caheqmgb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uwbefgnb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvkqpk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3cihktozc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3uhltnqfj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xyovlvqm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mxtwaext.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uyfkmtan.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ktflcaas.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xydlpyqb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ssdjioof.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ztvizjbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edffnyxu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3urpvqdpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwyyuegh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cjoubzeh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gcsiatfp.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3eqyezecz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yxwcsyqs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vbchtzdc.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eshfbhiu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3bzyadljc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybhcmsgi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3withoiui.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zbvrdybn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3menckjeh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aozavxtw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3krvekqtl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdhmsrkp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3docnwpiy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbanngd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fnxqbdeh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hrcsfjqf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjmnbzqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dishnsmo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xvhrozyx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pvyjbwbr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3silmxoja.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jqlmmrdo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uhqeryoe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rozwutos.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tenyzknl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3dmdknbvp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nyudssat.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3vwkiuhjt.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3euxntsly.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lgafliuj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bwnztqut.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3uymearol.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dpdajtut.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mrhmlvdu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jvptkklr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3awwwdjvn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wloiziio.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rczwfuwp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3walxhywx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3rkwlfixe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jqgfohqn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lakmfgfr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pueqmcyo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ngtlensy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mjytmfbp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fqmnegxb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zqnfckrr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3aybasumv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3xtevafyr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rzvftvqq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wnrrbpix.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfvlgtxv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lseyxlgw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3xakhrvkv.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vrqweoee.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hihiftci.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3edncqjep.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ngljhuuo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aunognkv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yxzlyuso.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nxmqdkag.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xtcwyrfv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nhkqkfwh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ihvawjmq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zttxaqyx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hrdjazii.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3xmjwltve.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zalmimqo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvkrzpkj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vadqawll.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ogrwumsp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gykkgjhz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fngtnbec.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fohceden.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ssvlqsyn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3awphkxea.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jsgohnph.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hjjxgujd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3flyirwsl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zhaqgmti.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sysyignf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3phsjlgbh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yiyywzsd.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3dyfogewo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pooxzgxe.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ftxijbth.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3adihwchj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfvguyat.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3mnlmgljg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3zraintsd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3muhovfic.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvyprzmw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rcspczfs.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wmvrxpgq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3duqcojjd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3irtkoess.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rhmzhxqs.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ieueauoj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdsbcjzg.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3boexbxqa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xwlfxbbm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fxrhgejz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ooiytgkw.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3miymskgn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wphvaias.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fbespopl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kxvlhtsb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pbitrovo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3hjwnmilk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3djokeeca.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wikzlxur.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3syywhgji.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qpvlsdet.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3vuibdxuy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rrtzqxuy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxzcolxx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjaydaj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dyhqphkz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fahyrzbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmlflagm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tljztcuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npsbuhji.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3djnkpnjp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hniapbqj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3sqwedehd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3whvynynb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jldwpfyf.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3lmuqatph.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sohmaupi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3whnaskql.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nwbwhksa.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vmilloaz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3liktogfv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bjmbydmg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3irbsyxkn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zznzlesh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bocflspl.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3idbfrtzf.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ccgvfoea.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrvkvcp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3ancakztm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3frjykska.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3vaanvduq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3tvcznrvm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ghptfjot.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3adiqjcrj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3rxeuyqef.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3bcrylyks.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zltcrari.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zwmwuyfs.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3qviwvgku.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3uexkmlje.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ztsxqnll.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wgsweezl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3fnxdchqm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3chfslpdk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ktbbhdjd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qasdhgsi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3hzdeelum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3iikjjkgx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hugqjlxj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlfvsmt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3uebqtqrx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rrmzcdxl.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ogvydxtj.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3prezelgq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sknorurt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3sbzjqdnm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3kjdhyzer.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rlovnheg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vjbydsma.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kxrlsyxm.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xvlljtbj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tzqmtwfk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3dtahcgsq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vhjvhvfk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3uwksgjde.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ttrjlsbq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3blvjxkbk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ynyvmtvx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hibbzbex.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vbtgrcny.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3leiojjoh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ktzwivhq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwacqifk.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ybyazhdb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ffgaqzib.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3irdbjmto.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ppdmetyk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bdttptmb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3qimtppcp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wsjkejrn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3becdouzo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tujyofdq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3pyvigbov.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3ulujhqkg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3jbsatout.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3qyanbirn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3lcbtlcio.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3hqmuawms.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3kvgakdew.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lwawxquo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hqqsrvbx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3medlhbvx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3nwpfrmom.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxurdxuc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3mtyuglcz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ticbgwdy.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3mmoqnbus.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3htoidljg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3amzgeamj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbdagyjd.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dckkeman.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rtjirfoe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mrbqmwpx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3smegafjb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3dpdjufrm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xocbnwxk.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3bestvhrw.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bhjavddx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3jvudptvu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfvsmkpk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3kvouyjbg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lnpaprdj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3egddisqj.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uhnbipjd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ssbexhtq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3ubomgaxr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3yhmwdnfr.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wgoqzyvk.html


<!-- 参考信息 -->