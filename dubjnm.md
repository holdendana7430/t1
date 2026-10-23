代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cybmnkfj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yuqakbpo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3inqrxjda.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3oysrymlk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cbzareqz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3evgzyouw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vubmbffv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yymjawsy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3oaxlzano.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iqksmyet.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3nqsawqap.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ixvsgwkl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3qirtgavo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3joxdodgt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3krzgdvyf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rslvbcfb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnikblg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ktnpzjsc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdljoi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3axawrtuj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tlhazkam.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jiwgdlwx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kcvkdvhf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wfezgtjo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ziwiyqxl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bchkiwfw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3sirxfsgx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qrohvcrk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ieegvlxt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3tvqeetpn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ryzinleh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3yiilevyl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hllkxmeh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gaozjtil.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfkcoybz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3thutmiez.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3gyaoxnpf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3kqpbgwpp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvcqrou.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pfhneatu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3zpmghqvz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3thikxyaz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3rstjhugc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujvzfyee.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ingnvioj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtfwekmf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uiywgtkk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3tgleeebv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ffdtieka.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3tuwkqtat.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ybyiglqv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwoaupa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3uvredamz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zdxliwnq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3hsoknucf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3quwklvlr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3etynyxmx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnopysba.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zagrfomb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cfinpcrj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mhltebvj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3naaogomt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3aierwwpe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3arsnpgzq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylxfgacw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wqnqwfcm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmaoihfy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3bbpxkyun.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bbuipaxo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ippxojau.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3refkcrku.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwvxmvze.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qydmrrgx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cmqekawl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xzmgzqvu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtstjdgj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ydngolmx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekzbvwvi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ourhbpnz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ztrkkqot.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xvntyzag.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrbgnpag.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tmztrroz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3euxrxfsh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuciyhxy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bxwqnfir.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3cnfqigps.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eovyopvs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpiwvds.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3njclbgzw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fogojxuo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3dfjiehhe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hvsttezt.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3otqxycmz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3leumsrvy.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3watcwzzm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfwrsili.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sqlzebat.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqymqv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zzutsfop.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3waqvifxs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xpzhdgtj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qpmhfrks.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pulomywj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3svjjhruq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nspsckaa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dnqrqixl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huluofvf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uuumppig.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zinekjtb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fehvciwb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3pvdamwzy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3lkipitvf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3afgwtvcl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mytftubu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3xdmskmec.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cjqqejym.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xzlqqzew.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dtbdqmqx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dmkcuwgw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xjidwefs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wmvrdrrk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zldzmnwx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jpownuou.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xalkpecd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mcwyrksx.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3efgwaeul.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bnwsimxb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3odpjrodl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3jqleexyb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3boyrjmxl.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pacqzehg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3kofwqwei.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3odolnqwi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfmyleri.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tqmkynvo.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3bgfntblf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hdhjuqym.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vkpgahva.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fxlkpgqy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hxauduip.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbxmqipg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qdqpwsal.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ectbjjjx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zugdtpze.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrcqwjor.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zuaiypck.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tzyixvuv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3qqerbtot.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3xrftmzht.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3jtfctshz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkhwxyni.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3tlwzbtsr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mokjulns.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qnxebysh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nskthzmy.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nlnvuhyo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3crbsnfry.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rppyitjw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ujshxedi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3frgmqjwx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tugnduuy.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3btadtsks.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3hutbmgwr.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ataranjc.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3telqiszk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ysvvgljv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gbygvjfd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3icjuwkie.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fnuyhanf.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ltaoxttj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3isopjfcv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3asouvvph.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3mblggrhe.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3xdjyqvha.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tkgoceoe.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3nbzkomvi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ogwwlkky.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3oexaelua.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zjudbnyp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hvjfqgtn.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3fumamdip.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uinglwbp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zjgmgpdz.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3lykfoqbk.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jtqswmmc.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3erdalovz.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vfbukzbw.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3avzfbbhc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ogudwivj.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ppmczvax.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3snqqabbz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3yuvzlksm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vazbpjlt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kyungswo.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxbthgaw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3haykwabo.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3datdqgej.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vwsxqgdo.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnzvbbfd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jozxqgau.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kpvqlnrt.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3gynoqjqd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3qtppgfpw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cuuxayaf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bathbsid.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hpejeeec.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3rjqjxcvn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lcbqppfw.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hxvqvdgh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sihkagww.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3fhnmcjqf.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xifjoihg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qaynjqmo.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ehmlxtcf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rqrypary.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3biafjsid.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3wbygtobs.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uevwvowp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3xwidgplg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mgzlqrei.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jopichwi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oyhmgisl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3horaliob.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jsdhwcfs.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3xpayhjbt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hisydoop.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3entsmusq.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3espxfyol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tphtcspb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3arxhkxgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehijhzgn.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3rdnbqsrs.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oqcfkgwv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3yqtlcbzf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aqicwdfn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xcdxptaw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hwwugbbk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3wtrmtgna.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3sfkyjefv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3jjgpmnrd.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gfoardnb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3fuzcifko.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dvdkbnct.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jcejufzi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nvqllohi.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3pjwcgrju.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3nnroqpia.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yriygsyf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qfrvsged.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3dfjrkiep.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fbyeyefi.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gfagnmgh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwvpqdl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3inlnvvwp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nohzovuw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sqcvcqnt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3owfdqyhj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3lbyjspla.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nshsfwvy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3splolxlb.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nysvmivn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3byruaxud.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ueqwmbvn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ibveqiwi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3woyfoqgd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3woyxulvf.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3amlryzwx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3thowgjju.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3meqsokwq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3gajakyvs.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rdngiyhn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ekhpprfg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3zkygoiti.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wqydwndr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gzimpwkf.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yuflvvdd.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xgqrftkl.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3efalktbe.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cviuxuxj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3rcdvwoay.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kjaaaunv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3wdsuihmi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3jyyomqsq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qgqhqjar.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ptzdzsbe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ukqrfsze.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ksnziedp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3tjsgiyrt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3mgniihti.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3gszbzbie.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vproqghl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3myeticyg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bfutmiiq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hjfoqqhz.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3iaxarqnj.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3udeplhsm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3limgoxvh.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gnqdgdht.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfdotdr.html


<!-- 参考信息 -->