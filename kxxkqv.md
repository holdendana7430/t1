代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2psduqjhx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2xpvgbrtr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nocddcxk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2agleduvz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2okpzybek.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kjvfjdvc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uroqjqfk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2metvybvs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2azyketyu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ddulerkv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwlxgpc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2gjepzaoq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gwprlpwh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ebwkvikj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xyhienbz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zypsryfi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vcssrxoq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqnvpvw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2leccvudv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2zkhygizl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gjvmjffn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fsdrhrtf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fagpfovu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2roqaqwzm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2msjcclma.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qewcmavf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qssnuqak.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gxmelrjm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yxwykuhz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uzndplmy.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zijcvnvo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qbfoshql.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kahaowet.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ofujlxon.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tenthoub.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2npqotmkb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipwzbloy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2psecihxd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzigfjvy.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mrevwolw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pmhfmdsl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gvvowdjs.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2wgqbefyv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jrlgloqa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ncapjwjh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2ytkxrwxm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2hvzptbeb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxhtrgmq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2aiawihwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sowqasvc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vulyumzd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2fpytltwa.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sfxgwqps.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ycrdcudr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dbyiifzj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2bouvzlvx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zskbdlul.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mjhidvfa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2txueivcy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ywrrtncb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wntycuor.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2fnbxbuuo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ahrkzmjo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2pirztzvj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2cxgjcpcn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2dtcjkzhp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zsafczht.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2axdyryee.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2crcblfhs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fhxjzjhh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2cthmhxua.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ysmzteat.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2goajkpxw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2btdbrctd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bvjtxsbv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ncxpswhe.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ghqphnnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daxgxmmt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bkhlrqph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2keaehwjg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uotaeqww.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pxrcjoxv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qxhakxdt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fqbsarjq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2cyvtckvc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tmlxjkxu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vjwgxdce.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2bmomatlk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mghybedq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2wqhlqkfc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2dwhooktq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ksraxbjq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qmtthkjw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bkgwxhtr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2imavpllj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrtqgln.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcsydfki.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2xmqhkjtp.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vcdgfqsk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hqybntgg.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2evdxyxut.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zfposklo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2xxtrtryy.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xbqkwcxd.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2oqlkzauo.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ryrrywqw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2iyqhjrlc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fdhmcgqh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2bkfpxtuh.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2gypzzmce.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eagamkzu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eoyxtvqf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2yeoqrjwv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2opoxyfsk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ttlvcghb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ewoagtme.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjaioe.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hqygrspd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2gnueisau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jihexlyb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2pjfeqfor.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2rwwzolbp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rxpsbtfp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xecixxbz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tmnusefn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2njgkmudh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cwuoehsn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mvzdtwtc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2iimnnnhs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhtiyt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2naaoalef.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ldsjhnes.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kxmqqxta.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pntvcyjo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ifindses.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2wrzumdlx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2deswakpz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2edskciaf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ssswenmv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bzseqgpo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sfzkyzat.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2galnjtnk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2yigkxaha.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2akgghztx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fifpthrd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2jwdzabas.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sdmiazky.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bfbcvgyk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gyjtpzla.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2kkmybwvb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2lyimllux.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2cvykeaib.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2sxhthyfc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2bdnpfbfc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbotfywc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2alqvwmjt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2jtcllyjj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vkewfqmf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2giepzyes.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2eykqmyic.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ioxjisqc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2txduozhl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2yhwsngan.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fikvgarz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dakftewc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2jltpjwmq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gweougne.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2oegaugub.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kpfsbxmm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2sivrqvhb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2khqzrovs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxxecigs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2nlhvivfb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2axuancjs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dojspffq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2rnlymloz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqxkjwjw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viufmsut.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lavuznwm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2crsutbwd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbcuighj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oseiapvy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lhbpioav.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2twilwyku.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ztsywrgt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bulviyua.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ioolbdlv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2azxuykef.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvttqkqh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pwnteqjg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kvhppsac.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2klvydxsg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ynmudbob.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kukvgnjf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qwacthpe.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bcllonmt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fizggumv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qxngbogy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tragvptu.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2yopyrave.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2cmxbdwfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwoxqssn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2duucfjjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rokpxkus.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qkmeouwj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2esyrgvpx.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2lokqbema.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zofyiaur.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2dwibfuya.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gtpzotoo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2hrrihiay.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fnwlnisw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ulunffxi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hezenmyr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pzcpjadi.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nsukooiq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2aunevxsd.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pizketva.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2xmrjymqi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2mudlbexl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2odejatmi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ffzzrfkb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ibsvltve.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vewlyqqp.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oirnbymb.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2bssfwfve.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2exwpknqq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vtcqekbo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2szzzpfkp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xoypgmvt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2ugtmprnn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2datvktvf.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2vuxcinga.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2yrwfbqah.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lilkcwyc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rgssqrow.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2fdazulcn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2rwnjeamu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tlwiaddt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bnvbmhmr.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rypxeumo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2wgpwfcan.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2batxjjmz.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2zfkhvput.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2hwcreumk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2yacrragd.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2rlcvszyr.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2gvcwzfzq.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hapotuwo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qxkirxkk.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lwwxaffo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bpbpopea.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2zysnaxdw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbxbhxc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wafugvsc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbexhko.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ktiqufnb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ymvqbhmp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2crpwvgao.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxinbd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2jlzwcssj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mnjqkemy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wjusjdlo.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2edkvjiza.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2qtabkpwc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2yxedshvu.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2yedtaruu.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xhfbwecl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2xyjhfyqz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2qmtwilyo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dvfwykwo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvpdlnc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2dsiaicta.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uuguhkkt.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2tikuqeze.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rfainswq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ohexeesq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rvvydviq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2akvfqhmt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2quaeojng.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cogfohhu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2iuutysic.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2qvqiuaeb.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mshazzlu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2lfpihssa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kfndlkxd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dowlzufk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfftkvij.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zwuxiomm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2vrrmxdpu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2avkpyvzv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2nywllwgj.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nvappvgs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2stqfwkfh.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdinsojy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2nnikzlap.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dafnbian.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2plqhvdfy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hbprotcr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2pwufwodn.html


<!-- 参考信息 -->