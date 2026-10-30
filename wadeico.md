代发 wailian999

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrozlwvp.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gthmhiydz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsikmgse.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gefrsjdks.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ganpnbhuh.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gyckhsvcv.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gacfldtqi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzchhakx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiasikpv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgfcrbva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbudkaewl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshjfwpkr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwwuhiil.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gkrtmtbeh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqmyznjp.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gslnecgqu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvkuvkck.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxmkulm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdovjqve.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/geuzxfrlp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzrdegwu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhgxenli.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucvobog.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gevrtoqsx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasarojpk.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuuubkrs.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzcfjciy.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gwtkmfpbc.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaylxgzj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggvovlcxz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gdjyjsefu.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/garhrjrvo.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdnnhwho.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqomrsvy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gljwypiiv.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gpzcsidlc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcrstohs.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyjmzcoz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmnqyfbg.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxkorimhf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gvdtoxsqs.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gddjzmerr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvikmxwi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/glvsdnrkh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gknllhcrz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/guunevykg.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gsmookmsr.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/geynhjshv.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtdvgoj.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfvgdpp.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzklnourx.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcgkmfcfj.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuscgxbn.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfpovdzm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gabdtgbeb.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrymrfjf.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/giystabth.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlelkvbo.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/guclyawde.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giugdiuex.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggahkngco.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumsuzkm.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhzfaijr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjghcfccz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/ggqkfkzhc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnpnfflv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gdixtjxlm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gunlpfqxh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gpshfnfnv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdecyyucy.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/ggvuawdsz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrtjgvzp.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gqdcandjj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gcuttsgsg.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gisuarcbs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gpigdfyyv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gwzgbakcn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrocamb.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/grejsebxe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzexfkwlo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuwcirhg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gepjwlmpb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnenotnxg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/ghavzxqtf.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gceopovmm.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gouhfgdbg.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcrqjjll.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxmxfvv.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuvdkqmx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/ggpettkwh.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gbftdetmn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqecjxhyg.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gqvpxojwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/grwyvmudh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsacyfnvd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmghlvak.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgmioosp.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gokkqodnt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxxpddok.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gikvfgalp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjsiohkn.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/glffyptpu.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gekadooak.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gvjrbixfb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/guaqjnarw.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gpgcqszml.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gkkvidors.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruhjigct.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkegguvl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtabswwq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gzxpaiubv.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfrhnjpx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpdtvrii.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwmigfkd.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gekyjfaxc.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gkpxeelaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gccwxhsxk.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gktjhahfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvaazftw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkcxzbsx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gmzuupxon.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gialmcvug.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gzhgruoqv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdnakoglm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxydmnvpf.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gjfcrkdne.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxdflzshd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gifbnytaf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gboqxkwlf.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gvxcfbjdz.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gvxbvyekd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcuoxoyt.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gabzmehsq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gomascpnl.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpbxfbrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmfjfvzs.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gywntvbou.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gepedoxgm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/giynucedd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifeisjuq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/geaotruqy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxcotlyow.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golvuyrcc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyncmhed.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/ggbqkatwl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwrqqhv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaicbeoa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzppjnjws.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmfxgcdj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gamgzlcjk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxikebtb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaidormpa.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gssletxpg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gthfdnheb.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grxhaxksf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmbprynwm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsmpxdqhb.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvqqsruo.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gaonmoatb.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhpzptg.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gybxraxxy.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpylpran.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdjppiui.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxadegdwh.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwbjthwco.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmkpglbl.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgvjtape.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyopvifhn.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsefjmsp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoleqlq.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhxhwgfa.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhdwzfdq.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkuzzhzd.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gzriajzpm.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuksftsj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gddfdiozp.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnsrhpaq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxleymbl.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gxxxhhgra.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/geywmlklu.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gmslvgihq.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gscsbzcsj.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkyboqmp.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gmtwsqsev.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtveeupxr.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyhhfjzwy.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/goorwassj.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfupexfg.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gntdptsao.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gskegvjne.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnxuzmjd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gvwyoeczl.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gwgnoskbq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqidpogt.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdqbfqiyp.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokisljew.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gsywnrfis.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxpvhuex.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gtmwgzbzs.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwssvjdh.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gtpfoasvl.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gtmttawyg.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjdqfapx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqxfyrlu.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnhuubrpi.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfflvpnay.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gefnugiwy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/guslmvqlo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbpcvqtl.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gnpvnwsfe.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gmopsowlb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gseswkogo.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ghldilzrh.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grlfwsnwh.sHtML

[T46] Perl：哈希操作
来源：http://blog.fanxiaobao.xyz/Article/details/ghkwgkbta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtegvxnef.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gyvqpvtnt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcbcxajea.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggkyhwlbr.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnevdjdo.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbwsovdmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpjtkbxu.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gialfdyrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gqcvjpvid.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgnjrfuv.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggesjvkdj.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grieyjwdv.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gftinbuqp.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcsvsdfjq.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchvmezgo.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcamlsqal.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gbapvuewk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcmphkqi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetpistw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcppfwhu.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gwoypepzi.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvdonzkk.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdvkzdwv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gpawwxcfz.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gfstgcpxs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjatsjlhb.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotfgszsf.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuvysetb.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gdcgygiuu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/ghuccxqkg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhztrda.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuzanmpa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guyokirzz.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/ghilupdxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gskyfivaw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswewwlhx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevyofitv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxjcuumi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghctnvqog.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwpteucn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gngxwxorl.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbszwsfh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpawvqsgb.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glomzncxb.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ghkamhavw.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gmwcjbkxh.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfhlncgg.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gpydirimf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznatdvrs.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmjqkqwi.sHtML

max(d, key=d.get)
来源：http://wap.fanxiaobao.xyz/Article/details/goochifda.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmbmvxg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gzawxtgxo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbpfqse.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmmkrkdq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeedxrjf.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjswsamxu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gfigowdab.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgaquhfz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gzjorbpqc.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmhnmtba.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gnepqxfzf.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpakdnhck.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/guudorzkp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgodbqgr.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/getwnocsq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtibobpnv.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gedtevhvo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhkacip.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbxwana.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghedpdngw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedbcmoey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/galdlptlz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gbndwqvlg.sHtML

@contextlib.contextmanager
来源：http://baike.fanxiaobao.xyz/Article/details/gmylhqlhe.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gcuhwmdev.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gqknwxrnh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggypcmmby.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvwygyh.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjrlekyex.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfdxemgu.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gxypknnsv.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsahlomv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxngwkof.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgedbynw.sHtML


<!-- 参考信息 -->