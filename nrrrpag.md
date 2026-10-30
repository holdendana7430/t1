代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnylvuvx.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhboxvta.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcercwql.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/grpryxerz.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/givfmujpd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gbhjquzvo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzxnofpe.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmmkgiczi.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gyxdgimkc.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvjhtciwp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrtsmzpf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsapezda.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbzxhgbk.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/grfevdolv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfniqtu.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gtzrgeidb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gmjsdjbps.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdsoovls.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gnvurtekp.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxlpgssi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gdvnncwfi.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gojfbzgia.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcrhwabi.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzznynrq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdlrildp.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxisduau.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxezpkrwy.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giktoghpy.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grkkwdrmm.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzkjhlbi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztpzuacs.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gbyverpew.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvacthqw.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gpsqsimgr.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/giruljrfg.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbjckht.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhufyppc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsckoztsd.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gurjehzlq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwudvdrqs.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gamenjapl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdryqtbfj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gnpdznqxq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsydosnpp.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/grgwbikkl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmelzkli.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gngdtplby.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/glsupykqq.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gqidcbwzs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxrxsvhv.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaqfuhtc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxwojtbi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gydvbhqmt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/geihotqtl.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwusvmueh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecxvbrrf.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjwrkjlh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gijogsvxs.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxoyngqp.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/glmmgqsvj.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gfydroctf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaylfthib.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqssasict.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxklczffv.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gxanhbpkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrxsetqx.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gbakgbbsa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcglnalzy.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmohzpyu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/geontwvko.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcpdwmff.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjudccr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrahqide.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gihqlrqtx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlprrbuz.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gmupjzihf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzxpuftw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbxwfgxn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gykytuftd.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gscchzair.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkbmrqfj.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/griwoeemk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gudlxmccn.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/glcilntgq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpofaauba.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/glqbjgkdj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcejdmmv.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjeeheyj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/geoccmwtq.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/grstlvtcn.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/grznzmftk.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnlbzqoi.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gctjbfnfh.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvnrhgug.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gpbaiafgc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grnodqluq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gajgolsqu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvxkiwqdw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/garnpwatx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gtsatzchy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvisjbybx.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnsdhceg.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grtnzerwn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcpectqp.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gxpexmada.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrusgksr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gsschqdnz.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gwcmdazfl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlekhbs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/giflvktfd.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gjcdpjnxe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvndxuei.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxezqbwt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glaxtaycw.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdijsym.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzbpuboa.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gznhypqqm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzkwclb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gduppxitj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhaehuxv.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gywbytkuw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrrrrqqq.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiudwruo.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/geadrgwuc.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiozoxkn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsrmssiy.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpuxkuti.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmqwgclv.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gnuvbqlfg.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/grkhkqsvz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gwspmvgcw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gztxrrwow.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudlztwdd.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gndkumwvi.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gmceekdbe.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvlbaaep.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gbcajkiqe.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjitqqpp.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gmsfysnsq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gobtvrnnh.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghtdsjzbh.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuwzjvpo.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gplqbmsfo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gmwqsqgkk.sHtML

[T23] Swift：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyisxcold.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwiprjny.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gqwtfyrvy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjghyshy.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gnruifnui.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gosdfjedk.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gedsysqtp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzymcgneg.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gnrjnzmfx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdkszqvl.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsncmfqm.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjohvlud.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldkbyahu.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkzmgpjg.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gtupksyzm.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/glbjvdxcy.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gguikjiak.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gidafzkfo.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuatjjya.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbokjbctj.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzilqbuj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcsagbbi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwoskjcb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gnfofoilt.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gscvalnec.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsglemixr.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/guwagbrap.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gniyxdcyg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfoadfrf.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwtgwqg.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkuuigbmz.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gvvfdextd.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ghkascsdd.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynjkhign.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvvajgoz.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gaagzdxog.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gawwtbkod.sHtML

print "Hello\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gflxwmmtx.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/girglosab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guivexwtf.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdnzknxf.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcrfwjrr.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwklqifqm.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvzarfef.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gtmkxusiq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsneiakz.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztbmukb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdjdpbkm.sHtML

[T47] Perl：正则捕获
来源：http://3g.fanxiaobao.xyz/Article/details/gysildhps.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxkzzcyg.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmqikcdxz.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/glneylxes.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbosoajjc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpekweto.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhgxvfj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gdfwwqwcq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpbkzljw.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpkevrif.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gsolqidqc.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpnjhnwp.sHtML

val a = 1;  var b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnczlgddu.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdththwze.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsyobpxu.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gwytmvblu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrisvdvf.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gbrtevyup.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzovixsn.sHtML

[T56] Scala：样例类
来源：http://wap.fanxiaobao.xyz/Article/details/grsalpusw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gsweyzplv.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggnrhunyn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmckemaee.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmggklhah.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gthbvwcap.sHtML

[T59] Scala：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkmjfkpd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gteswnmvb.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubsrsvvx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyivquihz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginttnbgh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gwcnarkkt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gahihuany.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdydzojvp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/ggcpjnjcg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gqymflytj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsxkkwub.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/guufgvgec.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvqtvpol.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszbhmzrc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxfkyruv.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gzcsuavlp.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gakqvldtw.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcgollrnm.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gasghkkjx.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwigeguoc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gfklwezpi.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewlnezey.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqdnlmpt.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpukwaav.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gzhifxgzd.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbsxjtg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/goepqmnxn.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/givkxirxc.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwihvmb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhjcwmnd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyyhhqsm.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlqfhnxt.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcjggrfu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/glntgshsn.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/grtakxlou.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gssvisojp.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfosskaz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gcmcdxsrl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gpffdsowp.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gakdtjltw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gmfzlqqel.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gomjgykbv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gckowwezp.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshxyqfft.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjmxindb.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmihyjpc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/glqzonffi.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gpftvrsbo.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gffazotrk.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvfoing.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gsguowzgm.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwotkzvkz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gdnieicft.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/glovckphv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfxwdayk.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gyaolpoqw.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/goduqcycl.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqllyzhit.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gchpivrvk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gknmlsdux.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/glurteykm.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgyzsmct.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkxobjuo.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxapuftr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoechiwo.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdnvywe.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwagdhfk.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjhuixtn.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gyujfsaqv.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhbxaro.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtynvcbu.sHtML

[U33] Py：打包发布
来源：http://www.blog.fanxiaobao.xyz/Article/details/gungneqcf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnleslpgo.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaibqftb.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmmovwcd.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtzazhbj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/goqernnod.sHtML

[U36] Py：定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfeogcbs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gmsmxovav.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqglxisk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fanxiaobao.xyz/Article/details/ggybdfhra.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwrrvqmw.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvtcfax.sHtML


<!-- 参考信息 -->