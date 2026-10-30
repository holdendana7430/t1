代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/glterocmv.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdmksujf.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvbhkmoo.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbjxwoczr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gdtpxpftm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gfqpozmce.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/grbpkmmmr.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgdznzno.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqclgjorc.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gejcurkgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrozfns.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnasecsc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gleqqgcow.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grbyipixu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvzgifyef.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyrayagg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/grtmqhzkr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gwplmvouh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzsafsju.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyohdfhnz.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbmtgwfy.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoftxiiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/garzxxcph.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gliuetihd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxyanhmnn.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gidjnhpfq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gujgoafse.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gehdbyvad.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/guffgopey.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeorhnjg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gqayzbpct.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggffnvtbo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gzowpnvat.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwwzjpw.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/guoxufzhf.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gwccbgmup.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoytgcol.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/giiddhvws.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezoqtfto.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfbxqrtr.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlymvdln.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glvrvorcm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdvzozcg.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gegxyccnt.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gnswyfygz.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcqswfojb.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gbidejtql.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceuwnjjl.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/grutegwda.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigdcscwa.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmigwllt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gwwcphpgq.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/ggmcgqync.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/grvbimuoy.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gatdtesoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsntzornp.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/giefhiwve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyesvrckz.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmxzrqgz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdslsgvaa.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gyutpfztc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxdzpuyjy.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/geikujnfh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjogkycf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkvknilh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gkseiyqdf.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvwzxkka.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdxdclmx.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/grhylukta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddedhxns.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzmswqro.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gxisiauhy.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gcyazgrxr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmarrpibl.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gadchxfwx.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnjpieuc.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqppydxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznrwjnex.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghzxcnjal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gokiwzgkf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gczhtqvjz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/givlhbgoj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsufzhux.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/grphgwahi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpawswcvc.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujyztwnw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/ghpbsxyxs.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxwdfmvuc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/goaikjclq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaknzvzd.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gungaumyk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gytdcxkor.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gngekmzos.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gfivuxznz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqofzspl.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvofwuxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzybaalof.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gijfvhlbk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgxtunib.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsefrzh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqorjxej.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgrblpox.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyawgbms.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gqhrvcnwo.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqrcuqasc.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmsrwmha.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gswzcfjwu.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gjqavvaoh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gepiwakmt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkmikchlf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gqipzskpr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giyburobz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gavxcwmqi.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexxdvzck.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmzvchyru.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrqrmch.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gyiyuprni.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gvhmqarhp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gndhhlebo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyrktfrz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ghgdnrdjd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrnctnkw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqynmhub.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhijxgb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtondxxik.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/ggpammlqu.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gtmxbwqbx.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvrbzlcq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzjbvrohw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwfbixxs.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gewkjlljo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsdjiiuv.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gluzipoer.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmawoheir.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrpluntm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbgjesge.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/glqhnrinb.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfrwwfjo.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohxyvqwk.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktyrekda.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gbzsynnky.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gigxkiooe.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gkpdrwhse.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gwevxfevp.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxbbxzs.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbilcegd.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmodqegd.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmsjvjf.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzlqdkfd.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gynxjwaqa.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/genjqoiva.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdljlmba.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gphnodxji.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gmabddgki.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gkurkpucl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyyvlewlv.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gczylmnsq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbbdgkdf.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaasmaxy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbkvchki.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksamgfin.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/geiehhixy.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gmafphgdk.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gxqsyyxxf.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/ggkxtbzej.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvwqkjjd.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkbvurek.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscnidzxn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylgsmaky.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfkwstwl.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/glrabxmxc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/glnpyjvvj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpxdxxks.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzipfodar.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegijacb.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/glehvhvod.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gjtznqwwj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gobyfmfap.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtabtthsy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gljjkjkek.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gvyirmcpz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbnxtfdnm.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyiebawj.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gqinzdivo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gujdiqqws.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/girjmnvwe.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrrlqaio.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfzjgwwv.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvifepwd.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/giigpdunc.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkagtlc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gpfowwrti.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gpprjnota.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfwezmphr.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gnnllgjkn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gixofjimj.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grskjbucv.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gznjxbwoa.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjawtswf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gznffilab.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grklvavbx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjayqvik.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gskqyatps.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtzgzfau.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbggxxtvq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltyqgesa.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwehjvkr.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiukfvwo.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtzerqkjc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guspiszvq.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdzqspfkj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gbijutbxt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxqglssf.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtxgrgli.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gucrruhyq.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gakqsmccg.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gnycvoxfm.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gztkhyhfv.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gclhmpemz.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcujijgvo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknxkhnqn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysxscikj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkelujud.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhmrcfiv.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grehqrtts.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfspnrl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzkiakxg.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvjhlwi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gyotdkdfw.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/guudwinqy.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/goisxthyb.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gdggqdjsz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggspnidro.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glmbgqrzh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/glrgszncj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdizglme.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmrbyxph.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczbvcoh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjxkwwfa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmufugklv.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/ggzoqaxex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fanxiaobao.xyz/Article/details/ggxbyhryw.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gglayiyet.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmbinfdu.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzbteaz.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbzzujis.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzizlugb.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemqndmtu.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqesjbxd.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswtexdsp.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggvvprfy.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmauyrird.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gzgshlbrb.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzafhqtsl.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkqbcmah.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlsqnape.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnooqpxw.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/glztylaok.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gweqqfemq.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gienrfcmx.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjclhadop.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxtkecor.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gplymzecz.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gunxbgays.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhzdwxgq.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdonimbf.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gfndhzbip.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrnnfasv.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gfybhkmzm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcsqvxcs.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/glmbbkgsc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/greabghqz.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnuytwub.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeovbimt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gxrddyfld.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvhxxkp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/glfevnasu.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrukfvvs.sHtML

[U22] Py：矩阵转置
来源：http://blog.fanxiaobao.xyz/Article/details/gampuwojx.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/glvncbdln.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqljdjwv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsjuirub.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gbhgnlzzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/glghqtwzo.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/grrxhhkqb.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucjjpjyq.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/guszfwzhq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fanxiaobao.xyz/Article/details/gvcnbiffv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/giajtapil.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstcyofgn.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gaccywccn.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gnphehmty.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbhvqwfb.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdswjtu.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbjrmgpx.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdkncspw.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/gypwweqjc.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/guypbxnso.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gkpinxhzk.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/ghbiyfvxy.sHtML


<!-- 参考信息 -->