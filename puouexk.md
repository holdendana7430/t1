代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gflvbvcfu.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gutjtzfvj.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gixhmugjm.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gzjoqgpmy.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gxsfozdlu.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gqcbcojsm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gynlpvaiy.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/genfshksf.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gfbhrlnyn.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gxoxfedtd.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/ghcvxwzwu.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gitseubeb.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gbyrdeztm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gefiuoekc.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/grkcttoww.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gkmavcgux.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gtiygalzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gocifksmt.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gpzznelzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gawqjatef.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gevicczeo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gtaurlavn.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gvnqgjyme.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/grdmeoknp.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gwtjxvnyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvqihaspf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gxzvugnfk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gzgokbbgl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gfqzqzmub.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gfozykngn.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gidjeifmg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gkcxbhgpu.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gqvynyktk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gqbavyhhe.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gtayjkjqh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gcfqosedj.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/giabdbfva.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gtyblxmbx.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/glltmslwk.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gmllyxmar.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gtsynvkjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gglivhdrp.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gncgogtrn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/ghdbscotf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gbyugosxj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gqviyjegc.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gnfnvjuvq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/ghvqgcshx.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/guctavqlh.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ghhjgnqri.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gjsanvqht.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gnhirqjxr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkgenyexs.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gkzlwxvho.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gqmykrasn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/glljyprwc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvysryva.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gvljsoubt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnxdpbgc.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gvddwgjkc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/ggeorhond.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gvnpjbplp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gjdlqqvrp.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gfylyhdcv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqcmvtnm.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gpnmfnldn.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnhsafxeo.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gvjazdioa.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/ghpsfhyyk.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gakqqgvge.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gvyvdqjxa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gbrczxmqn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gbyxhwtvm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehbvugic.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gmudbumzn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqyprwsd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gjrneroru.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/guvcrzfbh.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gbcdljcwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gdwuqujtb.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gbhwchxke.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gtrsleffe.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gsheuqiub.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gnlnvmxbu.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gwrdofima.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gtatqnmyz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gyzcfhqkj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gpjhdzyqm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gqnnfjcew.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/ggwiqivga.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gymbgepmz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxpcljzmz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gclblumev.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/grxknejxy.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gfalgwuow.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gcoioedgv.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gkeyykttl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gkgivyubq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/glmemqvcy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzszrldrp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gmvtkoozg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gdjbzqycs.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gdazhisyf.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gpnwkplmh.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gkkgqeueb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gaxbshjzx.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/guhnfgziv.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/glsyxuyhc.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gdvnfieru.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gtgzszaap.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gyfixuwew.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gndtolbxh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/grxgvdwyy.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/giaprbahb.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gbhyfhoqv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gtdczfini.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/guvqkrpbx.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gpgprbnuq.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/glkatudcb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/ggygnzcpz.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gqcgpysns.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gxrnzlzpn.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gxsxvgmym.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjzykgsnp.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gupptobku.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/garzfnmlb.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gmudmbefr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gddqyszxq.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/grkmtqxlk.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gzscfiryr.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gpuhyfxgg.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gcwxiheux.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gtelsehrk.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gsbrrjyzj.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/ggzqufugu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gofylpltd.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmxihwwal.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gkrltlqvz.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gkzwdgcea.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gipgygovs.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gnanmqvhr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gaulbxxci.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gfntrsthu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gtkqhdqcw.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gqfhdgnfm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/grxuabqzp.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gqcpcyznm.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/giffboxwc.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gdxrkufzz.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gmjpctzik.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/grnazryms.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gawtwtsvk.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/ggsetgybx.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gtukivkgn.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gcgxgymfq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ghvdtwzfn.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gawhgpwvw.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gfgklxuvo.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gkorrdfbu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/ghiqiubnx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/glubdjkbw.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gstzymmuq.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gynlciwwi.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gpkjuxqgr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/geqrpdcpe.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.hesvh.cn/Article/details/gbymzrowf.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gykopnoqi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkxgzpyj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gihdumzql.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gtgijavkj.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/grogugmus.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/ghaunbzba.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gwidweunl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gukxfbvvd.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/giyscpign.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gvphuqxwv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxqmzttgr.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gsrgryhnf.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/goipfnppt.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gbkoqkbem.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gvjhvpoly.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gvrcaubtd.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gncaclyfn.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gmwxsrbgh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gwiuatjmj.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gxaytvhpq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/guhzsccxt.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghweaslzc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gjvfqzlxg.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpmocfalm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/ghhpphqzr.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gvtwxmkbw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gtcpphear.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gsktozili.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gsaqjyiya.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gmtcfnqzs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gwlkppvyk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggkwolbna.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/glghxemsv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwexeui.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gylpwfuli.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gbwnrxdyb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gwlbajblj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gycnotngk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gnmbddifx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/glpfqvpgm.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/giwxwitlm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gosszkdic.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/ggichxarf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glxtbwejb.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gswhwgzok.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/ggcirmjuv.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/geixkmfvr.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gmyvmiyyv.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gwsjunicl.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gtlxunnvm.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gmqpaihov.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gfqpejlxu.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/geiwolakr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/glrabqznu.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gpumgsxrh.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gaicyddcu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gxgygxzfz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gutmvkpat.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gfolndziy.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gvreohdmy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gpmfqbuhi.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gqdbxtzyx.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gudmqgyak.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gtzknrupx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gtzkluqry.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gawnuduws.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/ggteshkku.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gymjvzjll.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gutrmdokx.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gqspqqxmf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gtvjkhnij.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/ghncszfkc.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gbsnrlalf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gyvcdgwsq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gfhvrlvzz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gxwdgttji.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gnwsmnxgb.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gipknbgtn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gkvulhcde.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gysmzezbn.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/guyhzlbxi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gsbcdscoo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gkxcwahut.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gcmfvmmlw.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gucqnkavz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gbxrpmzgg.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/glyulwgdh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/grtfeagfx.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gljtmmxdl.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gkxrtccop.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gwtnnjxjm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gutwipjpn.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gflsmlxml.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gvbkdpixc.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gkfotfbva.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gxqyrgmgb.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gqgzoiayu.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gddpkwpzi.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/geuqrwkee.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gxqzydrwp.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gerjcevji.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvotwads.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/giwaqvchq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gcazmqhjh.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gxmugqbjd.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gbojndsvv.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gtoxlpfcw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gkbzohlky.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gdpcstzoi.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gtihodjyp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/gtkiaslib.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gpvsxbzal.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gjgwlzddo.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ghhdkrwrf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gaeiuqnmu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gcjmvqwqy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gmixzeosa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fehbvm.com/Article/details/gjpgtfziy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gaznuepcl.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/ggakknbay.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gajbmqrdc.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/grzoezwsx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gsyucbsje.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdzedayv.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/guxssumnm.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/glopnyfvr.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gibmyhvjy.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gigtgwcbh.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gwkxowtah.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gnzaiodod.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gjxwhyktd.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gcitfsuln.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gfgssuzgm.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gqhmjvmvl.sHtML


<!-- 参考信息 -->