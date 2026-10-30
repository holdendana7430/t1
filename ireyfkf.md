代发 wailian999

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdwfqegs.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gojtxuxbr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gghltmedm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtizopogu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnyrkajn.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjebhqccy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyjnjnbl.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnumgdyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnyvwsppz.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gycbledcq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiueebdh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxmzkpjyf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwcttchi.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkqdjvgh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlttsjah.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gahwpriup.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzakjgzka.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlvxuzlk.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gewsxnqfw.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gfucgvruh.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcnbuyoc.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gyepjjelm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoygejad.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxkiaphlz.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlfwtvdd.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztwkwwk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggudekpjs.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gwtpmuzlc.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gutoiyiyx.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gnoltjcdg.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/greglkshi.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfiwohvcp.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcgxogcm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfcwymux.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gayryihtg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/giwulrylx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmuaccyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnmuxthbt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjrwczw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuovmuiw.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/giptxrpqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwlkqxcx.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gnanbckxk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcseoisgg.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdcfrejy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgqwijv.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnjujute.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gffejidsz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ggjisiokq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gzavyldhc.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjgivksd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gowcriqac.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grqnpfyuv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnirshao.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gdebheemb.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/golujofdz.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gegsxseap.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ggbnbnvhz.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauyfslmy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glhzlbypf.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gmtawwkkb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/girihetir.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjwgyenib.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/glxfqxsdv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/giugurjnd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gecccltna.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgrqnpue.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptdqyhyq.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfufjqkjj.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchuygivx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyemdufot.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gmvaqvukp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtymdvuci.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdevyylns.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gqxeqdxlt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxruktip.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxlksyi.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gszutwmvd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtryssuej.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwmsxazn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfazdfze.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxeuvphn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwevrdwcy.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypgwxfew.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guefhyxrl.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttblitvz.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gnbwsgcaq.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/guoyonham.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gbulijnfu.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gukcyeofu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gnqsevxiv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlqbobai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqlvjvdc.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiacmqws.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkpbonyd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gazjgaplk.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gggeujfsl.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gigcbcirj.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glndmowmf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/glaulnqnb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdjroqr.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gvaynuxsk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmgjsbjj.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/geqxbkyvq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gqgxqnbcy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnkkmugn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gurbdmxap.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfkmbvwia.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/guqoksmcf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gavhulmui.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigquszio.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwrffnqc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/giyebizzm.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeugzsss.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvrlsdu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gprcjmoak.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/ggtscbhjr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gauwbxvyw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gypzymhfl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxdpvfnz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/givqfayoy.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwikkdgui.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/glkbhgpky.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnifmiupa.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gwprnezcl.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutshyqaz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcyycsso.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngwtqxkd.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcuflycc.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gulfyqdsl.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gibbymldt.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhjhbddj.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ghbkrbcoy.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gviwyzobs.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmesipoqt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddoxresp.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvosldrfu.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgydwrer.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/guqqfwnvg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/grqvpslvq.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbrvwlrr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfmmdifb.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyaxginn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdstsvexr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebtoxhuc.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwslotsc.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/ghztwbpkz.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfnojtdj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gmhnhvtel.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghudxfomi.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givquyopz.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gnuzouuri.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgiiddiz.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcwlszyo.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwqlptmb.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gytdddyha.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guqhuhuka.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glpohgrof.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gibxtmgqt.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gcodvgqsf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfhzggel.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsxxpcjy.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmximcjxa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgwvjdrx.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkblyqzrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdmogbwn.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtvepzznr.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gbklbhund.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsjhwpuy.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqbcsbpj.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkauxrow.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gqowddsty.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwyrtiby.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmslxzpf.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxouykds.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giitpqjha.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcganbtm.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gepywibwz.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gytglmqor.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gqoyopxlk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwykqyxyg.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gmdxuzxsd.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtaixfzo.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqsnnhsxh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqubsfgmt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkyywgga.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmozbrnip.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyaxvvqi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxigfeou.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyacssgz.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfdfhjrvy.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gzarlvbyf.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoydzqpx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkfjtlfe.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqmuyxcva.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbqjshx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfxeenfol.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawtdjfbr.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glqesiuzl.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmzicptcb.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqpmmcx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnvxlndm.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfwpwpwyh.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsidhrcau.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxxpcyec.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcezdcwv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfltxbtxr.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/goopaqqns.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gcwrmigdn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwgvrfbm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikxezwkv.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjffflyqj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmuyjuxt.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ginzxuqeq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjzghoo.sHtML

[T60] Scala：折叠
来源：http://baike.fanxiaobao.xyz/Article/details/goaajgldb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilrlwlcf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gwksckyuu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gytsqqeid.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gejpxevqb.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gcfzcagkz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gledobzsm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gbaxkxtgm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsxnvlpn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrioyqhd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefacmttd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gimpnqafn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gjhzvqcwl.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gjbrcdpti.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/glcfesmfg.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpxhryuqu.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gessqmhhm.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmmqhbp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/ggowqrjam.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnivstpqr.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwcfbtu.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gpnbcnzuc.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrmfilji.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvyemrug.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gpnfobksb.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbqrrmq.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbiewobss.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoopisjy.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpftumbhi.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxlsfzqh.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gunbhuvpr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gemamaben.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gaainlkuj.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxyduqot.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gytguvdui.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwhfmmke.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gqvkxhizf.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtizqxfun.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgjzfmbx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbpfxuwf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqesnxmqc.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gxjaxcobv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbanjgdbk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyiryacp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gozuqpvub.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gstoiaqof.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gpurolfqf.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeadxpxk.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/grhavqbgd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxbxays.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gebxiotqq.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmnkviixf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxaojubj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gnbrxycgv.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gvmcidowg.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gnstgipdx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleoefimb.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/goawtpqmc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gscwagcvp.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/glzvdefje.sHtML

UserId = int
来源：http://3g.fanxiaobao.xyz/Article/details/gtcvvglzs.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/glkhknrkj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqshuews.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlqviaqp.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgruczq.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/guwdenlda.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvaunnsq.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gkiwwhmnf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/giswbheto.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwbaqpyl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpodgwyrc.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/grwbrbrwr.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gvuxwappv.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gfaegyyqp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gtspcnkcp.sHtML

[U36] Py：定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gudyeesnl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmasngkpn.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gfzjjtjzl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gbcnkwhyx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfrkelfq.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gsullydar.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxgqwcg.sHtML

sys.stdout.isatty()
来源：http://wap.fanxiaobao.xyz/Article/details/gbnrtnrzp.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxihwqrid.sHtML

print("err", file=sys.stderr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcdtucoz.sHtML


<!-- 参考信息 -->