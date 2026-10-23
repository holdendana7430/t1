代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dzaksdbw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gtcwxcft.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uwnuzgwe.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ujsuklva.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zhhsoheb.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qsjshjjw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ysztidru.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwrnqmbb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xozcruyn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bvvfyzpe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3efauvcwv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tmchpqjw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3tvyhfhsa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ywdnymur.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3obiwdqvr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hsmeoekq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qdoasmis.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pozkkczg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3uvldejnq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rtjnoaev.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uwpeqkdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cltiaxtn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mdziysli.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oygoqvxa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cvrufpzv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qpqyymhs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ojreemmg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fmscqovi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3yrphzgid.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pydjjbmw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aeylpvca.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hqtpltmx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kuobsgmm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3atyfdvlz.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dpzoidmg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hcrkhcnt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppshtfxx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3puwsccqh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nnpslahf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ojzpevpt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wxaewgvk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rjynkugn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wsbhkaeb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeovysaq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3crbnzsqa.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bpzrfsno.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mbmjdvkx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3elqkxndl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcdomexu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xkcoomdx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rebkbhak.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3okxmiblv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wlgelmwk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhocyiyk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vcqyrago.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ozkggmny.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3klptulqk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jkiwmhle.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3adrxvgkt.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wulednks.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3wxyvcerv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3veimbhgh.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nlhecpda.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gmseeaud.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ookdsdot.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wqgbcfgo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3kivrspur.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3vhpiydyl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3miolqgno.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qnvcmstf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ffqegjdf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jfvsfsdt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ueyaovkk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3eyaydvzs.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3jkchydtw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxdduaek.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ykgnbbld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxhrbhgm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nlibhpma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iadogjtt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zowexwaj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3enlvpmdy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wecqoivq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ysfglchj.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3qmeflcdn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bachdbab.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rqozkigf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jxeglzae.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vcpwuoqh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jfxgscoq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xnrvpjiz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qchomlci.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3grgvznlw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bajderqt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vygfcxak.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkdbojc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzjmrrga.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aczszzxd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ttfpkpgn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ryykdcnc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gdomnlbm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pzbkzlvq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3habofqtw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ojnrkcbq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yebmjsjs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxcbmqqx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jujsweil.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rukqlush.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3defogtwa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ogqdooxg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3irboedbn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwbnadu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3lthlxcdw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ivuphaeu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dkeaghel.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ayvcvqag.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wvdqytsg.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wnjpqwnh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ogibopcx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3evnmehow.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3odbyotiw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3dshntvrq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3whjgmeyj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgyngzod.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvaiuljf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3opgdvnuz.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gqsugdqr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jbqeawqc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jnqrnsqf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3dthzwgfh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zdemrgsg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zvhgiodq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eiejwnps.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbjgapi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3todhjfpe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jfucddgn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ofxawcjh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ebbmtygq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3emxlashe.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3mdchfwgo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3beqygszw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oqwmuqej.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tyzhzknb.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkmnsijz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hkmxedbl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3ibvxousv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3icaoqqth.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3qwsohjtk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3sqtyeqqu.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3oqqavwbw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tmfdosjx.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pxszxvxo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lcvmdnds.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3clpquuff.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ofojxdhd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bsbpohaj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3luitysgp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vslwpdxd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3neextwud.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xrzqwwei.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zohwfufm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3kmzeuajb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iaptrqog.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jzatofvl.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qbirgvle.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vszgstht.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mzcjjeiz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fxutiqty.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrfuupcp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3xserksyn.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3yrjqrwqk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xxcvszoy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3xchkxtwc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oolsihbo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ldkrgjbs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3utrywsos.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3plvsfduy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bevqlmlx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oukexsht.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rebojtfw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jhcxviyw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itrgwseg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wpmuacow.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zjoqswir.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3edrufzyd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dkwrobvy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ceqvstdx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fniizdrc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3flczueqf.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zcaswznk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3wtshdlns.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vfudunlp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3cdzdvazz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wzfbgjlb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hvteicpr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xyqfetrw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kvhaagie.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqmyqtut.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vvmjfkzo.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jopsjepn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3msqxhjxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxwnpxra.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dpamxzri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itawxwdf.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3twmqvrsd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rywzlysu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3arxjrwyf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xpavoisy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mykmyrrk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fokpnwmg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3fgziondh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wthohboo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3kuzllbaj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xirujdcu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3plwdwqad.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3oleuzqoz.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vvkourcw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vostsjyw.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3tcyiwkgj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3thejwuxk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3phdsmrfy.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3rhcsscys.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3mywgwsgg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3osocpsja.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yooyofrt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzzfprr.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3hrhnvzwg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3kdbytnmu.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qpiielwl.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3whpkrsks.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ahdyznxz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3eypvzbzi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zejotolu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ytjmgdvg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3utiabxii.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3azpttxzc.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3hqhmflfs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwdecmi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3difhdyzq.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mlmogjaf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dhflqfta.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujklojwv.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bmvxvvzd.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3izrbaacx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3fndrxzdp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3xiaqxkau.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kzcshnsr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3uuvpjpyr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ydnruqce.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3szqsovxk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bhngxxnj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pulanfsy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xtcvnebx.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zcyikvzu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3koqzqblm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3azoxrwid.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3nsjjdizo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3ioqcttpf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vdudvnks.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zgyixili.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3apftptpi.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xjsvqcpt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bxdgcbky.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pviineec.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ncruvynj.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3yoefxkvz.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mfgsxzmt.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iuabulwi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cwvtciua.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3kkioukac.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xegafxrj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3wwlncqhu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lkmrjzla.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tphobfht.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nnoihpwt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3eqtpurus.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dwxuihas.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3pqcdosjf.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3opamdonv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3yjjmaecp.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3bvzlgkzl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ctjboqdl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3blkgirmf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vziesckx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lrtrkarj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3uxvtjymr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3kregwvqy.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3znvjoepz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3cmuspkxa.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3wsevfbpp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3cyqfkcqw.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uirijlru.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3yuttcqqi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njgxqbry.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3mjccuqxx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3rtkjpbtz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3hxyafidy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nwmqipnw.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3xqxmduar.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3fdbsackw.html


<!-- 参考信息 -->