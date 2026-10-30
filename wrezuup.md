代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gowmyapsg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomzsxwrb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyitjhcte.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnutdnkvm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcyhvkh.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndmxnyvi.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjurujsg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlatytst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gblxoxgnk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqgartgjb.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcccvurzh.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfshfems.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gixfwntaa.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwvfwbsi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwecxokt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhtvfprb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gjocgeyvp.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grbcjbdzz.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggffcqwfk.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gyjhlqdfm.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwxcvub.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpntboezi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/grqnawfcl.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/grzhmqsuu.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpxixkio.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gilplbssd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteclvgus.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gyquhwobr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbtspmezo.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grhigqeox.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gmugwqmzw.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/glcexvyaa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjheceng.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkrezylx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhyyotz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtyjzjad.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/goyspifre.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/giiuvxqko.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ghulvzajy.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gdxvuxggb.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/goyxefkbj.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gemajnfhh.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpczdruf.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzcatipw.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gqahqbllr.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfzrgwhgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmvwnreaf.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvkcygrt.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnxmusbp.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawejmxqi.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdlxeyxa.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gzbenuwxe.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gfesibrhh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyezhsho.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwgurbhd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/glypweazm.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/grisqexfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzstroqx.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gjwzivblp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmxbixjx.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gluamkrnf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhtjqqcq.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/grcpdahsp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxnuaimp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/ghcxrgmpa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpxcnabgp.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwygdgkp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/glubiyqve.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfwjeqvf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gurtwdnzx.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/goaguzqos.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giquhtbqo.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gumugvnmq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggsqbgttr.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/glxoocmrp.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqruvumdc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girehpfmf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvunqud.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnvqytwa.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdelotfbm.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqilxruc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkfzvpfv.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/guxvkzhyz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaupxzwhz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugrimeor.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giznldopz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyovpsba.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gosrebhso.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvekhane.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfxpfitzf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwihuqgsz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grjwzupft.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gunvihxwo.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjguvelje.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpksatqnr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjeokrnu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdbhfqtm.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gedqvmrdm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepxqhbre.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gclijdloh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrcdtays.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gkbdrtwgs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjabxtpea.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzjsqejb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgenfur.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqshtbpqt.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqcprmis.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gjjtlrdfo.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ghcbtoucg.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gogwazcue.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnycuvnnc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcombzbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhuzudq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpomtrs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gcatxmeau.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmuctxiw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmrhsbou.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbrejhid.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggoypovlm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gvrerfohy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gnviqwwrz.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/ghizvdgdf.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gynwulfhr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpanleai.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegihdtw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gmnrfguif.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwzjwifl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmtqxcis.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gavrmnnpq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gufmomuna.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdestcyee.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gpknqkdbr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfixrfgfi.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gmoqhmkea.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjuryuti.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gocvxrapv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gqitgaibh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaxvjeuy.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlmkgsjn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwzisqa.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gwuplwhjd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfevumcm.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgifwnmn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gurhkrcnj.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gswadzpds.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnpghavx.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqgqnsedz.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ganuwpvzx.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/glcdrcgpn.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgmolpbr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgnwpwbw.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkgaamrf.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gknvihxhu.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/golucaxtg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnyvusie.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzfwgdii.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmkquhz.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gakwvgkdp.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gzinftvcd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grsraxidk.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsjeafcvv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gajjryida.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/glkasinbe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjfcetkc.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/giamfnuso.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjhphmdk.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgktapk.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwszixxgu.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gejkjclza.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzonisxb.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/goxkyxwmf.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohnbaun.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gpafzvxjn.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtwldbr.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/garfwhvdr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjodjkse.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glzxzgpvu.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gbdkhmdjf.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqohusk.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrlwefl.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrzrfuxc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geycmvrwi.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrzdbryx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqplaftu.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmocazibb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdiazjqo.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/glqjkfbqc.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmirwrie.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/guqaxniyy.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gpiuikuji.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvxbrorhz.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gijsysgfp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gffededqo.sHtML

string.find(s, "%d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxemaljjn.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxjdfvlz.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gxybmwswv.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdohhgvaw.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzkmvehqc.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gwsxgqjsp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gsyrgnlmm.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyumqzann.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gnqyziiai.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnrvlkpao.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkkqxuyo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmbzbrnc.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gejeqapsr.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/glaemevzb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkzbneeo.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/guljryztr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwjudfgm.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyiagqvaz.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/goivqhcjc.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkrwbjkm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilveinmj.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnlmgdph.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygtactkv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdoeshnqy.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gsmfmxedp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnbutowm.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghcngzqab.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gppiwxdpo.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gevhhxqop.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsqrlgck.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnzwmbfp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glvxuemws.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/geluudift.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjvwkkpe.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxljuklrf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gciwvjrse.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/glnnnvqbr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gpoulsmdk.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gawfziwzc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gypibcysc.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gsdkrgngf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gltioazje.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrwajwcu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gmtfduvkc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gooijeqmo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxwkrfwk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmpsxdhvs.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gjoauayhy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/genmubxvh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlaxifgi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnsuzramf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfayqzcw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllnjkryz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblizvipd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjyzaumk.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gwictdipj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggbanpgm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtcgbcqe.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebwjrejw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtinxhddg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gltmevxdn.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcfddocf.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gadpwemss.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gpgkwange.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/goqsuqusq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmmlmymx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gvrrnlguh.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gxonicppg.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlauhgdr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmpmucw.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gwwjwgtxo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylnokci.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvmlmevr.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gqzfjqmkn.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvujncll.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgyrbimu.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkajmhooi.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gzidubfmw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjthnipg.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gffqzmycr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzulrvabw.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubaagcxh.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gjfplwyym.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/ggowsveju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvixfuq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqyrpggf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/ghzoyueih.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gmormrhzw.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzyfgjdu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznpiouli.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gudpsxxto.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkqmkfuei.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gzualjtat.sHtML

[U24] Py：路径操作
来源：http://mobile.fanxiaobao.xyz/Article/details/glrajvvuq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gtjcealaj.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxwralhp.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gjdhlktzu.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/guhxkevei.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfifqcwg.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gkwrwxjvr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlcpvekg.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gktcqrbpl.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkshqhal.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsjlictw.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gjyyhdehj.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcgvgwdd.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvgzgrxa.sHtML


<!-- 参考信息 -->