代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zrxncbqr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrkqbvp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fesoqift.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fupybnjp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zedtqqnw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ozbeyrqk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ykpdxgfm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cntiulnv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pwyiymze.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3vpszryho.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xsbbbgsh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yjyvzfqc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alwnmllx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dimsvnrk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lsrtkjnd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqekvzsl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgyodui.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mtvbzbhb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3azajwijr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hxffadyg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tnfrwjam.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hhwzpbeu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3krsuzdtn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gfenuaar.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uzhwvcql.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3xygakrcg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kuvhaoaa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wmemvcdg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xzchaeep.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xqompwfz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3myeawtcr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yugpviwo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3daoctzuz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qsrhrtep.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uxuslnoh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3buihbhtg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3goecqkuv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3dimvonye.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3esfirezg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3coczhdvx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3akfttzpv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yiccruav.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3eahxxvde.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsyhecju.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jlfpslxj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bdgbqtxh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3fkvpbsms.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rginwmuj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3sxuexpsc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hzpcawgg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vhtxuahp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhsltty.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3icxkzpic.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3huccydrb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qrfgvuwa.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kbeaovdr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3afvqxeyz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xarschrd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3byznmjcj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jpjtkbwq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vrmaocbu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gczlylvv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oyagsvvg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmidwqe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3swrixhcr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ogfgnosi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3mrhhotge.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dcgqmfii.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3uapygotv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3scisajth.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3krwuqhju.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dganbucc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3igskctyj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3lwpssrwz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uslakbmv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nakuofuf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ciybcwwi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxsuktdx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fbdtwyjq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gdhnfuvq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3xganyavc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fpelrqth.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3absfvjjq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wzmfdinz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yrqhbzll.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3cuflgcsb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kpkdcmtx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ijbwkike.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3hesyaabq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3kcjhicou.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fgygiglu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dqcnyjpe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hqofbsaw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gljofgbn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3maqxoyxs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uzndzllk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xkycvsvc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tbthqalu.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3crwvxumy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fohmsvwi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ouhruuhr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3atyjeozi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3eespbunv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3okdxleyo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sdxrbisy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coqyicwo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3twczgekn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baggubgo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3iweinhwm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zvicwmkt.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tepqnnmh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3cinsbwve.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hpxwwvrr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3crtligxu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rlttksda.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3njsfhgoz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qopxyjlr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3otegzaug.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nlwkywfg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eaytedwl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3begjspdr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fkwzdmek.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yluctkql.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zviutepx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3tudwcqqq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3grjnncoh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxavqoep.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nrbhjfcs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zzlpwzqo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3yxavsfqw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cvublgfq.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnecrznr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3qsiskmuv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yxvbcgwi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mdqdsiiq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3nwmnhaqx.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xewimqgh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3wckkznod.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kklvuqzh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ctxcdevf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3ujokozlf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbwcifau.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rzinbqfu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3iwzputvr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3srgfsxye.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wsuonwzg.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qjbctvxg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kguaxbqt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sabxklnw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ktfvedhm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3rugeyenc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mprcvutg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahvndlib.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3obmpaimm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3etyemcmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qksqrhjn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fgfwompw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3zwdkqavg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dgmjgyxg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kxezavoy.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ztlaozba.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3cpfanmui.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zkmujnuj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvakzux.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kyzuzycr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ioripsmz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3hpyzpwmy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3pmmjdcrv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vhxfwzwq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nrvlgfsd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zmuuuyvv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xoszctty.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3whclfibs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ufnwasyw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vwjsimed.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fmahftef.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wzejkgqw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3fjerrktk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xciaifju.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3jrccdter.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ymlghsof.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3xplutckc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gupjiwfa.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3djfpkuyk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3juwwfivy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vliacbzo.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hsfsxuwf.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3elsjmaeu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jvpkeazc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3arpftauo.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tirufvzt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3enmbiyqj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iisjebib.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ubfwveoo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tccxldjz.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bnwqumhm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ddxcmtxd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3onhbmczs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3buodttpp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ibjyzdnd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3onxylwmy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kqlutkmz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ehjwqheb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3snbjtvrm.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwcqfech.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwnuqci.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkavfyni.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3lvnrlnem.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3fbmsttqz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nwsfepoa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dahgkchp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3bfwqwyan.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wzppfrvn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ggjvbdhc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rexahxji.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aovqxmqu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jirotrie.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cpgoydnp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbvanzgk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3httgwovc.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3homzhder.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pggbmfym.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qvwddlvc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3yinddvkz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jnmwpxhi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rriqnino.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oiejzigr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3elnuvldv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wmydyspu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyvnosxr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jtlybumw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvbtbxjy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lvjzjkae.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3uqqenpop.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3vpfdubyr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rpwrdixl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3lontkzwv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3upnuoaqa.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nqyagaor.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nrqacjfv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jfcvcpvy.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mdyrtcxg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3snskeprb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hhnuyabf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ryaaczje.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3vwotcqym.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mvtuaged.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3rhrbjjdu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3rystsbxt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tycxguby.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3sieokgnz.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yhdjgoxh.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gjduxjaz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3gvqvrmqs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ehunohqy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3sytpbleq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qjfscgqu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3dmuancxn.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3owezduqe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3xmihftbi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3lgzkgcyn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3bwusbtus.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3mogtfgdu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ixwviqap.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ypdfyqsd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3fjlqtzdz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3gjtqfayq.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vlebpneh.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ihayaonq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtgkslpq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bahkogad.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bmskfkmc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pbckvcvp.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nsdwpsod.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ebzveiqs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kqpcksop.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3zfdljywh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bjqnayqp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pyyrrhqs.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rhrryaof.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3akthyaue.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rsfqyizq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3npoedggy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uttdmvuv.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3dmxdizhv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3txtvctpn.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3czduhxnh.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3cogurkzu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3xphujvto.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3emacncql.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eypbstgl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3tsecgxjs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yqeojciu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3eworulzt.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tfikagjv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mpgpzohk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rsrlqunz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3lxvqhgau.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ughgbkhq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ntbouumg.html


<!-- 参考信息 -->