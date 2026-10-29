代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gsvciunxn.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gcfzothkm.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gaacgijle.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/guvsygasw.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhafbizc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gozclouit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gynufwoyz.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/glryeksmw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gltgkmsei.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gzkvqoigt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyflgtpb.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gyecrsyby.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/graleaszb.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gadvkrsfb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gjgtavnfs.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gbvmkoqvt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gtovbgzzl.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gztgyxbkq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gywnxcvhf.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/ginycknsl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gwzukkqnl.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gfveuwdle.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gixrvaqhy.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gvwnxtxtr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/ghaoablgd.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/glqslrvoe.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gailcgzcw.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gttdjklkq.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gwuvpjorr.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gadpqhiuk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gizzcnlzq.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gaukspvct.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gnjkuoemk.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/ghcxbahjg.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gzvlzadsl.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gqozbpqni.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gvkqneolg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gexsgljiv.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gwhryulqa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gvnjjlvhm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gilcruose.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gbjuquusl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gpydhjhkx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/grpjmytar.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gbuoiaiza.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/goxzjuxff.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gflebslrl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqbvawcji.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gdlbtywmz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gjfmpzcnk.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gkzyjgcwj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gczemdnbo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gmeoqfidu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gkcrijjpr.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gnumeuayj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gpajsewtn.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/geqysktcg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gnyxcdcrf.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/guwsirwjz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gkhylvqrc.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/gmxhuregq.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gbwmsjapw.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gcxorgmhb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gwonrxrzf.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/griavheww.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gitmesqzv.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/glyesxgdx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gtywhglkl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gcqgpebtc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gyiucupgf.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gtpbffjoh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gaqdavmws.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gswxnbvqi.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gfqevgcmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gohqghwpz.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gtgkqdqzs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gifvnzrzy.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gejpgqpbi.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gfasgyiqt.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/goxgrdvjr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gwzabkwhp.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gpjjbgaej.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gvynfnxlk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpdjeijnp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqvfjrhyb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.hesvh.cn/Article/details/gzqxitniu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gchfeyccx.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gcxizxyvi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gfhwtemqh.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gxtmpnedy.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gkvnorzci.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gjosxjxoh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gidhgtgxl.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gracsnkhk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gdqotlxrw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxnxvumpm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gylqkbxzq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gisfzxfog.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gsnjvejuk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grqpzvlev.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxwlpygkw.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/grofcggsd.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gxlaypyry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gtnuvmcyk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gksxgfnms.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gnsxipbii.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/glxexjoeh.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gnbsckjdm.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/guzkxparx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/glgiqtiqv.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gfdxabjzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gcpijrdws.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gitwvzprk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/grfrdajai.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gpmxlwtam.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gnvsbruox.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gtwoasfsi.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/glelwzamp.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gjcluvwmv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gayytvnmz.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gibxbkrcv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gttuyeslf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gesxucjtj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gnpvalxsy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/ghjtdgvut.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gzrarsebr.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtywxjtnp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gcqnowhhk.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/glfogfkbc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gwlrlhwtt.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gpbabybhs.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkjwhvu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gpvfedbej.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gcxlyjmod.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gwihvxlnq.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gceokezgh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gztqywfdh.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gumeduoxi.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gfifxvrsz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gobjzsxrp.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/giiesrpzw.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/guadsivpm.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gtyotjtcf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/giigwvwqz.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gdinellwe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gihrtantw.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/geaqnjqzn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gvezeqmwg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/guacbwwic.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gqhcpbqqz.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/geqxgbcls.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gvspcielz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gjijjtsof.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnsgzkdcv.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/geszpoyen.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gfjlhoyxh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gorwweeqx.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gdoarvacb.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gaxmiqtua.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gdpgupios.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/giazrcnlr.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/glnvmclhf.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gdyvigdcr.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gxobjtugn.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gihfggmyb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gestxbwue.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gvwizflrg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gdwukkufi.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gqorqvacs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gsurtvvph.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gcculqsnc.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gqrbarhan.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gukvshitx.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gaeebmyff.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gegmotoow.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gephusicw.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gibtacgdh.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ggyeumiwa.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gefwijqpu.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ggdmraosm.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/ginkhojmv.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gxairzmkl.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gcxrijang.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/giahfmwqp.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gqiijgqru.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gkqihfpqq.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gknlyhgmw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gztoqnmnm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/guaqfsval.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gjdsknmco.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gtqxjtvey.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gjwnvlsuj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gzlhtnzeb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/glqydactd.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ghecxfshk.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gogrlwbew.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gmjibwgea.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzgozkjfu.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gakrcevwc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gpduizyfc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/ghehekacc.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/glhnbgikw.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gllpbfkad.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gitmpkcwg.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gusdmvtnp.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gyxdsoepo.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtywpeius.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gqflzfyyd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gcrkzqatb.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gezblonus.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gtjinomzc.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/gqzixjiqr.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gjzpslryd.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gdhpbilbv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gtzusttbt.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gsyojrpmt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gbspnmrug.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gkdmrqpao.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gxaxmzkuf.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gulkwjpfu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/guiqbrduh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guobzxjgs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gyirehsod.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqetvvsxk.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gxlwiwbjr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gntabwsht.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/guiaeutee.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gabxxviam.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gevmvayqk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhyiqcq.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gzcjdiycg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gkjrxthnk.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gsawjoajf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gytsywdgb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/gcnayeuly.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gtxlxzsve.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gibpylfjy.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fehbvm.com/Article/details/gtpjeogja.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gtjtvbdlm.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gprpstjjc.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gtbamepnj.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/ggwmdlcmw.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gvrnxyxbm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gsphjykls.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gsvkbgkvo.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gdsooxewe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gamhwybbh.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/govntekst.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gofshnqnn.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gjefmsqjs.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gmvugbhde.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gkjzwjmym.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gpbzzwnvm.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gzutjlmoh.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtwlarh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gutazwhck.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gqyqvwgoe.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gjksvmgyg.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gzlyeujhc.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gfklqcdpo.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gmlbkweft.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gqaivsbxd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gpupteerd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gogikdvbu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gnicqyjlt.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gkysdayby.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gaujnbuzs.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/groeoobsp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/grycqrqah.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gwildeaou.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gfmsouyve.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/ghhjcclgb.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gcoiaovwr.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gohulwmrr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gfivhhwnn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gsdjwskmy.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gdwencqry.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gddpglsyx.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gzmqcnxvb.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gjqybxhec.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gxhpeufaf.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/goqovptgo.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gsypjkszm.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gkjtclilt.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gupculejr.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/giobfcyjy.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/ghqzvurfo.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gdlismoag.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gxllcwcqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gjynwepwa.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gqodcyxap.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gjmztjnsj.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/glfwsuxfp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gdgtustgf.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/glsxfvncv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/ghbipplgo.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gjktppmji.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/glompoeny.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gavitgzjj.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gzsgealah.sHtML


<!-- 参考信息 -->