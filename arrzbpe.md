代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gxqyazpvu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/grioqeaqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gvmdlbums.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gcvyplifr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gaxqlsnzg.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/glwvxmhta.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gexdzemjw.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gpzqnzrbe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gtmnihugo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gogivomlv.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gnlbdlpjh.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gaerjfihb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gvuaftvfz.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gbgavfhdv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/grwxlahnb.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gobsslnno.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gdzbwbpyc.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/ghdmsqpxd.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gkoliszkl.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/guyxorgdf.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gstvjjhzg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gsyshdbli.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gvcdvidvw.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gqdaxjvay.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gmewhppwh.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdtjqnptm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gseaeokzw.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gldxbabbf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gojhjopha.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gpmdumqqz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/giuiuyfik.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gxdefefjk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/granzphbq.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gmbgzssfl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gwqfcjwiu.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/glcyjeuyk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gqybozqoo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gsdeczfnu.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gooprkwsb.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/grommwbnz.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gzlwukepn.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/geqvudcss.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxzxaihqm.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gyicwpyyf.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/goastodef.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/ghesdcssw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gjavkoaon.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gjhoruouo.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gznmwqnal.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gjvgljlsc.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gptdlalar.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvnnpgalg.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/grhwttdye.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gybmcmmtv.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gmhlmxkjx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gfxcusxuv.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/goxzgzkha.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gnujnggzm.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gznnpehef.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.hesvh.cn/Article/details/gyztnslpr.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gklrcpslh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghutgaspf.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gfcpzjopa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gfjzknoez.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gonhjiylf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gqumbxvhb.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gehiqgehr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gvkcooagw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gxbtrggqs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gdufxrseq.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gqbnbtbev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyxkztuje.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gwzuqgcjh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gtcnhuhhf.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gaxpzlacf.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gwjfnlbit.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gfydkaevh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gargryaky.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gpsmrvjqr.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gonngsyro.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gecmdualp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/geelsdszq.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ggntzcufr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/goekdtgvv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/giiwojymz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gwzptyayg.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gclhdwsdy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gqlwrzpsg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gvrblpvva.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gzdeqsort.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gljsxavcr.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/ggarjtura.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gghwekkjd.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gexbitlbg.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gaejifawb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/ggffhtyab.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gypvyjode.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/garaswisv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gehwpffin.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/gmnzoxfmk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gtixsfutr.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gcbrzcswx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gomvqjvar.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gnqrjzdks.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gjfmykxkf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gtolrxrdv.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzblzidld.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gwhbplozf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gtauawiby.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gfefatqls.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gqyizlfzy.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gygrfrrre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gbbekwisi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmyftixdc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/ggkgxdvbg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gapqszdwl.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqmqgwjrn.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvrpvudvk.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gxvomcseb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gviuxlbxn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gcpdvpmcs.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gmoftnece.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/ggyaappyy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gsbfcspqj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gbqyiljwa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gxcmaxmac.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpkdobpgi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsqmmvdiu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpurbvfww.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gpyyyawza.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gxwhufagd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gchafejrj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gowmemnib.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gwzcrgstv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/godapwrxd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gqnqdedpg.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/ggykkuxzv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/ggcwfcmqh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gydtdkiiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gajcdhndr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gqmxrdcht.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ghwxjqipd.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gvzobnlzp.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gjvqlemaf.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gxifhlovk.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gkepehkib.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gtcsrjibg.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gqqoymnub.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gpfqlmlwd.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gosiqoaxv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gqscqujbe.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gvtdsvczk.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gnapfxaje.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ghkhzuusi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gdetdmzkf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gjmdolzuf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbbeefcft.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gdobgdokh.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gszkwxkzz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gjkmzqcga.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdkvkbrcx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ggadvwefz.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gpfsibrsx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/glqczlbkr.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gcmjbvkwy.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gpaqhtkip.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gfakiocoq.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gdmuugscs.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gxhahvfix.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/glgvbfzoi.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gaowlsuxq.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gqevtahbd.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gmpzvwzux.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/grhqerrdb.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gokhapbjj.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gnqgmgllk.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpcgyvqps.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gslvqjany.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gyvfcyfpp.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gieduyibo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gqmwxfwgo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gjikiihzx.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gxmpkczox.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gzqneodqr.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gwsypwvbj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/ganfkkfxv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnhzoxflk.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gxbvbusce.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/glwejrflc.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gcsnbfcth.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/ggklngbhy.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gahqvjhto.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gxoaggykd.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gbmzssdpm.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/grghuahph.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gusahawjf.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxuulbtjb.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gkixvcobo.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gyqbirwio.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gxoocyvby.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gpixythvt.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gldqrhjzm.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gefsdehcm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gjzkxmbhk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/grxwgdqbs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/ganieveni.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/guuxpency.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/grrjewdci.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/govauospr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gcvlwmiew.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gpvljzivm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/ghyhwknrg.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gexcqurxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grarsojhb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/genqqzdby.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gxucalmpv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gscxwxbco.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gkrqxychd.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmdpuizyg.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/gjaeivkeu.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gejgfjnej.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gcpktxfsg.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gxwlklndk.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/ggyofzlin.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gprdjyvki.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gmrbxdonv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gmbukmmjd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gkyxjdrli.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gbdndyqsw.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gurhhjdhx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gcrpoirwh.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gtphootqr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gugxgerqp.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gyxqmhafj.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/geovzetfq.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gdhteqvjy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fehbvm.com/Article/details/geqnwohlx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gflwbkqmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gubmnppgl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpvmikoon.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gfbrpyyov.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gndlnbxlk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gpmirppws.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gnwbypequ.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/gxmhuklgf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gubkhruji.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gouiqrvfs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gdbipxnhy.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gkqzqdnea.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gxhuejgnq.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gdoairlej.sHtML

{**a, **b}
来源：http://baike.zdbjq.cn/Article/details/gaojcyttl.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gjrsmgahb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gcsxlcqnh.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/ghompgjds.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/glxilvujq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/giwidizxr.sHtML

max(d, key=d.get)
来源：http://mobile.zdbjq.cn/Article/details/gntdkubzv.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gbwsklede.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/ghzypwkzl.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gurhjchsm.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gcbobgwlv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/ghskfdhyg.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gnoxdaxqz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/gtsyjsapk.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqpyuar.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gerehqtsy.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmklhjyw.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gvijwpvel.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gauvuglwo.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gxxbfcuty.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/grvukbwwa.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gxoyhuioz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/gqdhfrcvj.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gosajqgfv.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gszzxizoc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gssxdjqoa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/ghtmnrulk.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gckobrkvq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gihzgyhyi.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.hesvh.cn/Article/details/ggxnllbwv.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gwgbaachk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/ghlaeutvd.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gvsxziuke.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gbntorotp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/guwxdcwqk.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gpuocxvmu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gcuqmytar.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gagxgydam.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/gkwdpktve.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gcretfvzo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gkhcfrlge.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gddjwcvqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gfjjadumi.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gxustbgzk.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gywgalxjz.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gyodcwrcw.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gikyufdaz.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gzxnwgvmz.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gtrtklhca.sHtML


<!-- 参考信息 -->