代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gtsacghro.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gawwwluys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gaaeqhqrg.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gcejalexi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gohsynexc.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkznqohve.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuvlkwxa.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gujskfgcl.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gnxvrpkrb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvfvclsh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbyjmbua.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gfipegelm.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gezshkxwu.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gilhltuft.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/geoyfausq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgeznvi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/grazmaigp.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmuszdoj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnookjyqp.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswguadds.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnkglktd.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphkfjmdv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtrsibws.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwcmsxyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwuzthqm.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gzcgaxbbu.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhwacruz.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gaxkltrcj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmxkcjt.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsybpjwqt.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gqnjezyyd.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpcjdkft.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhtynxyr.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxbfxxui.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqfrvwgv.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpiisjjx.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsoytdfcr.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gljieaaar.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglhwgkur.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gffdfmqnw.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsznnvunn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guqlwcdyc.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/galtbqhhn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gykungcws.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gbxfzjlfr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqxduajh.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gnabwkvit.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjekuiat.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggybdxewt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzxapioi.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gpckkicvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdmxdlhu.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/geihwviqk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyrubans.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gedrbvxpo.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glhjktzuh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvtkxfosz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsxmetct.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gyarhzacc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxtppuos.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsosiesqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujwroagv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxjvppuff.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqdoarep.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/ghtxhglez.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gnrvkebtp.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gyszgtgqx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjpxfmud.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwklseto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyeybenf.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsiiketl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvoymfzj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ganklhsfb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdnqlizvo.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjgktbvvi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gflcoljed.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszerhggh.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaqbkimkw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqqpkdbn.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvqrepgpn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gvhnjodai.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxdenlxzf.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwwrnyegm.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/geeevmcrd.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasrgyumb.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gihyklogm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhobrwat.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghynxxpzg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkyzdgze.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gkipottji.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjcscmab.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgqkhgma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gorivpliw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafkvssni.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxotftgbl.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjdaolti.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gtzdfcpma.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwlxuold.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyfmuex.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlzpfitm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gblzxyyge.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gggfjnryk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/ggrjxjpqk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghgwcydam.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoqzxelm.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gnnwchywz.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gtmrxpwrg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gseimrvul.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gykhxqbxs.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gphjqrnvq.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gfgewjxpf.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/geeatdpln.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfmfsoab.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/glafmckzk.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gnebbebzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggelbfgmu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaymilyy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqpihdem.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gjowdvubb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjglywonf.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/guykiyjhq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/ggupreogu.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/guqdptlxw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtjnwwbn.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnxnintd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gshairroh.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gdzvakwlr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbdbndkg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvgkvpqd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gavtuynrw.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gttmwghff.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaonmcqd.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gpraztnxq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyoarsxx.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gteooxspj.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtffjyaz.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gxnfnrdzx.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gedikevvc.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxsyhvhgk.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gpubrpxdd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthasntoh.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqckvcj.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gfayomjeo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gcuusokjb.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gibatpefk.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyrkbvbj.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gmlrqzhvc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkethrjt.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gniweclkp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gmgknnquj.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gatajpxuk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhogwsfr.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gqwexhugo.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaxkvujv.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhdwrjnb.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/geprrznao.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gejvyngvh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpnjlbdb.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqvsouaex.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdajeljq.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzbbexoz.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gfpexiffx.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrwrfvnz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzzgdlxe.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ggufuslsv.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gueclgqzx.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnemztfzb.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/glpuwutqq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gemahlgzj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gogakflru.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gsfosdimj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gxhbgfafb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxemxaxm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/ghytlaxnz.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/goshbvqiy.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgdxgsrm.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedzmzwtn.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/geyhbkykk.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyicemola.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gpziwlgkn.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gysxqpovd.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnnjdqkm.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gcscduznu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/goohlhcis.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gmyigxieh.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gzocdfxnk.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdabjiae.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmlxhrqj.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzyqwbyc.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/gwencyajp.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/giuhhitvh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glzpjvsiv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgpdpjrc.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrfbhvpm.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gucdhewcc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxusqyzv.sHtML

[T47] Perl：正则捕获
来源：http://blog.fanxiaobao.xyz/Article/details/gtufsjiou.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grgleennp.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gyxdbzyrg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtqnrtqu.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjafslhn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsydglxmv.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnorofxrm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmedhuar.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxizygnyg.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/giclltkwu.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/glfgcbqjh.sHtML

[T52] Scala：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrpbniql.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxwlxeago.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/grpsixsxu.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gfxnpmekh.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gglkvybea.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkyscijx.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/germwpybc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcnyrlsdx.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/ghbgautqm.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvuapdag.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbdufwzk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqlspypeb.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gjsnkxerx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/grqjdddnk.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbcgvqxgg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyrzjfrv.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gtctgkmmy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/giutuivfc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsibetpc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpixodjsp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlksdunu.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fanxiaobao.xyz/Article/details/gqmizmbgo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmquvcu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/goxuunneo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxbgfvzju.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhnblhqs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgmlqxdr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunyvmfsn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fanxiaobao.xyz/Article/details/gfomwdhjd.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtyzcwyv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gczisohqf.sHtML

[U06] Py：合并两个字典
来源：http://blog.fanxiaobao.xyz/Article/details/gckvhoctf.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/gixbknkod.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gghuctjrs.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gduxkqwaw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gknbrpsex.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gextvgiuu.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/grfumcgzj.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuwvtach.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuplhogl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxclrger.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzmfuvjp.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcwepsgg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbskrpaza.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbyxbjmp.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/gzgondqhf.sHtML

deque(maxlen=10)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjrkbomj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/goikxjzhb.sHtML

defaultdict(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxljhzgf.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsnhbluq.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvswkhfj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwpzgjtu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gqsxtnngq.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrnaatap.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrvhnpog.sHtML

[U18] Py：预编译正则
来源：http://blog.fanxiaobao.xyz/Article/details/gpqkptmew.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/govizrbqw.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gttwvxzxq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjgrrgatr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/ghgcpxklq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/garokuury.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktvaanq.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjmqqazl.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxdlxxd.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqmjjgse.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gutpqrsrv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/ghgyoyfyy.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtfqfes.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gjcebewbc.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxidddtd.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/geoquxyfu.sHtML

[U26] Py：并发下载
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkkgovxu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtyldgw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gmontmagg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glynrfktp.sHtML

[U28] Py：类型别名
来源：http://blog.fanxiaobao.xyz/Article/details/gljimcibi.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhilearg.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gyspgnbka.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpamvmkb.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gmxbjkesy.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gudtxtyyj.sHtML

[U31] Py：单测
来源：http://baike.fanxiaobao.xyz/Article/details/gpdwprdjl.sHtML

python -m pytest -q
来源：http://wap.fanxiaobao.xyz/Article/details/gyvsdpdzp.sHtML

[U32] Py：代码格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gditwiftj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fanxiaobao.xyz/Article/details/gkdecwady.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/gpzimeoey.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gueqdajav.sHtML

[U34] Py：判断编码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgppeahw.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmtntkzl.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/ghwtpbwqj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/grfjnroar.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gvnoeskfb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gisiwxckj.sHtML


<!-- 参考信息 -->