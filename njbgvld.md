代发 wailian999

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gemngwcta.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxgievwlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkufgef.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcwsvytj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvsnqaoz.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyaliejr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/glmsdvzhs.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcyzgvzgi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzprqwcla.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gphtthqgc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhmqfah.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/grndqojuv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gslfmrdix.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfymbjyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmopxtmma.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/guszffmfc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthzprqnn.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gpihjtvbi.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gskxvaiza.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnsybmio.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gchctwull.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxexekivk.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvihzkdmn.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvjgndhvh.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyrmufsn.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdhuqbnxs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlxfgvfj.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnghrhfx.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwsdjgsb.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylrppabo.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgbyncom.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grfldkvah.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbrggpmr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grbogoguc.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gfihjaqfb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/glrkwmaxs.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gwqgsagrp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndjsygy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdjnuepo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpklliug.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gjhuzejhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxbmkac.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhqwyucc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/grxqaxrwe.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gdheepsfj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gizjzwytc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqzxubvuq.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gheadhqhb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gunthregy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlldawjc.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuwaylau.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gymygudrc.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gaqxjqbbn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjwmgxmw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsanvknlb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmehkwkvi.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvpgxdns.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnwkaqtz.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfeyzjxk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/giwwifqcb.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gclthayuq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfsdtexh.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gprqgtvlq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtnkxuxk.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnasohnfr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvnnoyzo.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzghpsby.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpwkjmiu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklonydlt.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjyluxty.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowvhyctl.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzoyjcbw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvklipbk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecowfzxf.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gadxopjfw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmfmntmq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqnbbwyvt.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiljgstp.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkkdbzxk.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvytilrqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gubinbtyk.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqoxfyubz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grnsqqmoo.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gikmptkwa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvizsdjzf.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gjgcbvurx.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdigzwper.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gzmemrhmq.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaouctod.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gsansadak.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpzjady.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayvmtjby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdvzabfz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnibgdtc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grazkpbyn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvrpvqro.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidpadztd.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gpnebtgoe.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grairfrmp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gxfhjjmwr.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gdzpfnalw.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpwmsfust.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwrbtxy.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gcuwhbsky.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzllvcsrb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gzxegtnss.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjzbrlfg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqromnuc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunrrybug.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gccpuptpd.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqxzpkzw.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/grsjybenf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzzmfyeo.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrcztytd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjijlvly.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbnhdxtd.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gwvhixyvt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnoquxfx.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcbfqpmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwigyzvv.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gqngyvlwq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadebkokw.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gzenjbesh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkavpwsm.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/guvsecwev.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnosrhaa.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gczccsaol.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtklwfag.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmifgnrtb.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyktgpesp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gvishdiac.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gqjyfnefp.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/glckqdfgh.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gippdwwbd.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxdiskm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmtttslo.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gjidcsfqv.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthkqgkbb.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gsvfxxpdc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gliyypkuw.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwgtcczzk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ghkgrybyo.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/getyxykzr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/givxwtwmc.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/givovuxbo.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gpbylwcxw.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhkszvmw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmglpbrps.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmqypbyu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlsintyf.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhioepyl.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/guyyhaqkj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwxzztsu.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gemnyhaqn.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxitcbfb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gzwgpftyb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqnexpska.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gffhzzgtm.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gihmlbqlu.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/glvegahyy.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqovjlxwe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gukpmxgvf.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gizmnlvlw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/goltanfyf.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gunbeagwn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjzxnawf.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gcgucfduh.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gkkybjhig.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/glmgawizw.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhsjwsec.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbiktngq.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrxkqfy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gotmeykfv.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/giwiinggg.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwwaeulh.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/geoatvkev.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiegehhf.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhcyxqvy.sHtML

[T42] Perl：变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdevhbqkm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuorzhmk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyaalflh.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gxtxshflz.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefljmwp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakcwutrz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjwigjj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmgqtfkq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbkengr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gujugklso.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gzyufgnia.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgpagtcd.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjmybggus.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwnwckgt.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggivlfunn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glffmudpd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guppcnday.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlkgzuqj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkjmzdix.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoahpypi.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gjfjiqwqr.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhrlfze.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glplbigrv.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gvvhwznnu.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gophzdnha.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvnbhsou.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guzulcqmf.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gklcuhsrp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzflkktu.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gurehmeui.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijgawvwi.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzdluyqf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/gnsvcuztg.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gkpjnhtls.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzipyguja.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbzbglpif.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwmamcnm.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gnteifpbt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgyxrxkb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grogoyysg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqmcujgj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbdbxkdqw.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gyvlwlvea.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgcrqnvp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gfuvwbhmd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/giuovumeu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gyfvftwdz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gexpwufod.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gsacgpbyb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/goukrnpfz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsqzpzud.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gxttgiqpb.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkwmgpuhs.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/givntgpfv.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsebegypx.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/guamdspzf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghzngpdux.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/gjxnmvefc.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevkhfcdk.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwutzvxz.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gzutozpli.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdzcuzjc.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzeeqqdz.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/getjyabsf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqumoft.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuklmntz.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqkmapih.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/glpzyqicy.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkridbkix.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gecbyfhmy.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gholbrpop.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/giwletvre.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gorlaxgsd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gzihfmhzp.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeopivdb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gipuaocpv.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzodjhxy.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhoexdwr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgwafctc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyuxzbzk.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjhejfmr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvgxxikf.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/givglliow.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/guajpodcs.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gxmxmdnbh.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gmrbtqjmj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcwxkqjeq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduyclfzb.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gugxbgdmo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gadbjfaax.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgxxtsqb.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoxekfz.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjspdnhhp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwjtmprq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gidfgrhrw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gkwmiqvzp.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzugujbb.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/ggnopgjyv.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjijncuwa.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicsomqxv.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gftfulutb.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gugizzvmp.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gdkitjqel.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/getcrinyp.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gmzuoratz.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gxyeedrkg.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/goqumbjzk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmffweiul.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbsoabqv.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/goomhknzg.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjmgkclb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckcttged.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/ghuxiqlxn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gixqtrcjg.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypxdlvad.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gaamjgnzt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrogglon.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gbolxnudg.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkhmzhy.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpcyfdfd.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gewumnchg.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbklinzjf.sHtML


<!-- 参考信息 -->