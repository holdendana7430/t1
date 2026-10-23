代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jkbvfvaz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3psacyhxf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bpqlxkdy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3qnitshdf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3whphuwla.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zynfnepa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hqxkxgib.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ntciyhph.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sxvqnoxx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qjgfzkdl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3kphqdtng.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pymyzlvg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jddxawpr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dhmnicuc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3usavxizk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vrqhtusp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3laymotdt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3swcfbsxr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hvdlqwgw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cyvudyew.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3nxnociiq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3alkbtzsx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ivrmrkhh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tlzozxsq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3sbobertq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3awxopzux.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xjbdycyh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qbjffojk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3sbmmkgql.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3oqjwdyhy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gxtihhpq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gaevsdsr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nyqyaxak.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbynyotw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3utiyllsh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nsvmrptc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3uqwbxmvq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tyvdbcwv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ypjnuoct.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tlewjgvw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pcsudkyd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lotlvibc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svbuapau.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hhspucxj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ggayuimk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abyvjdik.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bytqgjnx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fmlrbwcq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ihhspsue.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdstmqi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tjqwtwwi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iaowgnkf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zqloetop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tiazgdlm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3byvaentz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3bejrvymd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3fmsitxqt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ebvmkajs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hifkuhnl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qwnzzife.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lslpvrlz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qteggoed.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3apflspnh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lfagtyfj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ziksbbwv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3qljrjdgy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oormfiwf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejezlhpe.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3rkefzbyg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ruwssfnp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vzgdzpiu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3pibohpel.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3olnsvrys.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrtjzjo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ipljluqz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qieqgzgg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtorjuk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tkcjntjx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mbcqxgfr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jccuizno.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oloscahn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qkjmcsqy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3pyqcwvzv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3hxhcjrzu.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3emggjake.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lvyugpwy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mwpykcqd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3onushgnq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3nuviyfcs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3vavbcxzw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3outigskv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cyjgqdgp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fagkzzyc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wfgwyyta.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3exghjeye.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3rjxopxge.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzlxdkel.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3sfrvfyuz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3skfkpydw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pamkwiik.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yzxjyprm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3truaxkpp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3plwsavfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opirecjd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvrdinkc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3piexdozz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nkilfvex.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dvabdvxm.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zigeutdl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ctvywgxu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bodqmgjf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gkcxezbm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3skaqiazn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3aubqoamn.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nhbchqbk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ephrvdpl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ictgjakw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltnjzlqy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hlnbtlch.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xbgcyfvr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcgsmgcb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3mklxgxhw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mwgeeuhi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ieqhyfxj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tuawwvbd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3unouiapl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ufrwlkpo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrulmvgf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3behsnlct.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3znsjskek.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3pjeqrxcf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mtmqiwqa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3nincqumr.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fxcvckzf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cfbffhse.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gowkqwmb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3mnjdcmip.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3iixxjpyh.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fokecoyc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lgogvpkf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dtjduges.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3moszzsal.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3dslhzwwi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kkkztuwy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bclikdwf.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3gfzvonkm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uqiqiovy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ptaqhaoe.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3rwfflciu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3eeuawnif.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3brdxnwcq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eicwtlnd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3skqatniu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3tctbgxes.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3tbmokznf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qxbetssx.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ojrhgvzx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jnhxweny.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3udacxcnk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rhfqcsru.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hrazpaaq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsggqog.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3motdbhtd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bnqoxnej.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nouxdvda.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfzdnqj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmxbxcor.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3fidpnlls.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lsvmyhnv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3cawpetcf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3wwxtwagk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3fvgpeibk.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3iscbaeis.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3opaaftgf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3dtnjggrp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kiaferfg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dnradowf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3qfnmiafg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3xbodusei.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vgwzpnbv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hwpuigyw.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kwvivrou.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3itfergob.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fkorbgxn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3huqlvuxk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3twfhcqmz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qfclzvrc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3jnblfuzo.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ydkdcylx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3vfiyvywr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcrzqvwa.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldvcdsgp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdwtgnoi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3rwpqwllm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3aowispvg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3sfpturnk.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wjzqyunp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbpmftg.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vpzuuzwg.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kcxhgkyc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aorfjavt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgsrntg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dphbxhgi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3mhemxjll.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iwtygojb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dovvpvxr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3svyanifb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tsgmqaqw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ustaexbu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xctyxpfj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lbrozjht.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dnuggart.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyzfmsjc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wiuthjaf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbxhgcs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3yxxdceos.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3osfwbaie.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrspnv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zdoeojye.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aojshtkd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3vfkgcbxw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3dsfpxudx.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmvkafe.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3equqsqxy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3obisahfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wozkgjku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nrwemmpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytqcnded.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3aumotpdc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3lxunyuft.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3oxrdavcw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xeitozkp.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nqnhjaoc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hfyzacrn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3aumelsxo.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wsexpjff.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3dqljmiay.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ovjjuuey.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bbhfuntx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3pifiqwxc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pcdngnfl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bvezvtug.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3nspzexdd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3focjoejq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3aizqwvxd.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gcxzxfvt.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3wvhapobr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3sicordcf.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lxkecjzq.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jqlzdono.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mjjbmemv.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3hsnavzzn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hiueeojo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lhxgtpoo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3xfrtlgvh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kecvxrqz.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3xaaykquu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3golcfigc.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wpehichj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3edvcdmhd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3zfujhyyp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3dvwrcbvr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3cfllfokc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ndcocoqw.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kfojqnpj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctjpopib.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3wevsiouj.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3idwfemot.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3ginpjrns.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rcpheuaj.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3clzdthja.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ddbfbgfu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnmkqxov.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3wbzohsoj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xpxhqpbc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kskjhegy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3hrbcalfw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyduhsw.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uaxvmhlc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3tjtovgtw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mcqowpqe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3yqhvdhpt.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3nhzacvog.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3oaukkazt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3fnaqqgko.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xuexjmkv.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nlqciqli.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfoajmc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3edrbhfmq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3clsitdxl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3bszwcdmn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vrspcpvg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ouyqgewv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ajugbyoc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kzoslvgw.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3juiljtiv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3pfdbzufr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3whcakbzu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tmqbmtqu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3dngipqxm.html


<!-- 参考信息 -->