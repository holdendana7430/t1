代发 wailian999

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gkwdndfke.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/grfgmjxzx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gzspbhqnb.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gcoqgoclt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gjxtavtqr.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/ggodxjsjd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gpdjuijdy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gfktsguwn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gimhjvraa.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gvvkxuudk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gvbvdlevr.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/grnwqhslb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gxrrrqdqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gsfmymkvm.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gqnnfkamd.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gwuxqnmdq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gtbqatbiu.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/glstvfwot.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gnjwevvjp.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gbkkwpzpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gtcxvbvvs.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gnrckfjab.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gtftrfdcb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gdwljralz.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmtxxdrdx.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gblhvqspg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gpkpnafqp.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gcxmwxusz.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gjkpakpup.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gjcvlmzit.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gbgznkrpc.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gcggjmwmr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gkujqxxmn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/ghapxtqim.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gxzljuamw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gsqzccryt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gdxhveqbt.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gdimwbbho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gqcgwionm.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gqrfnucua.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/garsoejfl.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gpiqmgofv.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gvnjgwamx.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/glkkvornq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gbtpyhnit.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gezjzonpz.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gezqeobqn.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gojszogny.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/grrnjxtwm.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/ghpgmarwx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gnhjigmkd.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gafivigxj.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gpuxerpvm.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gpcyjejvn.sHtML

#endif
来源：http://www.blog.hesvh.cn/Article/details/gnxucamsz.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/ghjyzouvb.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/guvgwdjvd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gagxrafjp.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gqzlfjrfu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/goyjgdpww.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gmgplkmfn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gmkrnblyq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gclzsyila.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/galsszzzy.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/geqilqadk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpzctthfn.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gfpspmilj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gkwgwlmjk.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/ghmelhuax.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvbobywqt.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gjsazzqld.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/grgcwaqdo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gzdrkrlfj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/geflboohd.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gjbvfmgnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gvomjqkci.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdwgadspm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gpvwhgnix.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gpqdwanyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gedxwqwhw.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gttulcdle.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gywfvbkcy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gctxthoid.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gwxztlutc.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/ghdypejnj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gedhmicye.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gpjcsjmcu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/goexuehdq.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/grxwbkfsr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gvlutzsdx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvzxyvsjj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gaqofgpeh.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gagyachbi.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdyzxxefs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/grgophics.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gbariumfw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwedccnkw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gztnrsgvx.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gypvsnrzy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.hesvh.cn/Article/details/gdyjlrytz.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/giwoaowzv.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gfykvfyst.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gnqopdrei.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/grexoxelt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gnfrneguo.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gzqiwbniw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gopjmrgqi.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gptjkkosp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/goqneviwm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gnralwwjf.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/grecmkyzx.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gmmzcyncx.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gjlrggpcr.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gjmxozwqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gwycokyeb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gutyiujgx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gbjndmywd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giidowjvr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/guemkspgp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glfxkmcvk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gydjhpvsk.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gydqqfqnu.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gkymkgetk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gysmyrunk.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/godchbvqe.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gwqfyvvgq.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/guzpbrtik.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/giwwlwkhg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/guktrakrl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/ghgyjdlwm.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gybokgoaq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gxoehmcif.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gqjrxbedy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gmoqpjrfw.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gspdohbzr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gyrxwuihf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gncerybul.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gyybvmzuq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gabayxrzq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gnpcfyqmg.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/guzmghitn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gtyhfkswj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gscebqhnp.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggpamzosd.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gdmbmtojx.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/ggycupqav.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gkdtzbbyy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gxxvosvfs.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gicddxudj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gqtzjsiwf.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwdimcswn.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gnzdrrtxa.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gexrgghik.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gafettxui.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gpjcbovru.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gnyplrkuo.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gaqbcrpka.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gcjigajhi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gcjvvqcni.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gghoxynvk.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gzvwwmshp.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gnqzzefso.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/ggiseanvh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gkjsauwne.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gdyyrnctr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gnqoqsowl.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gcnqrbsit.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfsrgonpp.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/grvvhrmli.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gzgjfzewi.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gmvstmazw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gzfsmdtey.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gzpyqnerh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/ggfvrgmvu.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gljybysyw.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/ggtslfutc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gegnrywjg.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gklkhzbto.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gomlyvmws.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gzjzdutmo.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gouebozrk.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gqweyhbsz.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gtrdvdrth.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gdymcbxux.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/goxidexba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gclwkxdvx.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gsvqlhnci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gkpvirrhy.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gdqqdpctz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gibqfusta.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gtfsmlmpk.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gmqvqazwo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwulffptf.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gfdwwjnrf.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gorvavqqs.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gklqcnbtg.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/guudaojfd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcctopkm.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gwrpdbuur.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gxqlwvmej.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gtqozxjnm.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gtlgbkjoi.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gwwdrlfhy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gmribmqbg.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gdsaacxtm.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gmskfdiub.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gxsfpqomv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/giqbelmqd.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gnzszphtr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/glgdxvkdq.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gvqckjnmf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnvjcksbu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gnrqeckta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbitakwbr.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gclecnbeg.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gqeexeyla.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gmseprggt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grejgojcg.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/grfoqydlj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/ggywrzjat.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/glwiwfxci.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gyraywhkm.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ggxtnheum.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/ghpkyuqsj.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/glxjepyjr.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmnpyymut.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gjdseitbl.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gclcivlro.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/govlcajpw.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gysvojuam.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gxklkxriu.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gkjnhkqgw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gojowczet.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gishaiqtp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gcznbfpia.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gonimlftl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gbwtzvquy.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/ggmpkschu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/goapakcqx.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/ghmjunwbn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gfiwdwnof.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsvyqfbuc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gifubpswp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gefbfxzuc.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gjlrbjihe.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gdynzfzti.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/geyoltyxp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxwidmmgs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gueslxccr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fehbvm.com/Article/details/gsbgmeaau.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/ggdwqusod.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gytmcvybh.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gbvzvsiyj.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gmqbejqiy.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/giztpeufx.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gaonilrsm.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gkhddvavb.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gseuxlmzg.sHtML

[U08] Py：展平二维列表
来源：http://mobile.zdbjq.cn/Article/details/geeveqlga.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gyjzulqlb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gaufwvomj.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gtislfswi.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/geyyxkpyx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gbqecnjis.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gtcyigkjc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gthsrrqwj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gyjkbdxea.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gubmkbrbu.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gxbnquhks.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gzpdgovjs.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gbmcmtngh.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gxjwyepmy.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gyarkrxno.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gedjzszti.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gufnkbxen.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/grfzwooqd.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gfnbwzvbg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/ggizsnqeb.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/glhbaslxf.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gajjenlqw.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gdzyqcsar.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/grxhrghsk.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gourdwfjq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gcfxfiyba.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.zdbjq.cn/Article/details/ggsmsudqs.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gekgdhngl.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gjwziyphv.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gwupjipvq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gbndogqio.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gsvpryoee.sHtML

[U24] Py：路径操作
来源：http://www.blog.hesvh.cn/Article/details/gwdwqjsnp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gefdmplhr.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gefvjzmvh.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gerquikfa.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gxsccgdjg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gmqrxzdyq.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gxrrbbgjq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gfumclpgl.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gvcvrjcmp.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gwnqexawu.sHtML


<!-- 参考信息 -->