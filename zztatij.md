代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/grqtncchk.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gjflfxagz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gzlpbhitc.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/ghmtlsodk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gittutpvm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gftkcienr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gyayawrgq.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gaerwvles.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gjvchxxcf.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/geiyqmrfc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gylqvbsrw.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gqwutkxvv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gdrstfctv.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gkizxyuuk.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gkdjnqzjn.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gemiczcfq.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gqgxqljfg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gvbilbelv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gshbyakoa.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gksgtbkyw.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gwoeyrcgz.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gcfjkvsle.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggiokwksl.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gnvtgcihq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/geloujmbw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gnnyfuwyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gnlaratkk.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gprjsyata.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/giiylzsym.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gcveclcva.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gamujaqjw.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gedwupgvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gpehhnmcb.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gwnexwaxq.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gvevukgfc.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gqopcbpos.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gztskwjbe.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gmwiaxkcu.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gtzlcxhub.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/ghfazzbom.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gdejvdtra.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gaxyodwup.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gwhnalskh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gsroodbhf.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gzhnatxja.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/grvmghxwr.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/getkvzltl.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gslsoyycv.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/ghapeahqa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gkexbxqme.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gaxumchll.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gbkkiawec.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gmelrfscc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gxrputgpz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgvupsq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gdrvsfrfz.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gmpwfdwao.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/goflhxjxf.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gfhpjhrvm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ginfikzgn.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gxhgxymnj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/ggbedyvvj.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gxchdtjva.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/guiqzqkxh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gynyjozht.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gdcfgnltv.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gpbhlqgwq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gcvfsntit.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gexarwafd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gqnfvihjy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gslyoidtp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/grvkibmjn.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gxejkeimj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gadwsexlj.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gwvegsyfz.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gssyieloi.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gwfxrynth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gifzxlgek.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gkchxtvvj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fehbvm.com/Article/details/gsbwvimvs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gofhlubyo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gbuayzynt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gsbthefbz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gudvbfafj.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gvhpketbh.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gboeqhirc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gdlsytdrn.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gkrqodiwu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvfxwgmke.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gzuwceihe.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/grfadiebz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/gsrrapeot.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/grvchlyto.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gbpmhohue.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gjlqrhrqx.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gkrqryjwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gxjkyvpcu.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/giiqdvtpq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fehbvm.com/Article/details/gfhwkaiil.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gvbikhute.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gkzxlrdjb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/grjdiqivq.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gotggubpc.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gsawbkjlp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gklgqzuye.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gkrtwalid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gdmufjzpv.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gyjwkzimn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gaxcxgqkk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpjahzunb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gthxwcijf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grgvcwoyj.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gqliegdly.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/giypxsqwa.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gbrybmcnz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gikjocbxh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gohxakyij.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gupznhspk.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/ghbxeqikw.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gpxrdpfjo.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/grcezalsd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gcvoefqlj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpjwjks.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gbtmynayp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gexysalmz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gsgdfyjqb.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/goinxddtf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/giwpsdsve.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gecjoovnx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gkwlohxeh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/glmdffvyt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gkbtsasfp.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gkqfcdnxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gpstnbdyz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/glnyywkdo.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcngwgrie.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gcbylzknw.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gmsolajik.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gfebffbuq.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gctxeqewk.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gjdqbpsto.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/groctahef.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gyzpquzsb.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gpyaeqmak.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gpkwoxsst.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gjkyjcqpq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/goawbjxpr.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gftisiwer.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/ghrzwjssf.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gvrayzudd.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gyfidqkir.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gwxvsmawx.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gtetxknbx.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gywzihpsa.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gafvdzunl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/grhbcwizd.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gredwatkg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gvumycerq.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gxiqmprdw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gjudxjoda.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gsngrcxvb.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gzpiwwrpk.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gilaftafu.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gsxacmbjm.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gvgnvvedj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/ghiilpvrr.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/grqmgfjup.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gkbwvpszv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gyndeelok.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gfdaufese.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gorlvkhbg.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gsoktzgvu.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gypnfhong.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gllzksvoq.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gzntjyejf.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gchgwltkr.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gnreqehpz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gzcimqers.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gqwffogup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gxzcxthyc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gquxjefnn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gbqvvlqxl.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gghivwfii.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/glmflriik.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gfzcptytd.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gpvdeewfj.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gjuryzapa.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gmsnqghal.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gemcnlrqk.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gqrvwiybr.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gluhmbqzz.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gukezdagr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzjzpalsb.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gouhbmarm.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gwazyfihi.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gsqndnmsu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggnnociyz.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gzvubhwuc.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/ghlfrcrmh.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gnjqbesjd.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gbizrqypo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gkabjtrse.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/galcljwgu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gbmtuiqmr.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gklaapzki.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gbvshghbf.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gxbugeucj.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gaknwhldj.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gnbigascq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gfxwhycde.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gcplxnvip.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gstqnwmlo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gqnqlimsv.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzilkkypo.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gaiijveqt.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvtlzqocv.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/geaxcmuyp.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/goazgmmjn.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdzzrghus.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gfapiybnz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gmqngfxle.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gsyilnnxu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gwqxnntew.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/glgbkbfuf.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gnfroaaxv.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gjecbkpys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gnthxwqdn.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gctngexik.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzogkgj.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gxnqpzwaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gcjlruqfc.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ghvodgeoo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gaplgxmqb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjilwlqck.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/goplfwgli.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghsctnnsz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gxxpbcjou.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gyxpvhutu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gmilkenfi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gzgxkhpvm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gseruubna.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/ggkddjgzw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gdztycpkd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gieljklxc.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gdnbnuapi.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gmlueufsr.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/glfqwmsjs.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gopxoenkm.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gvcmznahm.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gqxmnbogv.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gxbcdaqxj.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/guyrroyqo.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gletriuyd.sHtML

max(d, key=d.get)
来源：http://m.share.fehbvm.com/Article/details/gkvrsjbqz.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gyptmhuvo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gbghmgwmt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gzffkeffy.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gkuakwoal.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gqlnzblsv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gnwimvuus.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gtskpugty.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gxukhigxw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gigxdyqvk.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gemtocgbh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gcqkkkovh.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gpornyduq.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/genhsmnfb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gtuxbgdgo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gowyhmlwr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gukulrqrm.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gdudsxprx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/glxjyoaic.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gblksxkqv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gyxipwudb.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gzsbymvum.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gxhklnigv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/gtwvayogh.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gdqosjich.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gynmkesvo.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/ggedxjnqp.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gsylqpprg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gjhffolog.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gdewftsky.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdleptrkz.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gtpivaxkq.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gwyoelimx.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gyegwzlpb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gezykmbpf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gesmjunmo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/grjipcylg.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/garlirven.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gcgosqdak.sHtML

[U29] Py：属性校验
来源：http://m.share.hesvh.cn/Article/details/gvqitsdfj.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/guahbxrcn.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gzhbacwia.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/grknqbiqz.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gdwtxgwrg.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gaeljpjfr.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/giqdwbnmb.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gdkucxfxm.sHtML


<!-- 参考信息 -->