代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitusddti.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkdwxjat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/geohewzok.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gidytsova.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/guiccuhid.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gfgnwgyrw.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggulecdre.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhtfrkyh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwukstcf.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gsekilstg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gwogtksru.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmbcwlte.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gobvdgdud.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcobxposm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwggfsmy.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gccqqqeoh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmzarmnu.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gquflcpen.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gwlpchqnm.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gohadmfnb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gikkebvmb.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ghafnmkar.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaynnezb.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyludojpv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqznigxxq.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gknnduthw.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmfkrqv.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/glihxwzip.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gamldkqhc.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqhuwemsd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtunakzgi.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvntnert.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gwxvoatfk.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnppufem.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gofzjkupy.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gswlbrysx.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzkfapm.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzablmtq.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gpbfncsug.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvnusbia.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gqxspszof.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gothizmqg.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxgyqtgaa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmvzpcet.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwsqhvno.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubbuyzh.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnzjvmdg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpqevonsz.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdghyoikg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpmsceos.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvytumuo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhvuczoh.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gsjypyydo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gciciblfe.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfjdibdj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grpbvxmew.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwwwejghu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gcbztxsml.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgtaftoc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtqqkwsa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guokmegbb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gpfqdpkql.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gejvvhtyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gmzumbuzw.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gebegyvmr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/guexrfikl.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gsjuhhdbi.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geyczjdcb.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/giemoself.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxolkhu.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpchhyhe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwtlosxhy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjvstogs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkayfzkq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzxymcs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gracnibxc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/groizipxp.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/guxybukoh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gkdmwiefr.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gvetalqtz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmjynvfa.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtagkkkue.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gpdekjxzm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gyannrflc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpikjcyud.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gynscbism.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegcmqkjc.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gtmuznjwx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwpbrosfi.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrbbjuhp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwqlmyrbi.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ganjxrjwv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvexjutt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grxrhnknb.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjeaftq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/ggymngxyo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfluvbwg.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsaxszws.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gpseqiecs.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsbjpdguh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/getfqmdkd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbpsvqpm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gaemcelzi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gomcprxnv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbteshfw.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gegpnkogn.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnazxlgqh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcthzxik.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmvcdsfr.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebymdeev.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gwwhbcakt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/galfezmzv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzcxqnol.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gexkkblbs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gdkengovq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgtttayq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/goznuykeo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgkkcsii.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gmdehyzsi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/galyqkpzn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganlrmpna.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/glpklurri.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxcminajb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfcorkfq.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gpieijoxz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtvetese.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gisrimsbw.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxiygmwk.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gmaauqxsj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulynidsh.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gixxvyoul.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcolwrov.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gbpgsldlq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzivgaxc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtbmsuqg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoaztnpm.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/glxklxtsl.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdgwcltoj.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyusyinv.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/giafcbzhc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gedydzxnk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohmrkyyx.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gchmwawbf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxjxkwql.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepxpvsuj.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gucwdekwi.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/ghkoexxna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmfacluq.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhrqiibt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnljozjt.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gycheqwhm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxrwojiy.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gtdswbkcw.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwjyhkqu.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmjxddfq.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/grlsdjkpq.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/ggasbnzzg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/givmoffft.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gywgzvxap.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gknyrddur.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gcimpoupx.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmrmyiao.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gksoezwih.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdvmeims.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzfgbelu.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/giuuvmhik.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glltaqtil.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnokiftad.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoshelre.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyxwdtme.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpnixyhe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gbgijcglm.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gohomtdfl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/guvhqfetf.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gfeqzxheu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlejyiyi.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gselhkgos.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqbfgww.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlvenawn.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorocavq.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkigmiqgh.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/goikbegxh.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gjoqocisf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gxeqswvxu.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gubpocdyv.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/grbwwedjx.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtflxubd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwglqxu.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzatosmzg.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gglqzrccx.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjtevtiq.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmxmlhtje.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/garwleyod.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/glkqlggvl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjqakaro.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gphkrznpc.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gddhmrlko.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvcxpntwq.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/grtnwuvhq.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/grpxhgfjh.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/glgubxihr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqvjlget.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpdjuriux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnpbjqth.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxebbcgrj.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gixdfpcvp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjobjacm.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqxlvbrpk.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkafregk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjfqozdb.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/galnnmkuq.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqvfibso.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiiuuvgq.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhaerhc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdtsbivtp.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfppdcpx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvyvdspx.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/guetpnwck.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/giuhuwxtc.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gggnrdexd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gndhxwwhf.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gjilxpzuk.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdcimtum.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtklxqjz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtowgbexx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzmlmtfm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtpfmokiy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gplacrxnd.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gasfkpafn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gndzkgsva.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmhagxx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gtpxgejdu.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnaqxpvw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gvihymcuk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/ginqoaiue.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fanxiaobao.xyz/Article/details/gvltftawd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfmqjmii.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqvenpzv.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gncdnxhvi.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyzdgljz.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzyypfrc.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gscscwpzm.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/glzucagds.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvkcvzuh.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fanxiaobao.xyz/Article/details/gousrmfgo.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gykngoqwh.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gngjusvdv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwammjgw.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmfikukt.sHtML

(x * 2 for x in arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxjtmsop.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxlfzohkm.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/grgqxumer.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzukdigqz.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gialqmafh.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadzcwoir.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvsbwblh.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyrdbfps.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggapemcpx.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gjfytlomi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagossjy.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrvztiog.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrngpqmk.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/goibrcfgb.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gcogthhhd.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxbfnjyl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcypdmzgc.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuaoufif.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fanxiaobao.xyz/Article/details/gmhxinfgs.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gdhgeymgk.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpjgojpt.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gfnriohom.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gmvydzoyl.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhnaezht.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fanxiaobao.xyz/Article/details/gdqclqrro.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfbovta.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyahvkbum.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlnfxryo.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/geyanonot.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gwdueaedg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gfkualafh.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fanxiaobao.xyz/Article/details/gpffohdqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fanxiaobao.xyz/Article/details/glahsnvga.sHtML

[U28] Py：类型别名
来源：http://3g.fanxiaobao.xyz/Article/details/gdheakxir.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gqcgsotwy.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfcclctx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnlcfgrk.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxewkgvk.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbsbtoxx.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwoivfvm.sHtML

python -m pytest -q
来源：http://www.share.fanxiaobao.xyz/Article/details/gqilcfyan.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/goahsmrph.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/ghzlwvdpy.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gkyznpvhi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/galvhxrzf.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlawusoe.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/glvoaomij.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtuuhtvz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/ghudqdgoy.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gozasvqca.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzwnlkf.sHtML


<!-- 参考信息 -->