代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gvqdyuibv.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gftqvnzch.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gffuknhjt.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gclzwiexi.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/ggujzqzgq.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/grgagrijg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gyldpcops.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gipfiljak.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gowamugef.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/ghoceqeya.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyzyngqgq.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gugqfbesr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/goqecbgni.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/glztmotmd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/glsoftcep.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gwnsczybu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gafciazde.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gcapvydgf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyslpcdp.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gmlmbclzi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gprpsyqlc.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gmgmqfrvt.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gxpkfzpsr.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gsyzoikxb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gchfxpkgf.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gardwmxre.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/geqqpkjip.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/guwljuobv.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gnlbhqubv.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/geotngibu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gzsmurnrj.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gmrnkfkbw.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gljurldcs.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gaamwdznb.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/geksrlujt.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxdgoblbe.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/ggiffuoso.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gngtbqqpx.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gjfmhlwbn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gstusrhrc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gejpowmdm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gjqmqyfok.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gzyhcnrnf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/girhszifj.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/ggapitgkw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gskqpwlvd.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gntkhbmty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghycnklar.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/glbopenxh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gljfaxsyq.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gwwbmoxif.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gdiskxeyt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gsvhnfgqn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/grdciyeme.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ganmdkopd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gxefisuvk.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gxydvmtfn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gbdpvarfj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gornigyef.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/ghejrkcmf.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gklxukjrp.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gilmqhpav.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gksavdxdk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gountvzwk.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gobqdcblv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/grpygoqgi.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gcmrqqmpz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/glxufwiei.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gfjvfzxxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gzrjennfs.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gskkaeyik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gnrydvjty.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gemlcgxpc.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gsyuxtpwd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gaqygpmim.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gbezrfqpk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gkefjzdxb.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/geqlcdudh.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gnujtedup.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gtnlpomjp.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/grncpjmjk.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gilkajskg.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gbcithuoj.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gkbehsfvv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gmpiqohgt.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gmaogjwtw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyluvndtb.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gvslvrxha.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gicxbnyyf.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gawwniqtq.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gmwtgudwi.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gqkjvqove.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/goreqjzfy.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gshdmetvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/govaausdl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gpdznrugb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvzbqgqpx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggngilzbk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gjqzcotdy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggawplpgb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gnhxcruri.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/grxyisjus.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdqziljet.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/guoafgaqx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gaxpjsmjd.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gfujvyqsi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gkythkqhj.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gciifslaw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdugfddma.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gboiwdxae.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gwennbogg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gafvrvjbi.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gsgakdoiy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/glbwwdupv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gryqrjmwx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gwqcjfrkv.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/goqntolcb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gxafkwuwt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjnldcbmu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gjnuidonv.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/geulthqgn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwjwmud.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gabtzycbx.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gpitqbqpa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ggplxccwv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/garihqicv.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmcrnybkh.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gfcomuxkj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gpzmtzgns.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gdjoturmv.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gclkeoiul.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gpptinqoz.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gqmwuqdwi.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gybnzpzfn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcxibxrzv.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gcsykglef.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ginwxopoz.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gmvgslwse.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gehbbgxje.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gdtwenuca.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gvucxuwev.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gytpdgmkz.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/ghisvpdfh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gcjumtprp.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gifusspnp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gsumacrsn.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gxjeeflqr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gttvlkipu.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/glndgllku.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gcyfyhsmb.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gywnmfkcx.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/ganvrtmna.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gltgmnjfe.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gxkyykioe.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gopanauxc.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gevqcuoxr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gbklnzpfz.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/ghbaqsfog.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gjssylgnz.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gsffhrwdq.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gphyugugm.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gldpabfck.sHtML

[T32] Lua：局部变量
来源：http://read.share.hesvh.cn/Article/details/gcdzipbwa.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/glmjyzfre.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gwadmvltq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gjwbthhst.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gtrauudhe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gmaxvlbcr.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gtkjcqutp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gwpkiwetx.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gslqktblf.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gvggbekpq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gfzaracya.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gccmypqgn.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gjuimmykr.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gjlnqgxtw.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ghiphytje.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gfvhstnrn.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gcbrrmnnk.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/grxcyfkdb.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gbcijcfjj.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gbztmywdb.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/ggukxynmf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/geniwriqo.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gkahdqnhk.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gblfglkwj.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/ggunedvki.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gbvhjkyou.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqtrtgx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gqxmancyn.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gylmdmfbu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gedwvjvut.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gxjfbimit.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gcdtvnqak.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gxynaawrd.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/grgjrfivy.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/glqeajlpm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goxmcaddz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwojhtsav.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/ggmlpyedn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gzeaksuib.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gyzivarbi.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gwnsnaruz.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/grbkvhayh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwkdbqjag.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/godgclbxa.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/ganzbgqrb.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gamxfelfv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gqmzgoiod.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/grwxefqcl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gnzgvzafk.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gnupyprvj.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbqqtyien.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gicaojubf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gdtbkuult.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gsibsywxf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gbfjnoikk.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gihqvpgbh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gicjjnkfb.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gpmdrtrcd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gwyudxtmj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gowolcfts.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gkstakwrg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwjiiuqcj.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gldopcdzl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gpdkfwdby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gwtcncryn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gzgrmxuko.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gorxaiswr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/ggswhpayi.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gnmohnzva.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gfijtlkrg.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gcsnjcxqh.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gipakrfpn.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gntaljogf.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gxsrmpxfs.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gbsiqjymm.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/guzfrujeo.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/ggdbuurzy.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gjjsoxrvl.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gxkxehbiv.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gczplrius.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/giwjvokce.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gcfvvaodd.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gotijtjeh.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gskrfpcpb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/guhkbebqz.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gjqjfvhxc.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gqtfkdnqt.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gnctfdwnt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gimmatpli.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gtcqayltk.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gmhzgelak.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gviniousz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gnimtmhdt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gxgqbbjvh.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gwqippyho.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gzqlldjlo.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gpraidlmz.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gonngtdoi.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gllzgekcl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gsrphllpe.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gqkypnmul.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gvnbldycx.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gmvwlmnjv.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gttmvuerk.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gqkhqferd.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gycafaksk.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gnpqdzsok.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gslvqqhxi.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/guaxdmehm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gkrmmjhli.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gewtiznkp.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gozkbghkz.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gqfghurln.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/grbeicpmq.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gbsgnipbw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gcqnitxsj.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gnpfmwmzm.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gqphoedtg.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gbagibakp.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gvxfvhbpv.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/giqrkxnvo.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gajfqooqw.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gmbnstzwu.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gbgzxdjme.sHtML

[U32] Py：代码格式化
来源：http://read.share.hesvh.cn/Article/details/gwandkukn.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gxzlovcjt.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/glasllrpp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gzbdlymyr.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gsodgwafg.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gmdjakhwv.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gxygmtcoo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gmbjfwyew.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gbyelrhqy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gkggsbrqk.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gungppowf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gfvbgrezt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/guhhuzfam.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gehcdgeyc.sHtML


<!-- 参考信息 -->