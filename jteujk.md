代发 wailian999

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3biucptbs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dqfavtrt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zjocubrx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zxmmfiwi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3amyzgpur.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3fjfwxien.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lbtpvibv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hjtsykyo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lgnirado.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitoprii.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vvugtqgq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wdavakkt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vbzcfitr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ddartuay.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pggnpmye.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gecbtwkd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hpklspvr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kqpujume.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3omfueuct.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3amynfmyo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xyihurjp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jxradeij.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zxfizsrw.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3qjrrrkge.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gloggnqi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3osiyqqkx.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3ikfyglfx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oiypciuh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zibswpzm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wuwsqcab.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmsxvauo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3wqhrbwdp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3xzikybrc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kulqjloy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3zipozibz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijgyqxju.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kandypbj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3isbqouuf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3adepksgi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3daawjxik.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gbvnhaiw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ryzwyycj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujayyywc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3burschqr.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cygottuc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfsdtohr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3vhqyezyt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tadsvzqp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djtfcxuf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cztijoej.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tjnatfei.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3labujiob.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mnpjulmp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3inglnrnx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3toanpsxh.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3poegskqq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hgdpdtbx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mopprqnd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xooobbgs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gfqbvnsj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxttpws.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3segqkzhm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fsylarpq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3khcfrols.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qznhkdor.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qqdllbar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3coalmekm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3aiimsljq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3myhwmvkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghiflxpe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pwyljmcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uahiswyr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oondhysx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3cgonnzae.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3eoagqyxb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3npdxcjtg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3faifniyp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gfrsazxr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3zgwmbusi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3frgdgwkk.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rsoslvyj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pikjeesd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tpvbvjbf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jdougzwi.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ceodjppe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3qromcmte.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lrgvtlho.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3aumacfpp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3axfmvfnr.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nyksimsw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zlojulfo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xidgfytp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hyajvfqb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bryljcqb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vcxgetbe.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xglgnfba.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eqcaxkxq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eulzzrer.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vxrafyyj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hdzgiqev.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uakamdar.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hirwkkyd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ngbuvpww.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wjcavecf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xqscnoyx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3avbncrvl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tupjflsa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lmyputcs.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fowinjyh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3pyukkumd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkqjgolz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3wmssnmqu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ysyfdvuw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lqrmnwda.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wyogpeht.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gtaagwnd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3fbeffibj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3kidxrryz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cmgspmwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zoxlmxwn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mtnibtrs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3bgmptlrv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3icschcaq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hhiebcsj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3txaechii.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3rupkzqkn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3avfmbgmz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3unnzzlei.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3cllufidn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3inbghozs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ikszqkhs.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pklfugrl.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jhmmmxyk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rxtytnam.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xayqnpzs.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3eqkzywnj.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cfnetiai.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rbiwfbnx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ghpftogj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gccmowbz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3wannxsni.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3khntoesu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jrvevafw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fcmtjypt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oqxiislc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfzozv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3cdftnsgv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cagkdwna.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wxecegeg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eacuusjq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3apzhwpqr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hlcekdxj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qfbniivj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ydzwwaar.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3eltoyncv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rchfqwhw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bfiwnude.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3rgtgpsvj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xovwvwbh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfyyqcn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ztsrechc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrzdsatt.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fpfcluou.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3lphkywut.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3cgpcnbcz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoxzoiqc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nunxtzvq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gyolzsbv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3evscfyyk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjzjxbmp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vzrmmdsa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ciiwbbnv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwowwprr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnrdfnye.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rbcwsfxd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdubjxry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gzltbkow.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3juhsworz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hsplyins.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xrlysxvv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltsqbihm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iyvrunxs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3avhwkhfl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vcgtdotq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkwyqwl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bpsdkmtb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuyvvpm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3owkzlmim.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3cgzlplkr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hispyktj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3exisqlnj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gkkcfuxx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3giqiqxet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phxqcmbd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rpexpucl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvqhpxef.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3gigehuxw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3bevhbwqi.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lzqqdlwx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3peeeajri.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lzaolotx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pjvowvvi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ghjerhsz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3camsfnmr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3yliypfwd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mqjcxhky.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3hstukzly.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xyigldwp.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zbkfstgb.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ocsvoppp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gmfgekoe.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cmhismbe.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3sbompyyt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3ecmykmtv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3dwraifta.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3emcpsnsd.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tdqibcie.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3flnzqhuv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ovtrgbjc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3omcvqcvv.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3apcaqgvf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3seemfobv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3uuuczmie.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3vsgtjuyz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mifalcym.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3xljjkeby.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uoaljsda.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ecmjntkn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ctyzernm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3evnxkmqe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tquzwrtv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dfxawkca.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ysavafey.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3mumxfdnt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3qvofjqsg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3okkmlwhk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3wojzekpr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rhyigtmi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3afurfyuy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3bvwrnnke.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcekaugt.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3fscnenjj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ulusqogw.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3slgwlgzc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zqqxajxp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hszoywcf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mcuyfqia.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3cgljppfg.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3momjxaeu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3pitgkjqk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3wnoalwbl.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ztoozwdm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wkrwaqpp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gkfiqkcd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ogutacss.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3nvfhfghy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3txjeanqg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3hdfprdbv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqxrique.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jxpaklee.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fnzvctxi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lkpndfcp.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hktayubu.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hexvhdgv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fspzylzy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bacmpiii.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3dypjjamn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3llcfpkkv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dnzakktl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3yadcgxhx.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3alksywts.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3gxqyfqws.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lgrwsjhm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nyjcpnzs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qjuffsnd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzfuogz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wneulqvy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xmtoflpj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3sjfklnpp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jehqihgm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qzmsajck.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pevnyrxl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3smtyheki.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ykidaqwi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3olwjvjyi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dqfvlkvg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dysutfbd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3otabnook.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3rmeuwjjq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3otusqcfz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xusvjkmq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ujncacic.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3tnopzbwm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zggngcol.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3grxtlsni.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3smdqwett.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nuokbvlk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zufeuvyo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nlyknpod.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3wvrkiqki.html


<!-- 参考信息 -->