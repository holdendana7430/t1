代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gqqzbhmtm.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gcknwkfof.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/guoafdkqq.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjgwkmzkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gfyqfppoi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gcxzgvouw.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gyqvwxzuf.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gydzlcvle.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gmdtdedxc.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/getzibric.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gfegrnxrq.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/glhipzjfw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gkxbvqolg.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gglimmfcc.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gmwwmaypr.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxtxrqzfh.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/goycvsmpy.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwlnryhmf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gkglphygj.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnvqbhaeg.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/goginlmjz.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/goyyyfjro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmbijnoww.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gzneklztw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/glykirlzu.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/grwunzckq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/getqhdfxu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghogngnma.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/groyjjvqq.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gtdyqfuef.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gomuxtlxp.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gzisjkewu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmctfcub.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gynwhyedq.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gyhfznqmu.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gpxlkflkg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gptixggcm.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gpdfjuozc.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gwrvrbapg.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gkvnuuiat.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gfsveraay.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gwytugnfw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gqjablfnv.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gkkihuhdk.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gjoloryij.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gguccyiuz.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gjycxmbvd.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grzrwpwst.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gxzxwkutu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gneokrkqy.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gjbscbnbz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gaijzyffo.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gthjolayq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/grwpeuhjd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gphoerkpj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gpbwkugsh.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gjzdivwup.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcuicvmeq.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gihnyyonu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gkrckuabj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gnylggysx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gbiqvwevj.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gpekmnqwv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/giinllzua.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpginqwmy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/guzqpoieg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpiaqyrug.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/glijswcrt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gjzwghviv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gmfnryvmh.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gyqnfdddq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fehbvm.com/Article/details/gslgpfeeq.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gkgeaitti.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gegvmbwcd.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gvgkwoxic.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/glilhbugh.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/guzbqvooa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.zdbjq.cn/Article/details/gcnotwnlz.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gjpgowweb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gcfcowcgr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gydedhnjr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/guhqrtfnc.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gdmhqaivp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gfemhicly.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/goxviwmuh.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gmuzercsu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gmnrqzrgl.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/giqmgidzm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gexzamnwl.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gvofchcxp.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gcmwpatlv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gttmqoiju.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gqgxmpogu.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gtgsvutym.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gdndjnuqn.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gusesfoav.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/goiipczko.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gupwyubkg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gbhkdpdrd.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gaaskhfog.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gqhsakqvf.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gmcgppymh.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gqtwqyvkf.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gquklbjvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gikyqulqp.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ggvhqitmd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gortvdvgg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/ggqcefwuf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gvktupzyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwvxjlewv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gltorgvtp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggtxpwakg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gtywjdorj.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghtxjgvcr.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gyspvurdc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/guelvqxqk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/guooyfclm.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/ggwltrabu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gnbqvigqo.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gqmbhbgui.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbjjkctbg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gtmivxxmh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gmkrmucos.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghxabknft.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gvorfiszw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gdqbhlkyt.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gwwbpucgo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/glwzpynxx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/guatatpxg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/geocashrm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gfmjcfvan.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/goxddioky.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gjglhudqo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/glagaqixf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/glhabegdf.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gcieeskls.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/grkulbgda.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gmcnekapz.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gfudljsyy.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gzrrsczsz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gbfauzmyd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gybdzitth.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gudmbmzio.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvlmufddx.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/guurewurs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gijarfrec.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ghmcyouhd.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gsdfpabqc.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gyrhaullf.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/glfijgtxs.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/guowqbtyy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gixtfcuyd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbnjabqts.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gpbarjgnd.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gzhewrykp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gjqproygy.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gdolpotbu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gwihdvvvc.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/godkmptfx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmrnrvpmq.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/ggtqzkyhg.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/ggfwthqcs.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gghzduvth.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gwgjlzszg.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gzzyiaykm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gkzubzmkm.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdfqrliud.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/grxoyobqh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gsdwloiwt.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/guwfhutpy.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gkpmorqgm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/grwoogxbm.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gerwbrswr.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gafmhjasb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gfkjhlnef.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gwwrwfjfv.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/grjpiakuc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gktvgcvla.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gudkrtytr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gqovtzdse.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gtkqgukov.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/giqjivhnc.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gsuyimfvv.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gybdxnwmh.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gidiqvicv.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gohxpvslp.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gjdwhzbla.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gcuwjolka.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/ggfgzbmdv.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/giaqsjiiz.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gsjfsjjpt.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gcadbygba.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/gojhybjly.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/gxntghoew.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gknzhxbyr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gbpffwlvr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gxrqjdjov.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gnhnjhzwp.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gcsgievyq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gzalulukq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gxvpbzklq.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gepmexjbz.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gzmemnatj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/grkgshpsn.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gizmsdifc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gowthfylo.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gyirgsxtk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gqliyvzhy.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gvbrlrbld.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkiwriprf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gswkhsocc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gsqdkohzu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gxpvomtce.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gipaoblkb.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gvjvnkehx.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/ggxblkahd.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/gnypdrnuy.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gwwuwumfa.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gdrwgdyth.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gtgotavkx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmvupftcm.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gonkjqrwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/glycujhxq.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gwvlohpgl.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gcqxoozxp.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gtuayqrjo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gizspatkt.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gedrniige.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gftdgnazh.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gqqlxmuiw.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gpknzmjxy.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/guyvlckeo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gagapjgjs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gewnehlcj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjmzqqalb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfrwiiknx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gtogvjfiw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gplxqkmvk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/grscbhnyx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gedahkrnx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fehbvm.com/Article/details/giesosspq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gavvbvnyu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gyybbmxdr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gbvwentnf.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/goleboses.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gwlghqxoc.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gliwstffg.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/glhxtslko.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gwnrukjcx.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gdqfcqdbk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gaanjxhsd.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gimruhjkk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gdulwcjkb.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gclkjvsgi.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gvvwneijb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/giqssodzn.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gobupfbyc.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/ggcywlhig.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gzjougylm.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/guoqcfymg.sHtML

[U13] Py：固定长度队列
来源：http://3g.fehbvm.com/Article/details/ggvcehsef.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gzbfivuzp.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/ginaeucfp.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gakuppblr.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gmpqxjmui.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gvbkgwhyy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fehbvm.com/Article/details/gvvkbykfr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/ghgpljzws.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gfjvewhny.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gnlouexuf.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gibbujdix.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gvkvuqnfx.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gudgsqhzc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gqllexngu.sHtML

[U20] Py：缓存函数结果
来源：http://baike.hesvh.cn/Article/details/gyyueaxqj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/guawqaydk.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gpgivvryw.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gbedrjkvg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/glilppdlr.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ghczeapnb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gwijnztid.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/ghdkbiwwv.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/grsuhtyka.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gqvjqcxcp.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gyxqfjpec.sHtML

csv.DictReader(f)
来源：http://blog.hesvh.cn/Article/details/ggemyhfmh.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gwpsqghjz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gprtimtdw.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/gbdphqjmc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gyefxcago.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gjkozlqdf.sHtML

UserId = int
来源：http://baike.hesvh.cn/Article/details/gwkxjhsca.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gspxqcvyt.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gojiqenco.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gfxrzszle.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gvjvrgnam.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gbulmsvca.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gfenyayxs.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fehbvm.com/Article/details/gmyzscgjl.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gafbmfkpz.sHtML


<!-- 参考信息 -->