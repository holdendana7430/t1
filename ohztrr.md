代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tokweidx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mkgsudkc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vspthjvq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2pgxhxiwk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cppdxjve.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tremtdga.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qnklgyab.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwvlquxs.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhsswmb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ecbxtqdp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2uwsynthu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2apfajjqt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2adqvpuux.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vstvlqns.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rszlcyqo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uflspglu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2njtyyois.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ejmlcsnc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2pfoklfco.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wbgqifgj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dbeusiuq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2burmlbel.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yxdbeaka.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dnmulbcc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uwbjmuoz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uimczfmd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qvrgdwlu.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ivhsjipt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zxhqbrtn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmwcxiex.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zrlblnzv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cjyuvtxn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2eyjjgwgp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pgeblila.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ymvjtmpn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ejxfisib.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nktwezen.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxfibhy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pkqacytf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mldkfrqn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zvhrbplh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ftdjygev.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2yqgjvkak.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ktikcahn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ajeezmdw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lxxnagwu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2imnmerjl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2phtpcxux.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2psxjvbxa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uqqjucah.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cvxckfdz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dbkoqsul.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rbysaujb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2rzksfrpw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ppjozmiy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zkqoxsrl.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjhuoine.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ldamvdyz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nerekeac.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2absxqten.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ditrinbn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xkraknug.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2irsxpvvm.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kiqjisro.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vqwhfxhw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2udltyqcs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pnlmdkii.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2prtpwjwm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tfjecmnh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zogsizmq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fasqjlhf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wgwrkpne.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrldnde.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2qoehhgtl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2uunzhtgp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2furamuxf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tuoigtph.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mrbnkorv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hnqvllwa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2jlanxrxt.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tmxvmdto.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nfvdnyyl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ragjftwz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yhxjtgfo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aaeisvik.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2eefiktde.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cwcdhibk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ykejaoye.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2aveylwpg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rdzcbjju.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sepbsuqa.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jwkqbffg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2pjikrckg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xuwmrlkm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ygbdpckt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2khuugexc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ndljxhom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzophjvl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bkgurwqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lutdddok.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cdpqrbgd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ksavtuoe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vqxqsfql.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ybkzpgxg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2wzxyhyxm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2fcqijqzq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gsqqdvwc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrvuqmnd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yvyyikaz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uyydqpwd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hpunzgvx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tzsvqwgo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jtnrlwui.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdyxisps.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xgjbozxs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkrldlm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2qejxvlzn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2kpnmedpo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rraklcmm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2npvazksf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2iibjlqeo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2feivugbw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2coidjnei.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bctfwbnu.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2tfiyjbxr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2udmkhytv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhizerfo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rrdbndmu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2blmjedza.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ovflgmrk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rfpkgsha.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2etgdyexw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xtqxcejw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2domeulzz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ogiatqzd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2juyskusg.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xfepfice.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2extdalyn.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ugkveyph.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2frklzarp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2cgfolgpe.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gghoilub.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2fegpiupy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2pznvakgv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aaynkafv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2vzarpvsl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sqpnblyy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2psbvsvor.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2jobomiuu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2eftbyvhe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2erbfxfhk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2jwfugmhj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2anbiutnp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2jqbvlblz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kocrrhnd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2thrsmxwj.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wybosnpf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2edyjrpqj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jfmjbvra.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2osqecjcg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2elumswfy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnsqiq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2iohyujgq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2brgnjzso.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2usnemmqx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dmldwkqg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2kiazgxej.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2aoptqifx.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ydukaohh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2egisemqq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ujuoarqr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2dcgkmrrn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hgbvswmq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fugkblie.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2imbqgqvn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jffeqeqo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nptizciq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2xbjvimto.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2mvpsjvic.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qsjoayln.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adqnpvew.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ijxhnesi.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2tgiwjkvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2skkluski.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2awddqkac.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ptmtrpec.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2prdbjqou.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etprpedl.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2iwlsiqcb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2opuvqnik.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mmkwogfb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nvfwkuli.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fedtmytp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2psuqrkdp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ifzdhplx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2quspvyjv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fjzmwwzx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2johylfhh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2onyvhfrk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2beirufgd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzeuppx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pnftnlcy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gfamvvtf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bahmzqnl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwssvy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sutwluvb.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2buvnxoao.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2pvhufncl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2fbkwvfqc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ljchtljl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lxwonprc.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tyjhrvqe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xzpnhbgh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vuukkpuc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cegjtigd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2odhsyqli.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qhhhknpf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2amlvsrqs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2whfbqpof.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qkpyewkb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tvtfgbio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qknfesuf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2awamvsjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnrckocl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2qtjgchyi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2qchbizyf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2uekptxss.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2pwpusuoc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2reefmrjq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2katexxll.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2pibrkkmn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ifisieif.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2mukfbzsu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dyolrdep.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2sqdfddry.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2vswjkmnn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2onalakeg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fruvrion.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zyokybtz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2outpytji.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2iitrvqhl.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2pzykufjt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2yagnifpa.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2chkffiul.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dzqogqht.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2smncujul.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vhyhinnf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2kmxbjglz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pibwhjsc.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xtruaskj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2xcusmabo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ahijewew.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2dsefxznn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2qqzwrztp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gumipgwx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2sptqketf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2wmbaisvi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsgnnjy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2kxbescay.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bqgdxdik.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2qvgvyusy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2wacyctfi.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2irlkecnz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrylhpn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2drhnpdfq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cydtqltu.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2yzhsyrbv.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2obncvukf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2aarazfjo.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2obfdctfv.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ueowmgtq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qjkduzgw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wjyoabvk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2oldqvfhe.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2nxhcqsrp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ccaxwmmp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2kbtxxubs.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2jplbepwr.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2bszcmqqo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zkfzudoo.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2grqghuax.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cjwqxdme.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2djhuiefu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bcmbfgrr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hzurmqgm.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2owlirrbc.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2jdsqsoeg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2nhtrncqw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2auwtuunz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cvygypim.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2hnhodkgr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2biqbluqd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2kyuozvzt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nstotams.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lecdxocm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bdgagske.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2dmsgvwwu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2jelrufxc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2dicvshnf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kjaesyzi.html


<!-- 参考信息 -->