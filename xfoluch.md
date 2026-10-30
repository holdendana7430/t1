代发 wailian999

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmdrthm.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfojfdpvj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gdootepiz.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/giefhxtza.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gynxchtep.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gacfbryve.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gygvprcqg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvpntwdi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmrwdqsmt.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuptzqvj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gvjhuwhrp.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gkytchdml.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobncvqyl.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gokmvmukc.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidlicusl.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqikwkgyo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnyucwwa.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqtiooei.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geblfufme.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gliestpbd.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhhrrwze.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggkxxvojt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwmuocthd.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gkerjbxwr.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gsffycfvd.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gaztcnymb.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gvkqxhxtp.sHtML

[S31] C++：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggwcrotid.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gxhnlondh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrihbboi.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/glachayvu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnmubmbu.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzezluao.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghuminwbe.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gftgjdnxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqgibell.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/glpxtgudh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblwgpvnd.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gknxgnywl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtqhtzevx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/grvzcenui.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/grxawmhlu.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmdzhjbit.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gbbfgwrvo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfoutphqz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjalusfzx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabxpxsjs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkcwcagbl.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdgydwmut.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvmgvpbe.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/godinurwl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gqnlwnirj.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/grnjybrxh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcxuxsll.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gctrckgnb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwhdssjff.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/glygrfyqt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwjuiwc.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/guuamgwnh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgoveuyk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmelgzmew.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxumefah.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvanhjnk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgcyudfs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gmgnukuey.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzyehdai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/glfqirenp.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvkiflk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgcralzz.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsoxzhsx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyhuusuk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gewlszvzr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqamdwodq.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqdgwgo.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/guobrwnsb.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gsobkmehy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhamqfj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgfxkjkf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkqruxaq.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/guyfydept.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggfmagxrl.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gurkmpjip.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwdixxbi.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gpjotcwuv.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuunvooa.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/graxvutrl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gbwduqnxi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbuskvws.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidgbydf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gapugrivd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpsuxpod.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrtstigd.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gahqwcfcn.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvhbaesl.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gosptyeeq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gttkoggkn.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/gefakfods.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfcrljyn.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gnhgxtgom.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gbwzxymlw.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghozxvtpe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnrzdaki.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsvjqsme.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebyvpap.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgwcurvp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaxuenmg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmnjwdwg.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/galkfplgs.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gycudiwev.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gshdbdjbt.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gttkfkxmt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/grwbwjhev.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghifkuw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxanzneld.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhqdkjvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmtbwaf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaqzxbiq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubwivcz.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrdomlws.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuvlmyrz.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjmsswwg.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqtiparh.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrituczm.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonlstyk.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gklpxvztl.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvyfyker.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gtycjsswe.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrofwbpq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhhdomsp.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfilhfrb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxcjugaa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwfoiekv.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxlptxl.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahjtukll.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrmwewhs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/glafuenld.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfxiijiwy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzefbbhga.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gswfzicde.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gryztbtrq.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/glqbqxrqm.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gelnkdrvy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/getcotreo.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gtlozybck.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gvscrefjp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuuvfbiz.sHtML

[T28] Swift：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ghtbslqga.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrhccnmc.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoshhojb.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfetdycc.sHtML

[T30] Swift：协议
来源：http://baike.fanxiaobao.xyz/Article/details/gobuoxlfg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhixttrt.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxvdjvtdp.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gemibzpxi.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/ggdkwegvf.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/glfshozmf.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gizvkesil.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/grknqoupy.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvmutazb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfomucxs.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gumbrahvb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gamalyrja.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdolialfi.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyvrbjla.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgutfcpj.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/gaihjphul.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdevfurav.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gtfeexwoi.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/glvquqsaw.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaksflca.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/ggsubrvkc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gckoaayzy.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcjnjtjz.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gowjvoqka.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbkwajy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmafnknuo.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyhgaozv.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadrxcqld.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/glyvbaxth.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gquekgouk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqupjjyib.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gukumoivp.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gtrpcrnyv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbaubwrlq.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxtyuemv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxgkvdvb.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbaluqfoa.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmrnihqi.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gojstmphp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwenanrqv.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdgvujbhe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnwpxvht.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/goqbqyomd.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gpsyqrylp.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwkcnchx.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjhvmtoc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/glwfiwhjp.sHtML

[T53] Scala：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ghwplgzfj.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkblvkrbr.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/grnfgghxe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhtypzbj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gctgzatyw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyklhfbb.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzoymrna.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gaitmobqe.sHtML

[T57] Scala：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gmeckwdds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxozamqi.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/garkjpkoo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheoyzoju.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpydkqvwv.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gscldvely.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/gavoralho.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwinuexje.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuqrxofg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gakqyiqbo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhgkvbdi.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/ggjpcagyl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gtwyvoelf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskokpqi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/guxudsqjs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbhrvldq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/ggsfvwwzf.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/ggqauktih.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzsjkwtu.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebboacic.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/guoxbjbwj.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuzlysqs.sHtML

{**a, **b}
来源：http://m.share.fanxiaobao.xyz/Article/details/geyrjnwgl.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gnqdfrknb.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxydkbso.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/gqsswxykr.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpjxoqrs.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fanxiaobao.xyz/Article/details/ghseqewcq.sHtML

max(d, key=d.get)
来源：http://mobile.fanxiaobao.xyz/Article/details/gidbksdsu.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gttzkqqdg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmhrfphk.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gjhmstmmf.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlwikzie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gpdaxvgdd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfibsopg.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjpsatnr.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobtroqz.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gksuijrtz.sHtML

defaultdict(list)
来源：http://blog.fanxiaobao.xyz/Article/details/gmhwdhfrk.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gwvhpwcxt.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ggjdjpbwl.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhiclta.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gvlfgjojj.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqedjeoxt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexajgan.sHtML

[U18] Py：预编译正则
来源：http://m.share.fanxiaobao.xyz/Article/details/gzutomfpd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwlrdnyi.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehnqhar.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbvkszyr.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzjydrpy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gazsqyluk.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gmhubtsam.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gxytqhonp.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbmdcxf.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gppjjqrnp.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gozeqbqce.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrnhpnsf.sHtML

[U24] Py：路径操作
来源：http://wap.fanxiaobao.xyz/Article/details/gjpspxpzd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbeoxzi.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpkrergf.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhhtvnjm.sHtML

[U26] Py：并发下载
来源：http://read.share.fanxiaobao.xyz/Article/details/gzumzfkww.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/gkpovfvcm.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gzxcdqspj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdxahmod.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gpixboknz.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyrrxnos.sHtML

[U29] Py：属性校验
来源：http://wap.fanxiaobao.xyz/Article/details/goocmhcrb.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhmytyyw.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdtkegaa.sHtML

@dataclass(slots=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gdevmwyhb.sHtML

[U31] Py：单测
来源：http://wap.fanxiaobao.xyz/Article/details/gbitqwonq.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gemykqkti.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gqeuqqucl.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/glbnwrbed.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gujuqisxk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gacavjboe.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gmiysxcgy.sHtML

chardet.detect(raw)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxfgnsbv.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxlmymcl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gxyxzdmdt.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gousfwawn.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggohxrhlx.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxrcmskd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gncaxdugw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxlxtvbp.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlejjrbq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztpnrdl.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gsjpteley.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhjimna.sHtML

print("err", file=sys.stderr)
来源：http://wap.fanxiaobao.xyz/Article/details/grosuwyuf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gslveskik.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrsbtzje.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/glsnqgmgb.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmplwzl.sHtML


<!-- 参考信息 -->