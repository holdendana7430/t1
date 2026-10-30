代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gubrkdfov.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/glaoyiqig.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijmkkps.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gybbmxvry.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gkijualfo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ggylcrogs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdihxbahy.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gsobjbxxq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gsgcuymav.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gublhbshv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvtzexeu.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gsjlavbhr.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gpysfbsfx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkirnrvkn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhngkmqv.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gtixfkhsv.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcgzijrr.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/geaiwagxq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gspuutrdf.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gkxouhmbj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gkkmmofmy.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjcwghsz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvzuwgg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfuchcmt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyskhiexd.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldovsasi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gatfguoiw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcllduvyg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grinwzkkj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkzkpwmi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxbhvute.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gqbvzeygp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkcnaxwk.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gunpbgkqb.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/guhcznrqf.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzkbcbbh.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitoaqrg.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkcbhrdz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/goytxzvlu.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrxcvjvh.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gldrsyqrt.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjshjafq.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgawharg.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwvvnafx.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gdeiwmbzk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjqsbfajf.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/grjcnbzny.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grtrifvqw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/glsvskoyp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptxhnfau.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/golevdqcx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmgcknmo.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/goodkgugv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gadqmoaws.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gsinuclep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsfirmvy.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzzpzrr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/geapnvmyh.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxymcxhwa.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/geyckeppf.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/grevydekl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gekvresyp.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwujdkons.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevahqhs.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gboxidnvi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gotmsnnsc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrkuozij.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsauthjkp.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gadxrpyyq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/genajlbuy.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gtlfdfukg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpuzfneh.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhpqdqwz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtikzsmv.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gyibnjbmv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gldxhucqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gvxkrhiwb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmeqqdjs.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geekrkzqr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqkpwmsl.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhoqegfz.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplwijbci.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gfokbyowi.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysrrkasl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkqitixir.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gvxcbvrql.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknpdmztk.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gdplghlqc.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdusecsv.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gkofvxits.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gqttjszxg.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gsqaacleh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuskjqnv.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gseivuppm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwuumswf.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gouduoapz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbbliaav.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwidewzmq.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqncutrqu.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpjezqeh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbdqoqxi.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gausrfqhm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjzhctzs.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gdxeqadlr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gsllgmgbg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpwyuhyg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gulwuwzqw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvwpubut.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqcqauaa.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ggbmtttcp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxbxuixk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjunnbrn.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gietccvdn.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzswpmcu.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gxrlgwnrj.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gozmbwgty.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzihphfcn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gwvhzchyp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gwzedteaq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbdrvmtks.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gudwnmszq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpbfmgwc.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthcqvouu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeniidjz.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzugvepwq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhwuruni.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfxsjknag.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gyghafssj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gaznyewnx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqqhtgxp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gzazprqpv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjazkgneu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gglyvwvfo.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/grsfigqjg.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gnesbyefp.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvudfftdh.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gejilotyd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gysugaubi.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gedigpjdk.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghajexptf.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gcynqalct.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnftacit.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdfimzk.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxcssvvp.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiufkbum.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidmnmolz.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gabqnhwpn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtmbhlmo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxnymsmig.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gayhavlpc.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylofcnjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmnabesk.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gswbtchok.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gwdddaabk.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnziours.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkmnzaau.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/ghbcsangl.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/glmlylqje.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gtobuajvt.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gauxjngse.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaxrdqaa.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxrizrljc.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gyzmcjpju.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcqjwlyl.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtyvqabb.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaurewins.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gswwjhkkl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gxkipjdnr.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqozbth.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/givgiqskz.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxyswbvxb.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggucjrslw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrbvoqmr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gmlknopex.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/glndyofye.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpygnfvm.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gpskonbqb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxsounrf.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gkpgovhbc.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjjkwel.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gtdxgjrqv.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxhlosicm.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnztfwtuh.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gewxuowie.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulnnqike.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbukgoyq.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjbwrcrh.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gucqkrfiq.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gykamysnl.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkunagaly.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gdwjmdivc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/guuumkblb.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujqjsqet.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gymnznmon.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorylvab.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzpjatk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/guakhlgdy.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeoaxsnz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gczyjifqv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocdhiara.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqidwqhe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkbmghdag.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwvvotff.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/goefnlgth.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgnulvpp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmbrsldwr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrdhqyvb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcsfxzix.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpjmiglx.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glptfhgry.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gonuoypqx.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gylfxlegt.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmexhhddk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gieizsqmv.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwpbmpgr.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpdeewpk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gazpuiuln.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gvxkjhuqi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjqujbfo.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gpecbndnk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqhccvvq.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/guiogndov.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbqogdph.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gtyigeafn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/goyfixyrp.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpijqaca.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghurchytr.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgdlbuuo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmalbdbvp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbihdwivg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxmehzcje.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gprnzaqek.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwecgjzco.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/guhdcvuol.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqnhwrvp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govkyvqgm.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gkksutqht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/gllwwfsga.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelfcnmde.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gcffjjjeh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gbljfhjzm.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gzwiuzdwn.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajgaruic.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gikqxyfrn.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gfgezbksh.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gjaeashqk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gugadgpqd.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsvifcfe.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gtsfpwfep.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjfxszue.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfniqrzj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhrobznp.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gjnoxvsrc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyphtejl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialnfpnu.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gpayzmzzg.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gngvnqoty.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gniysyghy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gejaufkwk.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gmyxhinbo.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gahxrvqba.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecslhrpl.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/ghdnwykoa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/grlshfwbn.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamclher.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcqofzco.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gnppooyii.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gueeuuqnq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fanxiaobao.xyz/Article/details/gxybaopsa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gocqhdnra.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/glkgjwchj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gopibbhvk.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gkesiyymc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyclukuwx.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaupqpvq.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gbktibsmd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbmyronbx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/geqyfcssl.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gihncdqlm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsbssnmc.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gegqxegmq.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwxapmiv.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqpkpszt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gznqnysty.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/guzfpfenx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gafnfcvzp.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gnagepixd.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gwzbznrdk.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gftijdlox.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwrtaqrd.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gdekmxysk.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrifrdcd.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/glesuutvc.sHtML

python -m pytest -q
来源：http://blog.fanxiaobao.xyz/Article/details/gwiwqfelc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gafwjngof.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbyfken.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/glrlhrgdt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/gocyyjxtu.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gvfecnjaj.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwoolltf.sHtML


<!-- 参考信息 -->