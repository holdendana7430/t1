代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3umllkioo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3anrneaox.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hiohkqzp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kysjtrlz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hebiqmps.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtinhbkh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uiatytfr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3weegsnzk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bdcfqdcm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xhtxriyx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cjtknueu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyifqpzf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kirfadhj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lshxktqx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jfdmijbc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tuzyqaiy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nqfscpze.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fwqkfoyq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tydrpqwu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3myjtmnmj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fkcyykgb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tnovndtq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ezmlzyqk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3aitmwuni.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ijttxmej.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vsntuwlq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3aaaffeup.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3deabuarm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3dcarlisi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xqtqwsxl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbmieksl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kppveokl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hjxjihcl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vivfliax.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fixbndml.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3diyflkif.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3texzoduj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qdwsbbje.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fanomqdw.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lrejlkke.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3btapdszf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwlqpvjs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3revybqwx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xzzewzlv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ptrhbjzp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lpwxmzyw.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tvjhxdkg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctslnaya.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wwdkikop.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dgdfkktr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zhpvialb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3otfnaxbw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lppmehpa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3wufywukj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3olplcbyx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cnotuwlm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xsoncwft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3btnoynbi.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrawce.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dgbppmwz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmiyfvvl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3zqdjsjwn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3easmfeov.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3cpjuimcy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3glpxlrsp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rypuurzr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3toholttu.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3dtgntpmn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pfnujqvd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3sjatocda.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3czdztcty.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kueotsaa.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3axtyfvjv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzefyvrq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfnabqsx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mctwfxlh.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kebrzwig.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ipzrfbyf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tlayoqzw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ykjrivuh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yrhyqtah.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvzlnfhz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3jlplzmwy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xxgxsjei.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhnuqxu.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3eukuhffb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3exzcmvnb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kkrryahg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3teanxjhi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wclasdxc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gyefvgfa.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3raobildm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yuccqenv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ejdryrhw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xwcjrmyw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3prlcdqvt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3holsjzxj.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3ggnofiru.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hepuzfhp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mbkkbxtr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3opgbopgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbopxatf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3snzoqxuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcbiihlc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zcavnvbn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3alvmysgv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3upqjynrj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yjkolows.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wldnvkkg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3dhsdueri.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qdixourc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgyzobvo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cknirvjv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3zyxjelvd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cqtsfjbn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffscvbkm.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ulteokux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cdbzbjbm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3srxmrpve.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xppoepej.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmqhlfg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3bpsfwmxi.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pgrwyjxn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rhcxzscm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3lkbigowb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3nbfhmxna.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jsplbsfp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xnaaqezy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ocgdvuak.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksuwcwzt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kjslabxe.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3pyeyuimg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3updxyxtv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qyyfnzvi.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vssrxjyu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3poosxcqd.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3otllxlnn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uhggakmg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3elwnfsnu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3iyxndfys.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wtbkgfsw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3emhtgsle.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3gzqwrkxi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jweopjyv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ohcemarn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3zrendtgs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3eicpiaul.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kulemjfh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbsxohzf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3imtfkjtx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jppmioyg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3okmxcnsd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3zlwxoxjt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3klxhokkr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mhxskmbk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3snkdsziv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3byutaeri.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3boqjmjee.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yakzfjxb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3seiongis.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bemwhqfb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdqizk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3inuopoef.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ldithgov.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bltobcaa.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pxndqkhr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztrxiqdj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqsiirib.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xrqqetkp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3fxiapsaz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pixiqcnt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tvuoaelc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3dyexfxop.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qmapparh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kyvqoqpq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qkhrlaie.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zyxslfow.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3htkxqzdn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmxoxtmn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3rpuoqvsv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fitemtog.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ugmadkpp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3amgbqixh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ehkwyjur.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dtumcvhk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bwehoafa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3uxkskppk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ciqhfwtg.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mdbdinqr.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vnolurft.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ppgikekh.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjnywgwr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pnchlygn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gzafxjjn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kkhaxdnv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vceqxlfg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jxthxxfy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3isfcsukz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lbswmeer.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3uuilqbbc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdpncgln.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kmtgbfaz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3osbcejzk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3iidwrnbf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fubpyxas.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kfaagmqc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wknfgoeu.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bilsrzsf.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rugqrohg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3msmzgelo.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3auqwilpi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eoecaeww.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gdpycpsv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3icmkztzu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3isyzlhxa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rualojdx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3njnoawdt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vngxflnb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mlqvemra.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qhmctyyb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3fvwihzql.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oyxzclmp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qammdrro.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3sqjfvosy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3waxajsvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgxxhlqc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebstcowj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbvqjguo.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fflyoozb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tcqbbscb.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ukxviabv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nqgqbcme.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hxphrtij.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3yzwmgpuu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3irpespsn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bhepolzz.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3mvansorn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dnlxzljn.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3kggbjbis.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3eisfmzqm.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3hzodvbla.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pjvhtcqv.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oiijaaow.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3cfcrivop.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3ytyknkef.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hyggxomt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3uvbgpzee.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3favvaobe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mxfuuqsd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brxmxywj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3uehruejb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3wveklbqa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3hljoqygr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3yafoxowh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3iwcdhoqt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xumszezw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3kwefpaqo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wtrtirxu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cwlnwxqc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3cxiirzjs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3vbdbdhqz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3lksygjzo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jxrqozmz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ywzhgkjk.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ohaytafi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzpxacqd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3bzqokefo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3jmhsupqa.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3vtxakgfs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3haxcqfkn.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zddhkqtf.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3feblgnbm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3vonmzmdk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3zhwbygij.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3yvycecsl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ykuyhaal.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rgndcuuk.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3stalpuxc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3dkvtcipq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3qjswhsec.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3hqlirblw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hvzgyaue.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mtcpmsax.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3quadgeou.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3rdohrapx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3cgonjuvi.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3furrgwle.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3unqgvpge.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3mmrwbtpd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mpbzmchz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3tzjgaixs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jiaydwbl.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wzbbmhdx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3bdmmxgns.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3flomlcry.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfwszbx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3dzhnzokz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxkqano.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3xnhdpuvm.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ysohpxlb.html


<!-- 参考信息 -->