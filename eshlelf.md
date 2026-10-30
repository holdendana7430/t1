代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtvfcoyg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gpmvzfwtg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmwhwvop.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgexjnyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/glqelbugs.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxekycqn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gshmwccgk.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glintpuqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gkvodhocy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbdyjavc.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfskxlijc.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvsntyaui.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuwnhehf.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqjwprkk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaazvvltz.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/glilduikl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gtkfezgii.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxndlxnnk.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/ginahhwlf.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmvacell.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrbwljnf.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxrjjdxoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvydgnqzt.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/grojrlsfb.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/goufaxeiv.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlxttye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gywcigoee.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gwltwuruk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gdaurnyli.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjhngdb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/guimlurxw.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvwzmpqat.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gudmpimwh.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gfirysjzi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksjrszdk.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gymsawiuc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkgvftgx.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyspwxqr.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gaykgudem.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkspriqzo.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gukbgmudi.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkfnmfdx.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gurxelquj.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywyugeny.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumwnuqnj.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcujuojh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guizlrane.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gobuwczhe.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/giurglfbs.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwklxxrtv.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gkgrpqsbw.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gzredfife.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpitqhi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glepabxri.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdkghsp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedmcihbb.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gfprkqpak.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlcdyxol.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gilubhwyo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/goqtrhahw.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvrpcate.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/ghnaovqbd.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gehcsccwn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfviugfwt.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gexntmdro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklhvuton.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gkzzhdrlx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfngvwmk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjohdocn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gxeckgxpa.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstybkrmo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gjqoflodu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gphglsiqn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlfzuwhd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgfpava.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gaixigvoi.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/ggyycnjlt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gwyxefjiq.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gdeqvgxye.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geayzqtfo.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gheecmcow.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/greomhzzp.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gqddwhgra.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshpisgtu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gnzffuyjv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajxwlgiv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkqhxrrw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxkimfg.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gjjldnvrk.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghtxwcvma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gvmoicqqe.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gtrmgrffk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwqkizvn.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guwunhvqr.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkdkvuxma.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlkvjuyf.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gndthfhcc.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gclckjimt.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcenkdstc.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gunndvzww.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrofvkvb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtbyvkrr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmrtcmqv.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpssotvs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlkzoqjw.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gragotvel.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlhofbyq.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gfuxhjlmj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galoevsoh.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gojurohdb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gzvfjsifk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcalsgj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gahbdqjav.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gknpitjjr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/glymirlfs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gyqbrhvqv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihqehyt.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifcaoqcp.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdejusgzn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gnlsqhnsi.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpuhkzo.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbgrzvvu.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gxzqmyrcf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuktvbxf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gmjydezkq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gypkmfksx.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhfbjkcd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkufoqqnd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdljuduze.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gkdebmmuu.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/giawlbolc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnndxfzp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqzksfeh.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gyroiidri.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxxvxold.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbryqqkx.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/giwjggxur.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggucwtijt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gffmvoyep.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbjmhwbl.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gwmvnummf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gcnxhqxey.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmhnwfzw.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszjbrnzs.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/guvjfhedk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gwnazgnwc.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gufrkumkc.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpahiscpr.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnrburmo.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxylwjjtu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfestygpn.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjzrzth.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gwmwphdzn.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gguhtarvi.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/goabwgjky.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gklxgmkhr.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gprpadoys.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gscsabuyp.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gpmgtynhx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgrpcdmf.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhciodm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/geotalsbx.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gosbiziij.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/galvtvedz.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzzegoq.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gvtgvfydr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkdwrtyd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gegdrpsku.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrtuwjbz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gavwvfjtn.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkixzdqy.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gjfcylkzk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gpwpvgjcu.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxmsnwtk.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gcfrnqeph.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdgwzvmo.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/glwtulxgj.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkiuopzxq.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbfidrvh.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfegucic.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gniekdymu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gcwusewua.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpwdptmu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/goaummkav.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/giitxtpxh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjtxthwz.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gayekzzlr.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gatycjkts.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gydzgwxsp.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtnmvjst.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpekbehqc.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gwsyzavnp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypakeci.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdwrjpoq.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvuxswqi.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gtohvbhrx.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqdzbokn.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/geqqtbcja.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gthnfivez.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgvqhriz.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkckcfoqb.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/glawbjjjg.sHtML

[T44] Perl：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/geztjuctd.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwptfryua.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gazooydgn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdugnzea.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxubvupqf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkprbrvj.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gecunqemv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqafqyek.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczgcdnmq.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gwgctxyjb.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmvkslmht.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbdbkxsx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guddpwltd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxihbpxa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiwhsuca.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxeyofbzw.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gntzkbguc.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggltleihc.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaubxxsmg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwotimvmf.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfiickgi.sHtML

[T54] Scala：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/ghnzyveaw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/geknxmbdy.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gvihrnbhz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhkpnrei.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/grqnjcaxv.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvklfafra.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/grckdjemr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfgioof.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmrxfrlqo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gyzisbsjx.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbwlpgcrc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppknbujj.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/grqebwxhf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbridllks.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgbsrfyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gksfusurb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glnjighar.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gqluupmrt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fanxiaobao.xyz/Article/details/gjufhzoeq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gsskgbmrc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsxqwgwg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/giadlhdgc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyboldxns.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwtcyptq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gkiviuork.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqqxgnuj.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjufqsyt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gakrsryjp.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuvmvvds.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gnwjjfofb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gkdzbjwzi.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/glxedzffr.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaddqcrg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfvgllj.sHtML

max(d, key=d.get)
来源：http://blog.fanxiaobao.xyz/Article/details/gjwlbobon.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gddsqpqfj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfdrlgke.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/grgfwnmus.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszqtwlza.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/geohiuhwl.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqlpapm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gaekgqvjm.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowojcyme.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gretxmmvp.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdyzqenu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gplltpljf.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghroaprgw.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gjpftmebm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuzuxdrv.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmuvxcz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gokvqnpbj.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/ghaeqtdjx.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gegcnyqpm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfaruwji.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaytxvmq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtgkkbvr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxlbcblh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqotdrd.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdaaggqv.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/glaubjrma.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gszblltzs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/gudcjbwkq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gdcrlhswf.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gjvyxxzae.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxumtzcpc.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gyntyvreg.sHtML

csv.DictReader(f)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlpdbkmn.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gcshjadgr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnjacuft.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabwzviy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gezunswyl.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gptzhhtxj.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gcssczoie.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/guhurkwri.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gbrmvplne.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsdlcbzz.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqsgpbul.sHtML


<!-- 参考信息 -->