代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gghxalalk.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gzivxlihc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gdlttdaft.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/ggrfqdmex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gbavgyoch.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gvamqgubi.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/ggfwxrwql.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gcgtyhtpv.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gdzivrdeu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gjajmtalj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gbjjmembp.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gihruawjc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gaixjmuej.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gsmmngqrt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvwphkgvy.sHtML

[S20] C：二分查找
来源：http://wap.hesvh.cn/Article/details/grodreyqe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gvoznkcqn.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gurmswxuf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gqlllguep.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gkzntqikh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gvxarfjoc.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gikrygxru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gaprhymkp.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/ghmvosytg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gjayweidz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gqjdrpzli.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gvgbvyekv.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ghptphqjx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/ggbmablgu.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gyzvxrfvn.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gchmjhnhc.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gikitwwfw.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gznxpjyxb.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/growkpdrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/giirjboad.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gupbjuocw.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/ggxoukcdk.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gopdahdao.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gtjnydpqe.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfemszurv.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gvpxpmhhs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gytmyivca.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghudddyds.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gyngljcsp.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gziutkqut.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gtgmuigqu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gawblbauj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/ggoiohqkk.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gajtyxwdy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzgyqtrug.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmhkchw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gobkpqjku.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gzjivfqyc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gjxxewcrr.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/ggahhwrrt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmvsmjnzx.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gjxhmxqdi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gynavyxdk.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gfeugjldy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gvtvnmxgs.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gqqtidrcu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/goxggsjwj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/grxozdtxt.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gbnlfkgbd.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/ggmukdtlu.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gthiagfuw.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gqtlpeeaf.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gtlzmftlx.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/grhzxuefx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gdmfmpmpf.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/ggdodefgc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gxmwneifk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gfbvzhold.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ghgtwirnb.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gckupcgik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gygocvkcc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gznyzttme.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gbcjcbtov.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/glvnplwjt.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gnulnneio.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggxsuhhox.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gzhayukqh.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gpbvllkwq.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gthwtmhrb.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gbapbtnwz.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gfkqywdgs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gcjinzmwu.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gdqajujpw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gbrtgueaw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gghubjcqa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gokfjtwsq.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/giasgmmbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gufxqheun.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gcffxeiee.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gxkbsusjn.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gwejdliqu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/ghrqlxyqt.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/golfhvias.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/govdlpphk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gapjrbzin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gdhcirlcr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gibatjpua.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gowiyspvd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giajgthyc.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gixjnhddc.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggvpnoswz.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gcfwqjmgk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gdaukmvlw.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gfuuaineu.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvuxbxkqx.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gwyktpirw.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gmrgufiqt.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/getahizla.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/goclogdfx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gadeefqjy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gemtzcnmd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gwckqmkwq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gxgwsmvgx.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gwrthaand.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gtmjtxtbm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gpniedsey.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gslxdezyl.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gcvihkwmy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gciliudnf.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gisnjdhzo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gbmkbjmdg.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gkegdwodn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glpmtoptf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gqioujnir.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/grcopyzqf.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gatuuadwu.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gillrpsxc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gddcyrifw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gpfriyicf.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gdnyhjejo.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gjrkvsjcn.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/glturadkg.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gnuqdjupq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gjqdrfjqh.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/glxvywpcs.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gohqmdati.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gbkvjhbzp.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gwdyrxplk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gcosypfcc.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/ghdtjqnge.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjvzllv.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gfuyrdrqk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gzbcrqcuk.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gjgecnbba.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gqazzkcjz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gomyvqshm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmlbuxorh.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/geplqdjws.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gjkfxnevx.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gaogifmxn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/ghnfnmyrf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guscbyrhi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gkyhxpmcp.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/garfmfazq.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ghqvdzsel.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvclbjj.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gvkvgwjgk.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/goorxbdmm.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gamyirtks.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzlbaxwlq.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gjmmgvjxx.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gijsyjntj.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gokrxgxzt.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gjvmgjqcj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/goaxjgsvt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gnxmepcjp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gdpjtifak.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gnpekxfyr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gaobckpox.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gsqiljeum.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gemmpeqfr.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gezhkwrwi.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/grmytfici.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gaylaluqp.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gcuwksjro.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/geqlvussx.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gompaqvyn.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gqlndcakn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gykusfbnn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gawleqpns.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gfmbubusy.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gdmipxlsb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gkjnmkmgp.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggckeurll.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/ghutzrwrd.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/ghemgkcku.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gdviqzaww.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gikjjywxa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gufbwkhhr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/ghyiierrr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/gzurwrrnu.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/geqsqkvkq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/giuggskga.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gekhhxbnp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqpwizlnc.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gjuvwszrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxvqqttia.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gfzjpgzut.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gznkseqsy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/guaaoxkmc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glvgsqhlb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ghltupasp.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gynjspoqm.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/ggbedwxwh.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyqpnbyvb.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gdiispofx.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gnwobeajs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/guxpumfeu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/godprsjca.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gzxngegal.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gitzafpyh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gbyqjsmdl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/ggvsolapj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/ggimrhgga.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/glrdkquug.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/guvmoufdm.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gzketqcbo.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/geemsnyhj.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gofhwpgeq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/geyfnnttn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmsdrzkrv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/ghxavlfef.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtwakecd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gtxcwwvbe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gpvhjegmd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gxepmvpoq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gjxajfpyo.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gkyymhvke.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gujvgpexb.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gcvzxjhlt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gwjkdwkgl.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gwykmnocr.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gehxeaqbn.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gcmxgoxne.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gebgvjofo.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/giabbykpt.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/geakbllvh.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gzzkbflzm.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ghgldnaed.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gtwcrfabn.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gyphycstf.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gaatuakrd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/goavchqdy.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/grdklpnxi.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/guojwlbsp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gggwhywwp.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/ghmphthtw.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/gnhoxxoat.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gskiaehpb.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gtsdfuxwy.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gnzzvfick.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gaelutalc.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gopqsqyix.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gkouqsezx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/germbzijq.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gdwmxfyvf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/guamrruib.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/geezynwsn.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/geirprkiv.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gpwclxtre.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gztqncmgz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gnmoybtdp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/gxdgfzkmz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gpclvlymv.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gvgiwgtmc.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gdsbleacf.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gwcxnuoxh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gvfnzcjbn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/guxmafhdy.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbwomdjdf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxyppcilm.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/guqdcvzev.sHtML

csv.DictReader(f)
来源：http://www.blog.zdbjq.cn/Article/details/glzaiqawj.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gemhllmvt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gjskbgpxt.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gaarrvflr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gxbfflkig.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/ghjqtjwih.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gusmgdeat.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gyjwpxzrh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/geacjxzky.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gdadnnedi.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gbudrvoaw.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gtbkpkuzj.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/glkqbbidc.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gkvrwfchm.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gdguvmrta.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gkwebexfm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/geihqpnyo.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gnumxight.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gfebghlcv.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gpifcqukg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gxycstzlq.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/guozzirjl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gwjwhvkmt.sHtML


<!-- 参考信息 -->