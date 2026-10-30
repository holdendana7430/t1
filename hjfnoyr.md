代发 wailian999

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsvtdqsy.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gepbcqhlt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqxppkc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpulurylk.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrzezwmq.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbzolkfse.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gbedtkslc.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjousjicb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gghjtnwya.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gixdxviep.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gkkwollzj.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gloyapgmn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gafsjsbif.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gnradioqq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxwbfqoj.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glilhksga.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczsouynz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjqeacst.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacmtjyrp.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gesxnobhi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbapkdn.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/glixwikak.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmpspjp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gpldrrhaa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlbvvall.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbfqmvbb.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gglhkmhky.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoyxtees.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gugarxkvy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdxedhen.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnokpbmzy.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwukgofav.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuorezaa.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxwluzaw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gtywemxwy.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gemdxwbus.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzevqilzi.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gmxznmzjb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gscgfgssa.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqitbuhp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gatmsqjmp.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkldmctk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqshaelm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrtlvrtu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpbaiuhb.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gcacorlwf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkfqhrnn.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gqhznenst.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuntdxwj.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkcilytb.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfgnysyk.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsogszvla.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gqebzcxwi.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gpgtmnybh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaygcrvs.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ggomduxot.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gindkwlwj.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/garozaiqf.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbiureej.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gptuylbte.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjapbxtoc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlfzlpyw.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwwlvtgk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/geozthmqq.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gdxllfiji.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gairtnoiu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbwtswd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxprjka.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwitctxx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqsspfzjx.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmidsktbf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/grirzedzh.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozzmped.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqxdhuswv.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzpbhgal.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/guanawpbi.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjqklgyf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzycssjn.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gnjtxhynr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gofuynshq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gokxmsojn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gejhewvru.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gsiplxnyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/glouncblm.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuezimvi.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grebhyzmf.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gnulyqmhm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guccnviut.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/golltknso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gutmheyca.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymyvnkqu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtquqinl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gigsmrvry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvqkjswi.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gerbpkbxa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiesspih.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpatjfdd.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsclkyrlj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/glrzztpzt.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/glyrdilkb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpimdajn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyhbsxre.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gviywbzvf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhfdfspe.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdljkbaiv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwdigwit.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdzxsdwp.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gdckwlxve.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gwkatgpjn.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzonytjgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gqrukwapz.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvdzozrq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzorgizm.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtsmrswlk.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gaktsczbj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlgefylw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gghvjmmlc.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gzpcdxiyk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxcmbceb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghohccdaz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/guyfyvbrq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geuzkybzh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdjywvwt.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnlmrslg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpybaedgz.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/giozcvpbb.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtqnlbiqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gudsmmycr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gufusuroq.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghxeolivl.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gkypovrwo.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcdkkgze.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmuygghwm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/goqxayhpk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gexxxvgfs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfunrsbep.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqisturfr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gxozqlcwv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gobmzpwmb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcepsdrn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfytdootx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmbmjxns.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goulrfcwp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gaqdssgtd.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gihjaookr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsidgpaiu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftnoxtrw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgyvvwgv.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gojythjem.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtymygpky.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gojzigokj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhddaqcl.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqttlsou.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gogombldq.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwzlzuems.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grajmwfab.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwkxqiepa.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnbqsesz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnocpkbde.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gopmqxddw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/giyxnzmgp.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmuaiauh.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufsruwwr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxefkvyr.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmmmswep.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/gsrzxipop.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gksqopgsd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdfpziw.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvezycvnz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gptsmenuu.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gfwwerqpi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gqorxulsx.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkudnaue.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmgowiwg.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gjeiynejx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gayycadpr.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gynhotfnj.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflugnwws.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukgjbgha.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjsbdfbv.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gepywzodv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdsnhglo.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpushwtrq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gilyavkqk.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gowlqrirh.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghluvsotu.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfurfip.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkkgehoq.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gkxwvwlhg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgresate.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbufpidj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gctvnavfm.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbfcilww.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gvwlabswq.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvorwubou.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gsdbifgim.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gotgjucyh.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gntwlgeuk.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiajvzku.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvaexhm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjuxitct.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gkwlajcfw.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gepyemjur.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gohaacqvt.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdxooil.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsxqlzxw.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gteiislci.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzhwmrtl.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcxhkthp.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/giusonpfk.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/glxvbybse.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqlwpwve.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhduzkt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyeaoeeeu.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gehwgdtqm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/goxmlrjyi.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfyoftjw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbqgtbkg.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnxemmds.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/guaixyqiv.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwsmhtow.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/girogpqyn.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxivbgeld.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhmmuvok.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhrkdjjl.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glputdwbx.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gccdzbuwi.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqexhcaz.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdagpxtr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbteyws.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhorcleg.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gkgwkbuwi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyymlapzp.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/goymssyci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbosjoshb.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/girpexfhf.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtxlyvrk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvvxnlyw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqckumahk.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtelgody.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhqrohii.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychahfzo.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gepcnxkjh.sHtML

[T60] Scala：折叠
来源：http://www.share.fanxiaobao.xyz/Article/details/gcayhsjpx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gwumykfjo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfnsmkrk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnlltzdl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmzkxzle.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjbbqnxv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkhnhbow.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtzilatl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdncggres.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gsamrwmdv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuxhulem.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gngosztnb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/grjxrlxdx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/grpsjtlix.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnbqcvgm.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/grzuxtmdl.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gylmxzzgy.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsponajv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsshzhmys.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghktuibof.sHtML

[y for x in nested for y in x]
来源：http://3g.fanxiaobao.xyz/Article/details/gxnuvqyge.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gwlxfdicx.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmlewgax.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gpubecvgw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnzqltbu.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gzkkdighk.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexlmsbnu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gcatdutoe.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyunwgph.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwokbryji.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gvxvjbpzl.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzkjyqr.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafcjgkla.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/glrcgpehm.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gydaikgei.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/gqozkwywy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gvqnlfkpn.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxzddqmt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/goadmlbqb.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gzwnmjbkf.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geczvgvzn.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gpyscmgne.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gewmvwijb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gakjsjvgo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaooacgx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyshagti.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gjegcfzeh.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmzpyjli.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkpuqasr.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggxuatbzs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gxtykvtpk.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfwkach.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqnqgxom.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuftrzzb.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfopsgvgd.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/gjzjqpohz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqwtvhbo.sHtML


<!-- 参考信息 -->