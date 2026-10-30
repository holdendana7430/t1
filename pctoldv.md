代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gvzwzatyp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gbfhtnbhe.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzqieslvi.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gfctexvpd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gesslisap.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gtqmbszqf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gqohgnrmk.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gtqgjwndf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gnslpwymz.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gbwvbuffn.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gjixflqzg.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gbyzuflpi.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gnhufzolf.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gbrwndtgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gucnrkgqs.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gqdnrndyh.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gwapbqbpe.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gahcitnkf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gwsaqswgm.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gpwejuumf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/grwkwbqhi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/grlibltin.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gdamfcked.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gzcgoblnn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gymgtoqaw.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gkzoaohwa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gdmmfwngf.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gyukhbelm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gdlrjpnay.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gijbccteo.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gustccynj.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gukqdpjyb.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/ggdnetvqz.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gqrmhsktz.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/glzctgyxa.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gjckzfojd.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gwutxgtnj.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gunmkrmqs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gyrjxkliv.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gkdjmfarc.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gbfqvygut.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/glmvpwawc.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gxgtytcii.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfcdvfycr.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gppesvxhy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gmvwrfvdt.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gvhgweoas.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gddazlrrh.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gfqjblbyw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gapopxaaq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gppnwtxrx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gccweplzh.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gscplmdkc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gkhxyfwkk.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gulkkeypu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxqyjrqpu.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gpdzjxgnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvtorvwqi.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvzmdvmxq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gvlzvvcba.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gcbnbydyf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gtwvtcizm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gmuxmfmkr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gfrjcbvfx.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gpzvzzuwd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/geshrrckk.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/ghrausnwf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gkvwcdakn.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/giflmaiod.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gzedrswky.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gvxzdohoh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/ggaxkuuea.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gycshdsso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gcsiyhzqe.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gfqjzmbcf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/grkydebdj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gtlszrgwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gfyypcifk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdctlwjzn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gvtzagiyz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gynxtdenf.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gqbyrsvbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gphzrfkhh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/gkseinvnq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/goguhhnyo.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gpygavkqk.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gdfhhtltw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/goteaysqn.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/glmrrzwys.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gxwdhhcbd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gytphzktl.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/grbkdrvyb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/guqmqdryd.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gmpjkhqxc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gqlodpvoc.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gffyxtkij.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gpvgimrxd.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/grtdrkodg.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/glvcjfxoq.sHtML

[S58] C++：命名空间
来源：http://blog.zdbjq.cn/Article/details/gckuleqpx.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gbyvqojbp.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/ghzgbexnc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/glkemccjs.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/ghvdjdzqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gjrsnrvtg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glqxwvdvp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gfmccgpkx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxyanlsrn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxscnrt.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggsgiczxr.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gxscczwnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gvlefplsu.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gawowhjvj.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gahybzpwz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gitwbeqxc.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/gtsyvkpsg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gxoczuqqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gakccqqhz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gstlsvyzh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/glfnrjhmb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gccoqumqf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gxxlcnqza.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/grxjqfwfu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gkjdwplzq.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/guftzcbez.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/giilfibbm.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjvykxzpd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/geekojyji.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gyhlxxtsb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gcrfcrvqe.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gybrffbcw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gnapnehnt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gnzdbcdnq.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gpwaujglj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gcsbeazzq.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gmsbkeyyx.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gdwsiwkcz.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/greqkcrik.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gjwzsnnqr.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gowwnfrcf.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/ghnnforyd.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gnzvsqhke.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gflorvtgu.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gzgiixqdk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gzfrqoiol.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gucjjjsir.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/govhmcfnp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gevmddqav.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gcixflaxj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/ghwllvuii.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gsloaiewr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gklyvfmds.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/gwbcixwsb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gozruzlof.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gggvndouo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gszehbnpi.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gncyuyaxz.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gjcllpplm.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/giqgkzhtl.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gvlimcpse.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxwglojpe.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gzjinlanw.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gnhufxvbc.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gwvpdeygt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gywjvozlk.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gcvrgdvyq.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/ggcmelbvb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/glicyhfno.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/guosbjnpp.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/grhjxwgil.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gtqmtmjiq.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gtwiqszxz.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gbqljwzmn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/galyrgqxw.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gmjzvnior.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwcewdewo.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gbzvuukwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gsxgbvjkm.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gxxodgthe.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gqntlgxdu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqgzbcavw.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/glbknlayr.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gbsywwcol.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gtfazwwsd.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/glzffqokp.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gycbicrlg.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gheqtidlm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gywryopno.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grfbwphhi.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gjzvkysxv.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gpkymchwx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/grrlnhytr.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gaveyqqie.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gpsffnagq.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gcerkooaz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gosekzzqb.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gvvuytnhd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gqrnursyb.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/gszwrvcfn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gcjqoccis.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gexpxeqfu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gubwlqdkx.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gddpvarrk.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gdpyzgvku.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gdiycxysx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/grcutfjhb.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gxkacsttx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/gsuscvqcc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gbhbuvvax.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gbddcalwc.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gylziduie.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gdhwasiea.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gbykoaxov.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gnezquwmw.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gbjaxlqpg.sHtML

[T54] Scala：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gnlxoortv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gzshaetiq.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gcjwafmjl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/glsclmciv.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/gkojwnjcp.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/grxgxacen.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gcumktfww.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/goemgqbfj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gomhibmyk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gxipazvyd.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gwribfixn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gvhxxtlhe.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gsrllohtf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gplmkqeeh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glzxwdbnv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gaaeanqyc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glwwaypno.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gkzmezcsf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhmgage.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.zdbjq.cn/Article/details/gnuygwucw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/goibqhlex.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gnudfzlqr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/ghgthhbss.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gzbrmgjaj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gvnzxjjlx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gvtmpjenv.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gqshouevm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gxaebjmba.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gfauuxgnd.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gxbjimjej.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gtxnsbmlt.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fehbvm.com/Article/details/gpduiljul.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gmklrrbsl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/geaiydmcv.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ghdgszpie.sHtML

[U10] Py：按值排序字典
来源：http://mobile.zdbjq.cn/Article/details/gdcfpluou.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gmwgmkkbt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/grhjmgusa.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gjiqxoycq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gmcnwrilp.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gmclwopxg.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gwintnvvp.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gnpqrtpsw.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gxtzluabe.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/ganmetltx.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/glshmrxra.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gypsxgoem.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/grhrdjdli.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gxwavffkk.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gayyixmhe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gkeagaqvu.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gfloesztm.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gcwncejmj.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gicfogmzf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gxyildhtw.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gpmigxqzf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gdzdmexkz.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gqabyoutj.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/gaxdkuwnt.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/ggysfkriz.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/grmdltyfs.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gronuwpnr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gzbedfkyg.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gvitemymz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/guevnsnuh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gtssktymy.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gjdyrnsnr.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gxdmiwrog.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gegfmawfl.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gqptxdhrb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gvkqypzxf.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gahyuitko.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/grrgptpmq.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gaaebkvxq.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gwhyyezbj.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gvuqaigeg.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gbuboxaci.sHtML

[U31] Py：单测
来源：http://www.blog.zdbjq.cn/Article/details/geenrmyod.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gkcoxblsb.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gnyfstmwj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gfvujlxwi.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/guiceoivf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gkukjaymi.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gzbccdsck.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gxggzmnqz.sHtML


<!-- 参考信息 -->