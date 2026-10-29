代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gmypyempz.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gxltzwglk.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/grtwegzch.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gerfhmcdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gfqwkfmrs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gdfpurmqv.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gzxgsoomj.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gthigjlvp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gnbvhgswl.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/ggvcbbzzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gcvwjjmwq.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/goxwlhoxd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gsrbrzryn.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gaxnqzlgi.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gjkvznsat.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/giwkpevun.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gxxpmktib.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsfwemmzc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gsornsdnv.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gfvkyesnt.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gqmfotruo.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gpeandujc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/grwgkzkrh.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gvbbxkbta.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gyrfygaej.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gkyswkdoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gvtsehjil.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ggoccvffc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gxcbiuuda.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grkhepjqm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gehflzspi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/geqmewust.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/geiffdsyw.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gjapncvpx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gkpmfbzgg.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/goibuhbxn.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/getnaubyh.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gipqgtzxu.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gqbrcceed.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gpgmuzuaf.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/ghkuyhyrm.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gsqpvjulc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gjllkrdwq.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/ggyopnbqp.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gkjtwzsme.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gvuloscwh.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/ghydcdzrq.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gprvwdkyy.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gryuwbbym.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/ghnvyjkqh.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/ghrjimaau.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gzvlbmjgz.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gmarhgrbz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhzbdci.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gkxteteqh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gcyrzcqju.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gmoyuytkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guzivuxxy.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gcefqmcae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gksmbzybt.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/ghzjtdllk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gghujwbcy.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gurderhzc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdrflghcl.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/glbasecpz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gjuiqlgzh.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gdiqwqele.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gdpgoycri.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/glxfueesl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gfrvvzgbe.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gnuaodrpt.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gipqpytnu.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gxposisxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gojptlrxq.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gvrvqmrcy.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gqohtvher.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/guliwnovk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gctpmqkpc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gngjgifmf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gvetrywzr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gbegaehtl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gefshpuyw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gztrfakqg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gfmxzmbej.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gqlwkrcyv.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gasizoniz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gbxcpyipu.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/glsmtnzii.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gesybrjjm.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ggnkpgffs.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gaxzifvvo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gugbohfnj.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/grhbojytj.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gcxdhsdcr.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/grkoovink.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gtrjvsdfy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gvarpnrhs.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gxruwbuic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gzxpsfwhq.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gptznwppz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gylmdncxf.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gngnhrgaa.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/ghbdwisdl.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gexfqltmy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gqvnevebx.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gumqynpre.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gpdlldoeq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gugnfokop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gzdmgjvnq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glzeszoww.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gkyqwauhr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsqvcozxd.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/goiefjnmn.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gycopomgy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/guxbdkegb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gbiacguaq.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/guynkruiv.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghwlycngr.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gliapzxod.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gixolluiw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gqkxkbunr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/ghrlnbqtd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/grwnflcmf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/grfjaeuib.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gbxujqckh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gqrmomejh.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/goshlfzfr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gxnmuwtrz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmkqqmf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gttrmdyvs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/ghbzxlfns.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/glloneopn.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gmyjenunz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gxpzfatha.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gnqfxmzpi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gqfvoztna.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gabuwsejg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gexaobcgy.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/grfawsjkr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmonzkjfz.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gpwfojvfi.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gzvygcppn.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggxmpfcsh.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gziwozfxw.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/grprndazv.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gimdxyhys.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghoztquqs.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gkyvifjtr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gkzsasycd.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gjcxstsfe.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gtzspqsje.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/gvoacvaqr.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gyzacnkal.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gaftkxgrq.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/ghucpxmat.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gbcphloxi.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gzsgngcdf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gfgbehmoh.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gulxqfhnn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gaizwanvy.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gbuoepoln.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gsvxmafqx.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gkrohihtm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gznilmgto.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gexjaidxg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/ganqlafzy.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gjvhigcsl.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ghlksrnap.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gstjpkpsy.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gxymzszzy.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/guzomzvxa.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gzmhdtsrc.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/guqptaepd.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/glykylbik.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gnypiqysj.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gubkqctzv.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/gkkwdntuy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gealosokj.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gggnelbxa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gxtbrhudb.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gwybtrjaz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/ggcitxshu.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ganecwglo.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gbxuzoxqf.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gerlykhom.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gwhlhcald.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/glozrsaee.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gjftmtsvb.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gniyvncfw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyguavql.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gthsnahyf.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/glppfpnus.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/grdtkjvfs.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gfypvyihn.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gihafrtrh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gonkhhzqv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gzlhdmiyw.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/grevbemtn.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gfxrqcvnf.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gknkuhuen.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggqvmmrah.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gfuplptis.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gwqrxiozo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ggagyiopj.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gvywbyznt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gpthhjnzz.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gqorwnuwp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gvaymiqnx.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gtcfvtedr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gepvgshzj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gktspgjwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gbtmuwlvs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gencrnybj.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsmihidpi.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/grluapcey.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gmivbyxcw.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gnygwftta.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gejyfaxue.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gwuhexvsh.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gdealgyxh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gdsgzaobp.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtdpgvkyd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gjrpikamq.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gtgotpgxo.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/goihyoios.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gfaygupho.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fehbvm.com/Article/details/gakchbflx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gsegzrubf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gqajvcdtd.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gggkijkbp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gogmvjnry.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gqizxcwoi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gbnjmweyg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grvpgknid.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gpmtucrwd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxrcxcdfz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gblrxfveg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/glkwszgki.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fehbvm.com/Article/details/gnfjokkju.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gjlptgbyl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gsejqtmal.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhayevgf.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gzlscyape.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/grmngvssu.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gfyobpyna.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gomtmamlb.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gjyipzssx.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gozoghlhf.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/glzpchleb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gxvxoaacz.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gvuxqvcam.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gmaagchzb.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gbrbbphmg.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gefqugypa.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gldbbstuw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gdizmaeif.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gmjitxvcu.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gpolbcmqa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gteuokfab.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.zdbjq.cn/Article/details/geyoqibex.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fehbvm.com/Article/details/ghjchajjp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/glxueuzwg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gpxesgwqy.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gejuspjtt.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gwupbxzhn.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gygdqcibd.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gpkgiizui.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gvnkzezsf.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gphplyirg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.zdbjq.cn/Article/details/gquixddop.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gexxlegxd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/geoxqjzbp.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gndbrzbcl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/grtwqifgh.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gxkkevqje.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfjjilg.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/goglolxjb.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/geyssxckh.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gefyxmoaz.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/glndikkiu.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gxsobhmyg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gkzpvmdht.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gnwtrcouj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcexybv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gfwxmtmje.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gcwupexhd.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/ggnggcpwk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gptblhxbl.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gidrjqiuf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gsiscfvik.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gispkdgss.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqiphuv.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gpgfgsbbq.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/galecyjse.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gcfrdtwem.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gjenmjesf.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gdmblhfxz.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gayotrmug.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ggbvtbcmu.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gocriftdf.sHtML


<!-- 参考信息 -->