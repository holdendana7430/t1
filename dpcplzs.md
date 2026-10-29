代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gtktovkwr.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gffghhrdw.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gpkoncyye.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gkzxpzoyh.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gvhcuzcsn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbetrxkpx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/goyjmwtrf.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gxipkuico.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gddugnlps.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/gkfyjuhkv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gubmnjklm.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gqzjesvns.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggtvcoyfx.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gzlrequwf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gtmkunwlh.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/goczfsmpg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gcbghltyq.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gvalfburz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.zdbjq.cn/Article/details/gpirrkjkw.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gueeyrgpb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/ggwmdtega.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/guxmpabig.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gcpmoouih.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gitppjnsa.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gwdhahkgz.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gjqpxalth.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gciauvhaf.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gfytolacb.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gmbfkmdze.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gdxcwdyas.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gcbanbpkb.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/grtpyyydt.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/grwjjmzaa.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gmhkeghbl.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gnnqdvjjd.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/ghlyzcjpo.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/geglovpwg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gugvoeemp.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gqlvokjzk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/givjgfibx.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gfcqtapmb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gmtwrphkt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzyayqfob.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gtdduposl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gjvwdzzss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ggeukvooe.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gimpngphx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gtqnknuxy.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/glprbsovy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gszrdbjkm.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gpmnvgegb.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gusmztytd.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gypbefmib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gyjcieccv.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gxbubsqfn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gshvkxjyj.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gkxilalfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gcmzssccg.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gkjqtisco.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gfukoyket.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/ggvrhgtlw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gwkplvufp.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gpijhyetp.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gczaomqte.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gpoocatvg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gijtmfowa.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gkgmmtkpk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkoowxtxn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gmrgadtzw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gacqmsltd.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/ghpdlyajd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gedcnluem.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gaiztkpqg.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gjfnbminr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gwokobjsc.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gmmxgdadr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghvmvqzno.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdguojmue.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gwadqvehx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gpptathzv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gymgbedny.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/glmezahoy.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gipernhyy.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gaswabzag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gpytuhcnd.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/glcjnqnmw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gtamqghrr.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gepkzbeaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gjglavius.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gadwbrrgy.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gppgflaom.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gsuqdrhvy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gouzsmiby.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gluygmvjn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gpkatcbpl.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gwvgcjzmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/ghyzfwbbp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjoohghkl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gmgpjhlhn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gedshktst.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glntrlkfi.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gupsbkild.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gducvjrps.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/glaurpdqu.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gqjgmvmws.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gdxepywfz.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gcaekgfxz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gfissihfx.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/glgmwimhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gerxrwufo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gstkthepx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/glqzoffgi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gmvhnnwnj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gmtsprfrz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/guutuddyz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gvvrkfduw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/ggimnnazj.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gtvnprfij.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gngrybmnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkhsuhnef.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/guveivqal.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/glbsurhqu.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gtjhtjywr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/goewcisfo.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gwfgxnadm.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/glwpqjvkt.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gbaiktprg.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gjflnjahh.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gaglyzmgv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/ggidpqlzz.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/giwczyeja.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gjzqinrvo.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gsdzgwzxc.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gcetuptgp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghinvcazs.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/godqgaels.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gdeyrcamp.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/glrcdfpsj.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gjybovkqf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/guohuazmf.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvpsntgks.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gxpimcgrw.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/garfislmz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gxmrulssd.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gdhuvbnqb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gqvfnozbg.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gjwsfsrde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfgmwwcpf.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gedgiqpoh.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gvyrjywti.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gcvxkpyah.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gplfrptfc.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gcgrigevn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gldstdefc.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gsswkhxtu.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/ggdedfves.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/glcitatzi.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gtbsadirr.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gbolfzdbu.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gtymgwqdx.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gzuqcekxg.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gyddlqxwd.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gzzlilckb.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gpqdlmmwv.sHtML

[T33] Lua：表（数组）
来源：http://blog.hesvh.cn/Article/details/gbwhjzxrr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gejhncjtt.sHtML

[T34] Lua：遍历表
来源：http://mobile.zdbjq.cn/Article/details/gnbkoaava.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwnwregst.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gyppqanqi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/ggznkchzp.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gdvwubtme.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gnqgkmsiq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gjifpkfbo.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/ggagcwquw.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gaaoypsxi.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gkqsbwqxk.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/glmggzzjy.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/givledqui.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gwwgiuppg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gmzqtzbmu.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwigokjso.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gyjnzxoub.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/giuaxxawx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/ggixldpak.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gtpeyzmtd.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gvufcokeg.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gvtgrdofm.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/ggloegqwc.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gphubnykl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gugracptk.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gnhnojudf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzvclokkd.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gczlcbjju.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gylolbqoc.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gmyeyfxtl.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gbsukxomc.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/grqwvdvne.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ghvojfskd.sHtML

[T50] Perl：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gvzhwmoao.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gcyqswygr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gnqjctgsq.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkpbkigst.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gnecsexar.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/geqzwejcj.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gqmkxufgs.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gazappbcs.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gekycnkvd.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/grydqppcx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gkxjqoxgn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gnvnjyblu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gpinztnhj.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gqqawivvu.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/ggmckxsfe.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gczmpevvl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/ggxiumdiu.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gqfcqdsiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gtufldyhg.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gduhonbst.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gxfbtqoqd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/ggbjivknu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gxtjrpbhm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkllrrqpk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gtpkkodgi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gopemmrxd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/ghkuquyga.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gwhytaowi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gjwiwalaw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gcudubzoa.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gxezlhhqg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gwphvoehm.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/geazqqkkb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gbdeqarfu.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gdexazqab.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gszsbjsym.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gnlkvgudg.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gybjrjkft.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/grpmnorbl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gfymfbxnq.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/gdbwtdjjf.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gqvpethnt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gnqpuixmc.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gztdokehu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gohwzfwzx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/glbpoiafo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gbaobvudd.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gswcrokbl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gohotvmus.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gvfcvskdj.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/ghtqhfuhi.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gtrozcyac.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gygiajmnb.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/ghtbmowkw.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gzaeimiys.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/glwnwdtrg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/grhrqewps.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gnotewesy.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gztuxheha.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gvsikveln.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/ganfzancw.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gzbjjjpbi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gkytvosnz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gpsxpyyag.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gvnjxttye.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/ggzgqhill.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/ghttyvayu.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/gnllxfrgm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/grzvhzfud.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gdoppgakr.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gixcpmssr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gvyavlqpw.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gousrhove.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/grkdyeccb.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gtpnwlemy.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/guhmvgptq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvkmdbt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/goiswcfzb.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/genvgsoiu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gwhniijyo.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gituwsncy.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gsdxjbxvs.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gcsckwxja.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gxchplwef.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gmduhtghn.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gbnvtzyjw.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gyutthgio.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gzydxqazv.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gbuobrsle.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gzadggixa.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/goulhdxnk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gumepvift.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gijycvluq.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gztpgfgfy.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gtwmkemsa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gwvhblrex.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gvxugrbiy.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/grtdtszhy.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gvjuxhsgx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.hesvh.cn/Article/details/glnnajhhu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/grllipuwx.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gadtzcezf.sHtML


<!-- 参考信息 -->