代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/goanopbyc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbviczs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/ghrmheaxx.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdejpmbvc.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gsmbypkgv.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfwzzdj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdqvskeo.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/geajjuxtb.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutforkwf.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gquwfphng.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/guuewqbki.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/guctcakyx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/goyixulfj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gybbyzgtu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvihvrmq.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gyukefsvz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcvlldwc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlfrhgsv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/grslnrcyr.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjvgydcyo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefbfirxq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ggqknfhpz.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/glzvsfuzb.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbismrykg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ggfdnrioo.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdhfnlly.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gueyjvzkc.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiojnpwk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gltiodcjv.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/geovlfqzw.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllkvjuq.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/glorrrszh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwegmwxg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grzxftwgq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucxumawp.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfarbdyzh.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gxtjpkchf.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/giktdmjrh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxttjjkk.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxjmqvme.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gotdxlihf.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvewhhigm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/goiestttl.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gfiouzdnj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzvryrbz.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaisvbji.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/grazxwctu.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gpbmenpof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoplsenk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigjdoxg.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpismpkq.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/glaluxdvm.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gywrdqret.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gajhhgkag.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gcznawanl.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrmzvuwv.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwktjzni.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsoqlwy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgdarnkm.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsplzlcz.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grforhrog.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqtjbpd.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gchtzggff.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqnblvcj.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmvcrjpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaaxjlpu.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gejmswhaf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyccwrdl.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxqcfei.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdkrfuwf.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gaiazrppq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glbglbisp.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gupqkxonc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gmxzpppvd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmqtgdrj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gpfubbaxr.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwwdebc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxfwbmjjk.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjqtontr.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gguydttux.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gdiupdrgb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/giwassjkk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzuwrzwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gczadgjjp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcuxjfbt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfpbchga.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvxiamilh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/giknvwusb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gsjzyrsvz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtbfyihx.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/geqzzcmnj.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtacdpuyd.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/getquylrm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzqlwlu.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfrbhgk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gocckgvxo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gaplmvrek.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtvgpxwxn.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxjdldbu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gurvfcgqd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjfrpbuaz.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gldhkzeeq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghojteeyk.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhbeebt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gqhgcbgaq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxocyqbog.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/guqlbwxom.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/guawkwtna.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnikgdzr.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutohugbb.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gtemsuola.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgayypu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzcaaisu.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gvlkgykcm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gmnmqhlyr.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gvpdeviou.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grybmijby.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhraifge.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznikucyv.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsvtyzlk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmatuwhop.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwlbvfoi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtopjls.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaobfmqkm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuwyzkwg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqutguess.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gnqofcmbc.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkedcayro.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqwnmryvi.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsjsokjr.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvqrvtrq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gclzirkvg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gnekfzfao.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmamvsnji.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gjffttzli.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotimpdh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoalnbdq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxzsavoi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gmwzgqytm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gqylufngq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gigvxdicg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkutkwgc.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gbryydnod.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gjsgjkkze.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqvctsen.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiluikuu.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gdjphgnxs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gemqxfxqu.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gwkdcfpsv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtortngkx.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmsoftlb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkbumudz.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gauhquefh.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzrgxmycp.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtxjhbcp.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gsthtbdwe.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjgrnvlx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/giqgoocis.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghputegen.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqxgwfxo.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbzsouftw.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjdlhhnk.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggbvbctkc.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gaxulairg.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gxmvvhzgb.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/grktcedck.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/glvnelbou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfckallbd.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glauaistb.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxuwsjft.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/glxklhoxu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadsntmft.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjhyavi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqxjvbzl.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gzlisrkig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gyvfkrvgr.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoklkwxa.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrxpzfw.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gctmuvjpy.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gtyljtmjx.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyvsiklv.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gugnfwdvk.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gkgdkojul.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gveqjjqus.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gtjraohvg.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggimwwdhc.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gctaulttb.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpiwfkpr.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/grhftabrs.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gattxdfqy.sHtML

[T32] Lua：局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghsneovkg.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrsidavu.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gpajwhxit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaudndbs.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gcssrpgcv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvznjoij.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfdozopu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyebbjxy.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwnmtkutk.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggndpjger.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrdildfz.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gpowqeznm.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/ghktvmojx.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhwhbpkv.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/genphpjeh.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gohxmvmlt.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/ggldpqewh.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gllcimycu.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grkljzoax.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gucgnkxgf.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gkmwmmszm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmbdnzwq.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdshmwu.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsmazekh.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbezfrmo.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoocovqy.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgolocpz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspmbfmtv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjwoghyu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gebqxubxu.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gdaudbazy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrefwgjm.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcvsxaykj.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppnodkli.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsykluuqs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gblkrcrpq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gssicasms.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/glczuhwuc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtnlmfzcg.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjsqcddet.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gckvmrcwj.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiroqekk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaagtxjd.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gcevanwor.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnjzpkth.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gdatvncld.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvfamtnz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbxsowgu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfajylfx.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gqierdess.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsrebcwri.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaqbvpot.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxdaxca.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvnrfgkn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzqmxyrx.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggllggtwz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxsolwu.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhzczkc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gzokqdwyh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/giyjjksbn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gztgbkcop.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzrbrmbn.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtlouhig.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/grknvxqxl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrcdawpd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gilvbuzyi.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/grvvbmnyv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztcbqfyg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvubzzdr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/grauvxsdt.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukixdqex.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gclhomveq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbwznwpj.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gsufzcjtp.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gjzmtjurx.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdengdwus.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gtynriksn.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/givkitcyx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajqncwyd.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrxbxpmb.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkwdzhef.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gwxwldiod.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkphafyde.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gubfworct.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gaclckdla.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykgvmgf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwzzqwxt.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsqrrnxt.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqscaqfn.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaeyuvov.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/ginbsqixe.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gfgqjwahe.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gorbunfzd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gkqrjrgaz.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvoiqhyj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlrqaxlr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrlduwyx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gvylutlji.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvkrjmw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/geopixffe.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gpugbqdvi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqsngfcs.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/grxmskzgp.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/ggpoubasi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxtrohsm.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmekektxn.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgwzrqjn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifrvarra.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/grfaqnuyj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepqggref.sHtML


<!-- 参考信息 -->