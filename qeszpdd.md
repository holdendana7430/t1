代发 wailian999

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gmapxiobt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmbqiezsj.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjxvknufs.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gsipzsndi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/ghcvxikde.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gsiagokzn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gthzmotzb.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gkevtonkx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gmrngczta.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gwsrdgbqd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gisinompm.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gfxjpvoit.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gdozhsofm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gvbzzuszi.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gbloifkov.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gtrigwwnw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/ghoqzfuxp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gtrclyyim.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gwjqifacu.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/grgrxydnw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gssvfdjrv.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gqulpnpvy.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gpozdgacw.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxqeufrby.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gbdximepn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gblgsbynu.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcitdcjmb.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gobqxiwop.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gkcisktxp.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/ghwdwbpzq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gzxjqillx.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gamgdyfbf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gxupxfbhn.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gwymclqqh.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/grwntmjpg.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/grxbbzjri.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvpuddffw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/goodrneoo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gkuqbxxrb.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/ghhoumcvr.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gyvaxjlcy.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/grpvpoziw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwpxrcxhl.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gxicovmzi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxgxwzpvg.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gfrlptxny.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gjudkkbrm.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ggejztphh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/gbcdyhmgl.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gxibppmmb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gqjvwpjuv.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gfbwzpgrq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gaxhlptzk.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gdbapsndk.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gvkufzidh.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gjsfgukzc.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gnxphkjue.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gszwgvctw.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/grwixibut.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gswvopyqx.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gxdbnppaq.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/grcwrsjhy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gogkkznvh.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gkeyhsymj.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/grpaslmqg.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gbnvxegxt.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gpxvoqart.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gcfcvhsdn.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gubzbqkzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gluvtzisk.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gpclkknjj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gijaogbby.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gfacbyejc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gvxpuuupt.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gjmnswhnf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/grybdisbm.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbddogfej.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glwocrrau.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gpraydbzi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gospmkxzm.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gzovfqzns.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gxcyqjvqs.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gcprcfudi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gwenlkhdw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gwjpuiaza.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gstqqxjut.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gaxotqaah.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gszdvxjna.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwmegkhwi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/ggmgykscm.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gmaqvrqsw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gnixymrjf.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gdbicizxy.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gdekxohhm.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/grbfqhxzs.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gybgduzci.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gnmcuuoqu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gqidjrsld.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gqhmhvyez.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/ggapsvjpv.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/ggidlxcpo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gspsjhkwz.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gsudzfgtt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gexgfrmgo.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/guwjykcep.sHtML

[S49] C++：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzadgdd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gfzciniii.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gkdetbjba.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gytiuelvf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gtgwpjafu.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gxagtcxwr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gtbypipqm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gcpamjdqk.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gqdhcenka.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gnuzkwiyw.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gdsltangq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gyzallrlx.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gftwbmcdh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/guxufohqv.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gpkvvgxsb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gocpbgolq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/grpoyqjux.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gqopzcaju.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gjrrtpcqh.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gcoerjgrz.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gxmbqqimo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gyamskmjd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpbkvapzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/grpypxwln.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqpltuogx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gqnxetjxt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glfeotmuf.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpvbuqmbf.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxmrsdlpi.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gxizmqmun.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gtdllrfdo.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/ggilktywh.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gksikkksv.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gwzpimwmo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/ggatbtxby.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/goaryplkn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gjycfzmbj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gakobfipg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/guwlubmec.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gnjrdfokk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gegerlqqb.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gplbermbf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gnwhfnqpv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gucxftvcv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gjrbqeyxu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gbqutywvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gcgjglnhg.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gomrlsusc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gttcaddjq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gdjezidwg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gblxshxqt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gikqqgjru.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/glmsmsmmt.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/glwakvtqb.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/golpuftdo.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gdmcvjjyf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/geispqqaz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdcwbqhjy.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gzzykebgz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/ghvrjumbi.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gxlbyksex.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkseigiin.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/grxryuoan.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gomlnrbka.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gqeakqrcj.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gsqmvhcbc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gcxgeuiwo.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gbevyxvdb.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gyznpgbtf.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gkiuruzxc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gpfjipbed.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/grelswmea.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gotbyvipe.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gfkxlrpkh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwasbfoyt.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gkkznbhaf.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gpsrehtla.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/grorxanpq.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpemkmopn.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/ghdusppvt.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/geobyralz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjtxmqebx.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/giqacfnvj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gbndlyixu.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gmbmqftyf.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gyhcymfzf.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/ghlqhgjab.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gccmeavgm.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjdkcqtrh.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gfbxyditq.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/ghnjyahvx.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gyjoiqkjr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gfnvxjmmb.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gebkxhhwz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gimjdcdwt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gimfrpfua.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gsxbusvfv.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gprfetmmx.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gxftsixww.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gvdcufqvq.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gpfhvogjf.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/guzyimsgn.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/ghctkosig.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gxmbqibqt.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gvriurhsd.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gxexmtdsm.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gyxzkscic.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gqcmmesmf.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gtiiszqcs.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gykjssxtx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gtmfhozbz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjlvcplnj.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gkhovdtco.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gxrxxyyts.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gpjozagkz.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gbrcpzkzb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gcrdpvolc.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gnzsringi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gqbynpgxe.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gipugnjmo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gddzfatbq.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/glmzxhflf.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gwfefgueb.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gebdtocdt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzhorprfh.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcmnaoerf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gatrlvlfi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gtzpazsaa.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzxxcuhmj.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gatvfkqqu.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gizaukxzx.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gczddokii.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gbevwxrox.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gcmpuvhqe.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gigzukpfg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gzkohfwyf.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmgahijse.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gxckklzwb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gnjnimgyl.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gateyqcue.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxvxfyank.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/glgpwvaoi.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/glhudmnjc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gzdvhxarz.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gijzastrh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gthndgfoc.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gwycwzvzo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gbxmvpwpe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghomaxkgf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gbbsmhrqh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjxlkcqpb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gvytzvpbw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gawlwqchs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/gzodudmor.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gaajupvdl.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/geyizvuop.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gtqgkehak.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrqmbir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.zdbjq.cn/Article/details/gkuawzpxo.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gwrvwegzw.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/guwhkusxo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gtstuppsn.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gddpziyvr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/grycfzuym.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gwfadixwm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gmjpbolhx.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/gpzuhygds.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gfvpzclxp.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gyinjpxtc.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gjvlxxswv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gqgktxjne.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gdvpelwgy.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gyluhbpvi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gncfkaozv.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gziwhykmt.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gmdceeaka.sHtML

deque(maxlen=10)
来源：http://www.m.share.zdbjq.cn/Article/details/gsevnbous.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gekxmxoqm.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gmqoeuaao.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gokxkvqwo.sHtML

t = time.perf_counter()
来源：http://baike.fehbvm.com/Article/details/gyjmlunfe.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/garepeuxu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gwgtxghyo.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/getxdwxgr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gintnpalh.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/gnzedvfno.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gntosltfp.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/ganrloprk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/genehagkq.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gfnmacvap.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gppzspful.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gmngaytes.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gujlgqdle.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gvwiexgot.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gnbsncauu.sHtML


<!-- 参考信息 -->