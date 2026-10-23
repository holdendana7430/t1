代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vmllzszg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gtcbpjeg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xifbyiqn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3eeyknyyo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hxxhjdjz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkkeajzp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wdzvpfmv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3kdastvvv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kdgzmltc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fdfnpqdn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3eyveghes.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dykoamgm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3tjcjlbjm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3uscmkeae.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3inqkoizr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bpmuweuw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uewaqnvn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3szuyjyix.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zdbkhcet.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pzhcsipx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3alrtukhw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mwixnwmp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3fkxxbtaa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uoxeugno.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qierpgpm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jvosiwtx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3mrbwymdd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mettsybt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3toskufuf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3svrdfmde.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgpvnqsr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rnrfsriw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bixiajvv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3tusogbiw.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3kqawshtm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hunyopat.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ptfdfbab.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dxzzmtls.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yojgtnqe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zfaczrzo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3spuruhlx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3gzcfhctv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3glcrzcqi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3glovstda.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hitbjtxn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3poliuezq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ffnpsgty.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3acmcijlo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fhshryir.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdcqlwgv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qdxauvyy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wcliauvy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jwwajegu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cggfgwxg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ozcsfhcx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bzmuplao.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xklysagl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ttlyxptt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3mlwneavw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3udqyzazu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qhssnyff.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gvalyzmr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3lundxrrb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3orqfkhvl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3geunmbnc.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dpklhitg.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3pghgsgcz.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3yyvmlvpx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbdiivn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3scrcxauz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vqdbokyj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lapqpwdd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3slhppuac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxquqpwy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wkhiwytm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnskssoh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dwiybskt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ozvfqivq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rzqkhgdl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qnxskvcs.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zcvathej.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kgcclbai.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rygetlzy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aekbmjrw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lujsfpqb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sjkljtsl.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3qcfgxsls.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ayrxatff.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zhbymplz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nolsgarw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kcqbyvnd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rehwhswn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcazayga.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hfvaabzv.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vfpwzgsi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tqyxeydu.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fmqnzjlg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3owftstbe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qzujemrn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3giktlfkx.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3bdwvjhxg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dzpqrfvm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ijqdkdhu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ndfdylwk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jlwzjmnn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3dlpzqbkd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3knrfzvqa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rhsxdszr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pnamjexs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nybtytei.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ihbebpjc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lwvzmqbd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xacwiqqg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3jcwsjsoa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xgxpveav.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qucbottc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yppqeuwg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3osejlmfg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3cwhryiwf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqhgaesx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqiuetyq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rmkipbwf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pzxfbuci.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dkxgzflk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3rqkjyjht.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3sxljjptb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3lebjbcnq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3luaqbqua.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iuqsbobf.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojiyjhup.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rjzrxlso.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3jxwksvvh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3vbqjtgkq.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yyitzmwk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3opsmwonr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hgpeyvrv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xrdtmsfm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cdjjtgwy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ghziwtfe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyuxduan.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mmogopdv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fkqpxrwv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3mlxxybur.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pvxcinuh.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nvdlifou.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xgwaittd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qmvdpdsh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jtckmocg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qaiugflg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ocwedkeo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3yncjfhor.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ziddhdsj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3toyyvfgv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3fgwwygep.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kpkopvia.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3inpshijx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kwvzyafs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dfedaspx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rdjonxcl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wxxugruc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ippiepow.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3oggmtxid.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dkommhtq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ygorjxfu.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wsbtcjne.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lpdsivxz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mgvbzydm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3accqszll.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gmjdiywm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ezzfcwkm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ktbutfna.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3mrtnqcnc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zuvmphcn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jawantfj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmsrdpyi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3vsybpgcc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3chwvyabl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iydlnart.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kdgwcefn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hlsatpei.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wqrfxars.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kenraark.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3lhogudmg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zmxhkihh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vmzucetk.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3lrkfmllo.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3uzmgrcgj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3biwfkdfe.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kbcbsljk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cymotudh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3divgkrde.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qadopltn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sttzahtv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3rbppxikq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzygxob.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3kmhcwdis.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kdwqrsen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tizgylxb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vnvqiszv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vulrrtvh.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3fwjxxisw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3sijqngef.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlovtm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mkhcsckb.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3eupqvqyt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3wanmtjot.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3gifgdgvw.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rygkgasd.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jzrpiayi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3blmjwhue.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qptmjruh.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3niygxrnl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lmxcbjuf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xynkcntw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3oxsbwnjj.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3epvhyjve.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3tfbkqwvt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3mdxwryhl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nehpmirn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3wfrtacuh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cgpaqlrw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzbkrph.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3azkiwthq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pitwbhpb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3ovtjtpko.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3efocodcs.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3abztftyk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3iljcomby.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cmkncfdi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3czdnxzzk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gjydsekb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3lqqilaao.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3cjujanhd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zkdptiwl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3xzmanswv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bdnmding.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cctifuhw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvrcfoo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3cyhrkntw.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wldjmdhd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3jcwuvnqt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3kfpyassw.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qcylulfl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zdsukadh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ycccrlkc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zvdbkorp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vnsjseij.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wikxpiwx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ycnjczqv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3emokycuv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3imopjxmu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ketehlmd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xpsvdakh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ysfemesj.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cwngglwl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3kkjxwzih.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rwowlhhb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3owtuwkxy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tmkfnzth.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3klbbfacl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3blekeiug.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3lvjgpynv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3kihzbgym.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ljnclhyh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3sxlvqswl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3psmzqizq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3eubukdvu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3jswelcsq.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3soudbjhs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3cfspykfi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xfdybiqc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3fexjruvu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vsdmynzj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3cmeqsnad.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tiotbqbz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3qkhptimg.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3wmkdpztt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ubsvwxuv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3knckeppb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3qghwtubx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3wjlbgeho.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3tvmjuuck.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3yaanjxmc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3pquqdzxm.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wzorkbyq.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rlbtgpzh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnnzgdzn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sohbhfkj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3qkrqdikn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3smyrbiur.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivvmapbd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3truqqwzb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdddntlq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3utknjxsf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mtbvmbam.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3zthrcnuy.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dsvvqvqd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hfeafqxy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3pcmxkvyj.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3mahkceor.html


<!-- 参考信息 -->