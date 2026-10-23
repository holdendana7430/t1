代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3utvcivvc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3colzbizi.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wryyvlal.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3auczjawy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rbknhfvk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nmdngwxl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jhcyrwyb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xjvvjlcj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hnsnccdp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pszwhgwq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ohoxzdpq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3evravkmm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3aokpluya.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cuoutkts.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uradzlcc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hxrzcugt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3bueemchj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kdzzxzcj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3pavsvoof.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tanweifu.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lfmuritz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzmrkuuf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3sopwbcsp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cngmoznd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3wlhdcusg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xripqgbj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ucehcqha.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3udvadeyp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3yyaxcipx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3phgoiwfu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3whnhalpi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ogageyfc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fylchzvy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yfbsfazb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3itfpskrs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhaxxnyw.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcuefhbs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ojfxdoig.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3msjhkqss.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cekhnsch.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wovmtwtm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wsnfkyxw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3raaboflu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqoypkwi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tnsvcelz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3aojznefq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zvyvzned.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3uyecwauz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3gzqtvrks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjejljju.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3urimdgeh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3gutqgiwv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqnmleu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmnilten.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fwpurfgs.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3oskznkep.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3asiaxwdd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ggrtcsvr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3mvbgxfgh.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3innokkkd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fulvrtyk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3gacpouuu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3gmbspaty.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3pciobubz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3kfvfkmgv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ulamdsma.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nrvqqokc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cqxxbkhc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pkgymytr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tlwphpgn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vsaqdvkb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qaievuqk.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfyjaipx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ifdnkjxs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3idgymhtt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3docqarug.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3acuuakec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3higkfsek.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kevtbjsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnvlpuit.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ccdlzclb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bdrtgycf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rtzfldzr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3rxjqpwxe.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sidktiht.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3avlhiqen.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3cltsjgxc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3etlatvdf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jkcxfwre.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dgcaxxbi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jajcleut.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vjacsohz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nwybtkoj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3magprnbh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fwnmxmlr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kuqsfaae.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fpwhuhxf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3xoxtvddu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kodbgzjt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3cytxkisf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sesboglm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kmocwlss.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3rprprfvp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvhpuqz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jmjmpntg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nyzqrkff.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3loiyspuv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tnddmamn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nhciaclo.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pomfxthi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pkuprvcw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vbrpmrdn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3bumcsavk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ogvelwyd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dpwytmgo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mmzropzw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3uywahrga.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3noggxoin.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jpqncalv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zxvghhyw.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygflatqg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zytbjpio.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fvcrsyrp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ywyyuizq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xhiaqdys.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3cdkwjzjf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hahxlxlh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qvrgmxsj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dzmdqhyi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jnlmpoxp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ymcioppi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3utqqhfxr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wzhshvvj.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mejejrob.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zbbcwqoh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uovyuorm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3lofxozux.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gzlbgbpt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kulwkyjo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wkxvohil.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pnhwsgyz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hjtggptn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hrkgrcqr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3nhadkslq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zxwpgzng.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3meircnuq.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eeecnyxh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3bkkyzvko.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rtblramf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3teturefo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3rjvytkcu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3poganaij.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pokkjspw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3recdncjm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nukufoub.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xcfswkqo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nfinwccv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3auznyqxn.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xdydqvbv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bvdlqloc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mleozzqt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iztrwzml.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cafpdacv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wlqiznsz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3igypgmqi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3tjyarrnx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pmgpmboj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hjviywro.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3xqbgvsog.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ufrvocwx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3lifanckd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qihzpvkg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ssounnri.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyfaoxal.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xiluvbgk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3edtyynre.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vssbawrq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyreyhpw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3klangbxb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dmuhtjrr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhjttwxo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3acwjctwu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vrdbkojm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pvdcsfmp.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rzognwsr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gtqqrqpi.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3znduxcsk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3aqwgsvbd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pekzopwg.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jeqtoory.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3iryolwjm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hapcyaxb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3syfywnua.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xlfxrujo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gknlimbt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wvtoayws.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3eguurnxk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ezbcajjd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ovnqawey.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gittwwjb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3yptixwvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbjlcyom.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fxjchleh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rsjjrggw.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zipvjxol.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3qoqtmjhh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yjfollux.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bqcrvuli.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sdbujlkw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3jdpoxlmn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qnuxixvp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3namehggd.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdijzq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tuezjopg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3pahzycsn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rdrpjdgt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ijuoejlr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hnagwhys.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ciqjmqcv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3uswuevrj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3kkmhytap.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tboysjsz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vwcmvtbc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3aroicakd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ibiqeqyi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eocyzndk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ohmeccyc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3gwpkucil.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kezrkxaa.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wmgzapjz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3qcgfwnpc.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fbdnxjex.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bxenmzyj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3zgvfghfz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3alismjst.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3wrhtfxyr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3axdcrdsm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdkluxc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lyojrmfl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fkdpwmiw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3emuahnwn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uwulcdpo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bxdgwmqi.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wdnyrejh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ikyivxuf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fybczscv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3oqiuyutk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dgjnvwct.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3epfjtypf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3hwnqlnwt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ayerwqci.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qydmrkxt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mmbiqaqc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ptxspmss.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3olurxmkl.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pzkcngwv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hzgmgfca.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hhtszmpg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lmygtekn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3orcxtrvh.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mesjjhho.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3plobwvjr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3umfgulvc.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3bdzbduow.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hyttklfo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3xdxksxvo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gwmvqxzq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3cxhsotfc.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3elkoqsiu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ramgvulf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vrbawlrf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ngzvpkbk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3kdnvbjqe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vzykrxgj.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3gdqsomga.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3dtukwkjx.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ciayvtgj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3xwwgvdhc.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3qingfzox.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ittkrazw.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ejrbzrgl.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3iatelekl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mlrxiohe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bflmisai.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3eilqmczc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3unqlfsqn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3johforvh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3jrrfnzlx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rbmeudcp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3xunvsohu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3scyagdfh.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3szoueheb.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3wofiqror.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3djnovdgd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fjrjuyoj.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3csjwdhdy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3exiwkdhe.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cbyutzcu.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ehjvogce.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gppmmkev.html


<!-- 参考信息 -->