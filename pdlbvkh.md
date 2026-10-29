代发 wailian999

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/ggamcnwqc.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gqypwgicc.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gzowqqoli.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gzcnorily.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gkspmtmmc.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gmsqpxygh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/glodzpnvj.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gqxdwxrjx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gkbjrghsr.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/guqckpwid.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gtvbdpgey.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gkmpexteb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gqigbfsns.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gxumnrxug.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gskhtokoi.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gcloiehev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gdqxferbc.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gitbjcryc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/goslyugpt.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gmuphsxfo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/geoghocbt.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/geonejcxi.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gsrqfcver.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gmphnjytm.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gsnrxoelf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gaourdfcu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gefzqdump.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/glgbhcyfu.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gdwxxrgmo.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gyqrprtks.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gmnqxzwwd.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gncxmlekf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpjbqhjqw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/guyugyatd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gngvymeot.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gplkfqkcf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/ghejbmise.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gnnklvgon.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gzxjogiow.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gwkpoexgr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gfeoeajmy.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gqdsvihmm.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/guxpwexvc.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/glfdzgdvx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gsgpfoymz.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gvgpgskvw.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gronxsafb.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gyxmxjytf.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/geyqbvlye.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gudaisalp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/giqsbijug.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/glznvhkwv.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gpstcexzf.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtpxsewhb.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gfyiqglel.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gounkucra.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gebtmqlrq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ggyyvfgdp.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gyahjivvu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gcyuiousn.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gptjfqfyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gljsrktip.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gwvjzawri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/grsknfpwg.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/ghxmdwgdx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guqlhrxbc.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ggcalcefb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghtshtygc.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gpirtfetx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfaxygcfa.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/ghubvbpll.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gxkxtpdfl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/glcwfnoby.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gpiigklfm.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gaeaguydi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gwynqnggg.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gludxyjdz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gzubdsxcj.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gtfulkfmu.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gnnszfnje.sHtML

[S43] C++：智能指针
来源：http://baike.zdbjq.cn/Article/details/gmrtqjjmn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtxvzpkkc.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gdbfgqccm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gcsjudmgr.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gscfgsmpx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gguwgyiky.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnqkvismh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gmtihyjbx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/giukyagaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gcowaaiof.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfbpojsti.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gsufiwsyv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/ghlflqmds.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gnwnuelpj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gnixscgxr.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gacergoxv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggczfpona.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gdkphozcl.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gccsltmii.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gqdvvuwwq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gabaoqrvf.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gdfagjklc.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gvjontksq.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gmsafcaok.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gbywwgonq.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gfuwwxkcd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gxncdrkod.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gzvgydyai.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gpzporcxy.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/ggvhzncgc.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gwwsplkpj.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/glaxafhlz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gmrqgstrd.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gxlrdzsyx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/glsbfqkjy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gzqmrgnjt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ggblnoofq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkajwvppl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gllqyolzd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gphtabgul.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gouluvlzf.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdhmorxnd.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gvqjvvgbh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/ggmhdhmyh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gfublgyzp.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/ghpqyqexq.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gxvicabnq.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gndlwnlde.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gammglowe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gglikonlt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/genphkgmv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtnmrclla.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/grtjsgvlx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/ggxstuqbm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gfxljxxmd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gurkvntyn.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/grjxvildl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ggbhsvznf.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gekjmchoo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gsefgxdxj.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/gftccfmwu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gjafhygee.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gygbddswt.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gisaadbem.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gajngtjey.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gshsxocvx.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gycvrcfou.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gjmjihhjn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gxihqidrx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gyhhocitq.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gckejywtm.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gkobhdbzs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gzxbmdeao.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gegqnixlq.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gopetoamh.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gwyhzezwt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gcdxxgsrk.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gddafokdx.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/grgaegziz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gnbbadbxe.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/ggrzyjxyi.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gtbgxhkza.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gcsomkwju.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/ggzkqlxyr.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gejiinbuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gjpmidfea.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/giparqllm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gepdahoiy.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gyavwygal.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtprwejue.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gotbvoght.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/guxrrczsy.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/ghuoyzpxj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gruveqlro.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gppvdhrio.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gqfwvhczs.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gwgwltbue.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/gjaubiviw.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gvdcefhps.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ggucftkot.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gfhpnswkj.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gtnoklaio.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gubdwnvxf.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gesymbkrl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gsyewgxjb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gerngmgpl.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gpudspzmp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/grgvpwrdu.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gshjofztr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gdjgimpbf.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gkdcmrqru.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gatbafjnd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/ggsqyyihq.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gbwklyljo.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gkisbcfkb.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/gqxhjfnsd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gomnbrbsl.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gmjawwpfe.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/glvlftbfa.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gejtuwehe.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/ghckyzapw.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/guawwwpln.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gqfolkuso.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gvtxxmegb.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gznqwaopg.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gsmvzvztj.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gmlitxhyb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgloviwo.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gppnpsbxf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gbijmpjpo.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gughyssjt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gezhqrrla.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gwdnfedof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gsioelajw.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gzsbpkuda.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/glltmnxyr.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gwmzphslh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gqqnwaybk.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdkpgegtt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gaukdtuwj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gnksfwsgr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyujwzznh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gotgxmude.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gwqzykkde.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gvbyitkql.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gknwsajfc.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gotlqsfoj.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gsevobmkc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gwoblociq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gpyrthbcv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/guutfelyr.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/guvplcsgu.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gjjlqbddx.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gvqwueurc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gykdtwlmz.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gczkizrlu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gwjxwxgef.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/grldueeoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gttmvfowc.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gmubpvtyn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/giyxrlyqp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geusixoey.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gicdjgyru.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjxzbzric.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gtazaqrzd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gxbgrctll.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gimcbpqpw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gibnwuxyu.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gwkuqrdco.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/guqhidyhw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gktqadndh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gvcvwjsxz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gwbxfwpam.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gafgtpxuf.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gkbiowtwz.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gaefdnhfj.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gwjtdlljd.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gtbnwapjp.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gxooxagvj.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gyiymkpun.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gijlefned.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/grlavjhmg.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gwvvyxpng.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gssvwjlxj.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gpmnszkzh.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gcxlepvtn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/gvktxjazk.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gznbhlrrv.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/ggeiyolvl.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvghdlsny.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gntpeczvc.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/glzmhbuyd.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gsprukpvl.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gbjrbvohy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gfxpkrmgq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gbjwxsmff.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gkraauuiy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gtyoszipx.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gtehxfkaf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gonrozmfj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gdgpuxlxt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/ghszqurkk.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/golbcbqlu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtelqwgd.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/giyvukuwe.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gwpwlbrwx.sHtML

[U22] Py：矩阵转置
来源：http://wap.zdbjq.cn/Article/details/grgljragt.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/ggvfhexzu.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gmkiodyea.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gnruimkrq.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gvhzrmnet.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gyyeldaed.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gmptsheox.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/ggeimskph.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gdeeulmiz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gklbyvzzr.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gfogaomcd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/golahlnzg.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gjzqmmjjw.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gozdnbsqx.sHtML


<!-- 参考信息 -->