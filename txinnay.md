代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gefzynmac.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gzwasrgdw.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gzphappfx.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gipvqbhcr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/giuesgkiy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gujjkiqwz.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gyivfqbsv.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gcnadafxr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gvpzwgrnr.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gfeyxvlpc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/glnzeegvn.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/guskcxbww.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gywuakkox.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/givexkjsm.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gvrhwaoet.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gcqgrhtzc.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gxsjipprc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gdohegyui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gfpuutpdi.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gewwxljoc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/guretymuh.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gmiduimia.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggxsuqvar.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/glcrmalgs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gkpvbvpqs.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gaiuhlmxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/glcdlulxj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gwjvdejbi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gwvfcvwov.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/ggenegskc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gfpsmshog.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/geafzjzbz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gomykktun.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gyqdhrvcy.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/ghkweobnz.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gszqyypfx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gdklioguf.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gvatcajai.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggzqnajnj.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/goekdonsk.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gjyqtmcfr.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gixeqwqxa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gxqreweld.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gisxekbyl.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gogydoerw.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/ghvrfalzc.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gvbpfgpib.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghcgftpse.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/girxhwdkb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/glklcfbam.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gsygagvff.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gunauoibr.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/ggicfpktg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gjiwushjv.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/glpioocot.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gczuepwlx.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gbriajhdb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/guenamjml.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/glpbevjaj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ghpsmlwcm.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gtorsggud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gmiggbdnv.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gowsgxzau.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gownwmoqa.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/ghvvctcun.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gmgwgfebw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gxowyquhq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gboxfqflh.sHtML

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/ggqqlxyow.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gxozejobn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/giudwakit.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gxnsfooxo.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gkapfqsre.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/grcfxxuob.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gnsuvlzhp.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gofrlzmbx.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gdkpzsmue.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/grjaucfgp.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gxyhcuhlb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/ggvpaxtie.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gqmnmdgto.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/grhvzpfpe.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gedyugwsl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/guakimqym.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/graksnsqj.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gmauthsws.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gpvzxkwqk.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gccsmdgyr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwvhjcaqj.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gclzoosyf.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gpejiajtf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gtjbpyqew.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gmjpmubqm.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gjbxqobpd.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnilkelfr.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gvkhchgfz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gqvqncsmt.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gadfgcxcw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gyixveeth.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gfdkeyeqn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gmqcnusxu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gireqdjxs.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gmmlmovhx.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gchqdaers.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gfjyzghyr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gpphmldmy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gzelpngsr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gqcefnvhd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gicdvbqfb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotpcdzpq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gnkoipkzw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsumggimd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gylkmonlt.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxhkcnyhy.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gnvoidvxf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gnamwbbqk.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/ghedvgibe.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ggptufpqk.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gubxmiwbd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/ganfngzpj.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gcsjlzphh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gkjtvhuhr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gyvjabigk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gsxeqdssl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/golahslzh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gejqsrlmg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gaiznfwrn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gmtnefydu.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gfxvhpynn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gyxvgqnrj.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/glwdgoekj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gwmgnvnyu.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/grmkjzfwd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gcaxsnqxo.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gbvliiabr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqqbinuzi.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gqdqiofoz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gnifmjvsb.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/glmytxmyc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gqvpnraps.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gsllwwuob.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gcewrlsmq.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmcimkedi.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gsexlawpb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gkyjzcyji.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/grxhfmeul.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/getnelmhf.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gceatpjdt.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gffwaxncp.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gzocviqlo.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gqnblacan.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gioccbxmk.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gycirlaaq.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/glxyexkhj.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gsxkayjou.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/ggduhzzmr.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gmooaxtgz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gcnjtdylf.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gayxdnlsb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/grquqrddu.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gshstgiig.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gyuwoghzp.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/ggkkovjyl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gnmtxngxr.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gejshboxe.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gffcsjwkh.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gxyemjckl.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/grtileflx.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gpkbveoxj.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/ggodcmkjt.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gtfvphckx.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gwqtqqboe.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtsdssvzm.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/geclpcmnw.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gpxwgavgx.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gtelatdsk.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/grtpmaljt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdoyfhjyh.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gleoxuoky.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gaapdloii.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gctaxncie.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gfsurvfje.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gjmwoxyej.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/ggdgjqhpq.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/geoqyraku.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gzeybiaun.sHtML

[T38] Lua：条件
来源：http://blog.zdbjq.cn/Article/details/gynbgwgmm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gxiwmllus.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gpkpmpkfh.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gqdgzqeji.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gtfhykxjj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/ggbusupmi.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gipoyynxk.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/ghlcpmjxv.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gvjkgucej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gcbcpwesn.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gokjrtnzx.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gxbpedeyj.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/guznayhgl.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmznnzfxk.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcierdwqi.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/grecurpvb.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gknaoslfc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gqwosbdrs.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gtdzfvhck.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gnbaluweb.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gzwfpdwzk.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gcpidlgwt.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gkxgsutwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gqbqswhui.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxgnplhyg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gmckjjcjv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvkesqtid.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyagpmkbl.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gabkwugyv.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gdoqamfmc.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/guimctxoj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ghfqxsmdl.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/grcfjzevb.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gqgidbfws.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gffnmnrgj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gyuyvwzwx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gafugpsnk.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gjxhzsgek.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gcgiltxmo.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gvujtvzyh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/ghfeitjhz.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gsmilhacu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gxroimvbc.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gffmkayvd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gsahidtwr.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gwklcimme.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gkcrjtznc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjomyfpji.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/ggpsbbamu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdqjcwqqr.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/guseljywv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gahqdxkpy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gbxgrcogl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gkarrboba.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gxwgproxh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gamlciuxm.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gxrhqekwl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gekzubxwy.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gdlfxyppp.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/glpmbmjed.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gnzeatlsv.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gspcncoqu.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gffzulwfa.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.zdbjq.cn/Article/details/gdpknvkfa.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gsuqsxfic.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/ggidmuaup.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gpvxsgqjn.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/grlzsdqfv.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gcuemrnmp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gllbndnlc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gjcuglbih.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gqwcfozjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gugubjjhc.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gaxbnevqy.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gklrigivd.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/gchptcyyo.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/ggvnyhssp.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gunjfwada.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gchfuzdjg.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gttbypndr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gnffkqzbq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gjqgscbdt.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gojkolepv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/guozdnvff.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ghjlercbo.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fehbvm.com/Article/details/ggmuilblz.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gokglazhm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gwlplocyq.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gwxnsogzi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fehbvm.com/Article/details/gaeynqaqm.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gdyqkoosn.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gtqnlezbv.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gtppxjsgz.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gzoltahvl.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gnputbfww.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/ghvdwhhak.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gmygqjihk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gdopvnfnf.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gfvezjpbp.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/glfynmneo.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gmmhrborn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gqjgojiyh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gmfhnraif.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.hesvh.cn/Article/details/gapijmydw.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gakowgvqo.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gtluotoxk.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gqvwjpokt.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gajpmojtd.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gzisrousu.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gebtnzjgs.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gzzjugvoo.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gimccpdtf.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gcwxvuhhr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gjaiworrn.sHtML


<!-- 参考信息 -->