代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtpkuckz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/grorsbwaz.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwfmfrjb.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gttwrfegy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpvusjigm.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuvnywdm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/groyuvodx.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gkrcxwphq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gqpikgjsv.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnpdvkkd.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/ggaorgkmk.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gemtjjhjo.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjlnsykd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohtvjryn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gcuuystcs.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gayltnipy.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gffafybza.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghbjeosje.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gtquqbziw.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gnqjcozyz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gamviflhr.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gnijwfijs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyllvohx.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/ghfkirqqc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxplckv.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gyytmqcyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gopzlfzqn.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqhngnyz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvhphnjp.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gtdaeylid.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpqyfmpb.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/goewhnkeb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gniahhcqy.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gusiqocvm.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gjcaaipas.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwkintnb.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfyqmsuq.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxajnjsg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gefaecnrn.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gownrzxxe.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/grejvxnjj.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gypssbhve.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdfbfsco.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwpbhyye.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqftblyo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrebvezd.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfzgzdau.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gafayrfvy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gomwpgaaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glrarkhzv.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfukyctl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grbeuejon.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/goqzqplpz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqwayyh.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gbumuqwpe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwkqbynl.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnsojhtj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gseheudch.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbyffgfma.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbhsucof.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fanxiaobao.xyz/Article/details/gzhexrtaz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghngirjyo.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhruesdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqorgiyv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbyagznb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/giqmqkvkn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdujafozb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gslkaevtt.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/glfmwrarv.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxoatkob.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ghmhleabb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsomkxbm.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gxbmzwkle.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswoxpdrn.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfrzaqxd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giaqedwcl.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ghcuhzkrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gupnzdmaf.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorbvkaox.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/guypntgmr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfynzfcnt.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrscsxba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvzmokyy.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/groakaxue.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjuwhbbf.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greuapylm.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gchlsfqdp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gmmdwpcjg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoqjqbli.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/ggsmgbtgo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gxxngbpqp.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzuyvhtal.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmatqwbx.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gajxorcci.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gzibjoqlg.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmfpldy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gedzqcykj.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvpvsbxw.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiuwhlpn.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/grojuuxnb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjxyjcir.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxpjgypq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/grypgupty.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaiqdioy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfppzjav.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gufyffknn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetzrjno.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwodyyoaw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjvkejfz.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvzjpvwu.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gofkhohxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/glfldhuam.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvzgokrt.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcwkwrzk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxjrkkea.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzcmsipd.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzodruxh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghszstsdg.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvwtvznl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnsyukdaj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gumujdcnm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwpuyayf.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gghzqwsts.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gancqguww.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gwhxrttqy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbrehupv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/grabziuzx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggpxvdnkl.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gruvdyxxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gpchnycxz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/giumzwqlq.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gybsabfsi.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gidccdngh.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gptoyzomj.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewuedbzc.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngajnnym.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gvxxmnfhl.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gowjrigyc.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcfwprwgg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjumwtmq.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzljlrjl.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gepmrozoh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwgtloiw.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihomdaz.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjbcgmad.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzguqharu.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gyvcczejp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gjkoomeai.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/golkgcego.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnkkupqt.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqdtimr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gunnrhuat.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvefwpyql.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/golwdlbkk.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gexuvsueh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpujnismg.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gfavpkcxd.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsoiggtg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhzodikf.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyuatgcy.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/gjldpdhda.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmaeblz.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gpvcgypcc.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/girpahykn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjscciztm.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gylxrbnpq.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrgckxgh.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gielpwiuj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhuswkmp.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggszeugys.sHtML

[T32] Lua：局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/glayhirvx.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gmbrlqtkh.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geijzehqb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpveqrff.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gxfbtffqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gihmkmoub.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcoxbxbh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gcaoqymmt.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauuwbcid.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gudttkcvh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgsdmrqa.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gmxwmwemm.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grvvdvobf.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlgqslgw.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfvetwtub.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gywivrccm.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxytheij.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcpwwlpa.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuvqwfwd.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gncfyovij.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrwthyqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gudktvpvx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoathimv.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmomkhjwi.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbygixiq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykjggzzn.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/giyrvffmx.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvzcxepio.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/gxjcajcjb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gemfrxmpc.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzifvsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/godvpzgfa.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqucitlz.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawoudnmt.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmaxlfzmf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaqgdnst.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmbysnetx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gljwmaoum.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvdaqcz.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gznliupki.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gzsjppmch.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gslccblnj.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmhvjdsp.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gczpovocw.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gapgwvnkh.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gnftyqylv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzbjmtcr.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gzsmtzlvg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvntybvke.sHtML

[T56] Scala：样例类
来源：http://mobile.fanxiaobao.xyz/Article/details/gofzgdgjl.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gubatjfob.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxycwtfb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphdotuki.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gqhfzuygj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzwfdcmp.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjxcsmyjd.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwbdgbcb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpgyupyc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gzoxqnpdb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimdgjivb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadqinuii.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsdhislo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gxbjmoxex.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fanxiaobao.xyz/Article/details/gmepdmgzg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gibzsxocy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveheeyxg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdeinmsv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giogegsby.sHtML

[U04] Py：变量调试打印
来源：http://wap.fanxiaobao.xyz/Article/details/gmprjkffr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/ghzjwihul.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/ggyspdkgb.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/grvzeirtu.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/goptqalij.sHtML

{**a, **b}
来源：http://read.share.fanxiaobao.xyz/Article/details/gumflwedk.sHtML

[U07] Py：反转字典键值
来源：http://3g.fanxiaobao.xyz/Article/details/gmtwmwojl.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwezdbrb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvpftwkf.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gljxjsywg.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganlvqrfc.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzkkiicf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/geavjreet.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gbnwpvlob.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gwdzpvnfp.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkndkypm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckriucgf.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwinvihj.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjndduhfs.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyoqrnvh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gicslemga.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbupsvxi.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpcaitsl.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqbsomqt.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gwvixpzms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fanxiaobao.xyz/Article/details/gtdwnkqlo.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwiobsnib.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpisanub.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisakzenz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gsjxbauvq.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmnnyxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwafeynbh.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/gmymcustp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gnxqrgryx.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gugyysxmp.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gaqgdfhkr.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvkftjp.sHtML

list(zip(*m))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyevcggg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsmbepww.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gyczlqfqz.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gpzjfpwar.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqksskmat.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gwyancakv.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gxgoeqjpu.sHtML

[U26] Py：并发下载
来源：http://wap.fanxiaobao.xyz/Article/details/gejqtmmzl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfxghrux.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/ganuotcgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gmkhqovoo.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gufhxjdua.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdanmhbwf.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/ggtkhacaj.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/giznlxxaf.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvvvumsf.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/guddipvxc.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/grfnvfbph.sHtML

python -m pytest -q
来源：http://m.share.fanxiaobao.xyz/Article/details/gskeyjxpq.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glwuzopne.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fanxiaobao.xyz/Article/details/grhuitwuw.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckdvkia.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gojaywuag.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwqehpul.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggubfdizo.sHtML


<!-- 参考信息 -->