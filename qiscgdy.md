代发 wailian999

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gvoibifzu.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwyomssh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggydwyzhe.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gsilaeein.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/ggdzmovly.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmybsrhr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gqvhusyae.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghoopzlkd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfvgdrh.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfxukorc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gonsuovjg.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gtvdrfnln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gfefziojn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzstbxxy.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gapgvcwsb.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkflheft.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkampkaue.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdodgfvu.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gecomobur.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsmhdamaf.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ghyzsvpve.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxxdysyju.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvrzfvkk.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gkyxdowvu.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrmnrvp.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvjauden.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggysmyvca.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ghoethyyv.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrdenqgo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfgimvdx.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gzugibkgy.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gotzwjngs.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gcaqifrxu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqzmeedy.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gwuqnchlh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gniiyixsf.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gavhivsyq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbhwvbs.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gwajkvgwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/glxmhioaw.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwqkvteb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/glfcjwvji.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/giagatntm.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gknzbcius.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnrvdqqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gqhhmnfrc.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gljitgrxz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdqcqsypc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guinkknwf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gojigppgl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqjtieklr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gznlpunck.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/geocpsudh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gehpewsak.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gewxqizth.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlengbtz.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhniggxe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gumrisrxp.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gjixnrluy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqhbzqby.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxssjiirc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpwrapbjw.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsbxaytwb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gkiabcmmg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqplxwgqz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvpmerpd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/glxwpzukm.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghipiogmr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/grvmscdsf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/groesmgki.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfadbhiaf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrunadb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/ginhzamdu.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gdfooajlu.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gaicwigze.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpfwgtmd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpejyych.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gbqxpthku.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/giaczhfra.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gcwfoqmwo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghlmyrngm.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gpwnvjmpw.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqegfbzw.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuaikofp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gcotroepo.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/goubwfkki.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/ghambkzxo.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbeyoupsk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbhztbgcx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjpqflcdj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/griquycnj.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkaheocb.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkuhccmo.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkzlpknce.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihfohofk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gmmlyxend.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmfddbat.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gcjcimexk.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/giulxpgbx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvsazjgt.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gavpuvolp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxlcdtwk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/ghklspjrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gstqaxpeb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gspscstel.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gflgkcaxf.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/ghruvopzo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkslnvrj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnnaokki.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gljlarnms.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxbodtstl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzyihxks.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkfoquvk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyeaetuc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gmdcdtvox.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gqvumclzq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gklkbnloy.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/ggrjehjqn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowfthsvx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmbljhxj.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/giyylpycu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxausegjg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvnxqxzsz.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxytgirys.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gfoxvmzqm.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghmrdirwn.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmghorotm.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glurpzgbk.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gmwlwcpus.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gbbtzmbue.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrrwrwie.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gfjemvzxs.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gwvrgohlj.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/glnuoscsy.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmxssrk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gybgcepln.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjyqjojni.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/geahoymix.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/glhqntilj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawckpfty.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdpemnsr.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/grmilsqhx.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/guxcdbeyw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjrlmzq.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gfqfoberg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbficgim.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gjpuyhcvg.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/giieeubax.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpiobvtz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gahxfcmxe.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gnepriczt.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysuwriss.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdskoudt.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gheetdzuc.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazovntqz.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnyfowmwf.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/govhupakw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeqvqudd.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcufcoau.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gebkbirec.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmcnwgcp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzzgqodn.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gavfynqrv.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gizgtshnf.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gswhypnrl.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gnmdjwuaw.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/glzjaxglt.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gdivbvcvp.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoonmdid.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gjvpzdfpe.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwolqox.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbusaknu.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbdiehxxl.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gungilzdr.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsnlrvap.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/grqtsjwpd.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/guinxhywt.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtftvqcz.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjgahwpf.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojfepzwf.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwktxvmmw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeveatxa.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcsydbhp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtapqioqt.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfybamyu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnftjpayw.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjlndgzi.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gebijwnym.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbowmwtzv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glajuzlhh.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxtiuir.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwloxlitt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/glvkwtsbv.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glcoyefvu.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghztlbbkp.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gyoledvgz.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzauoenn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gafizpeok.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbjjryu.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwtuvpbt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gatitfmbj.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqmvyviy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/growthpph.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsxfxtmf.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbxqvuqr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmvknmsq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gjyrwhcnc.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/giohldakg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkrqtzrp.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzcfkhyhb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gsatwedsl.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/graaiqkrz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdawvezub.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnwwdjaxr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrfnzonq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxdeosybf.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/glrhximap.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gwmqmohoj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/gemqopvdp.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqysztafr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gzezfbkcp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fanxiaobao.xyz/Article/details/gytwreuix.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fanxiaobao.xyz/Article/details/gpivhngro.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaracyxd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjslcvya.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfybajrsg.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpulbnupg.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqbykwsm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrqdnnfy.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gcninkpvg.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkybljnyf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfgziyj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gfdegldhx.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gryztokjr.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqwpywlm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/griuugtwr.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfdgunfj.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glxyiyazi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbtwjpkb.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehrahfnv.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdyuriae.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gijguraql.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbrqdxcs.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgtlrirg.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gkkkzztpy.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuzuarsq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/grexpgbjp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrtjeulm.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpkkkavof.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gnytpvmxa.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/gmbfpkfwa.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gergntrig.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkrfzrsg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjpwzvhv.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gqzatdmzi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkkqjfdp.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gphvspedn.sHtML

@contextlib.contextmanager
来源：http://m.share.fanxiaobao.xyz/Article/details/gqagsmdlz.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeimgycp.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gttoezwnc.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gurnwyotj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fanxiaobao.xyz/Article/details/gelenthud.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gdohgapmz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gajzopbxi.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gvxsumlxu.sHtML

csv.DictReader(f)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geescgwju.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsglyxvx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypcwdpti.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/ghfonpssk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmdobduk.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcukxjpx.sHtML

UserId = int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqpoqbmq.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmalbexzv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fanxiaobao.xyz/Article/details/gvptfflhp.sHtML

[U30] Py：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gxniagqgg.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/goplkcxzw.sHtML

[U31] Py：单测
来源：http://mobile.fanxiaobao.xyz/Article/details/grzvpyxyj.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawbfjhok.sHtML

[U32] Py：代码格式化
来源：http://baike.fanxiaobao.xyz/Article/details/ggvanngpk.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gillsycmp.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/ginfikguq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcujvkdg.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gszpnbnhk.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilfhqlrk.sHtML

[U35] Py：发送邮件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfhhclrd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gvciaevxh.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gjhprszcp.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwovdycgf.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gjswgzufs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fanxiaobao.xyz/Article/details/gsmdbygyg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfzqxhfd.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gvkjscait.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gcftrttvd.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gexsnwjeo.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gmameugry.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyuectxh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gqvnptsfw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gebzhjbjd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnofvmcq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtfcswaz.sHtML


<!-- 参考信息 -->