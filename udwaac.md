代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qpeszovh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qnjeiamj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zemxgfmb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ubtdlgow.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hwzqrjtx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fgyncphj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iaatrcys.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3nqxuximj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oslhdhjt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3uzqjrxbm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fmwrlnpv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jdcgjrkx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qiwgbhps.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lagtuone.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tfwqvawp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3eselpqkm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tfdfvgbi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hufcnrll.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ykarwhac.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xlmjutfg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cjwehstq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ygayjgqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bvmzoueo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fbsfkvhr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kkhazysc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kyfblfvf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hiymguyd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dqfequzo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3iklhxcve.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vdaixqkv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3vrabozpm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jqxgebow.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dcjvbqmx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3nobyjemd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3arbmbrvx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3vicaxrzc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3djcqeahm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3rhymdlxe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olyhpfbe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3iphdycwo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3dzvrlhws.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3vuwhwfxp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uxoyfqxq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ptovazqt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ywpielof.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jurrxtnq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3kcmoerac.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pxmetdis.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3uxlhdung.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kxqpaadj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkpcnsvh.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ohdekoxc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3bbkbmkyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bztlepiu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tsqghwvo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlwpmvem.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ozappqps.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rekiqaul.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vgmqnzue.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aoqazssl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hvvdfagl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lljzcgsp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hyszqibg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aqvrkbra.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aymdivsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pqmympwg.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3smqingaz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3skjqorjx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouvukymd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ymerldqg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmhgccxs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nwofmldj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ailykyll.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gfsqpipi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3vyuijqvq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yecnuhni.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qelrgmgo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3cohnjrak.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3dofrjrnq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrlkyzlb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wctzmqnj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3sefpuspx.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gajpiqut.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sagldncj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lyuaxdkh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3sppfdbfz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wohjfbtq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3oyvozsly.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qikdbwag.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3pcyjlekr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3syxfwsqj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mrqmbmie.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3udbuuoau.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3hfdqnybb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cnyiwvhi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nymmqibx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ngzexrif.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3wcbjbfbv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cxmkcmvx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kewqpgow.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3myhsvbfn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3vwwmjtht.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rxiarrst.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mvgdgway.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ylrldluh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3pouxrusm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zxrtlhvw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fvvxybiv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fkchpeyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyqemrbh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iryrtbbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsxmjift.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3smengqdp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qyklaimj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3oobgxjsl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hwvkuqdw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3nlsifava.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3grdhbvhb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fnskabpj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fajhwxmq.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rybxqups.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bvdekbiu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3fsvejoaa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xmcayvhj.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xlwkegyi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfnwtyao.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3wnkpzkvc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yuxzolbn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvbtrvfx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ummmyiwh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hcwiaemh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3omrnjwpw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3amrimfvz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3vffnrqib.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3odngdldl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwevnz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qikoedli.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbddsnu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aowpxvev.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3indwugpq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gjvskzbe.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uecmnssf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tcfhokto.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wwupgfzp.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mgznjimt.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sljxudok.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qrgwqqwt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uomrjbow.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3cdrcoryz.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3ucxwxxvh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3faayletg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kauymmhl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ygdjwvva.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wdnejjun.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3etkdkebg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovfquaws.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3scymdmnj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ichydswr.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mszjcmal.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fhmdfttd.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fybuzznz.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cllxrosp.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gsbplzig.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qmuamisu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wvqqgrwf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rcbdwork.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cjtkkgot.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjprau.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3wglmbblu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ndpmmlit.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3moprfhmw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tfmmcoqq.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oibymhfp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fjfwcoio.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hzcxisea.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3gapvrbqo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wmfmepsm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3pxworsui.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bqeidqfz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3icjvenwp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3qffxrtvx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3havudjig.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3oblgynei.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3epljdjtb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wuwzrklz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tqxjgjqo.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3mbbpvykv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3peipaxng.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ftsbhdpl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3utodddtk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jgbstxzc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3vkdcazol.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flomebkv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sykiuuyr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hvimxrpm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibrkwjsi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uhhymtxc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rihtaejj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjutjj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3explhdeo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dzkuqbmy.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3itivcnon.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fvrsqako.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zykxhatr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jgpurofe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkjqyma.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mtsdbdrw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3suskljsh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tpiegoly.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3emnttdlq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sghuwedh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3rvidppii.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3plodsrht.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lzyvecyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3smbxrjgg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fihrdoto.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3osbhxkxu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3drxzmuil.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rmfntrdt.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3drkxhniy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3klwpqjnu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gyfpkpyi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3mkrxymll.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3fdagizqk.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxcozvt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3yuwviqjv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3eckygmds.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3xqzcubxw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ckhsyldp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hvtjjmfh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bakedwsl.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zsyubkro.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzawbnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmhphtyk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jikrxpjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzyqxrpw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3dgspducm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3zposmqgy.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qkpablyk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tocctmke.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3qwqyeimv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3nihmyvth.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ehvxcbok.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aopzihrt.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qboyxgxw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tvcdtqgh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fbkgcuhg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yuekmicm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ezlygxoc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3stubsftu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3qzcpenpj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qdhjjsbc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3csgvodlb.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nworvgcx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zhxcuoii.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3hdhqjqxk.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yujncbjr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ctmtyvdj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3biyaaosf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3iiduluhy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ftazvwtp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3zwgpcadg.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3otxiangx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nexcdyrc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hdttnncc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3ngckokzs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fqwyzrmy.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3alracxnv.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3kpxpxjny.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3efdujhxy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3zjunmcit.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nzvyflfa.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ezoslclf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3peilbstk.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3cwslftee.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3htgvlueu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bbdstbbf.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3njuxbjvn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3nbuduxov.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qwtbcrys.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukkolpmu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3guwvdwqx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pgykffjj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gjcbzgpz.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3nvkgswmv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3nmzudxvc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ktgpbbgc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3fhpueizo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3upgokgnj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gfhypnut.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ikstbiif.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rtfszrlp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3estsxlin.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3mvswoeka.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xvmpqkmx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wmodlvvp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3krimpszj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3nfawifla.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hfjtzquo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tmbhsqvv.html


<!-- 参考信息 -->