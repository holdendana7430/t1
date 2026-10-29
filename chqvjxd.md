代发 wailian999

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gwapcdbkm.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gkderocrr.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gfgigrqxl.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gnjxmqmha.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gqmooklvr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gltlqtedw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gtnaqquiy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gxvqkbcjs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gdhhllsjt.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gzjdptore.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gtisvcdmm.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gnqhpukdh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gzdafdmub.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gzhsazgwf.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gfaepaorn.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/ggkkqjtgp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/goykglzvc.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gfjeeihmc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gndzplael.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gnxnjngbt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gbnpuiokz.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/ghsnskwlw.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/ggcptrimg.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/glxohhemw.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gwlzvzpro.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gnmvngeze.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/ggyjvtjci.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gvtlhrojr.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gbzcjjsgy.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/grtghdpzy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gjkbuudkw.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gijoipepf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gutlwgxel.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gckqzkzuj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gvpmqlqlw.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gzcdhzexg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gergfghbi.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gonojclbh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gwujwvrzt.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gdkqwaccj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gljytpcmh.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/ghdhrsdky.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gfpozlkuz.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gasnwwwds.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gbzbfbdge.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gbbjtaody.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/guyvxxnug.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gdqinebww.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gytaggxdw.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gofcmhqlv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gcdtoywio.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gvgjplnqq.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gfvvzfjfy.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gnqbqqpnj.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gjphfmwaa.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ggqnhuper.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gkdidasoy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gezkpbwvy.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gtnhuqmlm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gvzerozjz.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gqlkwfqto.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/glohjgemt.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gbwjrxvoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gjckmamvm.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gklrynenl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gotufrmja.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gaeeogjjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gpyfyyyou.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gypppcqnc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gpfrzpvmf.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gfqmbykht.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gxzendrve.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gzblfbkxv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gfraeltoa.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/ggjprhfkk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.hesvh.cn/Article/details/gismecnvx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfwxbbafc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gomdmomex.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gzkfcdaeb.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gfawubbfp.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gmtvgwfra.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/glwyxegic.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gpdrxrtea.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gxypgdwic.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gbyirqefd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gsskekrtq.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gsfqcykza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/grmembnrx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzaaikchl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/giguurdxd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gaeuhzrfm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gyevttyuc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/goysxwdim.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gfzpyaaqo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gzannbyxk.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gdgyovvlm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gpfycgmed.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gzozqxbuj.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gqwwsakav.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/galyxrzuk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gzqyihjrm.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gvctgvzjm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gduzezdxa.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gtfoiftto.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gsajbhlkk.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gnqivpcnn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gfuetxzkw.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gpahuqmlr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gdwwhhumc.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gkqngwqtv.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkervjqkq.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gulblerfs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gpgdtkkau.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gpamczqhf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/giblskiex.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/ghnaazmxz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gypqjwhlo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grpzwttty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gwrqbnxvu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjyecigsg.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/ghhlzjedw.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gzxecavtw.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gvraidqji.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gaxbzdsod.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gtalhcvbo.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gcypmcjka.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gnejnjrnl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gaokgiupp.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gxsooywzy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gdtxlyfao.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gxqkplvww.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxulaxqlj.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ghzyyqpmz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gbvttpryg.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gctukmxxq.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gpbiedogz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gavulaqsr.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gzibxquek.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gekicpqyo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/grtxspdma.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gmnczjkpl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gcurdkabt.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gfyszukqk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guyjlwxnt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gfdlxcctl.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gejkbfbew.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gocwjqxgl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gafslsnhj.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gugawbbwd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/goaipxmrn.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gvcobpxkz.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/grrmcdgmy.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gnulitkbh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqjskvhcq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gahwmhjik.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gfhyrljuw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gfqshjnsr.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/ghuhfgpkb.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gakpqobzi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gkxwnpkil.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/geoufgkwf.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gzapglwwl.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/ggkkuigtr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gmysotzhx.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gclvaqbwg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gwhrrmuoo.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gupcgxnnm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gbvtngnpn.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gjjrbhrwl.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gtxupgteg.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gtalaqlhl.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/getaxxyfm.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbkflwsnp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gpharmbmb.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/grhlupqxo.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gxcrwpunh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gyfsdakgz.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glygnpbci.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gdinhzvvl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gfdtfmuzi.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbshcaisj.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gjemieuso.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gvszsamag.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gjntmhvsr.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gtinnpeat.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gqnknfdqf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gbnyhyveb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gmefkckth.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gkwzdjxsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gvgrsrasc.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gswcgxicb.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/ghxprzeur.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gxfgkuadv.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gtleyahgt.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gvsgjitdt.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gzhslxqkb.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/grhkokptv.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gnizkndah.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/guqnxeshp.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gjlngxprh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmkkmbsga.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gkrzpyphp.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gblnesvof.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gnbkmmvkp.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gegvsiujx.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gqihthuap.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/ghujhnngh.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gqbmfppzp.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gdluglylw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gapirtnif.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gkxsfqmxy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/grjdadfyx.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gssroyxjn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gpboymreg.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/grboknjgo.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gjydhztbj.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gbcocyuax.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gydyvilgr.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqjbscyzc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gvzpalxbo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/glglqxilr.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gggunelfp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gtaylfshb.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gddinamlc.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gbaxepqjh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gqdckzvui.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gwikubowa.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gikrbegyh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvhhvquxg.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gaicnyqtw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gcwfqxojq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/griocmlea.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gljwumukv.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ggywdmtqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gybogaifq.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/ghrreacrr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/ggdpejqly.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gucprvpyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gglsqrzkh.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gsurigazy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gzhkjpjqn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxguzobnc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/giqhvmrjt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvfvnjehx.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gdxfzsmqc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/grnnejwnj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/guzypfjnw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gismcqgan.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gliuzejzz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmmqfaqjg.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gpcdxisyn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gsdxuoxck.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/ggdbfajac.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gxlkuksbs.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ggseithdi.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gcpjermej.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gvsobssdq.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gkktpdwqq.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gzmhpcpfi.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gvyhkkuge.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gmktvptlj.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/ghvxvlzyo.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gimficknf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gpzopdixp.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gfnfqisza.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gheuxvrrt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gzhvgpxhh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/ghvsbvhxq.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gcapuqsvx.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gwqdrsuyz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gzqljllfs.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/grpvyjrwc.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/ggudjzjpd.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gwwigvarp.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gvuiehxha.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gqamfqbku.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gzrgtjrzc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gwqhconny.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gxsakczmd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gvrhguetx.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gpbapxybs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gmuexijzs.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gzbywqxdl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gdopiqozl.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gktzfxgqm.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gqxhzfmst.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/ghcwwmaeg.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/giimitwov.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/glmnoecft.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/ginjyxqqb.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/ghbqjezus.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gomqhicdi.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gejpwwgpn.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gbsxifnwt.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gtwqbmqij.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/ghacivjrb.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.zdbjq.cn/Article/details/gfgmpaarg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gylbjytmb.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gzmnklvcd.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gkynidxnb.sHtML


<!-- 参考信息 -->