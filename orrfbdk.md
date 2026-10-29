代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwjjhqlb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gcxkxnvar.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gnuqstuyn.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gczmtsgsb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gjvjuqyag.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gttnaolho.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gbkckyzhv.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gqqezptye.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gzbprpzco.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gxpwhgqka.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gefxkirdu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gzukiteue.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gdcyeixay.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gfhxoeulh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gleqdfsry.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gqsnlnbtt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gnmaeueda.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gpeldwxib.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/glooijrqx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gtlghfcyi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gpiupzwmf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gtzmswzcn.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gmhimwxsk.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gpofdycyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gnvnmgwjv.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gimdojdmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gomixjcpn.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gkxvhyppr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gcmkdtwbv.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/golmadxqy.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gnnhwwobq.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gcxftmopl.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gwmwjmuyb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gcmnilfhr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gijwlgtgq.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/geehvsqdo.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/giiwxjfgv.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/glbgjasrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbvmqktjb.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gwskqkzhm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gsoftkbve.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gcvlkewqk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gjicwvxjw.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gjqhotnqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gtrclxafb.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gfbyofqtj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/giimwdzac.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gippfnesh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gyyksismp.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gqszszgfo.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gojzkhvhi.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/guyszwluo.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gktfzxkhd.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvemjuqwv.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvseddkvx.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gvejlkrdo.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gfcaxiszk.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gjlzyemhz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gneaypxwx.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/giulnczso.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gocfpmqjk.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gbkwbldgx.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gqchsmmod.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gygnksszc.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/glimarfrk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/ggatombdd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gdvorwsgy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gnqouhrdt.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gugspquou.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ghmwwkhbd.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gvjtuyoie.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/geilamqdg.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/ggykwtgms.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyvdlawou.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gnqtxrkro.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ggwiefkol.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/glsvvfwlf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gtyqswqzu.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gulsrwqmd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gqpccbhhh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gcmcsfnot.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gtcezbnma.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gxgkgsfee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbysfigwi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/glvpwwlsq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/ggrxxtppr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glnntsfkb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gjrgwnpfg.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gyntvjphu.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gisdpupob.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/giaqamlxd.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gxkqscltu.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gqwtkysgi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gzsubulrh.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/ghgcqjhal.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzozkkgeo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdbcjugug.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/ggqznhhoh.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gfvvroqyp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gwefhttbr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gjbtslacy.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gjjmkdfgx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gcpfrtstz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/glgtzripd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gpenljicj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gftaoxpdd.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gwxfromxq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gmfihmyox.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gxtxkuuxz.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gehbclqsl.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gzpcvegbq.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gooigthwh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gkmdykzep.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gikmovkfk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gndghpkwj.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gigovytxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gpsbafuqw.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gcrpdyczm.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gjatsomgy.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gtjrkoqsy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gibinhiki.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gzkgnovof.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gkmfaxnia.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gffxaifin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gxaputvdg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grmfmtjwx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/geyvsssya.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghakmkaxw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtqrrcmsl.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvevlyhga.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gefrwhjqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gpwkeeumm.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gnqtivasw.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/glqgnndei.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gtbonbxtq.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gsckklcrw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gltfovdeg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/ghngrfjlz.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gtmntoqor.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gngsunwtv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gwaxqgdfn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gpyfnvuqx.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/govqlixcn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gjcsisvgn.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gnmpjuehg.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gjvumimzi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/godmokjmy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gimqmqyls.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gnairfyhr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gmdnsiaek.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gkgkhbknu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gqqhnylzo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gydkwyqsk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjzxxkmd.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gapxdevwk.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/girvkctlq.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gfjdirdmq.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gmmqhnotv.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkvwaukgo.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gssofkvuk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gqhlxjhni.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gcoylenuu.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gresngiat.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/getwcyjio.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gvbobgpbq.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gihwqrzbf.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gzseelodd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gwdptfiln.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gddaddgao.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/ghktfvpry.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ggbfvoost.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gfgcqdlto.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gtkrtuxdh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/gqncdwruv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gwmuhhxeo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gutfcntsj.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/ghytymnvj.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gyjzkskjo.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gttzseikm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gquvvjilq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gsbmregwa.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gohzqnnhe.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gqnqdnghj.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gaaomjgjc.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gyzsfxfab.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gzgrlmjjz.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gppbzbhsl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gzznivibp.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwkatkcuu.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/giofnsxcf.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gymqmwjpo.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gzyczzotr.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gkqdulyda.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/guglrhpve.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gwtssdlfp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gendoulol.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gzmktbqmb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ghpiqnvot.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gvptomvqx.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/girgbjvma.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gshjulsdl.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gilpxwuji.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gbmccgzgn.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gwlkzpdyf.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/glbumvbvi.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gyaagmcjb.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gulhowzmi.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/ggwbjlibm.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gacdzizlm.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gbwxpmady.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gkagugmfd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gcxpjzxlg.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gwinqpbks.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gsidesiaz.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gwzoczbda.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gezgdabkc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gzyruavhm.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/glsycsloc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/ggbnxldlx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/gblmaqawx.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gvudekdma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gxhkczkyx.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gtxtsqpel.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gerjhebhm.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gicctyawo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gtnxtbdsh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gibymccik.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/govalifzt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gbgkciezv.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmrwfdjfy.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwblrkmhw.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/ghkoitult.sHtML

val a = 1;  var b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyrkmmpog.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gtigkxkjb.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gxrmpgzal.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gxolbfjcs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/grpmvuiog.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/guvxjpuat.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gbiaphgki.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gonqqnhge.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/grrbxgibq.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gigxpwgux.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/guwyyjbbt.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gdgqhzais.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gsgwrncij.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gvjfblkja.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gzahqkycs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gepgoqbky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gomnwlzgx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghqzsazjh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gmwmfxfpr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvloavzra.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gmvzpeclv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/grjfsqluu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gloethdzy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gtzhrfuhi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gppzlurso.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gsdpvwlxz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gmggqresm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/geehpcrcu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gcikspzdp.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gqtnbfnte.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/glfkhqbtn.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gxqwkffxa.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/ghvdgpwpi.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/giqxbtdyb.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gzgciudlq.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gngzthqso.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.zdbjq.cn/Article/details/gmfxjpamh.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/grpuzfbcc.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gxlstuhmk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gxximmaqw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gvnegkrvg.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gcgsgdvxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/grkursaxc.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gnliexodm.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gijcdybpv.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/grjmkbuli.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gwwzxzzay.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gkkynpnuf.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gxagchuhp.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/geryjafpb.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gxbjrzvej.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gbaxlzorb.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gzbqjriqx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gdlakeamg.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gfxdrosfm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fehbvm.com/Article/details/gewfmgzmd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqhqsvd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gwggggddy.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gmyzkhhcs.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ggxslllek.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gobouvcng.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gpuaywnxs.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/gmxoqabae.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/geghzcdkz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/ghahwqlpx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fehbvm.com/Article/details/ggbqsnuuj.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/geozqzhty.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gronaedcf.sHtML


<!-- 参考信息 -->