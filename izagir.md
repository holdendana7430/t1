代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zkrwnhhq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gmjzfjwo.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bosthawn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bkqreyxt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xjdbxhos.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpzwyem.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fvwhoggs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fbexsuom.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3woqsnqdn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hjncqhqd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3fdilgngh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkvwtgyx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vgxbasbg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbopqs.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lssxdbim.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3eaennufy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tpqhckty.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uqdjohmw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wjdyfbnd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rxmcvhqt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mayyvcov.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mxstrjzj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wkmpiyin.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xoltjzii.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwbnkzbt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3abwhppyb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkefev.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lpyiesql.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3yumtnigx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3oshldfbm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3espgqico.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gffvioxs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3txpemzhb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3eudnmscx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zqonxvwu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ieeustao.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kqxvgfiw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3hltjwofo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mvsgovcv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zarubele.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rgdsehwo.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3erwqosnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gjlgeffu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wxbqemtk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gynshkye.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zfnjqhyh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hiialmie.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wnrpdbfj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpfahoef.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3tvmzxmfw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ndwgzpvg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xqhzzlgt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3fbjhfdpw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vzmxhckf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3jdskiiyd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uddmaqlq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fvpuiorj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gnedqkzc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3altlkejl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3nowyhojm.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lgescgea.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wvsytzjh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rknlwlzb.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vmpczmji.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mddrmguw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huchidbq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iqoyksax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udufzixl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wkxjrdmy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmtwpst.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wzrwbiyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3stlvgjke.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3unxulqjy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ygdtqefr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zegjgmir.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3hkskdqbt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gvnqjlif.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3upzfkyfr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wvkiabcu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lruyqffg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uywzvqti.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wlseyjmp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zkodqtxy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kxbhwzzu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cyzxxkxz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3eykhxwii.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vdgqcdud.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wswphhck.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mmzeublw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vwhweqal.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cfhgcgwk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oqweovdh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zzwlerlc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hypyjdsn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zlhbnbee.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yflypsso.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kepkbprg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3swgcxueo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrcgifpk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zmfpiulw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xocsrvdt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3iceillwo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oubgofet.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gyoarsqd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lnktuyui.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3lemwfaue.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3nhvufydk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ovcbmpqk.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mirpubaj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3funprawu.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3mforfcez.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ciqtkdqr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3yxyrejyy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzwolvka.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ghgnubnc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kfjanznb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ezdfrxma.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kfkryfrs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wmnakwym.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3voriddyt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wzwbyibd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3vnicooka.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jakshiqq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3nufuguln.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3gbjnnfrj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gffporub.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xdabkaya.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3asthurgb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ubpewxtt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nclvsnra.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jsewxtug.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tbizlufl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ssnjvgqq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3oyttidjr.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3smxmuvao.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hsbhzzao.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zkutttlo.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tkwrihxy.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuhtmhoj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wgqwgiwv.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ynatkkmz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3tekutqbr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rgeqlzak.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3sfbudjds.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gpleleou.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3leqemdag.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qmtxmtxg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ickopffi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hpehpqvr.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ssxuwrvu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cnvibfnx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3fgtvyofp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3fowslyym.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ocvygtum.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3sepreuuc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3saetmare.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3gmymmbjg.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3unwmiyjc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lcuxdlhw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gillsvqb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpkdwl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zaafdbof.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3piqrbtlv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3cdqzfkmp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3iynnceqg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fckihhok.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bjvkuawg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vevbpxas.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3mempzdmc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihayrlab.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3izgfkqud.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdczgc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dyerudly.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3phktjmxq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mjmnbscr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ekhgizwm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oaiztrao.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxxsbo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iednmhik.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vcxxeogy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rolpwfaa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qiujbfem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tpuskuwr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3vcielspk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hyhjodik.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bnkoobhr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bicdpgyt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3homiizbz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lfdgtykd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnvqqhdr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mnnqkwfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tizufzlg.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mksrmjcj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zadgtiva.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3oqtveltt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vxuuuiom.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vrymkvej.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3waseyjzq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mmbuccwl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ksuywfgj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3jpeopwuh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oswgyivi.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3igggtcpx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3awtlqgzs.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ytfxorxr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ttaolwfc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qrdbgeqa.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3utgkdekp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3acctxfuo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pjcjvnun.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3colkbdjt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uvjblabw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3otsijaob.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zedlykmr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ohetnbnn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3grurkyvt.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ordmnrxd.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3tbdilkwf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ecjficjo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gijvqprw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bbdbxwdc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3dgpzqmih.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3guzihyax.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nogvwddt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wlydjrgu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3nhgmymmf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fofsxfrb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tyqafska.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kgmlsuxi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3bxyznnys.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gqsuefne.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3oouzkwvz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dgeknsao.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fowvkznp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xegeymoj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3yhslbsgl.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rdnhkzan.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3dewewfas.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3wmfudsap.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jbitddti.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3wcvowvrm.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3tcepnvql.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3pbjwpoax.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kbnohrop.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3jgfmqulu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3djkleuyv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kzwynapi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mvbhifrn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rlyrktej.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kcincqjv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bpefudle.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3oqfiagaa.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3cawkdhzi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3stxbjmcf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3phcsgdjh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3nicaykjn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3rsxrtukj.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3clnpczjj.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yzerpkxy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3midakomq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3opwwhwth.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3atqpnzac.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3rtvedjzc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wrgsdqwp.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3swpcrsif.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3wivddzna.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bbdgmmgt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3agihrefc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3agtdfrxs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jajtqmit.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3rzmqzjnz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3cesqaskt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3nwgepqkq.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hftdszab.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ghnohkjp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zsnvbzml.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aelvdsfl.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zzfisupj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zpwuivsh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iylcfuzd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3resmfqaa.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdeiwdb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrzcicbk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3iaztpprk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vnxejidv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3wyvkgvjs.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tnhqnhva.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsbqojqv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mwadezqk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3vqnejvif.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nsstrjjx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pkfkkhea.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3kmhifqda.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3twalnaeb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3umkrmoeu.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxxilvz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3hhqydulq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3smohvqdy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3wyuhgiyr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3mnynlcbl.html


<!-- 参考信息 -->