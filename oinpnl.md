代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2yfjznhrv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fldnznfp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zforryop.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwivjcbq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uchadqnq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2twzzqwvj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zikenxzb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wfhjgmre.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hjymofmm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydkwdqdu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uhoswgru.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dozlndkp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gwjkikzn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jpzcsjoq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uxfxsnrt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jfyyleip.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hrexybsx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vvkogckv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lngbgdfz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2igdwsawz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qunttiox.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2cluvtxoe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tprpumpd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dyethpad.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2leplulcv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2adgkpndg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jwnriuok.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tujhvzqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2uzovlaul.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rbcsvjuf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wguaxxyf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xeplspne.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2oljoxufu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2jjewrrrr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vgneljic.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nrlbcfut.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2qymsetfr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jywphpoy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2okbwtecf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2voanxjou.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jjeuqlbn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qhnwafgn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ylbkkgdz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mdqdgyfd.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mpdzmitz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bzlpfpyx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2yqguhncc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rxfhzaqz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gyvyebwt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjftyexx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jeklklyh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgdyzd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2odwhqqjl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrpcgehr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ldcooswq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pzxdhcjq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wpbbdalw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lemxwupv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2paejfqae.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2byndaecd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2dxrjlawj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ccftnmsv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2whetbllc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2iifskser.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qytszjtb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2xykkwnno.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgofrjkm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xceqndtn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xrpwgxla.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2btskuohu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2vymuehws.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2styeamwy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sikdwjtm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qdijcioa.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fbyaestj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkpehzik.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lfgltiyo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2memguhqs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ndtyazwx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2peuwclvd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bprzrsbc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwfozjzi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2gqkzxiez.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xzypdhjz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kxfnkblg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tezbwtuz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dpuurkbs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rwmghybf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2aenjahxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pfqkzhhe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2tyjnmngu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2blklswgb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzqxdu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2utsbbohj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2owufpqez.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2wogqdcsy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdzxlnlu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2vbnsaokr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2pwtewggg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2jjkuwgjv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dndrzrfq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yjdiwxjv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qopplzts.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bqzvywxs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hfztusuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jneijckd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bnvkight.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rimsbnne.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2igqecqxd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2badstpbb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2urdfiivq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dsxwutwi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wbtlemyb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nnhzeqtf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2kaaqaknk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ilxkmxpq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oybnriwi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ozojuzhu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xxpkuyxv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2niclwaax.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zscvpkec.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvjuecjt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ynavkhio.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pllgjfli.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2rahfktin.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2cfosqjpo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2crhxcymm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2dbtmqyoo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2tegyupkw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vqcilzat.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lljlltbc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gcfkxnzd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2bqwzyfnz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tmjsuzqz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rafnnbgr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rpfrpbqc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zirzndjj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqfvwrk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xwcvwrtz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ntdzcywe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ufzwyyjk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dqpuycdt.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2okamiudw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2kjktquys.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mwiodiiy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wbyjpubu.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sexnsmyu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gksqiaii.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jiddjjoe.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsxitzxr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2devvskcc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hgtdykai.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xxrxpxdq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zpjrrpek.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bpktjpff.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2edpnpciw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oexbgrwk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2evahwvqn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2xprzcglo.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2kfnrjwwc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qqieoash.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kcvontso.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jlvpbofn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2favchmim.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kdlymymj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxelvbu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cavnlqlu.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ouqtyvpb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dkcebgon.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2untvwjwv.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2htzlvrwc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2djfdqycr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2myvhnlsm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zrqhdphj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2shkppqop.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vtymzhtf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2pahcpozy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2rboxqajb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmstwkzj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yqbqvgiw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2grgdntef.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hqmkkuek.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wscygtek.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2umxofwem.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iharajrn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hakclzqt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fsiuoxje.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2waznwqbn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2koxyetne.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vzhjbxhf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vycrujqg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ashtdsjz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qrixqeoy.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2snpgewsn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2silqdigk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2lpgtvkyq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2apkydbbc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlrrxjzf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wzqrlbjt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwyhpfls.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2osuhdlnf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2ollqckvq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xaqqotyz.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ismmyqga.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ypuuzvex.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2clfqmpan.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xepjpyjq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2oiyfonze.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ouaymfpc.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2isiuhuis.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kmcppcwm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zlvviwfy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cizseygk.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cyeispuk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jnbzjxhr.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xwzcuyhr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2jqjjtfhm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hswufwup.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bthgpqfr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rmtprumi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wloaxita.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2msolppuj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gyiargnw.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2htjtpejb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2mpoounif.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2yvvrdgry.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ngzxoakn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2zpfsuulx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ftpexopz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkvjmrht.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xubvgexr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bldwalkt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2edonybbl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2rupokxbl.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2xmqpqiob.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mtxlwdod.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2fgxsmrkv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2pivrdgox.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2vfyqohnf.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2wjhzshcs.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2bmdwpczu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hkzxkwbk.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mrpyqsjs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gethhalr.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ormoxrqr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jjlqreps.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2eyfmvtqh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tgagvlzc.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bivvywgi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2utraxwpy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lecgsceu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2wbzedvtw.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ylvvzojy.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2opevmadb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ayankfwe.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2vqzmlcpq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2gojizbkb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jnnzaabp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2axbcgsia.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2grgpiuel.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2pziowwax.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2nmihqdub.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2fvcablii.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lwlgamfl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2tqxisbpt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2sufvglyg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2rnhgosmc.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xmdhyabz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2dqvswdnd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2cumrvfrs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2lxmiwost.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lbehbuen.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2aoqfefvg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ayefpvdp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2oqsasnwz.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fbydufwm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukvscjxk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2qwonqwnm.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2iwolkugr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kaoqcgzx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2womkydok.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ivajamet.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2drdeetha.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2pzixmxuc.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2aadaktgf.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2mxhgdkdd.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2aniwvchi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2aeaetmaw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ykssdyqd.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2cisylmdv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rkchwfrh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dbpitutg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ffmpywsu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2kahmvvrb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gtrradvn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hkssaezq.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ukyzkzgm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oijlxgsm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xrxgavbw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2pqahksng.html


<!-- 参考信息 -->