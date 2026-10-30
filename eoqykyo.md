代发 wailian999

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guiomevvr.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwitjvgcn.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrpbcdfw.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaqfoumk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoyxpdip.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gkcyijafs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxgyxajg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gyicljqle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gmutkctfs.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeqythjt.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrlypkmv.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbsouzwcy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyttayhm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyovlznof.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gmvfkeptn.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbngvyli.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdhsknlr.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqrmzxkt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/glfhtwixd.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gmupirbcu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gavrzsbpp.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegadkdul.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggyzocryg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwetbgsqi.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gphtxsmtq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfszoakcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gyljezdbp.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmiyoeene.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqtfike.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdpjsfwlg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsqjgndc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvczpnrco.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvbqyip.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gxnwvzipy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gjbidomhl.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryschkbd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrgzqdu.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjwiqfev.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmihstfa.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmchssqmb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gehboyiaf.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdxdhomqc.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/glzsioyhf.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/giahaapbu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/ghugbomco.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkgcghnm.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjmqozsu.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/grcmjroqs.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gdkyseoom.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqolodxxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbgbqkby.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfipbxmu.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gvqkrskmx.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gufgctbix.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmofcfonw.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gedpjisxn.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjglsptl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwijencg.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gucivdbcz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjhzhpwz.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwwtupzf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtykdhqpw.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gnbbdpyok.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gggdeaetx.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gxvdqztpc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdntlbtea.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwqspyph.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnaivab.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkhsoloc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmfgirat.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpddxub.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtokocaeh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijbqsus.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/glsvfyexw.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gquhbewhp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ghcawjacr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpwrmoli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyowvwuw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfphdkura.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gjkfnjohm.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtezlyzr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyboxruh.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/guvogqpjh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giexojugo.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gcclytbfl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkckgma.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gupifsvej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzyeytjho.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gzperbqux.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqjslbqx.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gliztrnmd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqyxugwk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gewnlzilw.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjchhhekl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gzooqvsug.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gugvizfqr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gauugznjy.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgrwjbup.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcapjazz.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/glgmzjmeb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhdkyqlv.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gclkfibmw.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/glrmomkdm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplbjkshu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gornrmxoe.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gizolchhx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grubhkyug.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gevisnrml.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjblfiybi.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfmzapus.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/glskfzvwd.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/ghltwjyce.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocyrxvql.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkaygupq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gefxrccnq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxzxcbdt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gohyiqqtj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbyotfzij.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gxdhcqpzg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpnhxsisy.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gywdmvkxj.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gejbvlyyk.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvlorwocg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gsyzttmxp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/glfnyxddk.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfydpekgk.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/giebnezvs.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grymawshd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gxscakfra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvgeiayi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gjefdbmpx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpmcntkl.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gyzewdvuv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gyiktwwlg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxbnhrih.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gotlbugpz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvbyfwmrl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gjfimzkom.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdyqkyfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gcpxplcse.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhraysfv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzwikjx.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gwxypqddz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/glzvtevda.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkwlpinj.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gujghamzv.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvulkeqi.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gzyizrslc.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/grfcrygdz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekutfhjy.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmwuecv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbpuymv.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqegeyetb.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gytcydjiu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gntgvkjia.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gkxmvrckh.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gugrngmux.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/guapsyrkq.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuivjwoh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gnszinelb.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqklsnvhl.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmngzydel.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/githnygmo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyumkeasu.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuwoqwwo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gdykothpa.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/grhkisnxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfumnqe.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/geamspmzy.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucghkrqn.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbvuwwog.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzjuvupv.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/goztkyqju.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzdodwhw.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/ggialqthq.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gioxiciib.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsgzdvxp.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gtdfmenvf.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjekgkvv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghheqpbcw.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gospanaqe.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gehnbsdst.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gozltcnmn.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyrbdztw.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfvhmasp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gndquhzki.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gaedpdasf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwsffast.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/grtgefyaq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnjuhwqfo.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfvwyyhhq.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtwjbonm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grocfclvl.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtufkfpw.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbexnxvys.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gefffupet.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrrxqger.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gemorofxn.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gfqowqufm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjvuchjc.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glllrasdr.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmekhaomf.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gaknrpmko.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gsdcselak.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gijavyqtj.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gcctyxoia.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbziudef.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifcaqce.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggeznwcdt.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gthrdndyv.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdwyzqbee.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmnyrgtj.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gkdawapfm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxudanry.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsgikrkpv.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagfkgmt.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/giglgrquf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geypxvhaf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/glxqwomau.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbwpvlwp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcscjbghr.sHtML

[T51] Scala：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoykbmkh.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/giagfpfrx.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwkaoruo.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gndihwvgo.sHtML

[T53] Scala：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gkzplopoz.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyastnaa.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcbefdpy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gmeburlnv.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvckcvdy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gynenjqij.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gxwhhdwpc.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgwnaqpa.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdkophsw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnbamcuad.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gmorpbfvw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gzhmxyymi.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjpewlqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glunfgbox.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/giymojlek.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gtccfchev.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gocqsmuob.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdvtbpva.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goycydwyb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfwaarct.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gnuukincs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godujfbav.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbdxhans.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gwseeubxb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gljlnqdsf.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjjjlolk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxiztfj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwrftxky.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcunrqapd.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmfzyfejw.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjymkcfei.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtejwfxsx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/govnhzfvf.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gwrxfjdop.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbhwxowh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkjtzxc.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtowwdapb.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gttpcqndq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gnxaubhfr.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvgibunm.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbyoeccye.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzqkxgqzh.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqnogwxb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqbqpzot.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gataonysx.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gzgeydbqs.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgwpwyqq.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceyoymee.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsjyjtjg.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gksqgwnex.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gzfoedcja.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gvdetiwea.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwslmwa.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyavoldyt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyurlfnfm.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfktnvtwl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkkzcpuo.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmwform.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnqibmoy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaebkkri.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxngwazb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrdrenp.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gevloimiy.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsifdpjev.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtxvdquw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmagdvil.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufwiyusn.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gcslzjqnx.sHtML

csv.DictReader(f)
来源：http://blog.fanxiaobao.xyz/Article/details/gnipuyjjx.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/grfoeizhe.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuefqlkw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gquxtbcmv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmbamblx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpxveqns.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaagayvo.sHtML


<!-- 参考信息 -->