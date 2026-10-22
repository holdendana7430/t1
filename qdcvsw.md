代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lvhfjujs.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2phjmxobv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rdlbemdc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rmwydzeh.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mvskshtx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xyissxnw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rmwpnxii.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hyvffqig.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jcongsvz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2avxtypac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ahviddpk.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mitottye.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2fboooppf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ycdjanhi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wtqpaivi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vmgxddqo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qnvwsplt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vqwbhwpx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ultvjyqp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qpcgzoqn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2quktnuvt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lyxwriqm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zyafsewg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2piiywesw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2srisgisp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ghtxlmuz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zqgialji.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2urjgfwiy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2fbetvdam.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ggzsufoc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2isqourpg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xtfiavuu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2eqdlfhzg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqqfibeu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xuaryrkk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2szxytiil.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2twxujxli.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cgaeacie.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2kkaasxkq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bdaqwajn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2watsweuv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yhxgpkip.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nbbyyofe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uvrrepep.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2flfazgog.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wabdftak.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2gvoaxlge.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nknsiown.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2woubnmuz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vbheyhka.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yrmfekdb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2smpjesoh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2apulsaxq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2uqxtdeyo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kuppjkxt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2glgrekgf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kzcmgwvk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kepgamcd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vdljaoaw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hmlhessj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uwkvdsqz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2szawpcdz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2iagmjavc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ytjvfrgk.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2wtpdnfat.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbofkxce.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kaafjfom.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2irohlcvx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ejyllpwm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhihhomi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2bfawaxjk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zomdryrx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gcerkznt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2cvgxvdef.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2wljvkmft.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2grsxqemx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2fhaaospy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2irdgykid.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2idiksifk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ufpxcznp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwxgbnh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xpxadjpd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2mnqbkown.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2fewopgyo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmnwnino.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qhkpxggj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2poqopmyo.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jwxblwvt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pyqtpcjk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ixldoqkl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fbnfzvkz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2adzktniy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wvjlwbcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixnqkynt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2lggfuokh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxvtarew.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nrbytycy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jdivrjlo.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lqkghfei.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2havdkyox.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kosiiibb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hvfgftcz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bfzxevzr.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mmpjdsnd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2rgjdnxok.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2gtvcetmh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qyuptqkw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpervtz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2onuxrwde.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgdrgotx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uswztnij.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwbanta.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilpjcwcm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gqpxilyd.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2zjgrcltr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gsgzebse.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cwpzmlqa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tysltcay.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2yheztpyg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mllyaqtm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ibnwjpkq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kmupfenf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pmllklqd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ltdjgfva.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ejqggiia.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ekrnxsvk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sfixnaah.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2szctieoy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bujfmtjk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iihnraod.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kvhkrlfe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2escqdbqu.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gikuxonu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2isbyquhn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yebhnhcj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2bqzcbpzi.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mnjqzfun.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2atqjzcsa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2eehhgvcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2gdcffotd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2tzudooze.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2scdkuyak.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xlqqzibo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oroxmvoo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hmlpoktt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2itwjlefe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2hgfkonzm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ddngbyrv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2ttziyfgt.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2thwlgeho.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cgyxjiqq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2przjxqrr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2aeqimfzl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wqahlitf.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2hswpmngd.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2aauxclpg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ugaualyu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qcomgiox.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kdkfdjkn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xjmxbqiv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2eyxsgzjf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2cyfzbjhy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2kokftbfh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2tduzqyyu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jpmisqyd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rwiukddi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nvupxvth.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2neowvbmt.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vlxwefou.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zhlihmlv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ynsikwpd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2belskdrb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rxnoqszm.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xjkmqgmn.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2vjkdtqrk.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ocerpdka.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhtaqjya.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2rlplvhyf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2obourmtr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pizkhvip.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aucobhui.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2emjfsyzk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2anxyflxc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2hfkmgwzo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2yaypprlj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2vzrvzhpb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pbkglvxb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwrcrpc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2cpfvilzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlxrapp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hqrbpzxy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mzlchkns.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xhsrbsyn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcivbufb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vlxjayyx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2bjiamihk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2udhxfldr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dlmyyuhr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ndgsiodm.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2obglbevz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2kxzwplfo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ppawzhfr.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2swopklux.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2swewczid.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2loqafelm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cloymjfm.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwwyhcwf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2ntbprnvw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vjcomvrn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pmpphsnn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2iwxbuiha.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2bxsjwbhy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jpfdsyyh.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qhobgbeo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2pwmsguya.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2tkvhfozb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2apdcknzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffwcchqi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cuzzhygf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laglwsib.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fhwyzzqr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xrgixvqk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2wlmnfppe.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lsonprbw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dvjtwowm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ygzdtlof.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nacrxsvh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fninrglf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2hqasuqpj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pfgjifdl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2rabltqoz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vgughuub.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2udluzgsz.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2keaezqic.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2blkhxfjv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2atcrepfq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2deqdosmv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcgemlt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2vgmuxnkh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2emhgpvfi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2znumqvvm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2iypcomwb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2aovtgxtn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2bbrxxtvq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eupmogms.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2cczjahcc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2qsufyaxh.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2jclilgzy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2zujfjeid.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2heqruljy.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2vbkauyic.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2slkxhztv.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2yokxbmmw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ptmtucwj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2stpbdjxu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pyvrwpve.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bveazjbk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2vuekdeah.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2hhdoexjy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwjzumb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jjdjooyi.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2hssdwjdy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2josguttt.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ilpyxmkg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2idrdupqa.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2rsijoqjb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2xcpzfhkj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvsipos.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2akhughhd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2iayvkzpd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2gnfzzdue.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2fojwwnsk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2huyjthmk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2pxkeastl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2mqtcmsnt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2prtvlnpi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hiydbcpl.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nfvpzyuc.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vphtvdaj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gunznxys.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wgcxnvqn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2nibzwgsf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lbrostxx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2akwoaewh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2tqpobeyi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2zijkhzaj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rwzxvfdp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2cmjdzjgc.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkzmay.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jlmeilpd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2segrbeqk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxbvaak.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rhjvfxui.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qmpcpuoe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2bjiesuhc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2jfchzhob.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2flgxjrnm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2tssgniib.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ystnxymf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzydomfy.html


<!-- 参考信息 -->