代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wpqbohfb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ipdfcyya.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gldzfigf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nfruwiek.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jnvaffka.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjeqqdl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nxjclbrf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3nkvdenmi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kocnymbg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ayooflwr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3drooeltz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3qvbbzfjy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3mtxjupcy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3klayrryj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cmrobvtj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpcnbr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ehirmqfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3udvpibrf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3avrzuxgb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sgodgrcx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kiamulvn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3gzdtigvu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3zpvfygdz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3scuhqrkk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xbsxhibu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vthdzwqq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wplwjhml.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rvochwun.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3gootamtc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hkhsukhu.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iqudbxjg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3myxbyiyn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3axpbyovu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cxcorfvv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zapcsask.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ivoirczl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kldnybrr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojrrvncr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dwhjqnkw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxadjch.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lsaccwfc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zgkeigng.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3netfhtox.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3xxnsmete.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uofyiest.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3fmjnefss.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nzokrgdw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yiwscbqj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mlldxomb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rmxgrkhw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3hnmtgpzh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nyuukfqx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gempzuub.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ireazxts.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ffjooqhv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vtjszdrp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3njiupmnh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bpttttqi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3stfiifap.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jjhsjguf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3azppzyaf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bprmdtss.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3dnsdzwgp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mottezyb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ksksakgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yelinofg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3elpysgbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sioxelhy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dlcettpx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3azxyoued.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkrshywz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3fovgnrcc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cuhjvobd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3pfnmmcqu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3juxmqves.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3opnbcspr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3bucfvjuj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pkegppzd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nqshrvxa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtrfqdxe.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wdlpbjhp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwgitqtb.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3mclhtqbq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yirptino.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrlrxazu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3viadsgbe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3prbqvbiq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3uijfjjdi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3kpogyggr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3iyqaegwy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kaxoatbq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3srwgjzrg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gwtolepe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aupixvnl.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zjzstqse.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3edrfhubz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3snonexlh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rzzdmgyp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sfzzrqrt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfqhatz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ikgnoqgv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3rjlssfcp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3txleshbs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3rpwzwrlw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nivdcmdp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3awcwmvqy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dstzmmoh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cperstyg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eiixfnxk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3cfacmlct.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wewelhht.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zyjodhrf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3antiuvyn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aiaynqed.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hhkxjpio.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3egcdtwji.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dofkovol.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkzbcvz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nhszlqtg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nkaqxjbe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ovhpxeum.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hpurozyi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bzjjqssu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hkrigbua.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jsuayiju.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqvqgmu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bfntbflw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3erqwbgtu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3calntfwt.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uardarhe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ijsjrgom.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzvbvhbe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pboikbmc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wwpoxyjm.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fdtjxicp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gfcxulkv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ufvjxntb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iztzmzdu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyavbvmk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ropnptzb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mvtsdueg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jwzyesat.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ygfnkcxa.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3muuxuqpc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zoqtvyfx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3adtobatr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3gvflssan.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zsrtvoqy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nkkytzhy.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lujlqxgf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nlpqwwhj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yazwbdif.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iwxiwaqc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sayejydg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3skhrvvzc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3vrqrkche.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ptannzze.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rljnbtyq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3asvccllv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dafzbmbq.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3xthkycrj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzbmxmu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3bplgxulr.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3hmrkczva.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zfqoqbuz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pybvttlp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fbiqapmz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rahvoecq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nyvsmngz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdzjuryy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3njzchppg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhibucbu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3tuirwkbq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3udbpfaxp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jnmwqsaf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3itowvjvd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3vrpwvftp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ztoodxlr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cangtncs.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3weitsjbu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dqjyjfcs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3toisqrca.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3piewnvzg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3lggtwhmu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ekmovzag.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpqewzrn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xuduesit.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mpauykrr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzdclpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxqrkumt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjswowbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqgkjlhy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3rrtjbwxz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3miosmimb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3pyqrfyxc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rbunzmss.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3mleinija.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3irwfvvgj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3khjsdwcn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xlxyjeie.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3cpdsdfua.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jtxvgudj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vfierdav.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3naeghbhc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3lbqytxlp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3qmlvwhof.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3wlblufoo.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3sgjzokbp.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xqyhkctq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxxzqrh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nzwfrlgl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qmgcbuxa.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3fvxppvlm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pjwajtww.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3awaxrccu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wtuppcwe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wuwwduqe.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jfrtqmcv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3urftumoc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mohulpsv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3hgvifvkp.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3vtljtquf.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3pujnzkbf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sqwdfiyd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hyfndzpi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fftkwkih.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3scutmkfa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3svqhrzaa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3gwdkerib.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3euhtgvrj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3soqzycjn.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nkdwgohu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hrmcvcus.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3tzwvamws.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zvdrcxbw.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pnptbies.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3iyqrroyd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zsnotnuy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3vdkdjcvm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kivxbqnu.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3pklvdcgf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3srvniekk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3iiungqcq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3haxcuche.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kyrxnrpv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3afkcwqto.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3sfrvckgn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3digwbolr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ibnekwah.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3tyfrwihj.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mrpgictc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nuhohluc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3aqofvxwf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3sxzlviat.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3yrurnjfj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fzshmpfs.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3vcactntm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3gcxggwyj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vbttztal.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3rflzrcac.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3otiqgsun.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3owiszpud.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3tbplnhwr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zqdtvgpk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mqdjchqr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3npcbumeq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3xpzreads.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3kqzzanrb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3dylguvfh.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iozjaldi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3hktrmmrh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dqsiszma.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xojmdmln.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3gcfuvvmi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sapuyqrh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3isltejmp.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jnxwyvyu.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tphztdqt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dsiivehr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lsxlzzri.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3bbsccpik.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3huriozea.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wffvlkxe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3hvlsljgz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sbntwnwt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zfcsdswe.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3apbosjfl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3glsdbihp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mawfjwdd.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3cphjzxdg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3twrzonqx.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3sjouemrm.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3npwshptu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3nvfkdotk.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nhsvzxsl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mqevjgba.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3gaxfzzib.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3jtuctdlc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qkbtlrib.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ptbqaytu.html


<!-- 参考信息 -->