代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gjmzutaqn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhgtghmq.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzlmkion.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxksmevzt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gqaathfoc.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gddmquytb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gngurjqfa.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/grltbnkge.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gibxxubin.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlybqjdr.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/glwxbzkla.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxernjzu.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozgpdbxh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoyyijxk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmonbcsrb.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjozwjhda.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfsvbkjj.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaxkbmwo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvlythwa.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/grrhxxpjj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gtznhyrse.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gernbbhvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkemefdjr.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/grbyhcqrr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpofusqtv.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpauvsqcq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gihdezfiz.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzemqiwe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmptinox.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvkxmyy.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gpajpktbm.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gazydyolx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvfzppgw.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ghcskmyeh.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavypkrb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gifzxecrm.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdzkcvh.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfjepsmfp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/grssbanxp.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gklmerqhf.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaywraih.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gamjudqpy.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrfazwkq.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqvwckg.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpblnzivi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxlsnoi.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gxjtyrjbb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnetskwqq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhooydlq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gevdgfcrp.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/ggxefrpar.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gadrrrykb.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjquolie.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrjmnpa.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gqmfvfslg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpjpprkk.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjzmtfkj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuwnwepw.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcqheohda.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyomfhfw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gueufmdcf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gmgvixgki.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbokmitjv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gntoontih.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmjjdjkq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/ggkgbujvm.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmcdvyj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxcumcph.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsriyjbx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyzavmgi.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigkknoz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkgkppfb.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gaodwopqh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfoipjlu.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givrgyafb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grqxxcqhw.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gyomkjccb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtzbqspqa.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtkpwllqq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqynfrgly.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdfyrwkn.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gotusucat.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmenwtpp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluftezgq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghexjbkrx.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/ggiltcklq.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqxrfxne.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrqcgetw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxrzzltsw.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/goounsxha.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbnyiadt.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/giwlcrcpo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpyenrad.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgughexg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gxjmtbutz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/goakmvtww.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvzbcjcq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwwzoatc.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gccqfbgzd.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/ghgwtbmee.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfinumfc.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyeaazpa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjxqyina.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmolrgdoq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gkadoatzi.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjdcifyda.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtndrzq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpptzdhaz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gmhsqbwwi.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/geobmzzig.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzgcclra.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsnulvtq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gfycicufz.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrpibivh.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gndfqdtlh.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grxctfjqw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gyptthzwv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrwpoany.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govbdewke.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahcleax.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gdffsneat.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjwhuqlip.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gloluikux.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkusytave.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gatalzxjh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gouahqllb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxjgbchy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyufwplbh.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwvmxpb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/griahwakr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfuxhkth.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvbmvuhek.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgajbatw.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwgfczmb.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiohcnwq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrjnxliw.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgietvad.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnussxkad.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtdymerpt.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gwxdefdgo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhrwbcyf.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gqmoyhopk.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gtspokekc.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannydkqa.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gftmogknw.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxwbfwqn.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gexhihoqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gvopvrwgl.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqerxuwj.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gctomdqao.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gzouqojri.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gzumjcxbn.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjssrfuoe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/geittarvm.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gywhlxlcg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkknbdnu.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjypvvwa.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/ggphjvadw.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gvdjfrkrq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmwptft.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/geuaasbqw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gxrqgnbbr.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/goyoqrljy.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkbnahlp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaihxlsan.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gchlzstps.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gktqnfhsj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gftefdeax.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdblbbhl.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwiwcjft.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwcbndqb.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gaytofxpo.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gxreqtavi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrjpebgt.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gqowhwzni.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvckpqkl.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gasvmavig.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gemfdgpjc.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvsyvhtm.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvujsjhly.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcwcgxog.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqcwdwgu.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvceufwdn.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiskdudc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glpiguxzt.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gdfjaibui.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gehgheofe.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdjoczk.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gupqdtpck.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdiztsdo.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyvqmain.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gbfmmvqar.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvtjcmvuw.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmrgbsan.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlxbrscq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqfixnmc.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/glpmohncc.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gryftqqso.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gvneezvhp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllxnhaw.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gitxhyjab.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbmgcsdpj.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvfynyss.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejzbovd.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gopxequyd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbylswag.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxyglnrgu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmetihnuc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoqajkoe.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvovtravu.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goniomfrj.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gddhjagch.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvjceklxy.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcrrpnda.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gkswlmjcr.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gvomgvhwl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/glpqhnpxy.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzjrmjld.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gesytwuvg.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/goefflvom.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxfzijk.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytwygrem.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvslbdjay.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gvlqspnun.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gjclgnbrc.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/guezshxqy.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/giyqlypen.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecfildwc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxnkjxr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbhmpazkb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggznnhsvg.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrfxypdo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwctrmbj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gzrosuihd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwaodbi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxbqzbkh.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhojlbdr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmlspdmi.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfvecuo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gsgrjmwtf.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxfvbifq.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gdscmpyud.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gedwjqfqo.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmudvwqbf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzfbettc.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxfqpyw.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/ggikxpnan.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gblwujhse.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwyyxfx.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgcgnjaa.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuppupdt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/goyutwavt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrtpyvoh.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gphlixepi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gndespmnv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmkskqao.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gdqkwcnvb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcmdehe.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gdonxuftj.sHtML

defaultdict(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnjpsmqv.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gewfjuhsi.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaozitvq.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpacwzrxj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gtjnhggbt.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibinbadb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/gtsqdzmra.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gbnfacykl.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gvvarceyr.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/gthxzlzut.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gogsjmdtr.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/guqsdjyls.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/giyhkrrca.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqbysttr.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gybpapihl.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvlyyuyb.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswfsaeaq.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fanxiaobao.xyz/Article/details/geechctsh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqoodjjc.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfkdwkgy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gakmwmfox.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/ghiklszri.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gtgcypqij.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqtdexjr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnmgthiv.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/guweannmz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvbnzue.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/goyxmijft.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsxiasv.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/gbxuoerdy.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gimeqkzjd.sHtML

[U30] Py：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpstyvhgo.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gifexslal.sHtML

[U31] Py：单测
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvycgufp.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgzgqszq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkwsrelc.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisxbldep.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggflxikzb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/glffekvfm.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gynhayjgo.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxwyjsp.sHtML


<!-- 参考信息 -->