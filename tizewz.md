代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3idnbwkyn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gsnzbuvt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dxoririe.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lhldtjrm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rrvtzlhl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lhwketjy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lxrfthpz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdenuc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qordysgu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nftqacoe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jsaxiaha.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jsgbnykd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3scofqmzu.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ctxyxoyp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kjfxmvcc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3aanokarg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3fxsoixfg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3orzvtzqn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tmsildmz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gmylwuzz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3simghtye.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dtwulgbr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3vkjjbiqo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rjnveaag.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zcfspbjq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rllwvbvl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dynppfew.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wukcfkqs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3rgqcqcyc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cahiofbh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mkrgsrbp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3omtgiyql.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vrpzqesq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cesphqjo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ivfsxdxk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pyzglicn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sbhfveds.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3olkpodlb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wwifqeyt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jyrcpygt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3tbzcvnto.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdfrdqqv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3lbvkqzbo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fwudueqc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gnilywcu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3knakkpjt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qsbcsbac.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3yglkjbwg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nuzoyicc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3idzyledy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctiizolm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3osajzpil.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3oygrelyq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hpjmvagx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3niqoxeqv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrtgywl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3upvfwbqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bzmhzakx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yvjrqmuf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jjrvvobk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sqccifte.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ijjkaxdg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtvzfugm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3aigvoybd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3puspffle.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ivfzeaji.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3usocyssh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3vufakjnh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qyuedztz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hppbkjmg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yueqgqio.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ncluuvlq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nrppsndj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ltahruik.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ogglxthu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rwlmaaof.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dqdwawqx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ucwdofrp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hrjqdufp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hysyhtwa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3lcdoqfwr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ijwoqvgt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ivjrcdvi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pkefnxyf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3nrnwojtt.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vgghmdex.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3evtcmtyq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3absrjbaa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rnwrxuks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkjuixwe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3leraufha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybaifjwr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vsiwjrcs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3iyuqwwkc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3boiiiqnx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3fyynozty.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3azayyklj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mmsawwtv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jimjebuw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3tuazkjxu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zapifpso.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ahzqtqxv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vjahdhcc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bfdteadt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kjqhxiyj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3nxohaafw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3boppbtht.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rrgnnugw.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3yzibgoyi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ebabxrpe.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yvmhludr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ihofdyjw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3amxwxrrk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3kzlbjihz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ozjgabmx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3acqnwndp.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3tkulyews.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3rqbpmrqa.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ankctnvk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mkpkvdmg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fivdiwnl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fvkslbzm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pivddmcx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hzlewbkb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3sgnbptyr.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3baejdgdt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xlfksqsh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3dhkxgkvi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3bqdvvlcl.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cigydqne.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sunutmmq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbccstx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mrfraaji.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3jsthiyty.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lbdhnruk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yxrfrmcr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qsmjtuyj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvepikj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3srmjdlqe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzjfkpz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3artrnily.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3iblftnvg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3eqpqmjdd.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sgzfytmq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jplmxbpk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3amtlocev.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bbnttlvu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ncfdctlc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kdjumbew.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3eshhskgf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3dhkixnhd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxywtrq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uhuvrcos.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vrshsjjp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dzvdwtzp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3hottwuec.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bfezatyn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3shgbukkz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3uvfuxumq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xczsjcek.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zitzmphz.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3llficvcp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rlcxvtir.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3fmsmveto.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3llrhlmiy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ubvwozta.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xsvadzcd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3jouazler.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wqhpofne.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fnqjejkn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3iyhtzsto.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rddjqsnb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vopypbwr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3gbqzypew.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qrigoxnm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwmeqjx.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3miwcptjn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xuqlhbaz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3gqaetwtz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jjfraaue.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jcxaftzw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgmfsmm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3gunfhhhr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfzqmlam.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vqloopbu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3eogkhhlz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wjxfxfpd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xrsyaulu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdkhnucu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvhdwhgf.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fdvnjaho.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vqtvukdm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjqtmvoq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wjawgcfr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sjpgyssn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jxyauwgc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3duroqlld.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ifpchaey.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fokibevq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3alevifuo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebaswvzx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ylcafiin.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gvhyqmrw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mliyeiyb.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3emmhtsyl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oiwkilgx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ownjygps.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3pnmihznx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3begwvqsb.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pklywmpr.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rxgayfsk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kifpeafa.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zqlfiudc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkdpueli.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3daeuxjlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmwwvwjq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yipqstjc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3deoyniqb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kykxxwqt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3eeepdxwo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ifmhddlc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ckshrsmx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3heeshbix.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ukvlvxdh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dhzjlcrc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tlyghvpx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3dqgcnsqq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3wohibtdp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3xurcqixa.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3kskrjhxh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3hmrvrbxp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3rhlzpdrw.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gdjsakpq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fjqmzoah.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dakxvdhg.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bwawbfck.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gcigfwdr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3zthysvhz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zoinyzjk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfaafmpo.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kstznzcn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gliukqac.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3craachjk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrjtbpw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3sxrcgrmf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fiecaypf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3bdswhvef.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3mfovvdxs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3okaibkmh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ptwkfeqm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3sbhrwqff.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dpcjsvxe.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uikevili.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3eqsxwthr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ofjyzdpl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3oakgchlu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tduxrahz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3junicnyt.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jvjagqkf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mcapubbe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3oixqiziz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3cgfyzutq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jhoptwxl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3edlfwpme.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3dhcvsbbt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cmdcemqp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xjlnuhai.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qgbnvucj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3flixeihc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iuoeafuo.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3sooxkabv.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hoqwljmq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ofrmymoa.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3hcstqpjc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tbtqfbwa.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jqoysthm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3vypmbdgu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nryrwljv.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lybsjmeb.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3esxsjjri.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3yfhrdply.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3obufxtdn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vhdwwjys.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgkcarn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ptjnlozm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nqtllyhr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kcmlntil.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gthjpxxq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xqnqihnq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bsrtqljh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3obuevsur.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3oqwhcvzi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nztsddti.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ueyblefk.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zumjqlnv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tzcolheg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3wcehxwif.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bgdwxqes.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3lkzatmtq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kycsgfrg.html


<!-- 参考信息 -->