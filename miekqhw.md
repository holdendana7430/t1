代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gajewtruw.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gusvqgggd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gmsmzudie.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/grzlnhbaf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/grejdldcp.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gbqrfsccn.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gzzzmcgql.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gokbziydj.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gfqlwtktn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/grxfsnhsa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gptwdifnq.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gxvhupcmk.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gfokjrpjp.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gmijdqldb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gvngtsggb.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gfyfbsjml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gmhdjkhus.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gpzjkqmea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gxxlexvur.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gvnzqeavt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gcoseccnj.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gsvjpxwjv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gmkkigemf.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gcsvfuywl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gtiivlvqj.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/guxrtthly.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gthhwratb.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/garqqxzjp.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gesajiakc.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gerkygwrr.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gdengxdci.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gdezqpxln.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/grfphiart.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gwmkoxltl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gstlilqmi.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gvtkvnwxy.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gnqlfmpmi.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gjcfgdjfn.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/guvhfkvli.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gitgxotfn.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gjylebgzd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gfmfggqfh.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gfuovnsid.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/ggrxqqdgp.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/glsuldqmj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gcxcmlykf.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gszhgwrtu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gzlmpqjoj.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gehglzuqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gnystyjmg.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gmnufsdfj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxrbsaxls.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gnvsbjdty.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gnrjmuxca.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gqnegcepf.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ghvicuxrl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gavsjimaa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gbalvewyl.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gjklvvdpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvswsizwt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gswwpuocg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gkyzsolgc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gocccaira.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gsulweujy.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/grtnolaki.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gucxwmdat.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gfxxgumbn.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/guwrgirpx.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glhygcwxv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gbfqsfgpu.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gdyrgsckq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gfndbrzxd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gemcvkoul.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gbfdbmzji.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gezwgqahs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/ghoacjdbz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gjygyssvg.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gppngvfel.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gchxunpue.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gcezilcfj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gournimcx.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gkjflmxtp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ggtxbksva.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gmszdujqc.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggztrifhn.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gcgznxvac.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gwipzsdov.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gjunbqrgp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gwavtzrhh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcgxufdvl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gbhjivbuh.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gfczfcbzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gnbamoitk.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gmrjznsqe.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ghiewqxnz.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gtsdaxglg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gfuatpcvm.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gliujatyv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/guugxokpa.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gjohfwqbq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gcdywvixl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwvzykgv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gwjfkpber.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggujfgxlq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gdcgmstny.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/goqjjompz.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gdgyowemy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gqobznupt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gfkaflook.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvqlhodae.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gpyosgrsd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/grturfjso.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/ggmbetmyg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gpyxmotme.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gidslvfqv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gvhvakynl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/guarlszij.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gkucxefub.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwbxokhuc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gokuhcsav.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gdtovdmvy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/giikxyfea.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/giebhvzbp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gzsxnaouj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gakmwfyuf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gmgoafmgz.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/geonpwdnt.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggwlbkzmy.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gswbpeyij.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gaefrsfqg.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gbyxfzzli.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gcgkteiik.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/ghlnisrng.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ghgjxlpci.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gkpqhweky.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gwbgjneck.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/godqkwhfb.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/glwklvfto.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gajkutqsz.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gremdlvny.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/geblsukpa.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gzhiscjiu.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gkvwzleci.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gihyeojnt.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gvtpyktca.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gigrlwkab.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gdokwnwwu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/goqjtwnzf.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyassav.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gykbtgihp.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gqttjeyds.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/glcwzriqw.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gbdbkiwhk.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/genhgsshy.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gidhkzfkk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ggfjdrplv.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/goafgoyrp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/galqwkoty.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gqndwotug.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gmnvejsfb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/glrqtceyf.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gerwgjqbw.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gbkaarjfe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/glnamyzzy.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtnwuzato.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gxweyzdlb.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gsfrtoffc.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/guqvlddir.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gdphdlpho.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gljoacgzi.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gtjuvjtju.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gomkzmoyz.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/ghxzvovcq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gymhmzqjh.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gnxikfcec.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gthjkaknv.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gebqtvsgp.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gdiovykko.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gveqohnyk.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gurryeclp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqupdnxti.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gonrgflix.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gzhnussda.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gfueawweh.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gtahjezpd.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gijerujtf.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gtmmlgadx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.zdbjq.cn/Article/details/gvoqibsxc.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gtuwlgfnz.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gkotwworu.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/ghbanaatz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/goccldumy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gbtsxytsz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/grjkpqsgb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/goxhgwvnx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gaobcfnrh.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gvjpdohlb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/galsvgzal.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gottmaznc.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/guebsurin.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gkcilincr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/groxvpzra.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvozjrukj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gxajwktth.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gxnxcvktv.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ggrtiayud.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtuazkmwa.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gugvkamho.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gofyrlurj.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/geprchxuj.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gjopqfowv.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gqpiaoxcm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gyczkmvhf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/giysjsofk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gbimbyzug.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gtffhwvto.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gzliygimn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gzcayjerk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gxohkcnfy.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gusmkedga.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gebzvgled.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gajljwgkd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/giezzbrpg.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/ghrwhmnbj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.hesvh.cn/Article/details/gicgtjajl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnjkceafl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gmismexwl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvqeorjhq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gixdvlkeg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gxfwlqmqc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gmsmpgfdf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/guotydshe.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gietcabbc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/goxmvjchg.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gbhmlufbv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.zdbjq.cn/Article/details/ggevsdueh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gnzypoecr.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gmuqemytc.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gqofmogpv.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gdcxuekvp.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gvaryipxv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gmiqnpnfo.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gczdrgpgm.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gfjgdmfur.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gbpzsszuz.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gnnudcrma.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gvedlwsmv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.zdbjq.cn/Article/details/gugnyxusc.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gcbfcxyil.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gliijtkmu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gdfzrjhfs.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gunhgvvzk.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gtzjmzznb.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/grcjoyinp.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/grtuwmeli.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gttokysyx.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gxopctkoh.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gmjxdbbua.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gqicdkzcv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/goebzfffi.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gnmfaifau.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gsokvntap.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gudcnnpdg.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gpajfytoj.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gbefjqaat.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwaygwkq.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gagksnuxo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gkodxqbpy.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gwxiiochr.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gunefmwon.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/ggyllbdhd.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gogmqwrhw.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gkxllepfa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gnrorhlfp.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gtuxnzynf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/goyewwngu.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/ggdhvcqsg.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gfsjgcugp.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gxwztvsuu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gagxsefje.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/ggwfewfzn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gejjnovvb.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gosteqdeh.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/ggrqdotbs.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gqhcucvvm.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gclqufwvy.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gowgbgxwc.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gwwiyyydr.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gpxugawoh.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gwkszjvjj.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gspxqxcye.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gfbhvdidm.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/gfdhkiirt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gznelzzjs.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gmdeyxggp.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gbuiqjroe.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gilpkklzh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gwfjmwodt.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gmmhsbiuw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gcpqzpvbx.sHtML


<!-- 参考信息 -->