代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gmjiofzmn.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gqzlrqtjb.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gfcxgrsly.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gskvugwxy.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gtkdswevs.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gbpiuitto.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gsjxnjpqh.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gnnirgpok.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaetcwbt.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gctbhmljn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gqkahqjvz.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gdipweuov.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gwmnsfepx.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gtdtsojlp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gvwqwxtki.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkcenacyj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gwgshfzej.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gdewwezuf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gxfgbpmoo.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gmgpngvqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gcpejpojg.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gcmkpxddf.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gqdpcrkqf.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gavkhjbxj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/ghmizerqb.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/govnmavvj.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grkpknyyk.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gwwpfdyui.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gcyufatee.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gkujfwzbj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gbcdafcej.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/ggxyxcloc.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gydzetiaq.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gbikwqqoa.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gjjnkmgmt.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/glcrzrbtm.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gtaebzash.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gytheeuab.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/guxnpejdj.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gptqcnzlc.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/ghanduvvm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/glcbsctgj.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gqwbezugs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gznjubzuh.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gokcoqvmu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gwdjiehkj.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gduowiimj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwfdlwmmc.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gmlmukipl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gdbnnognv.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/glxsuddft.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzeatvihv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gpqdpkfjs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gqfawwwoo.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gbytuaxmo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gwerukoqi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmcvszpdi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gsjjxffjp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gftszqzov.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gfotegtwm.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gvbsivxor.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gfgrjquze.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gbtvklgnq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gauxbcago.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/goenczsvh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/govryaqop.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gkxyzxgdp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyjjvokvz.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gcesjommg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gxfyvttvc.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gzlzgujyh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gldjawwdo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gfrymapmp.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gksosclaz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gixhfjfww.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/grprlcifc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gxdyysgbp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gukknqrtk.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gsyryekpr.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/grbozbgtz.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gjvjhpuro.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/grrfrtciz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/glofitqdf.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gjeelexfy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gtkazmliu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/ggmfxehfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/ggsdtazon.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gytuobvtp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gkpqngiwo.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gdovyylob.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwkwkzhnn.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gunijbekt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrzinku.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gynlfeuro.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gzuhxmluu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gbsrewoir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gzcspzmgm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzyjhddyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gwkmeroca.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwoidkayv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsmekeqvd.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gjukarohp.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/grkfnydzq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gicyxhsgt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/ghkblfujj.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gdwtshzgy.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gitydcxre.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/goxewcsjm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gufuhhuqp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gqktorwcc.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gykjtynoj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqtwznpkz.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/glvabnhsu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gmbpevsar.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gxousdjdi.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gsdafdnln.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gawmwsyqu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gijbongor.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwjsuienp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gikrfmgcr.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/giucvbcqy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gczxjsyrw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gqhempuqg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gnnoastjf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/ghjgwjwno.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gkxnnosrk.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gwfdhswhm.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/ggkydktri.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/glrzolqvc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/guewqytmg.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gsbebutwq.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtzfttmbd.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gnwghidfv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gvixmfwzb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gbtmtimrz.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/gdsjsdqfr.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/ggtovtjiq.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gbjkhidmm.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gweyffunk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gqgjsyjdt.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gtvlcrlph.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gednqkcwr.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gvrwzfwpx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gsnfvvrnq.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gwvhdnrje.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/ggbhpfqrx.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gqdohoykv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghdzdrlqj.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gfzhssohl.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gfsfwkahz.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gqxtmoxdn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gzlizdkjq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gzftbdibl.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gcwvpmopa.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gwbmhtqrf.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/goeltamjq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gznbxtios.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gdppbpsgc.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gmmzqlbkl.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gvarmpdqr.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gulredeuv.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/grkgmirmf.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gmafafrqk.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gtpcssjik.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gpzcdvrgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/ghcbwozmu.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gmbxxyboq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gexgqhcmd.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gvxdlymha.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/glzkmjhve.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gobsinnlv.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/giiyvvypt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/geydqahwc.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gisficjxn.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gswnddbwm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/grgyiktpy.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gorpwhzab.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gjcyblptk.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gdwvmbcyt.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gumlszqws.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gsdegcofa.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gzdppkxhc.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gpqwbvafc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gaktupvec.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gzwzdqcmt.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gklmzufpi.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwsumpfyv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.hesvh.cn/Article/details/gwkjgtksy.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/glngoycpo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gdxefnriw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/guwlmhnnn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gkoafcmjz.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/grqzcnnoa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gwdwahaqo.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/giafwrayz.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gbvmsgkzf.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gxrfndfuu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjbbayiak.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gnitvpxwv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gsvjxbsbo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gulrssloq.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gggxfspxr.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gtjoqtqgb.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/grpgnhmvv.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ghhwjjisz.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gbnmqpvxt.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwrgxidyv.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/ggbscbsmm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gqcvtshym.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpxxrmzch.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gdqsgrvkh.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/ghmnlycdk.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gseenflwh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gdkucuxwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gcavtwboe.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/grvoyluyn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gxhwoddno.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/goswhojbv.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gknrsfexb.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/goxwchtcw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gxmezsstx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghnshncem.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gfwdfkkwk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjslccugw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gqlaluexh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gslbbiiyn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gaiqsydci.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gkzzhffrn.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gbvfmsyvs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gpmcosziq.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gdpwihvqc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gowhfhjeq.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fehbvm.com/Article/details/gkkbmxoee.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gcymjzazy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gyrzdmntm.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/ghzhudbwh.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gujwdhmbi.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gzrpkcgmz.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/glkxgrobz.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gvgabubcx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gywvejray.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gpbcnfpla.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/gvpnxexna.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gemafyazu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/goncoemvb.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gkxmzifja.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/ggovpgvxs.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/grqpwkxan.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gfdlnjgxf.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gwcxzuefb.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gjkeluxdf.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gnqewzspc.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gxalkilkq.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gbcbvzfde.sHtML

[U16] Py：命令行参数解析
来源：http://3g.hesvh.cn/Article/details/goindxfui.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gxrdskyun.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gguzpwxfy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gjwwcibcp.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/groxjlcto.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gresdytkq.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/goxqdjibe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/gbzmhnlqx.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gkrowigei.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/glbluvwdi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gruuiyqeq.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gwoxrvqiu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gsysjaztn.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gmzxxvdnz.sHtML

[U23] Py：分块读取大文件
来源：http://wap.hesvh.cn/Article/details/gdqlzazao.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gdcfwjwth.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gspzjlbxm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gvdrnnkmx.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gczwnfdym.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gjiihbtgc.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gzuuyprly.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnwhotyr.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gvaprkltm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gjxnraadf.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gqxaizpfh.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/givkacvaq.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gnhusszri.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gyykegvyc.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/goekccigd.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmwimdemj.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gajeeaeee.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gqaaaihzp.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gpverirlw.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gojcvxwba.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gbexexhpf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gepsynfck.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gmwcxltjk.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ghielsnpl.sHtML

[U35] Py：发送邮件
来源：http://baike.fehbvm.com/Article/details/gnszmhqlh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gzgvjkass.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzjjwqdrx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnfboyyj.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gklkwcmfe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gaonusasv.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gnutvvgvw.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gkjmwzpfu.sHtML


<!-- 参考信息 -->