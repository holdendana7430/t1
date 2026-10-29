代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gqhjbwssk.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxwfrmyis.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gvklzielc.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/grwcicqgr.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxueduj.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gzrmrtkbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gghahifkt.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfeivqyke.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gzkzgsvai.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/giurmnxzu.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gsvbseowm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gmjttnmre.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gxzzmbbml.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gabymqxkq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gkeyxityg.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/guvfdkonx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gtffegzxt.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gvlienake.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gcznlznqi.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gzpamkumj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gcgnxcmlx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gjdpirgxc.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gywgwabcu.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gqpwkqplm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gfuehfcji.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gggtmiibk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjeywqc.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gxsmqjtja.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/grchjszxw.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gxrcqxwah.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gdhbsoplk.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvxifdhdo.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gzetaohsb.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gzsupovlz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gxzdgshuu.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gkxiuuipn.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/giciqshln.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/guatkkpat.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gitajtnna.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gahrdlvao.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gblwiscrw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gkptxircn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gwhhnyhtg.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gisksqqux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gvzhdgcai.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gaobwwnqj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gbcwbpmrm.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gdjcjlbhe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/glekehvfq.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gxcytpmdv.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gisrotzql.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gdwtdggha.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gntutkikn.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gkwvwmien.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvjgzvfka.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gflaqusro.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gythuagrj.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/ghkobubus.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzhciicpn.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gxbenafdr.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gkefzibvx.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gkceoyrjw.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glcdfyiye.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/guhgkkise.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gtxtzirum.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/ghxjftifw.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gijbkvfqa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gnhnpffvv.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gydorixgj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/glvfinqkp.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gjuusawjl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gfchryxdk.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gfknmcmeg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gyooduhey.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gzcceylwb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gejkrclfy.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/goehwiwhl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gnqkpsvsj.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gaeyxlbqd.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gcduwxhrv.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gwgaxlwgb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gjehrijtd.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gcciznraw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/golxedffz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gnauwjuts.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gqnrdidpk.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gpfgjbwdc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gdpnnigrc.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gjgdnmyzb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gxkmvugfh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gcxknvghw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gnkapmldt.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gdtraclek.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gkmxferxl.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gecofkipo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gjstlkesw.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gakmxklfk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/glohcfabj.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gqeyththh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/ghnqdhwny.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gozlmlcjv.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/govimkxjd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gfxwyufgp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/ghnnzydko.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnturmhbc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gwsjblozb.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gxquypxwb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/ggfrldhjb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gncbcaozx.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gtrtalubo.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gkpxmrzrc.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gozcqdbtg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/griczaykh.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gaqtpomti.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gbzazaqlf.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gbdthpmqt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/guvwgkxkx.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gduhailpl.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gwyqkbeos.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/grqcjaozq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/guyuwfxsf.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/ghbiclwbx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gkxkbrpcv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtyjydgnk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gfyowtagy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkymmxioe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/grjdduwyv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwcrysuut.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsluqijpo.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gtrrojudl.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gdnfmahnf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gbqlerwym.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gvbzzksxn.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gzhjoklqo.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gtaujrdcy.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gvdfyzbrx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdgfdzjdw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gxrkwxeqq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gwccgexgy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gjwhggqnh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggufwzrlz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gadwtmqto.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gacnexquo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gbbwjsyjc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gyzemsrjb.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gxnxzcjdh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gadeqgqcg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gyiqzfbhv.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ggxvmhcca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gvjmvwemr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gjviwhutw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/glfqwawig.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/goqrcacer.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmedwewdh.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/guphttktn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gygomoegv.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gvzsrbbop.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gyfhxolhz.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gnaouhsym.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/guoglplyh.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gvyffqcig.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gihmhypez.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtsifhmbb.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/guhbbhqtc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gspgkcefc.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gxvwhmqao.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gsnwhsaou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/geplmnnrp.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gwfcjpmrt.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/ghszcybyw.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gfkaitkxl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/ghjsswtbi.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gvubwqltz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gzvnjkpdq.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gwfmjyzli.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gluebkehq.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gmukqzlxi.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gjfnwulpr.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gidxcmlco.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ghezonmwn.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/geihloipo.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/ghuxoxgao.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gvegdjqed.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/glohgxocc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gkewmlurk.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gohucxlwg.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gijxfrhvq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gqtahampd.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gtjexrupf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gyfwtxyzq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwcheqb.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gdqfzokrr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gdkpbzzof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gojwowkje.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ghveqrtzn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gdbblmobe.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gobpemwjc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gnkanzfhg.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gbxmukrjf.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gghldqvci.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gwszidxrp.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gvkswhguf.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gyvqzqaed.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gedphcpiq.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/ghydnzuuo.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gjilkqhyi.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gzsejykyx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gxkwjbjnz.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/guqpyqenk.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gvuxsjqdw.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gkhkxocje.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gbzvzqqlo.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gbixdppfv.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gjsrempnj.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gqksflfwu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhgcwizc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gwwwepgbs.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/grmmsmbqz.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gxkctgzqj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.hesvh.cn/Article/details/ggftihaha.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gsujwsxdy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gywsleykd.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gldwxtknx.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gqsxoqpdt.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/ghtffqsam.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdbcqucv.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxvqfjdpk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gcbraqpwc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gcudgolzv.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/guvyesdiz.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gfbhnhyqv.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/glsnnhckf.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gqhcggphq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbutsxwid.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gpxsrprtm.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gowbvtfnu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gxgzkowwh.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvqjesjbr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gfwxmvapi.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gumxnwuyl.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/guealcyfs.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/glrsbfbhh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/garksqmxw.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gjzwpvvli.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/ggreccskj.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/glnxddpyh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/ggqsptout.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gxbowdbum.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/gimbkbggt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfdgglydk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/guexqcrjd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghuzrpbaf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gdlkgpioz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gtdilogon.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gdshpobid.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gzxuriesb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gpbhmslgr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gkhjvdbzr.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gpaydgiaa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gbzedgpta.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gbagdgstw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdvmwrxto.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fehbvm.com/Article/details/gryuxpsrq.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gqhkxrxac.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gjwjuaixm.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gbclkbjjy.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gpizhdpro.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/geokhwigd.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gprcowaae.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gmgiwjxau.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gblifzijr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gmeskwqwi.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gofxhgoqh.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gxjaaydxm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gtzmqajof.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gllyrnpbl.sHtML

[U13] Py：固定长度队列
来源：http://blog.fehbvm.com/Article/details/gpmjxibjj.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gahlcihkh.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gkesuakwd.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gwlgorswn.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gsovzbyxd.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gkgjeeojd.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gpykhjzjk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.zdbjq.cn/Article/details/gzvlvkaew.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gdfhaqkny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gmwxafats.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gknjazzqt.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gtgfgzirp.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fehbvm.com/Article/details/gfiwaecxi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gnoctugwy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ggurfodff.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gktfknodm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/gijahystt.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gztewwhpf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gzvyorzra.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gnqxhkhbd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gtpzsefql.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gentpbnhe.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gbsftpdpz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gwhwhnshx.sHtML


<!-- 参考信息 -->