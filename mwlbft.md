代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3mrugbcys.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3pvgprdep.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3oltownuj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqnlrhld.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tsebgeme.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ivhmxdni.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wxzkzxbb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ubbqkrxv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3upsjodke.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3txtufldy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3qxcvyelr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bsrnrprk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sfstduur.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pudvxmed.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fwaevicj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lbxuhody.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dcwtybfx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lzkjsfzo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bsplhisq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gdqeprem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3enamzwmj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uqsriixz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3obtqllvy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fogvyqvu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3jjrrxigg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mmrwjazi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yqbdbaoy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3igbrhgzk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3jcueefpe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bmgmnlwg.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ikbhlnxf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3gvlzwzla.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3njrozlny.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wrltmgcs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bfzxipge.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uwhphjbh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3czltprlt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3sdagokoa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3rpchwrny.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3xyucjmfa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3jpreyggq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ntiromge.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zptgdhde.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nturmngl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3fqahnwkz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3thzjmqef.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rtsnegky.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fbmywqmr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pxeirjgs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3jdxdwomj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vrnaqnjb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ofgcctqd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jtrmwydc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kzrpllko.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cpsayxwl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3expcwfok.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vbqzxonp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtbetfsd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rvzjirbm.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3staarxtt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vapywbvt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nvdhgwzi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gjwxarys.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ncpbkxgl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3auznuzsx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cobsblxg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xagcawto.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbqzja.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3sexirmvf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3mlrskldw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3trjldrlf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsgejmhm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eleehqnr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vrkxykql.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3covreqzc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsdmqqnn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jpnjtklo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajnxhmgo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qpgjleqo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3damxvnkt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yznmravf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xtqrzrup.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vqvlnhvb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ijrooxcs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dsvlbazj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3elfjzrbp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3adbukmib.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3iwriqwls.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qijoityc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wpzourpb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ihizwgfa.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3yzyifzdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jrowwxdp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3agxpihbu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ctkvlnit.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bshuhceq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3muxrtbpx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tyixfqpj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wpflowco.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3swvnzfwz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjbkbqes.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mcwlkyfk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zcrqzzww.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mukhuqde.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3elbyfjbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wljmqqxv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pwoqfdhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msgaegdd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uxgbakii.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fwdvwvob.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tqwavpha.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3juhpdgov.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3smomivts.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xlhaagpn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bwpaqdsk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jhvvmity.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3szwjoybf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3pbfffilb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3onwuvykp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rlvdcttt.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3doffmydy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3piabpsou.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ntbxiccx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fwypgmyh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nxlomgjt.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gppqdjto.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3jbdqyhdu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tdjfnrxk.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wkondkrz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3acxlyrca.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3glfizuod.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbeemojr.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3nmxvvbgm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwzpnub.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3cdqklixl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3youaduec.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3xpcpnlrc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3gjaygiyf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rnqfyisn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nlsjwhwr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3guyfihho.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3eqraytya.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lfnacfpg.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3daesdxwd.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3kmrghbsd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3csagslcq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3idwepokv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbdbegy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oqpiqsit.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3cwpvpwgr.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gezmfqlg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3zrayoehw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xhojpyat.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cludatvp.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ieqhwlnh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3arpotmfz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3asyzwycq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ahgsfosz.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3myakrerd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3fpzadvxu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xzfixdnu.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fuhmbgep.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3xbjpywkf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lixtkpkh.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gdizrjtl.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jmwwsvod.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jwysvcpk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jpcgttdn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ztrstlus.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ovzpoxli.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vvobyfci.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ehiyztcq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3bcxyneya.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xxwlirvc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3rkqglfmx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3zgtmbman.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bqptbeei.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qmlknisb.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmpxbhos.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ogvmqodn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kgsikzbh.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3xiapspvc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mqsijjqt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3hvzjsmkn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bqnmxuuc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iopfudhr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3otyqikkf.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3llgfxflo.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qsentnca.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jumbqtqm.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wbxovtmj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fbtzudww.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mnqqsixp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3hkvvxiih.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3bvnhebsx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3qfpafgtw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3cxycrqwb.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhapmgs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3fkulqxqw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrzvcvs.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jajyujnf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnveugcu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wfiarmzo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3wgsdnjfi.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjlxrkpi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ghjbyysb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwycwiem.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vqrxrgwg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3weaotcvi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xdotdlti.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ptetddqa.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xazrdqae.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwzfkdyj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cnvuvwff.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3habyewlv.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rojgsaqg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ykbapfku.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nzuwvrso.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjslxqfn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ryouiieg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fcgxqdox.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zbxcvxwc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gblnmrte.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sjrqyxlx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3niswoehu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vesldcoc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlykedqv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3zinywsyb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3nebwbscv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mudvrffb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubkzhcli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttgecodl.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fmoehejt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3cukflhll.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rkgilkap.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3zgkyfxse.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ylhkgwuw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ruijmajq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3oppmibrp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qbnianog.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uvjeazmu.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vnvayibd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3eopbezma.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3xstwikjs.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sjfufprw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jzhjuqqc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3znhdgqev.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ckdgbjtb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gyzlqtxt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ffemciuh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3pilvipva.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3gzhncdyc.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zlhjlnxd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vxoksqsp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3yuasxebg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cikvlrrm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3zrkcpjev.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3doimemje.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bwswnjtz.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3dtvunaej.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3vgwkkoja.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fwzrxvxc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3vbzhwggj.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3lwcbooof.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3qrxtyufc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qehjxymn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3tcgttugo.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdsgfze.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3omnhpuez.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3efyqhusj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3iyyuxgvy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3emozvtay.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uhsfdwup.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xiakmiqq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ojzpzfmn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tqlvbtay.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtxbrxnl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bsxdklto.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zlbveqbp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bjvyvhus.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yklkhcoo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3xprpnsaa.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3wirxdcjs.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3wdfaoobt.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3xenqpeyw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3obxjuing.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rszeeegz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fwiesyvw.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3lpvbgwjo.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hxxqhrjn.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ctzcbxrv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ajtqqggk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3fqvypwgu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ruevcnaq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3jcwwauwp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ehkybbzm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3ktrmzqjz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3eyselbxt.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3scdieztj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ctdpqmvs.html


<!-- 参考信息 -->