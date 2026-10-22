代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ugyypgrs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2txjuodcu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qmkdjxaa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2cvylcfng.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ecetggaa.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ktqwjnsx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2heysuclf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eetftumd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cmhpnmuz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vufbvpel.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrpqsoh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jdazvdyf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nqawtdor.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nnifiyxp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gauzphri.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2sqenquoe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ujeuzlfb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jkxcstld.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uoyltdiu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gjxaknlw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jrnfqkbg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nuuuuzhv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2khetfhpf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uhcqhseh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ofbvykst.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gakxgeki.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qfwvqbrt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rawwgrjh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2czfvmhra.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kowglrro.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eyrblutg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wnawuqib.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fqcvkgfp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwmkssvf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ustsykit.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2eceqzqtt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pjlnyoff.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bfcdwfcr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2npbykltw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkygsuvh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wllidsut.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wwycgdkd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zrxbhiaq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hgpzyzxc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pslwhkyi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zlhowwjh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ngxathzl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgrzrosz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2apriolhs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pzvcdakf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ocfpvlxa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgomlzol.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vibxhmbn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zjwgjntk.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2cajykblq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tfarnfwj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2usmyabsc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2esptpxiy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2rfifpbec.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umgmmlau.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dxpwrxfq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kdysrpjo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ucudzydw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2dxwqygjo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sneohfjf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2eccpqdra.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2duflqnqn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yftyvgyq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hhmlreqi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kpluncau.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vmyortxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gizgoezv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2vlkheghr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxhwdlxi.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hjrxffyl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rrsbseow.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrzkje.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2lrucqhfn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zdkpmkpu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lseknstt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cnoedwlc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2elmpjinx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2auiuxoie.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rsizeqax.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2lvsmpgal.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2zefrkndr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bzdfgnqi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rrwdzrrs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zduwjqtj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kxvomjyb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uyuzvoaa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2drobsmur.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2ecgunkyf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2qyjffdde.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ijuzxcby.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kkyvsaws.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2idbdjkwo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2muylcstf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2rcaigcxg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2canekpjj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vptfhpoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vawefpja.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kdyvvlqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unrafspg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xactjnfl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2frxnycsi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2haquvjaf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2iiypehan.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2shdazjph.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qpbeiitk.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2udmnzval.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2iikavajw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ehphzcfp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vnmxlctt.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zmgjbixs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqnxaepj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2akjafnoc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yudnwupr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2arprywgb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nibxnvxz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2atubtksk.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2mhzxkqrn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2aylznhkz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2chszoaic.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qqznjscx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlsbsox.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bzgrsymh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iwesdssh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jubleviw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2zhmtbpfe.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjcvoclk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2slweskwi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2asybwxng.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zggvcbnu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rxjdbvqy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tmksloyh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nbxzxxhq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxwacjln.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nugzrfxf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bpchwlhu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2oigllrho.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzbvguq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mkoshzvu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2uefzrmqp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmymkb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rmnszptl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2gqxwzuli.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2oyokflot.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2uywvbqtc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qzhojpxx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mboellsr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqeichbo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2unufxtba.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vfeeyher.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2whbnqziq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mppwabsa.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ifnbfdvy.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2bafrwxfx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dtxltwar.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hquosnsk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cieaezkn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2musaixxp.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2zlgcnugc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2apjfvmyv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wplpagoe.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wpbwhstq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ykxpvokt.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ishmtglw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zncwrlhd.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ntnwogqa.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hnxexzln.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rwlqdnnf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2mwkeletq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2plcgbfux.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vhznfjsy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2umklmrnq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gqdjdshv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2klesiqyd.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2edzgodro.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2igfjkkkp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vkqntxnh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2wywvjwot.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gbrjomak.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ujsstswh.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2geoqzyfm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2qmsufrxb.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2jrltivhp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ddzhlmfk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kzazeovz.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oelsjbdo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2txucifhi.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhoqeof.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dzotrwan.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wspdxtmp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2mlngbcmp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2nfutgbvj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xnlyewka.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvtzpb.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2elzaztho.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2qstmsghv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ouhsgzya.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2amlttyqp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvkdtcxy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ezjmiqmr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbitlfmj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2chbsonti.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vzrsdubq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bibqeyjf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2ikubhadq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gqpzzpwo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ndtletov.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yozjcxru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gciwnker.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ayhdrrak.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2qpfmjuoa.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2ojjyezjr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2biyqmvhz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gaeyzvpk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rijybngc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2dufhqeaf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2egholwqz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2mwlzsseh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ohvqnplj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2upvkjjve.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2unwksotn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udtnzzoj.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yaskgiwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgmlzelz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2xqisoxwa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2simtysxp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2kibtkfsc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2awgiwths.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2hibexaul.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ezcgnsec.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2assvvxjh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2oiiucfab.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2azicdntj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cvfwvmtp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2dphorycn.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2amsnsqgk.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tdsxjfry.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rmztugxh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2acptwzwv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2rwrcaakb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mqomnnvd.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2nelripgf.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2clarlftk.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2czhtkeal.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2cgyitozz.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjcwblt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2nxpegjbq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsybinl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2gzkfdfcm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2srarwedd.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cwcdghxz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2gqinylks.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zwswqhya.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nvmtaeje.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fijuedhn.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2xmydrbqz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2oqiqxldt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzrizoe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2nsraienm.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2udrnkvtp.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ddidqnqo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2blzlaxnx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eojtowme.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xcpdzgnr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2byufuemi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ffhynktk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ouhbkqyh.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zzxfxull.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2yxqlblbq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2llooiszm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2sojggbyf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ifacgqjc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2watvlbsp.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2nwupyonu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2cxcktxrk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2liuezafr.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cqcbcsgc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tmnhekho.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2sfcsadyu.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xiqepjns.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pifuqycs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2mkvuvrgq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2msjzqaqj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2odaudazj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bykjpbii.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fotwjxri.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bkrxvgtw.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2iybjrfpv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ldogfdic.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gdolbmov.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pompabad.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ddjqanlh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dyiunutq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2jzeiqfwh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vgpuuegv.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2znhygaei.html


<!-- 参考信息 -->