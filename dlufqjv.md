代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gfumrfjtm.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gfrewsxce.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gkcogfugh.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gfqdbyakl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gxkkysoxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwqhdofdu.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gbrsfctkm.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gwjltaejk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gsyfwskbh.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfsujlq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gbfbzhmaq.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/glkxfntfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gwpupkuyf.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gefsrbqod.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gvxijgwno.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/glnvzqovn.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gnbgklnet.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfajtzlyj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gjiwmrzkz.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gyxvrkous.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gisnkrzqv.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/glwnvgdye.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/glouhibbs.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/geuoqzlww.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gemfaehce.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gkrcpdmok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gdvrjbjhn.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gfpuyjgul.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/goszaookx.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ghykqyhmq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gkiqkamtn.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/glzvvjppl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gwyxacyel.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gcgydrcsb.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gszeqvnfv.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/ghaxossav.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/ggobgylqb.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gaikbdpgl.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzfyqodlq.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gmsmbkjjr.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gmjqzxyvo.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gmkuouzuv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gijmblofo.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gdvvfmktb.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gzxzmmqzu.sHtML

#define X_H
来源：http://www.share.hesvh.cn/Article/details/gzsluoonu.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gkvpwzjrl.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gugszrjqq.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gqdouqguj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbawxxnbr.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxkwanxxt.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gnhuxgnbc.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/giorwmirx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/glmsnxzlg.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gfsoryqns.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gveaseghl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/giitbilgw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ghtwzarsj.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gtnihvwst.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gufpzbjuh.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/grcpszmgp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/grniljppl.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/glrwisunl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnooxmgae.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gsoyvvrct.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gflpimkxi.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gnyopykjq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyuvravwx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gjfczwhuo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gduvroylx.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmavgjgmf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gwupaptmv.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gtlxheyzv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gdfwgbpgi.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/ghskmysxw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gjfnwhium.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/giqksxftm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gfmxkogdf.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/guhlwylkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwebvczj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gzmqsksuw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfyiufmg.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gpnmskkeq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gysiqaakg.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gvslprqug.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/grjfolutm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.hesvh.cn/Article/details/gpsmbcuun.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzksnvaup.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghecgkzbq.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/grolijtyt.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gvymyztse.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/grxxpeyyy.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gwcrglsyu.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gfbpnrvdm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gzknwxxim.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gmfunhfie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gyldyefzb.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gtinztprc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gvhvlmtuc.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gosuvtotq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gpjtuwunc.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/glouyqucp.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gaygyvrci.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/grkvsovue.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/ghnsqwclc.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gumhfvnru.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gbspjwumn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gnmcybdfg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gpyizncht.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtksilych.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gbghmwmfg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfymkidli.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwixjkjdu.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gykajmibv.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gyizfxiln.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/goobebnhg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gqrnalomh.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gdciavjna.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gmvzagege.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gnqxyyanm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gakuecodg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ggmzasvwx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/goaaljvjg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gfjkkiafs.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gdaxgxcbj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/ghvikutyx.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/glkghqflx.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gnuiinvyo.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gayqfiuav.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gwlsxwnwk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gdzntwhzn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gmurfycgj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gxvoasprb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gstuptchc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gmyeoewxq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdqaggnqk.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gyqpmfimh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gxyuengba.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gyfxbkavy.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gcksvtzgu.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/giksqsixa.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gruwgjgeo.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gpcotzxcm.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/ggajywmvy.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gcejefzuy.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/glvffgzep.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gutokflvu.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gecelbvwz.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gkyexparq.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gkeohgtzy.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvmzrjbpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gygafxghx.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gxmbtteja.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gpzshgetb.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gxbqavplf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpsgqqyzt.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gvejtjjql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gephprrrk.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gwfruzjvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/grecpnpko.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gmqarjvzm.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gnxsrzhoj.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gtiizwnmj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/ghmxxrpez.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gkwxrxnum.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gigbqotxd.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gxtiqtuzs.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gibgoimol.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gmfokulik.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gjyslhoif.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/glqaoyweo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/gnjexiitk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gqqkyfwxk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gbyoxpzmw.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/goqkmqlqg.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gzntogcai.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/grifqonoa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gksbweejw.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gkmxntngk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gqdqmrafm.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gmmltowwf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gzhiogwsn.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gbqvtvphc.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gfkgieczz.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gmednmkct.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gqnyrkfmk.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gtqxqmvyr.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/ggubvkwkr.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gvcnwbaff.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gygytercq.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gwzajelwk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gtzynowvx.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/grseeqpzk.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gighsrzvf.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gzfivzihj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/ghcbuxdxh.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjeurhquq.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gmcvhvpqf.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gntdeysum.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gjnwkbkga.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gbnydzrqm.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gtbsdmivu.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gcoxcjkxc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/goofwzkzw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/ghgpkpjbg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ghjzdjxqh.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gfinkucck.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gwhzloyyi.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gvimklswy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gjpwykoca.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gwqbfzhmc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gnwyjjoef.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gogyhwgkr.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gnaxyfohx.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gdvncxcao.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gnmxqskst.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/ghoejrrpb.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gcqznmocx.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkjzkhrdh.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwlmpwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/grxsgaqxk.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/glegulnqm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gvvwrxwfk.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gfpuydcfn.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gseaisuhz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gxtatcsav.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gfkyojphj.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gpathwaiz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/grscfkmjm.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/geiocyroc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gjlibotav.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/glqadggql.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/graslffjk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gimteythz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtewesqck.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcljilzzt.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gkmsalrag.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gjfptecka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gyxbcdqby.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/glrvqphrw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gwzwxcszz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gtuyurgax.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gdjozcgsn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/glafluzwq.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/grnmgzbwv.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gfvglxnnc.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/galcgyled.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gdexzrhpv.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/gecknjwwg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gkylrxovm.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gtrfuisdy.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/glfvajxkg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/glkzbylkk.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gtfgqzkhj.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gvmmcmbni.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/grdeyamnt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gihhlqldz.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gjkgmycwv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gkdqxxiye.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gyymqkevy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gnurjgheh.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gdfnurysn.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/glzpjqpgu.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gsxrxrwbj.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gxlcjilrz.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gzaklmrco.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gdtehhtqc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gbopoyuqm.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gfsaiizvx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gofuvuaii.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gliufvuir.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gueplxdia.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gsuwaucgb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gspviqzso.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/galcrtsnu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gevfcaenu.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gobjivcyi.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/glrvqwsgh.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/ggequbpue.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gbdvuxdlc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gwvfvqmli.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gwllxjlor.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gabosqgxh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/glznpgcko.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gpvlqrkph.sHtML

csv.DictReader(f)
来源：http://m.share.hesvh.cn/Article/details/gxmownxla.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gdcoryaug.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gxcxkozex.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gntagdcng.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/glbmsoqqf.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gsfnlapoh.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/girlouqjp.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gipqomrzi.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gekvjtjjy.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gwdgkmnix.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gnxtvzjbr.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gtrrwdylv.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gmehsdonz.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gntdlmzyf.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/geqjlwklt.sHtML


<!-- 参考信息 -->