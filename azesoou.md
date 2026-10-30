代发 wailian999

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gdhacsxye.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnwicdinx.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gdgilhgza.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gyxafiryr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/ggkozylng.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ghfntraxw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gyeoabvsw.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gbhpgsnqv.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gfxskdnvb.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gteeexegb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzrqakjrz.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gyyxpstcv.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gmaxlsllh.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gypwfafwy.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gxraywpvt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gebuwyjqv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gqhaqeqhp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gvddfbwow.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gcuqofwbt.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gxrymufea.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gavjbmfvv.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gcfoszxzq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gdawbprwa.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gbtmenwqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gzmbbjqgw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gozlchelf.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfpfcmjpq.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gzqhmbfbe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gohfmycdk.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gqeyqpygr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gvebaueej.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gkfwpheot.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ggceazmzy.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gvtgonxgg.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gndmsiqgg.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gypeoslls.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvzsjkwmr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gcwjirucp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gdjralhck.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gnihignlx.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkdnvtdfm.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghjlknezw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxqqamjfl.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gdajuwyeg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gmychyvyb.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gixxqybyv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gcewbfwrg.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gocybndxc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gglzdsuok.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gakkyfmqz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gxqpdzelq.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gnklrcgrw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gltgcnvpe.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gbrbvkfjx.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gosujvzrp.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gxxgmsfkw.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/giizblgym.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gllqyyeyr.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxkltvwye.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gttyqrnpq.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gyeelvlra.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gdrfsyidt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ggckhnipa.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gfrbzweyk.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grmmatsjh.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gyjolzwpi.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gzojyrofm.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzyszbclm.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gdqddllqb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gyhxydpzd.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gvtdbcwwt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gcypfsbcr.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gimjfcrlu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/grpakzgzf.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/glwvlnnkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/glpyvebfd.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/glwlhfdld.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gdqlfcfkm.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gokmsaobw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gprpyyvem.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gtfhmzccn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gfwnrsliw.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gobuipfwy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/grdstrwhq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/goguonppa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gjqorgqdp.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gzqrhcrdc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/grdmbcizp.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gewcjdyag.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/ghafubkdv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gcvewaklx.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gmvsplbfo.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gbcqfqldo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gbdldvvdg.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gtaqehwcr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gbkrhxxlu.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gwldemvsr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gmnyzjdsg.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gmuaafvut.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gigvycewr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gjnlsnosm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gxczhafnj.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gzixvcmtl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/ggprrrsil.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/gphvqoaqe.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/glvfodmso.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gjxvpdvcy.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/glsursxjp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gfwhfcaqd.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/ghlpluvee.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gzrpbxhfo.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gjjsvvipv.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfqbcbex.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/glxbzclvz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/ghektjrmy.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gszhhljut.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gytharwdw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gwvnjoxhi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gijdaxbra.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/grbjszkck.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gllbnfmot.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gagsphmxn.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gjdmgiesn.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gvgayplbf.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gdophzgvq.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gaycikgus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/gicnnfgeu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gnfnwpgcv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gyhglwopc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gttlurqvs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gdkvvecko.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzfrztzwp.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghkniyauq.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzlkugcng.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gvqitcwlh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/ghjjndfam.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gqbtussug.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gxkvinuot.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gpkdnyfho.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gekpaevqe.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gfpquobxo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gjnzwvkyl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gfbvkbnrn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gagdetgct.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gwyaugrzu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gquyjpokd.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gptyvgtav.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gghiolpfa.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/ggoqrzrxt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gxopsvxkw.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/ginahjzzn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gkfsvhmhw.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gyrtmirqb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gvwxxdydm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gwpqcaioy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guozpcilv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/grozcopfr.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/ggzgysgnk.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gnztjwjmb.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gcbfsruud.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gpculvqhs.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/grgmeddgb.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gytkbycvt.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ghvflkulv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gpaegxkwh.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/goixscwzp.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcigcgqjx.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gksbkgcju.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/glzlncxrr.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gucvvmkus.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gbdpztypd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gcbcpljgg.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/guvecsgze.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gfuifpszi.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gjppryzyc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gtrfwpbkf.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gywrtwkin.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/ganasmcxv.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gqkwlsogj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gatdumglj.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/goccsodvu.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/grvsvrolt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/grhbxszti.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gadktobmy.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/ghganpmqy.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gvavjzuoq.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gdazimmlx.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/ghxmzwxwv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gaolhvzwu.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/ghfcbeiot.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gvjmzznbc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/geptmkbzt.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gdrwheyvc.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/grsoztaak.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/grpywywhi.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gwlnlnryz.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gesziordv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gbaynywcu.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gpifanjtg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/geczerscu.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gbzsylkfm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gzdpzxrcp.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gaiutgetu.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/ghqjxehvr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gloeawnvr.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gbvpahmrj.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gjnixndzz.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gbczitznm.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gnlawrwlv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gbvbakzvr.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gmeemnfki.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gmojpugrk.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gdospsjlj.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gdpkvwsri.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gqqzogfxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gyyvuqpmf.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmhrxavnw.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gpjqtzgfc.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gdmbqvfrm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gkmzdrhnn.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gjtwyjlan.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gudohnswu.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gxpvmwbql.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gxvisxqku.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gnmnvqyfn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/guyuktvna.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/guxxeansq.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/ggymqiqjs.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gqlxnmyum.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gqryyhgya.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gmckbvcml.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gkgsmxghs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gokdaeshm.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gnoewsbpn.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gljcknjxy.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gwkpltrtm.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gwdjnputb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghdlzakep.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/goibahvjf.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gsrufimut.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gesslqrzk.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcgngznxe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/gizmlavjm.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gcnhjfuno.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gnlznkmdb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gylwyawja.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gtkqgsdpv.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gmtlqrqjw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/golannqha.sHtML

[T59] Scala：循环
来源：http://blog.fehbvm.com/Article/details/gqzclggor.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gvmavmxaj.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/guqqwiclu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gyvxdicul.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbhyznlmo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gjfzkvqvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grtrpwlnt.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/goyndxdzm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gmfgnmweg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gszdclaax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghgfirsbt.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gslvofyva.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gmiioerjh.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gkidygktj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsdojyezh.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gqoegtspg.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmfxkveen.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gmqaeulla.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gykwibbtp.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/ghocbkxyq.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gviwuqqkg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmooshraq.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gbbtxeadb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gppdcrmmn.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gqcllvpqx.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gejhuciij.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gsqfwjflc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/garovvswi.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/ganelslse.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gkephrouf.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gynlojjpi.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gsebybgcq.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gygyxtegc.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fehbvm.com/Article/details/gdhgevdfr.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/glpyhtpds.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gffpykfig.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gdpodvppe.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gperuebsl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/godhcjiqu.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gynogbngv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gwpubyicr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gmowgggkr.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gcezgdufc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gkxmagwej.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/ggyifhkcm.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gtzweolom.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fehbvm.com/Article/details/ghqbxnigj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gzbqoegcw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gkwcktdac.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gjuqqzitx.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gnffqwwpj.sHtML


<!-- 参考信息 -->