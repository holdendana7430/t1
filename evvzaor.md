代发 wailian999

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gvmeauabg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnxrcgkb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gsrkudskq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/grlqtattj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gdqxxagwf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtamemmxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkafwgzw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gnekualfb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gotxzrppk.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gvswzpnzw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzocqcehr.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfooznlf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gshnwmgtg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkptbzio.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gxvcyzvud.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpozxekgw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqjmoqry.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gucrtyiwt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtmvouzw.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gsufouxer.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkwgswbh.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gchxnaqje.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/grtutzkzl.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdujesmc.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gtrgbzytg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjgfewjx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgapzfwv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnapqgyw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhvexsvh.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqaryqzf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gptpwbmot.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbwpekbn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godxztztp.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gyciifjrs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/ggayfvgyq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjboclyz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmauybqfn.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjkdgjod.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrbhtghw.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gomxiveva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxewyjfp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gbaffpwrd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gklhcmfkg.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqdyfooq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlxofszz.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjfylckqv.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyroyowi.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwshzci.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxqurmhd.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqttqsyj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbmafed.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjcbntie.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjzlmura.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gcxdawtsn.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gvudvbsov.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnkxqrgx.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxatfvtxp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvqsnyib.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ghjpajetf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtetgsfbq.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/grdcfmhsc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdqnszyo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/garldkqzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmykzfcjm.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqdtnnan.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxqgbhfn.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gkggimvjq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjutbnccx.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/grdrkxdxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiotujvv.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gqdhdabiz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/godzhputz.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghfbropmx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmhawkri.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxtrwmg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/giswvloub.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gasfpydtx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqogcyih.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/grruwsxjn.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gmdejaodb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzlfuxgd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbsqbzrq.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gyjpdhowo.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudxosxgg.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gsidcgdts.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmtpzfqd.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfryduvgc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrxrvesp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/grhygzkdm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixbdrpyz.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gydiseqmr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gekzndqeq.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhyymyn.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/ggzbutxme.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzslaitg.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdgmgxlw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcaqswyu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gknaedhhv.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gtupjoknh.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypvsuxe.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/glzfkjyjr.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/geysnfepc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpagpexr.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gyikudcyn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gknwxzxtd.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/guwriwmsy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxhcccdj.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/glrcsvith.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gijobmeut.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggwrmoftz.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcdrapci.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtotnxxdp.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/griwbdnwl.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gnqzomryw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxegdhgg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/giqeaciij.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcoqqkzm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnisxvknh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzklyuroy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqglbzps.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwmdyrj.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gufhypynn.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gochdotqp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuiibjma.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gtdambmxd.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmjnnokbg.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gfcxaaaub.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbawlbjg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gezcfmqhe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gkynxfgtu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwkwgiwo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwyyykjpr.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbqzoxmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpesqmgqs.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/grkevywao.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcmwwqxi.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glygbjgbw.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlygirql.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geezwpoqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllraagj.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gzevtqnlg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyxgnern.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmszxltsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdefforp.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gixecgbii.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmnctrhy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukofyqcd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmadromv.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gluqdrbwo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gppsuzkhh.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyqondvlm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcixqxfu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloubikqq.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdxgzyczl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gklcacdtm.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozlomcko.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gyokxivtp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdvtfuusb.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyeqkmjw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grblkegvn.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/giyhfnggq.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gaftvthyz.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/glvenuwqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkomyjftl.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfsahrzx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbheuqspy.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfmhtbis.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gegntcqnk.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdbndkkk.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gealxxzmj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gklendymo.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyvfotft.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gatryukbk.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmufawohv.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gujqilmql.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/geksrtdmr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbsyxyl.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gvmucuwbt.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gviocjhnx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gmagrnhou.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gxqdanuet.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtvobzut.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcedoolr.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgnzqbgp.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxfygxoy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gvrynhrpx.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxdueaee.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqenkcji.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpgtfypn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtndrxewa.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqceceuyu.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gihdxtgyw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuwolzwz.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gzqlcfsrt.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzvjsccgv.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsbvsgcp.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gshasjqmq.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gngnfmaly.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gncpmsdek.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gujlcirlk.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjejfxxt.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/geaugjihi.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gbalzguvf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/guadwqkyx.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gldrqgbho.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubhomno.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvkndvgme.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbmyveso.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkucpzzp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghunkjojo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghoskbjcv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grnjksnch.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gfyipsmce.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnxikutr.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grqmuhybz.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkwulzvg.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gzjesekju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquvdjszq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyuzmqfnw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhgstkq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjazsqjfb.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrqapizx.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gzbtapbxk.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfeauogy.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ghyglpqsc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gujtskrur.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gygirzynd.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gfpqupjth.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gaqhecxdj.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ggtjhgmsg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gblqescbv.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gywpfnifx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gynarhrcq.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpikvnhxn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjzmkelt.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjntpwva.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjfozrc.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggllhugyw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/goiytunxa.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gygtagkza.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmpxtuhi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjzdjsuh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gdcgqrgcs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnuwealg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzhjllbr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gpaxjxrnv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gwyhtyqtg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsndhvjnb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrstuczf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrveiykr.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/glspbgjkc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorlbzkhx.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjzorhxs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gzeedvbhp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxzupkkt.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndowsgmg.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gnyvtsxnf.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbkhltsv.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/ghktpwvxc.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gmvppgffw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrneuyb.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdxhzgka.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/geatlccck.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gvboopidy.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexfinjcv.sHtML

(x * 2 for x in arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gdnyxyjdv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gulpzsxgn.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gymeoshib.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/guissopth.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmunqvxq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvjzxucz.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gevrxxdcb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqopdzzu.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlxhscoz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwvuancu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gaqktlsbi.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjklwpsso.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/guceaowks.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gshohmrkc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gazphream.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gypzxiipd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fanxiaobao.xyz/Article/details/gukbtjmbr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gztvmhgfv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzkszkft.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdosxslrm.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrkkvywy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gikrtflxq.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gosnspggf.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjdxqask.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxdwyyns.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gtudtkfuu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbozkuwrw.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdyyqygn.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gcqggqxft.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvgneps.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajsmurz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtqarnvn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbytqnah.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/grmpypzte.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/guwmdzvfk.sHtML


<!-- 参考信息 -->