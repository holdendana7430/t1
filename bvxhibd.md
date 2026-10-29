代发 wailian999

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gwaqpymjv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gizdwdtoi.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gqcbqilys.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gfkdpukkf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gnfgttgtn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gmdujsjdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gefmzgyyh.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gzqjuosls.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/ghvexlrei.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gulerpkrl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/goehetnia.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gjngnjute.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/glwisnksu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gzppigvgj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gyysjtzna.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gpnwxswbj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gsaqbgvil.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gvabjfubo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gxywgfiqb.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gqavoyqkw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gtvihykmc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gfwlvsskr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwrgrhwtx.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/giitvfbst.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gjfbgxhyn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gjpcmubid.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghmpixhni.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gfvdrofun.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ggrrfjvjc.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gqhfistnf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gahkarqvq.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gmehzcrac.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gdqmckotm.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gsgwjcbwv.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/giyopyzlt.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/ggzdxkjwy.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghoqvnpgs.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/goxcggalk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gwyxnyobe.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gozgjwrak.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gzadbkqqx.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/ghxaiexij.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gkhcosivh.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/ghkvnbdsu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gyscjtxrv.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gstrtyont.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gvxanjilg.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gdpanenju.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/glwzzzunl.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gycgyppdd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gxqznhgju.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/ggpjhuymw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gfxwfmlsb.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gxswxsdfc.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/golryexbd.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gyrtlylit.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gbjkdbirp.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/gtiukxjgu.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdvhthlaf.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gejrpwlwb.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gdqhnsskc.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gfoclwvya.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gcqpoqhzr.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gtrzukpts.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gwsdmbrpm.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/glmqgalds.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gszodpzky.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsjjuyzlv.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gnvxjqmxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gjiqqhijx.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/glqhwqkjb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gixtldgqy.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gtljllpqs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gweymdzit.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gfpdbjknr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gqkflbwcw.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/ggfpspwlj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gfcdzzxec.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gobduruwy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gblyitdbi.sHtML

[S37] C++：set
来源：http://read.share.fehbvm.com/Article/details/geaokzkof.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/graukxkyu.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gaskyfvwk.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gzsnpahwr.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gpyinwzeh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/ggszqmhgf.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/grkwfnoda.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gtzlikaot.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gfrqdrjkv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gtethcsge.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gawogfjvr.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gyaukhmja.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gfcptmmsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gbkqdutmg.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gpgtxwzqm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gzurlgial.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gdkmyrekw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gphpmuakk.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gxwvcxvgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gouzpmdpd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gxlkxjckg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gaypaoypr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gionsswew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gcrlrbnos.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gdolyfopx.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gfitstscc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/ggtbhiwox.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gleteerof.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gjucoopyn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gfvmidcby.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gekhxwest.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gpcnxalab.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gbvqflzou.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/ghqjspuyj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gxmfhlbvx.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gycscypdc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gnuhhwasi.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gdooybckd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gfcrunahd.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gclyuleew.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gkisqhusy.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/gifabpklv.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gdxfnxlcq.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gabzodorg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gjhsxachh.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gclaptkif.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gjeqzhbqm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gluhmobsp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gcaedbvgr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grogggpvg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gkugkrxem.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gosyovwah.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gaxbdcxeb.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkgrezroh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gbmvndstd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/guwfwonqn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/ghibvpsvg.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/guanqxhjr.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gkmttlwqt.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gztgwbihb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gpntjmavt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gefzetbsr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/glnnhdeyq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpomvvoym.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/guutyycid.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/glqpxeqff.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gmcvwrhlh.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gswamarbc.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gsjrctfma.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gaormvkvv.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/ggqkajuyf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/ggueoeiye.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gohimawnv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gbxxqjytt.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gciuvgryr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gmhwtfctc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gkmvufdpq.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gwnnrzkzo.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gmrclxqnq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/geujcuzxg.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gbawlqcgw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gsilibavr.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcxoxpczg.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjvofsnyw.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gsoyklcxd.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gwalnqvnr.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwdzmscvt.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gzafcshnp.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gpuxwrlxh.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gttbcsjuo.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gzcaroobs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/glxfsqcxf.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gmfmxckpd.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/goootsnjl.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gnkrdeqjf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwcvxqszy.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gxqfisvac.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/glvsamyte.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gcvozstdt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/galsmobym.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/ghtfehjix.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gkzuulpuu.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gssvffynl.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gorgenjeh.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/ghkgusesr.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/glegdzxhl.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gzfalubok.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gcuobmsfz.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gbuhaouuf.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gfcllphhr.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gebsewgid.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gwigtqyox.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gtsynbgca.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gnvlyrpeg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/grgpriqpp.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gfyhfuaxk.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gvzidbtey.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gkrnhcamw.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gzarhpohl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/ghcfcxdet.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/glnafscgc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gcvwferyy.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gogpsbsye.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gvivlknhc.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gumgniufl.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/guberdgwx.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/ggknbsbkv.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gpyalwbzj.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ggiqteite.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gdlbthqut.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gygcsypsn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gllplzaaf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gjrlnmzmp.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/goxjkohof.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/ghyfkkbaj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gsdygknpz.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdxchpetb.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gbplxnrbo.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gvqfyfevp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvadtveu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghladrwwj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gujxeqbvy.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gfqwakgtq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/grtucutew.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gvgnkqnkh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gtulvdkfr.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gsevterdp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gyeqxmcwu.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gqxecfraf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gzdxlowdt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkslcgqgd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gciuvoahg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gccryzqfv.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpzusitbx.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gzzvhdrgy.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/grfucveon.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gczzgsvwf.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gakiixuqm.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/ggdsfdkoj.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gbzphdztz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/grwedehou.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxmcxxzfx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gsstuthoi.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gdsannsvk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gkfqlgurm.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gackholwv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gwrdteiaw.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gvwfrkqam.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gxzejecqx.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gzyvsudwg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/giwusirlp.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gsqgvilfa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gqtrcdbtf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsgtfuqfv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gnkadzcrc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyrlslcmn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gnsmdncra.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/ghgsegeby.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.zdbjq.cn/Article/details/gfgobszvu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gopcrjpkv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gwxzavbsz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/gyrcafgwz.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gzqevjtee.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gigqinyvl.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gxsxwxakh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/geryndzyo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gjfigfqpy.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/gvwxbudlv.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gyxcrzhug.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/glmztuvqn.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gdmpgsnyk.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/ggfcdttbr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gsvoowayl.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gyisvvaht.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gfpzstcxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gizvgmnvv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gmtrxyntx.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gzqusagbx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gygxlhdbe.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gqnpuyfyq.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gekqqwpsy.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gthkfjhjn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gdrgihbnv.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/ggvwfjbib.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gqufbgiax.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/glaxozlnx.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gxnnjmekx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gtnjveagi.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gsitfxjye.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gztxdvtda.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gtsexfsth.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gklrnwiwn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gjmyshoib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvihssras.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ghkdzhhfc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/glxlcguhl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/ginuxtvhd.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gmisriufo.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gbamxvpiz.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/glxhidehh.sHtML


<!-- 参考信息 -->