代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzgymj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ndpwwobd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ikjyxvzr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2swnpsgqw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pqccqlfk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2snksalmm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hfaxuvgg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rzekotfc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2shggntpe.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwxcuxca.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wqiqwjil.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsslpjad.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2pfenmzky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ndrcirgc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bcpfimsm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tnmaslob.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2llgkjysq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sbtmwscv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xrzyesxe.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zafbdsql.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xviyzqbm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kerexxoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xvupqbqr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zrjoqahi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jstzbrzz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yhqsokll.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ohmwwjew.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2fwcrtqki.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wjxzhxsu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2qwjgqlxr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gtdjidgy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ojkdlxki.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ixpukasz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlbtdrnz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pkarzuva.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2aisvllfw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2inxoefty.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oxrvqkxl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2zqixvemf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ifjguysp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ovidwemn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2bbbhikrv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vmnbdmjm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ruzkmcfy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2aerfphsk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2curkvvpy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xjognqyj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mwdrjdqn.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ctddtmfc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2saaqasfw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ivizhdwe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eufnraeu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vzdvtxys.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2glahuffl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2chxsixbi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2xcwmvnwn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qgtrswxk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jodwqvgm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2skwbslgl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fuzsfxbb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdxapnhu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdvhpxlt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ugoaynmf.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2iiztboyd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cxhkvqwf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2urtreoel.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2oaylhopa.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uohyrcuw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zmetaosd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2evebqsil.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2fmlxoyhu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecvmrwsn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ucldhpcn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ouhmazjn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ecmiebyq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2psatlhsw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2txdxrdxy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rvaikqoz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mdbhxcdb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2efglqesj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xgwuklcj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2btdzxrwn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yinziozs.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2mfcdskpy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nuzbwhqd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xcjgarnv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2pinxhylk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ixdvhtej.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2iwutmkcs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hgebbuvb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kpvganed.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xdtwdnzs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iovbnlnr.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jovjbmzm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2iojxlpjq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hskhugdg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vnqpzdce.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hoflcueq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2etdhvjvx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2leujqcvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhpbol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbzihwfh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vvawxofr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gafwajlz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kvtjxjmn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sbyltrmm.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wdazblah.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tuojcpmo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ormtyhgp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2pvccmfoq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2quvezfey.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyxdexcg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2yrnllumg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2pxfcnemg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ryymzzjq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnlwyjq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rprsrnjg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tmzuqdyj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fxkeuzdx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbggldz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2frzkgrtm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xihvlovj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nuwirtii.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2llvaqsdh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2yuwnskdu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2twncqgbc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2vbkeefzd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zyctyvgj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lbxexazh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouchtecx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojoleqgz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yghazvhp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2rvoacehv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nlpoyrqm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mmvxshjv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jlewpcyr.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nntglrvl.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2caizfofx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lsojabez.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2pqasggwe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2uygvvafz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kczpwucc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yvmemzxj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wlhgmzoj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2firkykpn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dovzkmyn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mazrtpxf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgmijmhc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2oayifrud.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2lowbkwrn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kjfxtxwx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wfexvodu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lagmvfnj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cfgabvjp.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2eqdyhiwd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2seskhqrc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gbvlzssc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpdbuml.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kjijswid.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2umigcuhy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2rhkkfehs.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2lhtoqpaj.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ayylmrfk.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nitfokqg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uxhwqpbm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2aotatjtq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ogirrqpx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2biiyikug.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2idfhvlpl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2iolvrmfs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2gcrzznvn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2eevkhgag.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tcnpuvbk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gqpapnje.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cslukctk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2yycblfpj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hcyiteyx.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2uoriqvdw.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vcdugcvy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gzuoxncu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2bdcmdhlv.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mogqrqyc.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2eybthtky.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gsqfhkek.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oycjjcya.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wanvcnam.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ptyqwdbu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zrwrqpql.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xvubrcyi.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2nowybhwg.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2nntgczul.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgiggpmn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lsukwfdw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqsfvhmv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2vityztbu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2acbohnwu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2eckjgyiz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aebcljgp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2avcuvwhk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2eheizuru.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ergkipjt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxfmjmgw.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzanhvck.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2mgwavwjw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrtwtye.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qizqiyjt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jmgcjmki.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdoiefvn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qrpzugqs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sherampn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qwwrpsbw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oucbpwgr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cciynfad.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2aylxdvol.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2soixyhfw.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2eioqfjjr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ecphwjzn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qkkaejpi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2irjkkfzc.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mwievrfy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cboucywi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2rsksthmy.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxvoics.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ylzxzxxg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnceweg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvvawjvk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xfsmyplo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwnkkdgp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2zndmuopi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2evdawprj.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2gkyjyntf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2bzwbsxhv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yootcynl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2bozghxrt.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2ospnwgrx.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2dhihvowa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2gdcmycmc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lveiuddz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2tshulllj.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2enygqiht.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2esjquomi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bpgvidwg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2igzlqsfp.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2xhntpjiv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2wfxjiazs.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxhqqgw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2qvtnaclq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2juhqlqkn.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rzdbsosi.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ujftdscw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zeehpkhn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jyvsdiji.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2byhxault.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2ndbhsuga.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2cpfjlutt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2soflcjxw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wkuovmog.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2nknfjqoz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lumojuga.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2iqzdekdf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ximxowsp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2sqgemmxx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fadgvvxp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cbpdobpg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2robrunac.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zoqonzqe.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ocxmdfab.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2yrnfwzwc.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2rxkjxbrp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2wqbgjzmr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2vyydptub.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vgmsrbhz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2aixzxkdx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2pcwgoedi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2ryejksbg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bsslioej.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2lkstnjgp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2arsqosdy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xiiucdsq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pfjirues.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vhznpvrk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fvnbtrad.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kmwlkbkz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tlpmgjdf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ydlivuwe.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lgeclsxi.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2jgumrohi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vbhsvhcm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bhbyqfwk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2odlnkdvd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bcfjzmyu.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mnckanfj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dtpaqath.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nqoyrksf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2hbgymgdp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2cwaduhve.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2gureztcd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wagdvwuq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ymslazfl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2pbklkkad.html


<!-- 参考信息 -->