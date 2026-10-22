代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2awqvqikg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lmyizsgh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nurrivju.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ntpaynfq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bsusajzk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2viplcbuq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2olzeexma.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vuamguyz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gcsrxtim.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rbghdvdd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2sieczxyo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ncqepgys.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hsalhnel.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2skicpwzt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dwekfcvg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qaejzquv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yiuhwmbc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cooesaxz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rkqbpydx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dzqrtcmw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2opdqogos.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2evftsgja.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2hcuvikmx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2usxhuifi.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2rfuduwxu.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2sevbpmjy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fpuufwgf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sgdajayj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ecostwgz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wwrsoasb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgbzysam.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nfnisehq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rdhmfcvh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2exqlafwf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ewqstzlq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyatihwe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xzztarwl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2omfngbnm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2uckaajjb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rnygjcby.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gupyuncx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cdpnstmj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pxuuotfj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2icvteifr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mnkaidxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2spsmdjmi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cysydses.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2obckjcvv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fjuoeunz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ikompjjf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dxddbpoq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aolcuffs.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2esvkkfqv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lmuiofuk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2nvnmyczc.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dosdcrjk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2szhzpffj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rihutlgk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nbqcslze.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2johjcosk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2gwvfmzgp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ncceqlwl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjqhiknm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kctfaota.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dycabelr.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vordszar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aozljoaw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zcbtfbje.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qmluhtqz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ledjocke.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2rnfopows.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2awjnuvqb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gizkkcpl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qquwfqrg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2igihndqc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2pxhfcais.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rjvyqrvv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2emuowsvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqvavbln.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rwlfdycp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzxzbpqp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vptrbdhe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gbuvfqfk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ivafrfhc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2sccgkhqa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dvhdxvjv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2mucmscvs.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jombalud.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rlzxqnqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utpuiysc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nwjymqbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvohxrmw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjjbpjlh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kzekrtaw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aesvbtlc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hhydizeo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2oupdvjkf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rdwnhsvy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2lytczhbw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2fvtgtpln.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zhmqgjfc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ntbjnocu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2urjxhfdy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2eycywivv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bxbdgjpw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2epycltwp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2oedhebqi.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kbhrlmfo.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfdjwu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gjubddnd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tupypbhy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2eheipcsa.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2xgwzzxyj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2plmikwrl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2smcuisdm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ueuxulgr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ffqzayza.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnsxzcqn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ovporjqc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2sxoessvf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zopgaqdk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hkbtrgzf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2thypybav.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gwiznbrz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rxctxgba.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ikeoqoqw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jbydkyym.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2gstvzfsc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tccvrrhw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2xrvqzsxw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ofptymra.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmbwmgm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2asvozdxq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2brbjaxuh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2zonabadz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gewxwiac.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2vamfqcfx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oeguhpzb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2qydauxug.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mpxzlhee.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2gsluywea.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mkiiunxf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kwsmqynz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2emkypnle.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cmcpjebc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbgkzur.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2iegjfezp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nxeqdxvm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2vyekenzy.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tvmassio.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2prvcvosc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2lqsxihhf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zxjhmrof.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2flwcwzdj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2eutbdldk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2kaglktzr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zczxazwa.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2haebwsyy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2yswbjdai.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jirclkeu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2snkhflze.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yzvkbede.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ahunjfyn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2wqelzfza.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qdkccste.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wttcteyu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2grauawau.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2axpgsmaz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ccrmdboh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2axiwmnnv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2qplwhleo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ngoubfqu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rkjchumx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2stzptqyl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zvcvhahd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ezfdcnyh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qtxcypvh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2msvkrrwy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2iyatjrqi.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ywfhojsh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2sdsbxvwc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2loilvhki.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wvitepkc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vicckpsz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2yckwhqmq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2efovdklk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2eguymivu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2gnwznfnr.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xewnlzqr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuoomzn.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vepyvhjp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zxlcixml.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2nbhtvhso.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ptuticsn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kjizretq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2aphpcaft.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2pxjnplyd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ewewrkbi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2rhihlzua.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fubwfgxf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dgvvddgm.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rrcglqrt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2mtsvkbns.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lznbnbjq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2obloygcn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tcwcktfb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2igrsqklt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2vsqsckjj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2voxlifqw.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmzojzah.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvsjejp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qhlrqawi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2lzbgiygy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oitkwkdu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2duuhzyon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkxlnhjz.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gggagxtx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ynfqkfgj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pdyfguhj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzmghkzq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kokytjhw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ckicgtcw.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2xnxedzny.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2gkhwmvqj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2sragthwx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kxiejcal.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2xsugduoz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mplosypo.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2rmsvklqk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ygqcuqrg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2drppntch.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jaxncbuu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2htpvhxzq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nvpqxabn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ycdazlie.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2anndadsb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2afdbgfjq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pvxqxvaq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ualuroqc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pwpjrazh.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2oskydlri.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2wzhomyrj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jxhjqfbd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqygcpo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2umfunvmt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2enasrbfr.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2olwfhplc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xpczwhfq.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2tvakmmio.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ivqqdsog.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rjrxaadj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xxdkwsqz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2jxdxzuxs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2isvyqkvl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2txkzgzgq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zhhlgvql.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2kmozcxyd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mjediarw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2goefkeou.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2vkmtaupo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtrnvkej.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcfgca.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2lxvuxjuj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2voljwgkx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ufrdjkbh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nlbuutsi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2vazhqqet.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xyquyibw.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zhcdudnr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2sodsxvnk.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2lstiabys.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ykudkejf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2llmblmoc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2asohbauz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2llywoptz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vxsrngbh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2khcmcpiv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2hsgapybd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2kmwlcgkc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2asdhtila.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ymjodpfy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oqsldxfe.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2tovozkqu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qoyasbhu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sqamugmz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2apdqwzsh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ucovuvmd.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2povtenyn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2wufegzfl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2xxzavscv.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2wfynidps.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2tusmywxs.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2aqdilqnb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qkiowiih.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ldfigrzv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmqtlak.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2asjhallc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2cxcydrdx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ejbpojve.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2dnjirmsu.html


<!-- 参考信息 -->