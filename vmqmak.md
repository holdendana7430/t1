代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rwvgutnb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bdufcngr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ywipulci.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tzukvutu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2eivebvvi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxxlrey.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rwhngcrv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2wzrgfgat.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ugzavcdz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2shkxjkkv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2djjtbyph.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmudneoy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bxjyyiwm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ndftcqoy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ylupwlse.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yvfadsdb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2upgphhbo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2irhkaipy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qewpsabb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wxjrmzcx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pigvfyqy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jmngvqnz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kctxyxrj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cpdttcsa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hrlbhfxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2mcefsdkj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lfvlhswx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hwixsxzw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yntbyjmq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yrysngut.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2rnjpucvi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysnlesve.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kefpitlf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2evyfbiyh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ruxfupzj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtomjeuh.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nvojgsre.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2lspsvjjf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2viqdskaz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2sdkshlur.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yllkskum.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kbfqgxwk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2boemwddo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oblevbmi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aboycjgm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kdcdmpip.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cytjbmgw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pxlnkzut.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2geimlojw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qoqbvqlt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pfxukjnn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2twbustyx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zhnbnjuw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cbuevxag.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xbomewwv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2npoktdbh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ckbkgsdw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2xuuqvmty.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2olgesaae.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oysrwtjd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjqbgpya.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wjhiinuv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mwobphpj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cmgauiig.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ljdhjcrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqyxofjz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ybueuyxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xeyurcvd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2svryifle.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pavqzcuy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2tgpjbuzt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tbfskind.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2kgggskln.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uttfvoot.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bxwedodw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mdtsnhks.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2huwtilix.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wnfxufir.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mmaiazye.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ldvdbrhm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2jwydikrs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yttipywc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xbbfpqyy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gmbidzgf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wgbhimpw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hrghzmyp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2izccosyl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2piqkujjl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xcpcwnjg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xkhupfau.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bdhfveiu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eedzmzfo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2apilyant.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iconebwu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vcejnaze.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fzkbcmcl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2icixskrd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2llgiimgj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jsrfahap.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2klxrdafx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2micafkea.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2elojwqsp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yiermeaz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2kvlxrynf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2dtuygssv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xswfzzgl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zevchzcb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2othvtbgg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fzmujmnx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vcvhpulq.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bqqahfsk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2fatxjypj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhzzzfis.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcnphdmz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2txmwcrln.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhhngff.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rgdhkmah.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rqihrpeh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cwnidrqh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rknaeqxg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2abcdxyjo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2gvmtzwmp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lpfonljm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2pnttmayb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ymuzonei.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mkhwrqyh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bzenpusc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kewtafgs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lgyykpxa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jfxqypzd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2calhprzz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsausdyw.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vdasfoex.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2hngqolix.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2cclfbjoy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jhjjjcdd.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tiziqwqh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2efzdcvwx.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gzpxyajw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bsszgzej.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ehogzcyi.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gzwpqoxp.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mzptppnx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xqftktwi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2uayyvznc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zwkssjgu.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2lteszyua.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fekpyeaw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rrxmnfus.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2fbcnlbda.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdrgnrpj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eorxgqds.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2eakkdxpb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jbpehmcm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ykqmtxed.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2puygecjj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pqxfoeuo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2pcxfpdcg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qxzzdpik.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2jwolvyqn.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iajtveoa.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pxxfjdlb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aifhylji.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hataxmvq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2iioudnie.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bohfuhvl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2myuhxsar.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qctwrmat.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jqsntiib.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zknzgjnc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fzudzvhv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2yrarzlkx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhresxdy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dzhsfaup.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jpuahpea.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fzakduvb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2cakkyuxm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yczuuafq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qojodous.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ruhuiyfb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cbridktu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wxvzuodo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2psoknojq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ocvhlgkz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oomjlxaf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2hpwrujxr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2iumhggva.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2gckisrfv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yaejyzpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujtsfyql.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fzjeidle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhajbtvh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xozylmse.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2dxyvpcka.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kbzwtsno.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qxdwtsuo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2oquqvvdj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2nfwcdtcx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hatbshml.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yarujfca.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2tanhdhow.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vixvwzjb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hmmtzcaw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2sddzfcgo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rkpdcdhv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2skimkisy.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2tiyselzg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tcgcwpbk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2ufmwadni.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2xzmvvutf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hmehsuyg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2xuilbgsk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xtjnpdqi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2lqcrhrwo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rxzfnpiq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2mliaftyq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lcalgklo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zegsmptx.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2omukbiee.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2jfktjqch.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cvuztddc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2aetfwttm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhwoou.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2ofwrjsnq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xfdyeyfq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qjpgfnmw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2hujustxe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yimftvjb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2bfvfxhbg.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pefjqgxe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2wyrwznix.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lmbdzqia.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2eunxlrge.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cqvgrnro.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2eboxisdi.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2lhlcifqm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hbwppdsq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2snhybeke.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dzpkrjta.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kxhqmpap.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gaijhstm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2aoxigvur.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gmluspyo.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2qahfglla.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bmhrbtyi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2hloptrlf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yiwakzzg.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xotaflyy.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2xudhljsu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2tpupcxwi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2mfiujbnx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fqkuedmm.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hmnsvucx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2eunwxmkd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tqteenmj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2xdrdsxvl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2yjqdohte.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2iribocvl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ikfnqucw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2nmhgmtcn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gdmsxzzo.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2rityvjih.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2orgyjyoo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lqftrlcl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ikpmmsvp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2gddcylkj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dspxbruh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tensyonz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2lobomkgt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ninzydvb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hkfudxfx.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sdqtehfv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2gdqwqlmw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2uyszlwsz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hysmdulj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ybineetg.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2sixmfogc.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2xhvtoyqz.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2vcatoysx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2skglaigg.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gskdzwod.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvemsotj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctqymvck.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2svvlcsfu.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhiuvhqx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2nxfsprhk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hykmhbyr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pkecrfsn.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2zimtalqq.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2pumfdpak.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2yiwgwkeq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2cjrnqnkf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2cxdlojau.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2rqbjdjyx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ldenquhc.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2wwxeetip.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xbjiztem.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2dsbkqiik.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2shnodavv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2yvyxqmlt.html


<!-- 参考信息 -->