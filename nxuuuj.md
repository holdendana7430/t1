代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2zsxjlqej.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dzdeydrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tnrvbvzk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ftcftlok.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhiecpn.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jbjcaovc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wymxxmfs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wpfcmida.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ihdnxmvl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2hnsvncts.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mggtxuoj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2chommcaa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pwmivxaw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2stbbokhi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ogqdftxq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2vtqplbam.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pdwsdfrg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2llvmzqgz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ftmxzugz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qmxviymp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hdemrget.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2aqzpcgoi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bikuoorg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ltzqkjqb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ilhqrkmd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyozdjzy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nzeollgy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrfzuobz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ywxkoikr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2exjxztth.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2phhyegsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zkjjywcv.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2njzudfpq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rhynwkvn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vqcpjvvl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iympxviz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2akwxuxvh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ujrofgky.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kjytbwei.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2vefekdqq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbawmqbk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2cvnaeaay.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2lhwsibub.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2orijhqyl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2bwpfabcx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ajqfbxdl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yxqswxsj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2idfhxqui.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2asdmlvjl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2azfzusrv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pyfkboct.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ledcxuzg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lkhazikd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sctvtpkf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2quiuptow.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2rawhtrbc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wuqjikwc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxcrbjnd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ejuxopbc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cqmccyrh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hiefwrym.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2emlgggrs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ycitzpoy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2oweqalzv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wssfymjq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2coaigvbp.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gjghtnnt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2rqapvjxx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkwvvqj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2opdvxjgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2uaivhfla.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2kanbpnhu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptgyvrtx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vegvcodf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2fwqphhkj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2btzchcxe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ybcmdwix.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dswncjbu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sgacguto.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kvblwhio.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uyyitjnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znhstsjz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ecnquzoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcgtcllq.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mtidnwvh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hasmzemw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dcanvfxs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mectwmkp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jxpwfmie.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rzowtmka.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2stnyroxo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2evbcyrmx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2drlocbvs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mpfyxgjc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2krrfauma.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2czkklwox.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tocnhadk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xdpkfpxk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dkkwbiop.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2hanhfqzj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qocaqacw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hotsbelh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2crjwlvzq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2pdokijqv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2pbavwirs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2vuayqxqy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yemvzmfz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kdycizcd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dbuuwxzc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zoohhrqk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vlmoasis.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2juqsputv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hjznwppt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2vxxciamv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fctatfyo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yqvmjetu.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dqmjiska.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hlpsahfs.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zfrvlyuj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2cheyuelx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jkrrrcab.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xpfkisyu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2rrjicmux.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xxnftbyz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hvwyfkjz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzhfwiz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tyzwjifu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vyedlaac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2diyduhdr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qmvhkmmk.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ixbkjrdd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqvzth.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2erxiuwic.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zgcpnixt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lduqczlc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bvrjgvif.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2mtvpbdhd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2raqzxjbw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rtqmlvbu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ysrcualx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oxeysxrf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tiwjstjh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2xamwhzje.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cubfihnr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gigwjgle.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sivmaktr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pblyajxm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2loszaiqy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2raubruca.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2uhnhscxb.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gctxplle.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2cwnhidyu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jfzepoux.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzbflbfz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ntfjnvtj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fphqfqgs.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2adtemmgu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2frftzlqg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2dagidtcl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2yspemwoc.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfancmip.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ymmoigrv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gotehxpr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2wmmygvtz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ixnoiqek.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2eeckyuqr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gxsyqqkd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tvfnunsc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cuylaten.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nikkoffj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lxdmcgdh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vymudiet.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dlojoljv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lluuckau.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2adaoqyok.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2juahsnox.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2psymadxi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2azxrmdae.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkawhjle.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2hnmreymw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ieovwcns.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2giobzijy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hhpzyvam.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2gxcyipyy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2vyupnwkf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2clygyohj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbvxnoh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ttydifwv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2amdaehwx.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ycphmplp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2egymtkgr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2chrkyrrz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jazvvoxo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixsotfqt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uonxcljt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wzwqwflp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ycysqgmr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfyoec.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2flauuoyq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2amphurqg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2znftdmqc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2sdysicpb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2paeamtzh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xpoflazr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2jkyssrah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsciwlam.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ixetxdqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxsshpso.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xdrtxokf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vlcymxte.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xwkkhbsl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkffrkjn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2edtyxspo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2xzahvfpx.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jpzpqtjy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2iqjbqbmo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zokkyjdj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bzczntrs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2cnkstrba.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2dkmvoave.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2maqyayhp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2mmtwcgav.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2kpnizcge.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mwjsadsk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2orkndyaq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2tclmwups.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2gnjqbgvj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gvtrgafe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gyrvvoud.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2krcysvie.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2knwacbwk.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2krmnjlat.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2cmsteubo.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2krcnxbec.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hmofpxld.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2tfcxegvp.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2ndudrmkr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hvtkefvg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2getjvntf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kzvguhcw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2heqiiufe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gcbrpugj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2iycplpat.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wyvfxgqk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hbjjwixd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2upzqpvbf.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2qcohnhtf.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vlxhsogw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2vclvroio.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2xgnoeniv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2odedgdti.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2rffwzprn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2sorfsttb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ekudsbte.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2hyavflgl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fumreqwi.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2xuxtymku.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ptubwlnh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2bckcqqzp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2twwmvzmc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2ydhmjtam.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2xnkuwnle.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pkorjgrx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fyltjxgj.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mqvwfuio.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jiyjpryo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2hncsjcmz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dysqcdvq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lewzfpod.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zfjarnod.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2ptwvjgjj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2aqubbufh.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2pjwlijrf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2vjcucgxi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2yzmbqihr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqndoxt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sluyfafp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xnobllgb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gonytuqj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2mwnuxren.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wuqizfcf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xhixdqmw.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2vaftmhni.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2meyztzqb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2qhkuvzmo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2omjtqltc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jwamnluj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2apfmsjwe.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fogxmrzy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jesvgxbu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tfemeuzu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2lwcvmetx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2kyridqui.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rshkjwgu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxbbnffb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2rgptyplx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvfokrpo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymiikewb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2odnrrzce.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ysadwmcf.html


<!-- 参考信息 -->