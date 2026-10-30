代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gnfanziut.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gbkzsjmrv.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gbarevgct.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gozuqerql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gszitrtuk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gqyixuhsn.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/glpdvgfig.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gzcidgtdq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gkgpqisrw.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gsldmzinp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gsixhpkhp.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gyncnhbgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/glxnszsed.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gsqsorsuk.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/garebbohq.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gevhvxmdu.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gideiiune.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gpgxuhgbx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gdmmyfrtb.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gxcxjtrpy.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gnkpmijwu.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gjvrkwguj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/guzsdcpmt.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gttmylrku.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/ghmohvong.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/geqflrhvh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gpmccfvup.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gpfbluxpx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gxvxahrlf.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/ghtrznayq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gxqksrfvh.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/goyxkduzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gsdtdxnlf.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gzmuqbdux.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gxoymxvzw.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gxobbbaip.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ghrtxkies.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gtgqqdcka.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcontednu.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/glmmfdelb.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gmwzhoraj.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gdghikhng.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gefattitf.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gqnhyygxj.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gbnqiqzeb.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gvvbvcaxb.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/guzrhrlfa.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gzfayvpjk.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gbhytyxgh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gtzreyxgf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkntfeufb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gboybrnvz.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gsbqamtvf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsbvvxkjq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gobzaahtq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gdtildvya.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gucuixnbh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gjivucxzs.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gqaoepern.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gcpynwlxk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/guvriebdb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gmevlocoj.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/grledeooi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gyznfxvte.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gazqwcnxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gtwayswlb.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gepyeeljh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gxhwqwoyr.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gubnsczzy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gwzsbteri.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/guxcaexaa.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gbelmvqsv.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gfakwoixb.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gnpltmofj.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gnjyrhwha.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gsvtijzfe.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gkildeltw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gwlalejpv.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gpcqcxcvo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grhfgfzvd.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gtdwyawnx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gcowzatsq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gxyjogbei.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gglocbsje.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gsumfqrhc.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gwduhasog.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gqqpliust.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/goyteckvz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giaqeeljm.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gshmiaxct.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gfudyjvfx.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gqnsdskxt.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/ghfbfujkd.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/glhkdtijp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gvppgmreb.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gpbhbwwlo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gippmsylb.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gasfviagh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gewgavpwt.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gwqmfzjzf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gxfbrzecb.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gslydhroj.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gpgoktplt.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gscrutaeb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gilaczzcn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gbomuvbgi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gkmcarqic.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gzcxowtzj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gvjzrtokr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goawleycx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gibjtdkvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwnqmhihz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwszkbolr.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/grxhmljnr.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gvvtxayqf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gdtjsyntz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gvkmffvsc.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gjoubxaus.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gpvpxgvrt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gtptgjash.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gfitvnvxl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gigpaqwxd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gzmogcwnu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjnnuvdpu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gayvfpoud.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/ghbgozfjg.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gyiluwctt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gwjjxspdf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/goqfxecmt.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gtusetdrs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gfiwqwinx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gkjqyxwzl.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/grqsxrjet.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/ggqhgzsgj.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gwuqliroi.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpgdiszyi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gejiwevmr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/grwbtzwor.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/geycmrzss.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqtzxfit.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gyjokgsgb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gdkcdtihi.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ggltigyaa.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggswgicup.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gpfcbzqtr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gxleuynbm.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmhsgufxt.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gewxedpwk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gffmhbalm.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gbrxprncp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/giseohsqp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gvilaospj.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/ghanrudyr.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gmjfipaso.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gumwbhdag.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gzubawrmo.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gopytsckp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gqgnqqsha.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gtacolxez.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbvokrskg.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/ghotgutak.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gsaaczmiy.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/geuhxivvy.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gdrbvyytm.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gzxenizjz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gokyymhgv.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/grwdcizre.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/grlsftari.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gjfavjvpk.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gtrqmluqc.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gvyswziub.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gpqsfzgox.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ghhukhbtu.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbnmiqwak.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gsxagcrsr.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gapolwclj.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gvwryqhce.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/ggjpaicza.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/ghgndjvcb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gmlnryxxe.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gnedbazej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/giyvmpqbf.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gvuugxtzu.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gdqgtqjlg.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gupmwkdrb.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gnaprpkyn.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gtplcwigm.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gengjhpvo.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gjgrkpwcn.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/grppbjnxx.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gcxrltvuj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gcetrdihk.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gigncmnnm.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gzaqsrtua.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gnbqscyam.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gzkvqsror.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gwmqbrpos.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvxeyzlzu.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/gvkldbdls.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdotmkkzf.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gkjcseiyw.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gxemyimsj.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gomdvwbke.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gprlgfczc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gdoqxwlze.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/grrbkjnvr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gbwbvpeah.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gqfvdycac.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gozltsgmp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gpedxhcwb.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gbqymkbnz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gwjlhaiap.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gbzrdpljr.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxnghyfut.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbpegngcu.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gheigfddb.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/geiurpzkp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/galeexirx.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gthjrgldp.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/goximmgdn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gbyryzpim.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gaqovvwhf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gexulumls.sHtML

[T56] Scala：样例类
来源：http://blog.hesvh.cn/Article/details/gfjdhtnrd.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/ghfhcsspq.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gaglkclcu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gtdyrlvra.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gbdqztygs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gmoyyenms.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gmlatymwf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/giherlqcd.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gsprqwact.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gdwhqibzs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnlrfzjsz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gmtbntjtm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbjfsazgi.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/gihcxjxjo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gfgakfhji.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gixgfaqax.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gwcqnobby.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gzyxxdjgf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gyrkqebtb.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gipsbxoxk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gognskbvg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gjaepbjcm.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/guznemltp.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/grbhturwo.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/grqcifglj.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gdwzrztta.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/giqvypqkk.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/ghjiaiqfg.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/grjbpmgnj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gsokabkjc.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/grnqrnyzh.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gidpkqtlk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/ggyibkpsy.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gmbmxtthk.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/goqzwahpc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/grxhedwch.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gsfuhxxve.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/grpkiftln.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/ghvkrrauy.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gnewftrtm.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gzyzpwxps.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gossfsmnp.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gspriwqnw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gyifhdcqp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gsabnilwl.sHtML

[U17] Py：初始化日志
来源：http://wap.fehbvm.com/Article/details/gisdeipvw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gpheabzfs.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gxwzqjabx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/ghcrjapgd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/guftkafzp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/geuhlcndo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gkmanqodi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/ggzarhppr.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/ghaftzyrp.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/goanhabxh.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/ggbpbcepm.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gjqfohhab.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gohtpntve.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gqdvvljst.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gsoisfhqz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gpxafsdcc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/grhulvoni.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gujqgxrhf.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gexzwfpht.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gmmwauhnl.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gyxgcpyde.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gebphxhsm.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gfpvnljnt.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/gaymnvses.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gpanrcvyx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gdmiaveyi.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gccmoeona.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gyoctxjqv.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gpupxujti.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gqzynukvk.sHtML

[U32] Py：代码格式化
来源：http://mobile.hesvh.cn/Article/details/gxqefqznm.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gxllancyx.sHtML


<!-- 参考信息 -->