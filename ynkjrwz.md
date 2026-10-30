代发 wailian999

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gganfognz.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gngrizuvh.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gwrfdybqt.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginjwpxwk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdhfjszu.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gitetbdxx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gcmdooevv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndrsdqur.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvfoejpj.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsdykzfx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeksyxop.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwldqjmex.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gredzkesz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnebzpjqm.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmckeurif.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdffvajqf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gedicsxwn.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/griwnykuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gugkqwzem.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gpvcwtkrr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlftszds.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gngmmlgaf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjzcaxke.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpuojpyg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmequsgxf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcgoodzl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gvaxrzqld.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhhkeoxn.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gntgebzid.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/geiqjjlsw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtnprtkv.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsripfye.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/geueidksj.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwcdiegn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjczpqztk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gmpibkkfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuwmanpk.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/godkhojry.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprnfprjf.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqcmqgdw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdufzyazk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttvskgyq.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghauluaha.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlwlycej.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gchbpznok.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gakwumwqb.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gjlsuqnhk.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsiiyste.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpylawhu.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwlhyyvz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtlzttui.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gjgmympwe.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/geuwodajs.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gucdehors.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssexcszi.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqptcws.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiubccae.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbyvluiwn.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwhqugfs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpkfclue.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gyadlffwi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gecvipozt.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ghesacvni.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gluvngzzg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxwkidef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuixhtmm.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gnvjkpvqw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/giubnkspc.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gywuzexln.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gwqowzrxm.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpvnjmwo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmopizzyh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gurrfjoaz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gbraxoall.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gqcluoacn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gncckbenp.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glqonbruf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtfdyvhy.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmisefkty.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxbyaso.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/grdubzlzi.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbreuzrhv.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gtpcflhzn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goyfkpydf.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gfyujpnuf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gweshhnue.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/goldiclja.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqlrhzyq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzmbsyzm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmsawueo.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkyyjdfs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gaexdmftd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnweeioaw.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfoejquu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbmrtvtr.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gchrfanaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gpqznuenc.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtrqshngn.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/ghbtxlavd.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkzkcorn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghnpwxhpo.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaflcokuy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhaoeldg.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gnneanvay.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gqhtqdqvu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxhnjjnq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuhssdjk.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcoqxkoup.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gprelnelp.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrkjbop.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuonhdjq.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrbwskur.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gnqnbipdn.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsnnnef.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/ghnetdqyu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glbgpmdln.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoxnaece.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkmmaoyp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gofvoigai.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gatslmoxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gczqmndjn.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gamfdxbpi.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gndhkbpro.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqgkdueq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gffztdsnx.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gfchmruam.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfjreqke.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gukisslls.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/galohffnx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeyfawro.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gyecinxwu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbvwqlpd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfaztnmh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjeubliun.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/goexwwcxp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gysxsrztq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcijjrbpd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvycektuk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gymprqsjg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdhtsfmup.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gixahesfj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnaeghyl.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/glgyuxhxi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnidlzano.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/glxogsnou.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjlgvmyo.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwpbmwwr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcnswnlw.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfdagsjs.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyfpmwvi.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gdlnagpsx.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdevuqha.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqgtcjxr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttzhnfam.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjkshlbr.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gilgafrid.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsxdsbq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gttgwjnjt.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gfutmzhrg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/golpmclab.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gteerdgud.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdpqmepd.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxoghip.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpokzwxte.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gflaesnmf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gefvhbwai.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpshkssw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gohefewht.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdhycxlf.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gbphdfoxi.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gahjxlixk.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqfewvl.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggejhoslp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvszsxgjz.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzstwksyd.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyswnhgw.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gzmrymkob.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/giuaqebjg.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gpadcfzjp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcakglyod.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgicxie.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzbcuzevo.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnyzjhnjg.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gdijmtryu.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/grqtktpfn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gkrhjsyuf.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gploaqxup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjgxrsfg.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/giicdread.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gynhqbgri.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gynkhojxs.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnxcpcdk.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gvmnyaqfi.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuxdabcm.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjxjozpcy.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gmgayekqr.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghskoeaha.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/grutgccxe.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsthgmsyv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnogsfwc.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvotjqh.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuubjeao.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gnsjgxftc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclsrqjy.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/godyqandl.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gqpnkrjea.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjyfcylm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcvnuqafy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgsawyd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goguucqyo.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzcwareg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxdrczcj.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwbzbhjm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwwpjhah.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyeqhhp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/govmirnfi.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxgsltb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzznocow.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnstmncq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsonfzryy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvukqzfe.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfivikkuc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmlnhajr.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giueunxqs.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpatlomh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxlpmjyrq.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmvhzxte.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gixrmvvra.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhhjouzv.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfqygplm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhuhyfth.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjrfuixx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gdyxxvfyn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghklpikka.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gndjycnvf.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/ggsqsvsvg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gqefcfpcc.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyudbsxcl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gdskpwsyq.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gohahsfmc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gumqzroib.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhnuqagm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwsjxhcx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkhltfui.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/grhmpkruz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gtineikjy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmcvzjcu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtxjqahlt.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gcgeyufes.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpucltlz.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcvcorqt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gffzjruxr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/ghdsepnzd.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxrggofh.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/geikbmwsk.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gmevmkmia.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbqocxad.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkkokkl.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/glfxbbenn.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/ghgqrqeju.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfxlldio.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gmawatrhu.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqxquyuo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkbapysf.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbdkztuxa.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuydmfcm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gypgyqelr.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/grhbceinu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqphqtml.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gilzimlgj.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmgajpun.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvnktqzd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsaytdoy.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gyzktgrxo.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gezgsbknq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyuuxtlf.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gylhijuss.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdkxihxj.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/goaeltbsl.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvowvrywx.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gumcmnlgq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gikobyols.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/guafpshkx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gsmdcdeel.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gcriarxsu.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpstrdrss.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gdgtolvps.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiafqlpe.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gewbemplj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/ggsaaxhsh.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosuwcxen.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gjiipjxhx.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gkakwbvva.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gzohwwbrr.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfmofvgq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gofizbbaf.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/galvikvoa.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/gyhkppcsn.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfvbqakx.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/glegagrjl.sHtML


<!-- 参考信息 -->