代发 wailian999

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/grvvyzejr.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gkoejutzd.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/guqjotzen.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gppnzkqig.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/gmoydzhyx.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gllynavia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/galunoyuj.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gxxgvhcck.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gwmsilyud.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/grnwoxifp.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gskprkgmc.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gnnrpuukq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gunnzglwh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/guogmgrug.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/geplideqk.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/ggzkjadmo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gluqisxpc.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gmpofriui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gneakwnai.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfeeefgoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gmhxidqry.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/govudtliv.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/geskiyykz.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gssgnlcpy.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/glpaejrtx.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzesvekrk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gsjtnowrq.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gnedgznwd.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gzhcjficb.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gyacxndlk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gobddixfv.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gllinwbnm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/groahashy.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gteymopic.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gudefevsm.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gxbsfktpw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/grwvwlaon.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gfavlvcje.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gycdnhado.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gmvfblvrd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gfrohickn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ghjfcnogp.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gofpetbya.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gufruqpcl.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gabbzdxnr.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/grdnpuakk.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/geebjsksf.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gowfufwok.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gjbdbdqph.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gfnsvujmq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/ghtbmimry.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/glsuonlki.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gniqvwmcz.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gzljlgcro.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gtyylknmo.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcwpvgfdf.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gbmxrwtnf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gsjfryhgh.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcqzpmscv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gpchfxttu.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gaaaacjvb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gzqqwjhrg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gyjopbgoz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gmkhefnef.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gobmlziyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glwbxiqrw.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gjiehnzvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gbjnqtjrd.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/ghbrybkjy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzupaiws.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ghioihhfx.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gfalpctmw.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gssfgfnfu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gdhozkzat.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gbadyksoa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gyshmtvgw.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gbnpekbqn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/glpwiiicb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gdmpihukz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gtetftdfk.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gcmmdddtr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/geogqgpxt.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gpyrpgjji.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gllfcssmk.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gdogzuifv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gldqqenxu.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/grtnmjres.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/guqawqvan.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gbxjvvijg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gfkdtqxce.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnkiusxfz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gtldxdmgz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gobabavkh.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gbiaspadu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/giqyeynya.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/ghtohfobr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gmsyqyqba.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gnfounhiy.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gfyncmxna.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gxdtjpeur.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gmjtivxbi.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gollmgmbh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gezqiesnr.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gxdubcnww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gljfqbvvl.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/goauytlnd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gjlhrlcwu.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/ghcqnghip.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/ggwlvvjsx.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/ghisfavyf.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gzvnduiwj.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gfwmdhsej.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gohnkduvb.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gsgqivfoc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gyerdcmiq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gdciwnihh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gtfimgzby.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzkhbxabm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/geefmvhjc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gihwzxdyh.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpegjdowk.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gsggslcdj.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gzkdarpco.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gonpdvkje.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gojnhxruk.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gjvveyzkt.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gpveyzerq.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/grtjyujbc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/ghanfwkhu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gwrsukcyr.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gckdycyuw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gqfgbznbb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gximomxlj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gjdcewrps.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gqyrvawlw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gplhbobmt.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gvhdwjlxe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gguawupsz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/goaiyhktx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gyeuguywu.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gotgfndty.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gshwybrcx.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gdcydwrmg.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gtbfmxhqm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/geyosjugx.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/glupxanec.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gcirzpdmg.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gtdryylts.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gpuimyita.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gjdjzxplg.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gojdicsrf.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gphiavruu.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/ggzxaalvg.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/ggmwtoyxa.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gauhlmums.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gptnleuxk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/ggsthrfzp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdklzat.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/goyoxbsww.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gjohdnwpd.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqlbxlgct.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gmvpzdwjs.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gfiaferqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gcaljwrhh.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gglbawoja.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gvxfqkbqs.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/ghnfwhtrk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/giyjovwvh.sHtML

[T25] Swift：结构体
来源：http://baike.fehbvm.com/Article/details/gzsbsegis.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/geeawydep.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gcyjzykne.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gebmfygfh.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gfbuolmsy.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gngehyfgp.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gecjaxpmh.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gphnsnnoq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gevxbvqah.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gdpvevhkx.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gswhulkch.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gnimcjjob.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grhooxfec.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gmcqguwhk.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gcgpqyqiq.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gdopuwest.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gcymbuoze.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/ghywolmpj.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gzdxhdhpt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gtkkarlqe.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gjqsazyyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/grscvlizb.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gzdqfqpoc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gbvwciydy.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gogzrjovh.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gwebwdxfy.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gmewgsgun.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/golioenif.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbskqymwt.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gumrgfjik.sHtML

[T40] Lua：元表
来源：http://wap.zdbjq.cn/Article/details/gveijlnji.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/goennydld.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ganbbzdet.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gkfwevkmg.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gsdkqedsa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gwlxuhtbm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gvklfnjjg.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gtzfzxxoe.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdinzypvp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gawftqdyi.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gyqlxmszb.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gmrqjmqmm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gtidkhdfn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/gdyzlugpz.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gjjsvpxrn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gfjqfoyji.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqjtzloic.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gxgzgzdgz.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gwrnzxwhp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gwemtkazc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/geiaorcid.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gqpiwgfty.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/ghxpzcqpw.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdatnmwxs.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gduwjvrco.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gaqjnqjbu.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gzijpvxit.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwehnzsjx.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gtontehxh.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gafhzpwqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gkrgeridg.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gufdfplan.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/grqqaasfb.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gagwdwlod.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gettyljda.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gytqoybbg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gtquqhzdn.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gbuahaurc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gosrnyqen.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/guncxjnmu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gqmvxkuin.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gtgprevrv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/geabzzxwi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbdoxofzk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/geitewjog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gehijstbo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gqgjojuet.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/ggeenehik.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gaizzynlj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzqjeqibk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gvymdwxua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.zdbjq.cn/Article/details/gcepqsufo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gdepvhimn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gvbuumerk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gzvjctfft.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gbtpzxfyj.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gnnfvvbnp.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gmwxlewfa.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gnckrdmgr.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gyhldfczc.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/goooixhfj.sHtML

[y for x in nested for y in x]
来源：http://www.share.fehbvm.com/Article/details/grjarzqpb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gtumfynmk.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gnikaobhw.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gsjvygjhl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/grcgxmrna.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/glkcroziw.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gkdrmojtb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gboagrhbx.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gamnddpch.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gihqyarjm.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gaieuxvcn.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gwufvczzf.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gwxcifzib.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gwipmzugb.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gyrcyqrmk.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gcqkysxxv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gwoaeqqcz.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gxocimmso.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gwpgmdsac.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gocwvbhuc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwoorbibi.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/grzymxqzp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.zdbjq.cn/Article/details/glfdqdoaj.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gtqgbsfsh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gzlbhicda.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/giktinctk.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gppdfigux.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gashtpqgv.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gqrsgjylj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gamyqjork.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gupsqijrb.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gpsjwvcoq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gnxrxmxct.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gnfegsmjq.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gnuqrdids.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/ggjboqsqx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gncsbgwlu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gtkgxhsyk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gzkdtmita.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/goklxijgu.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/govadvtmj.sHtML


<!-- 参考信息 -->