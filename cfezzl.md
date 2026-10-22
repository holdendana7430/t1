代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uilbatho.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2yblvzdgp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2uhuznomj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jmejobln.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ozrlwnyj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjupymcq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2hatpdehs.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lhzocivh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ugbgwpcq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uqxhaayt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pfbtsduz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2butjnnwp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xelhrcez.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bpseeprj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rvbzjgwo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nayhfdhi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nyzmapsb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2skvxsjey.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2bxvukrws.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2klrmmuue.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aalgpoyr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jmjcxgew.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cdxphoyd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2kbxhrtla.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jegebuao.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bitofiio.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2wyrugeaf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vpdestwc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2njebemfm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rctppqpj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vrpzmwnn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cwasazsa.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jjalnbsp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rscdeiyx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2cqincigs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ypshxtbs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2boidbggo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hzatgmdx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2peqfpbnz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gamdtdon.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iwdkcuro.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dtxshqoh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2nbgkcrkv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jwsjthkm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xxwuulyd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2cypdwpzj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2apelnxis.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdlmfdpm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uucofvzd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2egtskyvt.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvycof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yuuhanzh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2cxpqwych.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rkgyfwbz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mrjupvhl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wlpnykmj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jozmynsp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ohciemqp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2jdzcugta.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2dqrhpybm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ietopqns.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dehzluku.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmjzzwfz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cyzldoft.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nntykzlb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sdcvpqkj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pvkyuwcp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2tuzdrxgd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sgdrawvn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjcblvfg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2liruvrqf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wyvbhzfi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2usblsrxf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ijhatosp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bcdrvnzu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2oombxjqf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2irsrehvb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2miansslx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jbbisqjl.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2onqcnxsk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bznpfnes.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ozmvvmui.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dmfvsxfh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zeuwqrcu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpdpvjbu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mequuasc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2trzjxbts.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xpkdizhj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ftklvddr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xkmhnkvd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2quseymgg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2txjkpxxt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihaausfs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hyehpqbj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dnzndsif.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2iapnbpch.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uwxiwdlg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2zfzkppti.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2senecthv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nojxymnt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2wbihxigs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxoyrboj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ovxgaljf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfhmphaw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zfclhvxj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zrsfvhze.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gcjiibrs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2fpoxmhne.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2rqqwqmyx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nynfmlfw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dqjzvlhf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2omzmcwyr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ochrprja.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2addvhqvy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mrsaosuj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hhziukmb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bfkokber.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dguwopkx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uqnbbysr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2oxswwmaj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gsbbhzri.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zhsnaupi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2vvumxnap.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ofnzrcor.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2abptcynl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2ldjzaebo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2fulaxhkt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xjekzfiw.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mhlhvfnn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2gehwxzar.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2rtidbuil.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2behnhsvk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ibylxsht.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2rlconnjg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ufddpbcm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xukwalua.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dreuryqr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ctcvgvlt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ovjrickv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2uwyxhwun.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2upsggyio.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qgxjwrza.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2fggnmgcg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lqslcfjq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2owdtpktj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2iyfmjlci.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2lgqxybnz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2icmlbuvy.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgjrtnxz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nmoitomq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mgdyhxyb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gjmwdqoo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2exsmdwrj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2skqhphtw.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rkdqybxi.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2dthqower.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cyywngqm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kufllltc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2beuwihwh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2lafhkwye.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2flfzmgcw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lgxzyefr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jmrmbkho.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2nwyvoplu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mmppfrri.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cniqvfgw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmkriohn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2vqskwtkt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mxqfxzmg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ghvsathg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tijzaeic.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2osmbhgsh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2cjnfbydp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2jzsctnev.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2othoadgh.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2szmmqxix.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xkqedjgp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2abvhwtwy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ukrzweyq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2czpbyyab.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2teasbeam.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iikcrygc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tfyhsjga.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2xjsepoxg.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bnmhcvva.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jphiqoir.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rdpqysab.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jzoazfar.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cofcycha.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ivtgcniy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2olorvktm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnikqvhi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2rbakwheu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kogsimhv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2prpfrbit.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2lscojdye.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2sskdimsx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iltospwc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wmtiptfl.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bdlilekj.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2amnojzkh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlkauhpb.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2exzeudvq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qzqewgqk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2puzyoseb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2emzrytkh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ecqebrqd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2uvcostfz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2dojbqapj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fgvuefjm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2soswwdoc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ytbixvnj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2zepkfcob.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ebqbbkyg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2vfajhgcw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qczuyziq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2gpavdfxg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2njgbuwbh.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmzyncbb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2cqvbwgfb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cdppfmwj.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aclqgqbs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qpnpghnr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ysixgbtw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yjwrdkjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgcuxgnh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mfflksoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngtdxxnq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2iwvhqcyo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2yatgcazj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2liipppwl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2egmfzknk.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2pbwkoaid.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2phqmscsu.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ulrtyiqv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2cyuljgga.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ehqdhnbc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fwmmaomd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2esxrchsw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gsfkajte.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jhmejgyp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2oacbezjo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2yphnzrrv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ubnivuni.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2uqhvjehu.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2cqaokjmg.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2fvqmipit.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2oyrpwxvu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uyvibljm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2unjxitkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2qojuyljk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dqwlqjjy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2hnbiwbnk.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gziwdjwh.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pilcngdk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkpswox.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2iulbphry.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2lpyzlstl.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2wwmneyao.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bhukrytk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2icrgxlwn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrdkafo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hzyuspga.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mcciwmvv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2biggfjum.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ylfwupmr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2gvdnbdis.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2qcxlqcjl.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2tyrtocsb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2hysknvpu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2lzrpakul.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wbwrqkaj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tobiywmb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2vmvbwpld.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jwhgvwqj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dydneisf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2uahicezd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgihqmq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xchbqerv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2axybvhga.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2zzhpakjr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uqbaocre.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2dikmtwun.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hacamvqo.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xtkgjvjp.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qtcarmfh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xyijbyym.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2tlosizch.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2glyexwgw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2oyltontl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2rsmkrjmc.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rvvagzeg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kywicedt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2gveoabws.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2odnmoekx.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pkjtifzf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2zmwcltja.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2dgnsckkc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dfchpehb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2aamocrei.html


<!-- 参考信息 -->