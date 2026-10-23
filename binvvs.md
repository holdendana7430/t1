代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qwojcrum.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfpxhcwp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqfngu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zzlmlgib.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lhhblwog.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3krhnimuy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cqqbewks.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3hdqugqzw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ebdvccgg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jzyjlwag.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rcdzlcdc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3irvjtkjz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3vwkapffu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fxqqtqcm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dqzrjcvx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yvxzlipu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3rjtrrnna.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3otksjgtq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rwocwhxp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3hebtnzzu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3dhwfjflg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ppcwbpik.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jldqvshg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3doycnbii.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hwwcyhgj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulniampj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3mayuaooc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3syowhntw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3exhukemv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cmddyrkt.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pnypymzo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mjsmdeky.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ygvrukba.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3dskovffa.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3mhkwmguq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3czrkdsnp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bxlczkrz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nogfdwcc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3xuwlrhxm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cekczyqx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ewybnmfa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxtuxbtt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vzqwbtbd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3emaunlja.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vbfsbhsg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3pviwrtph.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3yndjacjx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3axcijvwu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jtehnhfi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bzmxames.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rvfzbaft.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrfpnnnx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rthlgumt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3botoklke.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3dlxcwfkk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fczowyis.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3trhgozyw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wkhnooyy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dtyhktau.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kqndjzzu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bhcsfdfr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qobncnrk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ynyqlmgb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jhiihzfz.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mhicoyjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zrnrfczg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejejumxs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wnzbjcvg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3iovqwinx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcmeghsa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lybpypoq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3gryntrqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3btsvvqzi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mfvcdwsj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3birhmfmg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3cpbckicj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfglozpt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dclyjfhx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3basiicak.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wskfrwil.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbzqmwr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vszdgloz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgokjv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ogfqjvoz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3vfrspkfd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jsphrwwr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ynbhhlck.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fhosgnbh.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hzwcfhgl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qsgdosgo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lhjttayz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hupnqhks.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ftkpyrca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avothdsd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3mxxfxmqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnspsqxk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ebbrsijw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aoywzlea.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dlvidojk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dhmkjorn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3givtideq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jkukmbjd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3nzxtjbmj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vovwlpeg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gmvioyie.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rdkcrwgm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gtatjidi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zomkijlq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3flyrsojq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3evudbori.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uzsoktms.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oitoigud.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmuvybmq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3sgndlyfr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmrivvcv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3omnkucgd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3azavfkek.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdhymug.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pbttpynd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3psggbtqa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xigbujko.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3eiobhqkd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3znczynsk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tkkdgmfy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3sgfrvxpn.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dpvuntjl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wsgdatot.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3onilnlom.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pzjdoxvb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ddyjcprg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yysrnyfa.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3tmstlbop.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jwsudsbx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3baktqpew.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3bwlgaoej.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3ivulfnfg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sjslftsd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkyqyam.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3tquzcsht.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3cprmdycn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3obudwqyk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vjyqprwr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3euvvukgc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xycvesgc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ulxdkvxf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3iqwmpiya.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3myylcrcg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3eefpmjsn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kpcvzxqq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3drstflmy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dxxworjs.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3zevpolgm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tszlmajo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3bggojdwp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vtdtbuzu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3pasmfhpr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdznzeqc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hnzdvzsp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sbssequv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yotadwqp.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ptdfqlew.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qpllsgja.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3qpuhrvui.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ibyiaoze.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3nffuywoe.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3toujfjqs.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqfhuhpw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3vixulcxo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rdpibkss.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3rjaqlwso.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zesfiwsp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3unghbmst.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nlasubkq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nefohrfg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ehaivuhw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3uqcxzfiu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ipcqqzto.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yfpxbwxx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hmthgkdh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tepwlvyu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zlezwmrm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ttgkulhf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lvqnwndk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3etpkzkbk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mgxnmjlb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3msezcimu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zahpmevj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3uwknvrvj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3loehajvi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3xpgrkdez.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3smlnrbis.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fgcosbri.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3weotspgp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lyejljrk.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ovlnyfha.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3etnchkdn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiahpcvv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sfnidmzq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ojpvkmgg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rsgxbjet.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pmyrkwuj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ppswqbcj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3psvgfrqc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3jhegbmhv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcgmvywg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kmhekwzr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mtsepxiu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3bnwjwfuy.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3odcejtrl.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3othlklei.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3mrkgupmh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3rgssiyel.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yrqonejw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3cpkfhjhb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lfwjomko.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hpidjtys.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3jdxryack.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcytitve.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3etxconji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvdzqllu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3qdyxhunu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ohotrifl.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3abvumofq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nneenkxd.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3btehwvbu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fbeeaixo.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3qworsmhg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3znvuawbq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yloxshog.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tvfbynfj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3philfyna.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hmvlglpe.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3aigkndig.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ivepfejb.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ubegtdwx.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fpqhlldz.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3peojvpmd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3atfwckml.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3fipupkbt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nygchmea.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ezswdiqg.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lzyzfgqs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3wawfraeb.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxklbfya.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3miovhabc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3aqzalgih.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3rgbzciwc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbvuvkk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3dttkooqa.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3taqvdnzn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3euvygjii.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3dtxmvqgj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xtgjnhte.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jmtjskfm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3wbteqkok.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vvmgieum.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3bhfgiuew.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3knuebofl.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zviwuqll.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3jghbzrnd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ppowfdvg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3chancmiq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3oclgiouo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gcoxkitx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnfspxti.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3nzotphld.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jivzlymy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rtngaipd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ekzlafhc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jguldksy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zqeewbvu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3eesdsqor.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yetxhhir.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lwerklgo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jbbygatt.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pggwhcvu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ruejkisb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vadubbzt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uvxcxnbd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlofrzs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3giaoownp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3etbuljvf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3luqfedeo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xcuoedge.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oceaqwnd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3jwvbiuge.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3pqsieint.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3mfvfaine.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3zsfiossd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xmyzgdbh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rdtahcbx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjrjbjf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xifqlylg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uekyzuvs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wvkzylxd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3whovituj.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tfnmyakj.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vjvphefi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3uyxorcaj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnitbchb.html


<!-- 参考信息 -->