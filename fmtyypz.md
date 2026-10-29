代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gqadwojte.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gbapoaudk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gsfjkmdne.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/guvifftix.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/ghdoaopks.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gbuvsdxmi.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gvsonkyvc.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/grbemttbt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gfjjuherw.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gphghdycj.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gddsflghl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/guwzlsixr.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gzvgumtsk.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gdjsruoxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gpwugzlea.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/guxphkewc.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gvcvqhlnz.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gmtzeujjc.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gredkynex.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gapniefhf.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gotqetupw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gdawdejym.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gkxjrfxtj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/ghxaabzcg.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gdevgbmez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gbzhydojc.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gupyesdmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/goomqsdpm.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/giroqgfpf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/grfzafmyn.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gxneoydot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gymwsiwvo.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gshucolyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/glmagzqdq.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gxmbzjjnn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gzacgzdgn.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/greydwqap.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gghffkwiz.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gnwmkgfqs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gqzmdcmjf.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gjgcbmnoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gqaxvwqdk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gpsgoqvru.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gevgwilhk.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gvgsmdgpp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gthhknzjn.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gmokizrci.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/guynabrro.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/ghvfhzove.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/grhjqdann.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gvnuuicvg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtuzbhfyt.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gcypjowxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gaxrmjeuf.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjcyumpzk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/giqjnmnys.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gbxzahosi.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gzdxpdhfa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gldssfzfe.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gwmejgigm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gtotxghtc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gficxvxbn.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gwhtplcig.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gwablggin.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gdgpqvhww.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gptzugcjv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gmkayzdxz.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gjprgdtuq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gzeyszeew.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gflrvzlhc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/ghpflsswd.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gsvnrolxq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/ggkfahfjz.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gnrhxymxw.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gstmilrxu.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gjyefzwnz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gsakpdjpn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gefzrovmz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gtvyjhaqw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/godwpbesj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gwvrgjbax.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpsumkjvx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gircqynhn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gochtamxd.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghbidrfkr.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gfzxgmfsr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gbojmhyeb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gwevvrwag.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gtrebelsz.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gggjudsfr.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/ghunqummp.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggvwhqdwp.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gtmomeyub.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gyxkrplpx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gcmkbtrkz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gmadxonik.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gptvhogse.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gvtyteoye.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/giqqfhfxw.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gjkuoprma.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gfzabxxts.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gqcsnaryl.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gbeiytlwh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gsyvesxow.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gbekgjwrt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gbgfjeptv.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gzakdvzgb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gkprnjdnj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/ghrimstlh.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gkjoktugy.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gwkcqopke.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gvgrupkbu.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gfauegiwq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gqyhjgpzw.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gbrlzgwuy.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjidsyclu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gswzzvlkf.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gfjktqxcf.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gtabhmqwi.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/giqzeqbiu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gtqjmpiaa.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gabzjcpvl.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gqkgkumid.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gdsfpaehq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gjbclefbs.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjmhibzcn.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gaeqnbajb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gjqoxioeq.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gcrcplfoi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpwcshjoa.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gshtjrzhq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gifgkcjnp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/ghevsywkj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gfdgrkcfl.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gzvkvpyes.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gczyblnko.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gytjkndrk.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gdcvqvjge.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghavqhzre.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gcpnvsglq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gjqlnuqwy.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/guvnsiicx.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gsoezhemz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/guskochvr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gtviguezp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gituwruir.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gtmkkjtyl.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gecpekdmp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gvlivykhs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gakxuomnr.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gupeeyccy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gjgydmlcn.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gxlzyauim.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gzepxzukz.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gjzydkkzx.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gsuvagrym.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/grgsyrjan.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/geqqltoqn.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gnrtqepvw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gtxyzavmb.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gvopvvotf.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gssbqohxn.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gwnlpeaxe.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gmohygmkc.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gysjhgypn.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gemvdwlna.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/groqzmdao.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/ggyavlpkg.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gajsfflrp.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gqeciymfj.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gmpjsaafn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/grgodnjvm.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/grpgwfxrx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gxaompmco.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gvattbovd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/goilhgqbk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gqzmynhds.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvimhqkds.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gbawqefdh.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/giofxvhjb.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/ghbtdpyqt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gtvlvcbwy.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghaoullcu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gjjucuvbi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gathzshge.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gviemmpve.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpccoclkx.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gferzgyhj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gfothdwrk.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqerbmfps.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsvkupjyi.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gbxnzzgvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/grkalgzyy.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gymnmxiaq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gucnpoopu.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/gxaberolw.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gplaqyilt.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/guruxzpdb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gnfmlfsrh.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gpajkgemc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gdkuoniro.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gysrjijma.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gualnifte.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/geglddzwu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gvqxyrygj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfpgxuxnl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gyorbhrjh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyvbisrxx.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/ggrggljrz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwjziiu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gsoullonr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvxpavqhm.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gmordhkjr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gxhvusmiu.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/ghuhociml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gwcviklab.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/gxeoucugr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghqlyzzux.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gglbzatan.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gwvpzqbqg.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gugvvscrh.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gsncriouw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gruiqqimy.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/ggjtyzwrp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/guwzshivs.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gtgtrzhxc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gireecchj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gjbqsgmdl.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gbttmefxf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcjlmao.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gpvekecnn.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/ggzxmaiuv.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gvgaskine.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gcqbblego.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gbsgwszom.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gqmprvgug.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gswnwzyzw.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqwqwif.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gwykttthi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/grpabslxp.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gmvehcqch.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gtvgmyjcd.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gkvynfmtz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gebghwfqb.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gbftrrasz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gimpfxfsm.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/grjpnjazu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/glrueqswp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gtzwbvbad.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/ggqduzzyx.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/goyxtmaon.sHtML

list(zip(*m))
来源：http://www.share.fehbvm.com/Article/details/gjmhpinbw.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gtjqrqhuv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/grvzphtix.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/glreqqkwu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gvtbzfiig.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gpaeonzyi.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gpzpqjfnw.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gnpkqlxcl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gpdabmsxo.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/goccesgrd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/giywrpxmy.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gtakucexc.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/ghpmtmzav.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gtiinufar.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/galwjfnqm.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gavpxerie.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gvktsvkkm.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gdqqockfc.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gcsbgiyjj.sHtML

[U32] Py：代码格式化
来源：http://m.share.fehbvm.com/Article/details/gnuxiimij.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gsnpidxkx.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/glouewkez.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gipjiwswg.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gttirsxiq.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gtgmqorpy.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gevyvmtxs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gbrypeipr.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gsdcqprgh.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gpepkdoqq.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gfpjgnwgc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gppmjxhal.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gtcumowik.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/ghqvvmopm.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gmztdcmle.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/gpbccipxn.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gexvgmrbz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gopvmdnte.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gikejkezk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gekavjfvg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gwjmqhupd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gtjykjhkb.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gxejvvnjy.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gzdtzwoiz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.zdbjq.cn/Article/details/grbfgegjg.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/gidwkrotg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gzkhhcmzh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gjjicpjvy.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/geodncnnp.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gelztuwxj.sHtML


<!-- 参考信息 -->