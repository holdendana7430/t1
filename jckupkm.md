代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gcveiofcx.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpmugecd.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gksovykpp.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekdrcdk.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/goeqcuevu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhjfliqa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ghpgleyhs.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/genjzmffd.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gkynxjugu.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gprafieqk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtmddlil.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/goxzqvdsg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnilfofxs.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gelegmupv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gadkqgvjk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gkkywpesh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklrfshed.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxjnals.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gfgbidlmk.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfrpmyqma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/guqdcmazx.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gddjunbhp.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/geiyqglld.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkzcpxmw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gvypribre.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnrjfwhg.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gkaknmzxs.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gepszwkpx.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gujzccwaw.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwruroed.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzelvyzq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbnoafpe.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiuxzhmm.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtffpebpj.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gufqxqykw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goznbwvls.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxirwtcm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblhekucm.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxiduaftq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gnhvvbnsz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqordbypw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelyxqezp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gzyecrbyo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkkzksry.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuzerpyl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsbydunxt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxgjosal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmzvdwsb.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoexftgx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvfdaogdr.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gztieaowl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gwyotykik.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gvreywdgy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gtqzvegjl.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqfncclxr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ghvzhneck.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqzfnnvjy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxakbkeis.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzwsipls.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmvfxjoh.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gaejzrgav.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbumkkqih.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gsnpngfvz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhqtldfp.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxxyszdf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvicsijh.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywjdemcq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaswatgsp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gofndblan.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjrarquwn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmbiygdc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/givorword.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcubnybt.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqyaonf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyummqga.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxsvsemgw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gglupgmcm.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/giiciyzad.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaqjueds.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/gsdgugdjm.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxdldcqrl.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtqljxwe.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadmfoeis.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghielnszg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghstvlueo.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/grxlwmwhl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxazixkia.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqnwjwfo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcxxshau.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeegyrnd.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilwoyoxw.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcywmncc.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopkqjukx.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/geewpxabz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncimocmv.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxzcacei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gjodgtuoz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpozzjszk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbzbvqir.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdvgkvyig.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkayarcc.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxdciuhci.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfgvslx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gjqdlglhr.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnaylegd.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrbjnmzp.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/glncpzvfv.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gqwxadbwl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgxczmdt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gguwhffqi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdybvnvfy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhutacae.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gibwjtlor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkywiwctp.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gddivplyy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfusfrumu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyehxzwe.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkcdokfn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggrzowiha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnirmcqwx.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/guljdvvac.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnwdvqds.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucwbatmr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrnmmqim.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gyovpmejn.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gythxezor.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/glxthfeyi.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyoklekk.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gahxuombx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnbmsmlz.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwezfkjpb.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glqbijrbu.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/giqwhxvch.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/godxnkibu.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmcwwjrc.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gdwmnnuvn.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxincqnhp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjuyrpls.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqvwqrbz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdrawxfe.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gzkhliwrh.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnmxctl.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkokhqjhk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gssajcpna.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkfqpmmes.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxlhazqc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozshskil.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gxvgpljkj.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gogzgmxhz.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqcftpzt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybuznrjo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giswclqxn.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gqwlhzvsn.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/ghttafoiw.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gusljsoiy.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gzmxxsant.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gibitaqzl.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gfttzovmt.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gtumjzmwu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqjakyot.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyzkxwha.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gzmenbrxw.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoyvwjlm.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gxyhgxbdr.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gzykjzoaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gxwrybtqd.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gfhmgshul.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfknszsqv.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gxytyrfke.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokgsgmjx.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/glgafzzxy.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gnebghxzn.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/goqyshivo.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvsieatn.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxxyjpgy.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gqtdusptj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gexplaaum.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gylvdkfjm.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqpjqjcb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqxivpzq.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdksqumus.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghutbftsg.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/grrlpxobo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmtzpdtf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggchjohgy.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpakhxqeb.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbekckzqp.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgsbjkg.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gajnfloxz.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcyxegmp.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gvdnnfcdj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafrokhfz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqicoqkpi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmyniocgz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjqwqdx.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gdggspupc.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilmgolkp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmkqcfir.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyikzyowz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/geiivlwvw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gswilnuhx.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/glmxdxfxo.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glodchgcx.sHtML

[T52] Scala：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqvkgfpzv.sHtML

val a = 1;  var b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gduahyhxz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujxwsyg.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgrcwgiu.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gonabozro.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbmusuvch.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gckfucwdq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnwcbesc.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gistaxjcq.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzalpxc.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gxujqhhow.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavyvazep.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqacplrf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjlkkqpi.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gubrvbkwa.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcutguoen.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gksayvkmc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/geaiocltv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggwfnmyki.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gonjiubsg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmspjugrr.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ggilfrqxa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkjcdrfr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnghkrjij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdamcwbbj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gulgmexex.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqylilo.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gekcwzfvq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gjuetyevk.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gusumopia.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gqqckqiki.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskikmslb.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeemdmrz.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gxcwlbwtb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gsryydnki.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/guujomjqi.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gmhppbvfv.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfsxhibo.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchfzybhr.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glchibsto.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqzbrcqj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfpnnrwk.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/grxvctfde.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpezpeeg.sHtML

Counter(arr).most_common(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gwegpaisc.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gnwwshwac.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gvpjcslnm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gkdxkdkjf.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gsafeatjj.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gandbasto.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfahbbnph.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbrjatzj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtizmstds.sHtML

[U17] Py：初始化日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqdncpwk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhslibsp.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwidaxdps.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gblulzmrn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrsvugrt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnlduyljw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fanxiaobao.xyz/Article/details/glfwdkmgu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaebzzhue.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fanxiaobao.xyz/Article/details/gpmghzepl.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/groltwsnm.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gznwbfbas.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhigmjlk.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavaqumkv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gpoybxiex.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/gdhcighhz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghwwmfqd.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gitgannpt.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjprfwnr.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefelwywa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjqsbctx.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueanvlgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fanxiaobao.xyz/Article/details/gobsnfaeo.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gbfccrzug.sHtML

UserId = int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsmhsnfi.sHtML

[U29] Py：属性校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsfclllx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gotbcunoe.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcejejhr.sHtML

@dataclass(slots=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gemhpdsow.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/giitbndzq.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbrpzgqa.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnflalxzv.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtnjwbln.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbwwauyc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gndevavha.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/giykktdwe.sHtML

chardet.detect(raw)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxoyhrwg.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gwjktrlnx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gvchdakcw.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gpzkzrucr.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gqskhpxpp.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/goqmmblby.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdbzorv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gopblmynf.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gadhjgvoo.sHtML


<!-- 参考信息 -->