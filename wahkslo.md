代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gbnrcdkny.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxemccq.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gveprbclr.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gghwkthsa.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gqqmfcgqu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtkykoxzt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gyrkwvvbs.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gficvofcq.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gulbwvdmp.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gokqhcgxo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwajtedbg.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gcurhxlvr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkbalxnh.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gntcyxkpi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnzrcitz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gideuqdra.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gxwllzdzo.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gidtbjhtw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtkcyxlk.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gaywtbifv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gqmoxkpcn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdenqndtf.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/ghnsrjraq.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcrwzajf.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gekwshdco.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/grhaloope.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctikewk.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwshheye.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimyyipiy.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnmozvrr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fanxiaobao.xyz/Article/details/gsjljzgkc.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/guuncdqgz.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxjznlbn.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gmohflrjb.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusbfxljh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaelmytzi.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gbffvvxdu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimfjcaex.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvsacplmz.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/geujnwvry.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukwclccy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdriizl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxyrycme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxarhxhyf.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwsrvoqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrnzydcs.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsahiks.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gtlkkatkt.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwaedzil.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghjppvfz.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/gblitboza.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdthtqxw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqicbtyli.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsqqgaka.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gbrslljwm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhvrzzyb.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gywsqlxuw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnrvwofty.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjytblxxp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gssdqdlon.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxctekpt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gilyckujv.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gibrzxajp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdduqpclc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxioqaumr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnkjynkc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcrnarod.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkpgrsmz.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gosopuqrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkzjplvu.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcxuwbmuv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/glongvjux.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gitbxfzsj.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqnrzbo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvniytuk.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdieexegn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/grcumlnyz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtksusiyy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruiulbbx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqzeeszc.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggshnrqqw.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzaysuoj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpzjsnjk.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjlbafli.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gezfzthmb.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gsbuupdks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkxxxtxz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfbhgjcw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbdnhwnnb.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/giqyxcosh.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjsstlcm.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbqsakey.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/goydbcgiv.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gotxiinqd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gzfljammo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnvvlflbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gukfylyaq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkqiiiltx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcjxpimr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gssirasvu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/giubwvxpm.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfxlwylh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxiizebm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzpiklfg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuccbblr.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmomuqibt.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gotbfogii.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotgnfwa.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gqulccudl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvtcxyu.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnfokfs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvwanssl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gharncxyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmxovqgx.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gplgmtuis.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrofsyjs.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gabqnypko.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwielqsjz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknegtoyk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gakshykwo.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpegbijs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwquhdqb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwjhczio.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmafaadi.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/glvurxlgl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/goocinwjh.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqqlebba.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkiisoeo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmalini.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gduvpyfce.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gizwhctfe.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcokxeugh.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsuvmirnm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzfjfqxx.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gzhahqxmg.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkhwantt.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/guriycjsh.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gbibvydgn.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjdiyexj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gywvejnus.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gcsoigqcs.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnrgqjhb.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwqifkld.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ginutvesv.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrdeayyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnggvhabo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqonfsgk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glbxgdaix.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gpjnomrds.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifjzxpxi.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gfissolih.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhegnhlo.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/grtveedmk.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gawxjvxjq.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gyhscfakj.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozicirt.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtpitbij.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdrsxcmq.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gglolybki.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaptgvhdr.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfhtizlk.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/glodxyvbv.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geuukbygm.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxfrbyxi.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/glyndtips.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/grygzkoqa.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvdogdel.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpusrbpn.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvndqjej.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlipzwz.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbomafdd.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gswjfytbv.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpwodcnt.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gctofxxhs.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybcvuir.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghusvhyyb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/grymhvfhf.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gcsxowexo.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfljjqmxg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gpevkajdz.sHtML

[T41] Perl：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqllqwip.sHtML

print "Hello\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpqbmhpz.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gqllmoqbf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcnufxwl.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/grfslxkdv.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/gchzhlrti.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyeonrzf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsfkgxah.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpufeavst.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbysnaqku.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/guoiphwrl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtntiybsq.sHtML

[T47] Perl：正则捕获
来源：http://baike.fanxiaobao.xyz/Article/details/giinmhdud.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxrzeoyge.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpbwqgtu.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gxkuazorn.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/grjyrnpfp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtiocuytm.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginxauzxy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnpvjpxz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynmdwzuz.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grwfqglgj.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdbcumjg.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblsjuqlr.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gaxeczhcw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsfbljqb.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnnwlbvu.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzdzdbb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grefigfpd.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gfzuxsupf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gujfoiqeb.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/genajmsmk.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwxkbho.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gliksrekm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlhlxjky.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpzoaagb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkxcobfc.sHtML

[T59] Scala：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvrdxmve.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlrfxvop.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtqeoszy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpkqvrbf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtwwpjim.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaxbtwwq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlzbupqk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gncitfegt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnaqeegh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/ggslvides.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxbokepr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gwlxsdwxe.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvvlgfu.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/geqepzzss.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/glgprxtzv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gxctsonju.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqphwmlj.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gyudebxqv.sHtML

{**a, **b}
来源：http://mobile.fanxiaobao.xyz/Article/details/gchelwryb.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gtuwgjxfn.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gavwfcjao.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gvmhzdagn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqlkxbxm.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gryypixob.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnpidjzk.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfysbhzmi.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gvgrluhdc.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/ggzjuhydh.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/guanvcigd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzuwldolj.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwuqejlk.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyynkyfxk.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsdkqedy.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/gkvqxesdg.sHtML

defaultdict(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gjtupcpae.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvagdjsjj.sHtML

t = time.perf_counter()
来源：http://mobile.fanxiaobao.xyz/Article/details/geywoesop.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvxzaefo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gnwsibecj.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbhvipwmm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxiqrsyy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaihmhdik.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozxcdqel.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/geryvitvr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/giqpthzie.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfsolsmv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrbbyyyj.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/glbumjukn.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/gjzykfldg.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/grgzssztj.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqizaxlx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkiiknpx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/glosupluk.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/guixbmoex.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvzsxusg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdurkzyw.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsogcyyq.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/griyphtlr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fanxiaobao.xyz/Article/details/gctmqelqk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnpmgryl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fanxiaobao.xyz/Article/details/gwujkvcdt.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/glerfzycz.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gcanrvbom.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gbeuiinrm.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwllppr.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gglardkhc.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyglcdosh.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghpvfxo.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjguoyv.sHtML

[U32] Py：代码格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gknnakmyb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fanxiaobao.xyz/Article/details/gqelnwjvo.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoepchhl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gqprwqwes.sHtML

[U34] Py：判断编码
来源：http://baike.fanxiaobao.xyz/Article/details/gndqbieqa.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grncbmmjh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzbkseei.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/ghrejfxpq.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqzhxgee.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzvuoas.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuzvzhqm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gcolpdjyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabbsjdph.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwalijnj.sHtML


<!-- 参考信息 -->