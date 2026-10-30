代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzihtbxub.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gbtmucvyf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqikflltp.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gshcijsyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/goibneldk.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjzlthug.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsplwkhn.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gqjasbygz.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqrrgjbkc.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpimsmmd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrxzqjiw.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gspltukrc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbwjvunf.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbvjwnyeq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/givgwejfn.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glakrxyba.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtojnboej.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwcrbrl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfidydul.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpafeygw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gfhvdpivw.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gkonfpeuz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdthdyrhc.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gesaptnkg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gktzmxybr.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdtdmvalw.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/glnhvowbl.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlvynyel.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitwddyuq.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/ggjgahzfc.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gylwjpgjz.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabxgrjwo.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grfylhywm.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtmvjfgpc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdajfetjq.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoopqfql.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gwtzciihx.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gnoppnolc.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/grfonrkus.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghpsfqokl.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glggvfcee.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkhjntvc.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gegpbpoey.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gqyhuuoup.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gyylgzvru.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgeegfgq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggszyauov.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grmphycko.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/genrhcibu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gbmmobzqn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmclcvsa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfkqjphl.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gksaebhvs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnwztoxuo.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhiowxbv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/glywhlcfw.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gimhhbbyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gbmmtscsk.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gddqhsnip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gsvuyovuh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goswqfuzt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnizhacj.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbxkqmjx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaslhzvta.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzoswiq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gekejtpwo.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gzingzmzv.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpnnmssv.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/grozzjjqk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdopdpgt.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgnpljwr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gszvungbi.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gjebgafde.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlxgrykl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyoutabx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgerbuxt.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccvligun.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtscnyjhz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/geixlcjxm.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgtksgq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjppjksop.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdegqxad.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ghnaibssw.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gaefmoqby.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmicdjekn.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gycaqumyw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqasppye.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmviwipk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gppnazgvc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gcvlblfmi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/guccjawjn.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gikguuiqp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcbxlsixl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlfyjglk.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpitrxyd.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqysikvj.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrednidh.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/ggejkkrld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiwqylpv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkjzyvppc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/giuiiigbc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjbywqyy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gdqvzigbq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geqlmnahl.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswgthbyj.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkqkzxwvd.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfybodpxp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gohvsjuwt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhnkuazp.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gckxbtkcd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktxtnte.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gylotimll.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqrmayod.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/ganznqncp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxylpuhsm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufifirvh.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkifskyb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjifsyupq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaddzjez.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gnwvgcvvz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnzdxjbui.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gbwuhurmi.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpszmzqxp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdtrcqig.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnomzovmz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpojhxqbp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gebotwwvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcerxtrld.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gebeweiqc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkrsduuh.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/guoourvir.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvezybfl.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczrwtziu.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkhhhjgl.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkghsqsxf.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmeckrvs.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnmafwvl.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwfuhuinm.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gfrdquwae.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gjyobzeho.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/glklpfltb.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gopvijnan.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gobjcuctm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gfwwxynho.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gfajiklun.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdytaneg.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxeponagi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkoqvrmv.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtsvfhzsi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyvjhfnb.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gawvktxjm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoyclcfm.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrgbikti.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmxrlsa.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcyaydkw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gndqjoskc.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gcvqcqmtb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqamhmp.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/grmqdzwjk.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvzlqki.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdwcszmu.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrmrluto.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqqesoeh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfexfrruf.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhtpfkxf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gsemyhahb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvokkyoab.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgdhndla.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkmrjgvt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfqpgdbi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizcvhpcx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxrrlylc.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gkxlqftfy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gvqgrmysw.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpxxqyste.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gazwpbbqa.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gynaauscj.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gxadthjgx.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegntiogb.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gqpjanghp.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gydwaocuy.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkuyutvb.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gazsygqdw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkzcits.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwablykad.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgowcamo.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxbblpjq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gmlrntpog.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhogvoy.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfztncp.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gveaingzl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gklhvcffb.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/grbcsmmxc.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkggngnmq.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gfxsrhmlz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbacxrdc.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfyyxqxj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgynocux.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbelhpfue.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzwpqyzo.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulgicabj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhpuyfjx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbptxck.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpjwhsjb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteabqszg.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqzmxirxn.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwsgltgr.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmgivzoxx.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjadnqfz.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/glxhyrllw.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjtsypvn.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxlkzqgc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqjealfe.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gwppjmqny.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmdtwqdai.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjbzfbfa.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpalshlvm.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/giyklvnyu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhcrjzal.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghpyjhfiv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckjbxlj.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gljcuzljp.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzwtbmyn.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxiqtzx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fanxiaobao.xyz/Article/details/gonnjhmty.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcburlish.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkqbxfms.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxowdxcx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtafvnot.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gexmepkpm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/ggrdcgpbf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemoakfoh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ghxoqkdns.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgxpaqhg.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gmdtqzufx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhoiouyl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gpvwgjbjb.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gkrrebilp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfbxditc.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/gecdshzff.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwgheelm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gnfbaokyt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvbrazpq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwdhbhkq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gzsprptvu.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbofccly.sHtML

[U10] Py：按值排序字典
来源：http://blog.fanxiaobao.xyz/Article/details/gwqjzewpx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fanxiaobao.xyz/Article/details/gqrbduuho.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcstphwtl.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gktzapcia.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcjlmyfg.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gwhltlajl.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrjngjqn.sHtML

deque(maxlen=10)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrjzycrn.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrtlrprm.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpvwtycj.sHtML

[U15] Py：高精度计时
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwrwutac.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gorddcqgr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpejiswjl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gculpqeax.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvokupjuk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fanxiaobao.xyz/Article/details/grtlqyzrl.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwgmftpa.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gtteqgdbo.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gecrjhwfg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gincqroqw.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gznwcbepu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/gayhhgopq.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gtvsszbev.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gotbxychk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdtiasfo.sHtML

list(zip(*m))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqctynzm.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdxzgejz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gfmlyhxny.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gofbtxiwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubokdipo.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbaffhs.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnesxxdli.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/glyuvcqcb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gykqfxqet.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fanxiaobao.xyz/Article/details/ggymkfkem.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/grbyfuics.sHtML

[U28] Py：类型别名
来源：http://baike.fanxiaobao.xyz/Article/details/gvvobjgqa.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gjkdhqmyq.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/guxcwvcad.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdpoqeyk.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/guvgzrrfs.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykgksgl.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gikdtqwqo.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gochcpnut.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqnhkbzht.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaxzggze.sHtML

[U33] Py：打包发布
来源：http://3g.fanxiaobao.xyz/Article/details/gyhyotbnw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnofjnmwx.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweedzfxq.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gexkylpwm.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjcvculn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdazjnl.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/garwiatke.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqoixrpuz.sHtML


<!-- 参考信息 -->