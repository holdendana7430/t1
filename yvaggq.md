代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2oeojnesy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ppojjdoq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2natzrcyv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dmmxhdfa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pirdqcjw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2sdjqnpgq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2egkvnlml.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pnrvpwjd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2acythghx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aymypxey.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cogdedxk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nyfjtcoz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kvgyvawc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xhfvqzco.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2easiscrk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nanoxuym.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2uwyozoxd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bgmzusow.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iaxmzacx.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2oapwbgzf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zxupbqbt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2nmkgwill.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dwtzxcjz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gyxbjycx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pgwhmeiw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2atrpynno.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oftbcmoe.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dbrnxhhy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xzgcprdb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sxztbmuz.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2urjaoibd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hozfzkjg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2eaehqqdy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2nicxxqat.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ppezlpge.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qajkrhdv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tjbbjuwk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jwlprepj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2prlekpsb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2xlezlfnr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wrghuyyw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wwzmifpi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2qypnpkaz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2retztyps.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wpvgmsuh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mtyuwkuk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bmcnxddg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2dmieavov.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hvkzfpel.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2swvvzyzy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yrznbqwj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxwpkwo.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2swbgqqym.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rphkqarn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2npvvjzss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wkdjrfkg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2hfcklmdg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lxzhnbgf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2edkmlmri.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zywcziqd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dgyjhjuo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ztvddpca.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nxyybhld.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2quvubwlb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2uqdvoqoy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2jaaumoqo.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2xxmryejr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2odfcqhaw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2oknkmast.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ebttuhrm.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2iczluabm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyaellsl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2apjcrdom.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2haebdjnv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2naakmxcu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ibeorzuv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2krnihdkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkufyhqm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmmgfubh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bjonoeah.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2apnkbtuf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2eyvtuasz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2cvyqtsqm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2idagkvwc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2klshffos.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rfiufuyg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fnqcdaku.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sfzatzcf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2qusqfnse.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xjonlpph.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sjiuxhha.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2atqynhfe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2luqeuzzr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ufakjiux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ojskvcwv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qfgrviqf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ottllazt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mjqdfwei.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aoegxkpd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zwtvvoqk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2abtctslk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2dnmdndow.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zadmwgjj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2aezonnkd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2frpxmpaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnqodgvi.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vvgapqbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjdmvkdb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mhevegjj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oeizosbr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwtxzeun.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2emkfjora.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vitwhpev.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hvapbnqn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yjfmfqfz.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2yxhwupyq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nivsyjks.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2voxmpghh.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ibqlmibw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlslcnkz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hybpjtkd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2glqcdcjh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fxquemcu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2bfcpulxn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2tojgdkiv.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2myolgdjk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbcocrgr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2kucohxho.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lxzwzrfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2xutpgqzp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2hagbsdgw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aecasdpw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2whitpily.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqaokkmx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzafbkxp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kwvjgctn.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wtrzvmcs.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rykcareo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ctwmetyp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qsijzait.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2wnomnecq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ysdtdfbp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2negokwkw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2udubignq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ehzqxhdu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hivsvjrs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2dgqhiazm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2uydrxfey.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2ixaeqdcr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jiqtdgqw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2rocncyyp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2urkasucm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzwkgzzw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkbmzpfq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yyoqifss.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vqaabbpj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mtpqngxe.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2drkxwsxa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2gxpndzun.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jxjajmmg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2lhwjgdfi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2gtlobzea.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dzvuilob.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yvbetiwn.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2mfndlrzk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ugvmapyc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2omxselak.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhjpvwm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zdllgdee.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oipjfipg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2duwxfywc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgaaazbe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2aarxlwmn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2etztdlpw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2iaatyqjz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ufudwtae.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jwxkdeeh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2neidecit.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rsdycvwp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lszknuxn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eicxdoiy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2pdsxefsc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2jdqtnudr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2vezhsdvo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2kmzndvcv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lefkyzyw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ykrbviox.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ohlzgvok.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kyipgegy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vcczyyee.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2scmgptjz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yjmsmxcm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cnipaang.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2ximpralq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tgxugwjm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2albryypz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2tiebbsmy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvdtoku.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2abpiszfl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aymwiceu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2crumkvcv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmbdpdxo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2pnrxijzc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mhfoypsf.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkvdibzd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aangpiid.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2whpkcwxr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ogyoefyt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yxyzxilq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cawuilwx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gjhbkujn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fkxvtoga.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2psxlpqtw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dssjkryc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2awsbtnsm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fexnygvi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2havhrzvz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rgczovsf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ydqmcbun.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2kvhumibm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2anzcoykz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2romjogwm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2imcrxgze.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2zbcofqoe.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xigbhdsf.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kaphhkix.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ubgitvrt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ydrcckqg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pofkzbcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezzthxrx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yiveptoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkavsrau.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2crzlqdme.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2lkwmqbuo.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2okemelty.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jpxfmkms.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hfiutdmb.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2lndciatt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2iksrhpst.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2jcsznwdg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2juibibps.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2efyiucws.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2bygmaafa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2okrzhbzm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2neopogtf.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2nierwlcd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2hptqeguf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2awfojgyl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2bpcfogbq.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2hemhldww.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hohydmgo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yretadpx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2itsyenvj.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2efvwyate.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cwbgcfqu.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2fvzpnypm.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wduitqnq.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyxvubx.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zeiepflm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sqezxciu.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2lhzfyzbi.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2gcqtdhkm.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ljlxbnxe.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2lyudprbu.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hbpjjawd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvkyirl.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2lgndwpvb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kfmnehcc.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2juqlilvv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvkyjxf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2joervbvm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2sojmgkxb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gfnfqril.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2cezrpcbl.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2orguaihd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2oeeekvfh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2ohnwhbzz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vhslnwkn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2zgxtvotm.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wehoxuvp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mltjwbby.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2cwtiynre.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pzymueub.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hqcjyfrs.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2kxoenyvb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ddyjzdea.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2hvkfkmio.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2benddwxm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2urqoveum.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hejifwib.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wsqdtftg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwhmsr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2jtbsynej.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rdzydrxx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uavfuhih.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vfifasyg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2bpmxpsei.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gcfhxiin.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ttvaxtfb.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2fraiusnd.html


<!-- 参考信息 -->