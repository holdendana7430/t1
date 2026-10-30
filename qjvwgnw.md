代发 wailian999

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gywonxmfr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtceswzqa.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/guhljpcvx.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gmjdnhepw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpuvrmed.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjsfhkox.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gchytuuzt.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gfaebbwum.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gproxeibn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrnafvdy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnlpwqsu.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqlmhgnaq.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwnhocbnb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzteawyph.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gxbrhnqft.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxwtllbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gycuabjxx.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gfvzidaqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsruzhde.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlkcvtey.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfsllfrt.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gsaibdagb.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gursaoojg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmydrcrs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwpxwcca.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjlcxexw.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqhrzqae.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gozhjrqis.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gkqkebcwr.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gwpatapbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gdlvijyfp.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmsqvfee.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuqmnlsw.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gviiorgkn.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkhyoisvd.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwsnudla.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/goncjwrny.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gidkofyfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gynwryant.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnmqissl.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gdszpdfvu.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbotqfbo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gbgtddyfx.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcgznovh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gyjjxpjfp.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbkbwfxvs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gnybazcbk.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdytsnasi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/garteydbh.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gncbvcfxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggovpmwhh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxioopzc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gmherfkdr.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjstocw.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofusldlj.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gmkvmepyj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhegieqk.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwguqqjnd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylofkkju.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcvbpzk.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyogtukzi.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfiqgxrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkecjcaf.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gyxyjsazc.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/goglyjbhb.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/golgdxoav.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/giwgfydfr.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibudkotd.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjfbzueh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcmnhllvf.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gearvwcld.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gukaebthv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/georegaet.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/giudmjgbv.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gadaafeia.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggycdnluk.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxrryfm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaweuuluv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvgtgzlt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glcurrhdx.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcyqcihe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ghcgvxfqf.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpiudrncl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwnsttts.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggghhgzfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdnrekia.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdnbempe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvaewqxwt.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/glmeevesm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmxdkmejf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaalsxlj.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/glkogqzgi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfeczykc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gpvtfqzas.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsftnzpm.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gshylngsg.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gvobhekcc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcuncxjz.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/grqjerctb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabwnbxi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfohkron.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gacxvenpf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzkbdwug.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gouimrgjq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpsjqsxw.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkennuems.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gwgymmunv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgjrzznd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsvgdlsn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzpbldtr.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/geenehphv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxojdiod.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqltsyrf.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/grnbtttmr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqexywio.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gpaqltxcl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpputlcnc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiurmtec.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gvafteohg.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqxwaqca.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswmrcroa.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxbpigts.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxmxiin.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gnreneyfe.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhsitaaj.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxiduopqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmioufsvj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gllczkoqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gamyczhcq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssnpduv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfavzesa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvadrbrg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gasouorlp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghmyixztc.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gftosvhjg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gitmcqnfv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyggeovu.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gozjjmenl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/glhlaoaos.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gsenqmqra.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcztponzt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmgqqkej.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkywlcie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxeismte.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdixcdshf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gnqfdyefy.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gffbcsktf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblkbtyrp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjybufgbn.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/guftxsrcz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmtoiubk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gsaruykil.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzezufgvc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmttklic.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/grurvgxeo.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjnwqtiw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzynjofix.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmiinydea.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdbzaqlpp.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gcreftjkp.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gvnqstlyz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/giizllcbm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqrohzpb.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhmqkmjh.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdnnkakk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjkndzz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gymfvjlny.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsuskdsb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoycympl.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqarnfra.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gcuroaogz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glekwyuej.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gcmdqyjyc.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcjuiexr.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghrewlxcg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxvzyppjp.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gytuhupbl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gzapdigjy.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzmavxd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmqbvsye.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gyevhxptm.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvvnwull.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsriodrs.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzkojaev.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxvljxz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcuncqtz.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gvymcarya.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gswkobjjp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gqibomurv.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqexjxhk.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/geucvibnn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/ghesfabjy.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmoonqyf.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwmhmaat.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxycfpuf.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohlezcby.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlxgswgc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/gzuyvcmax.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcffqydw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtvhxzxa.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gasrzdgfk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdcwigxu.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gzgtabojo.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gusbpnsqm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gmafkvmjx.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjfqonzg.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkspxhntv.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/ghbwjmhow.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/glfhqqeun.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gojqvdefl.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxoppgwh.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/girqfeksm.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gejwduuce.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrdhctd.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/giepohkla.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gqeaqiimp.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gadstyfgp.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gcautuhfr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltxzknmq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtppgflor.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gzchytyqo.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gafumldtd.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/grxwjjoxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkmtqcyt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkdpkreq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmhnpgyg.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gijekdpkq.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gzjjgftwr.sHtML

[T49] Perl：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhpatdkr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/getamdwic.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmldwidpc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzqxizzf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gygpeqckl.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpnppbn.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjzcrcwc.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkumvtyo.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpmersapd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gguuplons.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnayxamd.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gyeflejev.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gnxdxyqxy.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/guuiwysjp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkchxhdgc.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/gvpgwjfvl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrkxttvt.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gpyzsphaf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzigngssm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiivtxyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gziluszny.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gdctphyul.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gqobhgduy.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/grxcpjpjj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqyfhpnb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrzdzums.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzcffkqay.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjyuwibw.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gatlcircu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gvriftmon.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwmsugl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnnmgquxu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyalbcul.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotybmuih.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/guqnqgvyk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gqnaoyzcz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/geyonuunp.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgvlwvhb.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gvbnmhlto.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/gjjfivyfw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajzfkamu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjtvzify.sHtML

[U08] Py：展平二维列表
来源：http://3g.fanxiaobao.xyz/Article/details/gucfhkmyq.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnwroeqy.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/giiyvczqm.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssjitrnq.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gpxfblhbm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gqaxaqrva.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdccycuh.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqjhzbc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gihmkwnxs.sHtML

Counter(arr).most_common(3)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyejxjgk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfxvwpn.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdpawtbs.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvekwgms.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gouuyxber.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdierjsa.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gtfygkbhe.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gzegfntfa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneqbnjxm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujgnrgwv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giozbwkso.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gnvpnaejb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gploqgaxc.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gysblnhye.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gastvuvrk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/glpyuvtjx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gulpfmysq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gshawmhnt.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gajoytpbf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkuypmjq.sHtML

list(zip(*m))
来源：http://3g.fanxiaobao.xyz/Article/details/gogqijqpc.sHtML


<!-- 参考信息 -->