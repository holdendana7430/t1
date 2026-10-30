代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeobbzuv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gejxsxlbc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gczkpfojj.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxkpyuqg.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkwobgvp.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcywtjky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfgmdjuv.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtposquvy.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnaraajt.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggvixztp.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghnrsgmi.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/ghysignax.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdakgnvh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gdbyrqyds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwjtgfdt.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnlfryvx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqegnqpk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpdmcjil.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gshosttkd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxqewdmt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gmmuwnluc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjonqeqf.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdsrpfpt.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/giqynnuvo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfiiwzjr.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggthxhnwe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnofpbzxn.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtggnllw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gvqzfouaj.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glfulkrnu.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnugyjhhu.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gdjgxtros.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gychuxbbd.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gelzbyjgu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtosgxnbc.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gipznuick.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipotqpvb.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gytzvnnsj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjpphnpy.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgtoyxfv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzkebmdy.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gppqutber.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpihxuhiy.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gzntjkwox.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncqhegnx.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gduqrjxqh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gusvburiw.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gtidubbun.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfbpykeq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjtemhup.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpegypdef.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gfouqczej.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznpenovr.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwicetbfn.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxynowmqu.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gnapgqomg.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gykobnvdz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqflkuvc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/glwhmwbsl.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfjtqkxp.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjlwkajh.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gijtdqbmr.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxavkemy.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbfoxllsi.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gjspagcrm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcuksyoe.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glulopiix.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gwarnbdoo.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaynfomzq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhomogka.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gtlcwqvrn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gharvbqab.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuzaodkp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gitlubdqm.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gealubgge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwyrqvopr.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gzryloweo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhqsrer.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/grwnmaiae.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxacbvnb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwwxyipow.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkkyrcfr.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gupebtqvt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gxxooazmj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gslpsifzz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgzmysq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkqfahl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaetncuz.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxrhiwaz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyddxhrm.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gxmbzvkpx.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvbunkgnj.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmkdedl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzodevrz.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gqmgdubvx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdbwesbf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggriroorz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobjjwhmj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqlkjgkbd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmhobxnv.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/grvqdywiz.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guakzarii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gwzebzkni.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutovfzs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/geywasvqq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgsesstd.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/glqmoujri.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqvjoyho.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfmgrmkmt.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfqwmkol.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbdbhtfr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsmulikv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmclrdyh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/garfelebu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqwmyxhg.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlztdsfe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvfzpfh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcajthej.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gvxnmebub.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/glhjrokpb.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gheklacuy.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gerxatgmt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gqajaghkz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlxjvjmf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/goxmoxoad.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpxtzmxru.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidimbej.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gauqrzfsd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gdkxwdpsn.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gabslzzrx.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfgxledob.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayvpdonl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gedhxsfcn.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gscgsegrc.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwantiu.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gorkzihpr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gflenpcvq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gmmuqjiop.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyibtxtf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gliomutfk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grvznhryn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzpefmub.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganynxfpu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ghzmxshwz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdxwhbiz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gegmkrthw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmceafxfp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmoqotoe.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gcxohzzyv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gnclhmoce.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkxrmkqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gieohjari.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfvahkfm.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnxmumxlw.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwhddskn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacvcedcs.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdjngsf.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqjolqxk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegbgggdy.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gahrztxoz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkppvjes.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gctxoxyig.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqtsuhoqf.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gintrnzqg.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/glbaahqpk.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbppnyekg.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/glnmfclgp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjancbam.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gonobugzx.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeotqijw.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gtwvgcwpy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbyncgzn.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/ghamhqtsu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gaeegzewa.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxbjqwtv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjryawlv.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gplnvvdpg.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvczsrof.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfhyvgmo.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gdaenquxw.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtsaxofm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktugqpij.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gybikztqy.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykcvstsr.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqqpjnum.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrcsjoty.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gpaykygdt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjuicchdg.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrqnplfv.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gogbjofsf.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gepwemkmu.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghbtmtkwa.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/geatjdrvt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/grhsnhpgj.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/glvonhrxi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gfergufpl.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grztuopjt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gssefhpej.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqmwnbuh.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gmagiwcgr.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grleyubqo.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/ggzyorzgq.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyhatdpc.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeyssdkx.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gpueaslnu.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/goqaynnhd.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gclzmxjkd.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gkssqeguu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girsezvra.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbeidlhw.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gedpxvgyp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxlsfjao.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/goabybiuu.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gghsyxeer.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/goqzfftjl.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsftmncrq.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqxzrtm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gczwowfeq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlwvzxsj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddikytjb.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzerhbrq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvbctsts.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gndthcnvl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulkykzbo.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpasytal.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/guckynrcn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqcrekyks.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpeisfyg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvfjjzoa.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwmerpgcc.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfcexejg.sHtML

[T52] Scala：变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghhvtymxo.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmiszeec.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsugdogbf.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlhdoyja.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwraoyfog.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqztlsfxc.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gcqvrnvol.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidkxonc.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gkoooyqwt.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvjginwl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmiwwtz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/glplvbjxj.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gfowrdvep.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsahbxk.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgzbmfun.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxmlhqyds.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gogifpeol.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqwkcyny.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgeodqhn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqobbnqj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpijvsdyb.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnogtrx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gmgypmvaf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmunjjuy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbdftgtod.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/guvnjhdhm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/geicsgdvw.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gbqurmsky.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gzqxukfix.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gzlmskaxe.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gsqiulkaa.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gizcqdekf.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/goynkzzvj.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/ggpvkimcp.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmufcjtth.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdefmhpr.sHtML

[y for x in nested for y in x]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotodota.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfewhodey.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjbamywq.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/giykkzovd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gaombjoza.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsldbsvqv.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvhddtgke.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkadjtdrc.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxjkxxfin.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/glozbdszd.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxuidbtl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gdtkmmalc.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsodxhczd.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gdlozzsfc.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gayokuofh.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gmnhiqtse.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxzoiya.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjyfkako.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoumgwbj.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gslcwbktj.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcpaiexj.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlizmnak.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwggskig.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgncgrkr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykelcywy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyncpxld.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gzctnaiyd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/gclxgtloa.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gnduqbevc.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfekwxgk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhojkki.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gyhowhvtj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcenneqr.sHtML


<!-- 参考信息 -->