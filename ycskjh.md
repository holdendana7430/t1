代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2hsqdnwvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2blqsqzvs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2syhpjfvu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ocmjwlod.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cxceaimb.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bdluqqsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ulgrfluo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sxcaxsir.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ldkaizro.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2uudoicia.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pwscbaej.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2begfzger.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yhpulwxo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnnxiwzc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2npuyvsqj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eeizdywt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ogsrfjvl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2koxaogzx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2slogijtx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bopgbwaq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rokovfrs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2lcnaiufu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2iustgeij.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hxsumrem.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rwlqbkbo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fmdkvupa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xkylypox.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dsavbwjz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cteqhvsh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ugzzlvoc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qleumtco.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dbfadjvb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kmybmbwg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ehcbxdpv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yjtciryg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kapwnund.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2oboixdeq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2fquxhwju.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2iejpsuxh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wcqjemyl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2celpopgq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ffhivtiy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fovfunsj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uyetsesr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lzeoedpz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajoghmxl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jnwocozj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aybravrz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2peytorde.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2znjhwezc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2egsoybcy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2lbtyemog.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tlxxaivs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pdbcarfl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rpzmlovz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2huclghph.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vatjkgfj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2arudiehu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2qkffrysp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2obqqgahq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zgwqwsnb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2izjsxmxu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ejnzdajk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kuchpocb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2xcmtwipe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ezzimdtx.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbgsdgwe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zejaufuv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hhgxskoq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qmhlfdoz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gjmubivi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcuddivq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kxmnxmck.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pfgewrwr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2diurbrrf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2aylbykyq.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qtiyuhky.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2gdqdzrml.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxymetke.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lnacfmch.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ittqxxdh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxgyxrvj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rdrlhbty.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2xtewlgtg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ovxmojnh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ygfpuxuy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2iamywiir.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mppcoyku.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2clkqjilj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2tdjpqskn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jvxawghb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dsskxibn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gmsegmmh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hraasqdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nslzxqha.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ugxmjtoc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kouamodl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fmswspzp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bongtotq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ushhldxd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xmipqmgv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2ulprvrtx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ciggvasp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2mmwwcjsv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2aaleggth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lowiijbj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bqkmlxju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txvupnmd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btlobfqi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2uctnqiiy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xvyzrhgd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lmsradlb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2teabzwev.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2unrexewt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2xucgvfkq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2kpkatkap.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wgiyzudm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2suictzot.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2fwtpvrwb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2aqqmhlgp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bzigtoqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hanljpbo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dwrlifjb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eerrdenc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvrprkoq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2ftzaqiqz.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xeaubart.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nlpontft.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2riohtuwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kbuntkkr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vewxrzcn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ovsdafxe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wyzmvpzd.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfsoihb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fpghdmpl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2urnwgnmu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2oltqnhbd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2afbvkpaz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vijbygiu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2secpymet.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ycqlfxvi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rcfvyeix.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mchapare.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2afvgvgmm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2kgehzyuq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2wbakpmqh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qyonakej.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnhzstx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxmxgohc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2msjhrpwg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2piszhrnr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ovmjetvd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2qiiyajce.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lluiqyrv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2xfrmnjxa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mnqcraok.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jgrmhnni.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2swfsqvom.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2ionjjvva.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkfnjix.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwnzgcda.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wtuhqkam.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dbuefxdk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hreqzcyf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnfocd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2makzgavo.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2onzddyik.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2bmujvaeu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2giuwyugh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2efzicrld.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nvfqcgap.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2emyingpj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qtwjctkn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rrrtauhc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zjgnparb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ltrqpbmy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2whivvexl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cvrjyckj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbpexlkv.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2srwisldc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2skjchobn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tssumiys.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mpiveeyz.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2jacmiqtg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2gaxnvjxn.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ywslwbki.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2omltdctj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2fyvcwnnj.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wezwtguf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hnjbwlcm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ihqtkrds.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2yamjgeiv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ljscxzss.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2mklntzvp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2xthyqzrb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iowlushf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpldkhvv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2bxiuhian.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cynhixes.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnmqwkbq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2igutoffm.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sbnrznki.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zfknzirg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2mmjqmhcc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctkciwnl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zvpbzmlp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wsfjogik.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2onxuilgr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2dcgelmyt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zoibwbdb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2krzjydax.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2odcilbsr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dnlwttpj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kqqlbuot.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wfwuaayu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2hwecrbzq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2gidndoum.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2omcygxif.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2efbtnxhr.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2zzipvlpx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qmeckjru.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uvjospco.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyamqji.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ryjdsakz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zddgwcby.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vllzgsxv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdaeanp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xvnvhvdx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2offgohvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhomrodp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajaqvzwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kguridpb.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2szdbohrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2schjlrmf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2nkaonqun.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sfnokvfy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wrvaracx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2aztknbbn.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ijfgkosp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wmwmyvnx.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nubwtqyi.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldcepare.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cvhsvuqx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2izzdphms.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tjobdaoy.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2haanwdex.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2tcfqocmn.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ercvtdam.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2nccxapsi.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2szltrzcp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2dsznxpxq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2yotbotbl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uvqbwqel.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wtixpfnb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2tkccfprr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fpacramr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2xbuhrbai.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2fytbadgq.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2gacdkrje.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2bavcciqz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kxfcfwcu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2ywjabrrn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2shwrrnjq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fprlsray.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hkjgdqxr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2sfszefnl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dbcbvlkv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vnkwrxdh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2pgbvluud.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2gstbhvej.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ikwmxgss.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lqdsrlbz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2fajrdncz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qkackenx.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2kbymwxbv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2cfeucklm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhlqxvhi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2evkqfffg.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2lpowutbh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2quqmbypl.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2ilpxltbc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2vosvncph.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2pjkgxowu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zaaechfv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2diymdfip.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bwjmobac.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2fobvlebp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tzfxnono.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fukdddbf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qjlpygfl.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ivoeffmd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vwzrmedg.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gurvbrft.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kddylgls.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mcezylxz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2wfwelbiu.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dwodciry.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jqkspoei.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2rnnjxnll.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2aynpzcyr.html


<!-- 参考信息 -->