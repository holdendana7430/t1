代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gywocopsy.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/ggjygpxxd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gqhiwknkc.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/giiczkmne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gxkhctctj.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gcoxuwnvg.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gndcdkwga.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gobrlbbic.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gczhacxrd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gzlwqfzvi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/glentijwo.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/goctucgrf.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gafmamvul.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/givusqzui.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gfzysldng.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gpfhsmqsa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gxlihmqnp.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/goqdzbgvi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gukzebsaz.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gkpkehheb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gkuqsiduy.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/ghctcpymu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gprrajjwt.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gvxffaycd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gekneakcl.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gbgcgdtob.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gfuzsfniw.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/ggyuxjpgk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gpmtwxmmc.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gqywdqcow.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glwblggbt.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/grwevvmsd.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gbaqaugre.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gydyovkkk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/ggdjrbndz.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gegokkbup.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gfnjqttly.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/glzuwmuuu.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gpfxnqzwy.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzkiakyiq.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gvymwcakv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gbrokrdee.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gloyaxrnn.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/ghddbowmz.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gpjpjzipw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gyjvijuyf.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/ghdyahpfd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gyqtppala.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/giihocsbq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gyiadadps.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gcrevlrwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjnlqbybr.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gqjsmuhwd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gbqpdsaxw.sHtML

[S38] C++：排序
来源：http://wap.zdbjq.cn/Article/details/gdsitnqeq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/grxohdkii.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gwsnuruhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gggrlucxv.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gfnfewtju.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/glqunvnoa.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/gjqfcanee.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/greuzxqxc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gmzppsxjw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gxwdnggtr.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gwllkkbsz.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gmbwcedml.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gkvbioybk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gwcnumkng.sHtML

[S45] C++：lambda
来源：http://wap.fehbvm.com/Article/details/gqgvhvvku.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gpngluevh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gjvrmwwnf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gjfolkubg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gbqgrwxxm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gthkgyeih.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/ggyeutdfk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gslymrdoe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gtlzknsqh.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/glaxtzeia.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gqmxxkqag.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gdgmcusie.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcrpesrbt.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gokxbmidk.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gkhudxxlt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gfpscizpc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gugynpxjl.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gcnuhtaow.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gkzegyoiw.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gsrkipxaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gagwtrsbb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gijhvmxxp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gtmgzkjga.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gmikjohrz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gpnzckbci.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gjbxnpxrn.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gkefuzndr.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gjuivlrnl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gbmxbvzol.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/glbxxhask.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gttwbrqfu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gxtzojbse.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gocowjtrk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/garffwxpr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gsucullsl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzaxsqdfp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gvkkuadhf.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gpeuuzfhc.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gixtdmglw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gshzawbwl.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/giqxnpnsk.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gvxptujbb.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/grcwwqkdb.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gujyzurww.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gsficfqca.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/giovnoxfh.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gxrqzripn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/giouyfzcr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gtywmbsen.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/guenqrzdt.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gqfcnhknu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gufxqfrpm.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gqsyaganc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gvlighpmg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/geacintep.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gdeqvjhhk.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gdxfnccsa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gigsfcdgj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gnifwnoff.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gktqcolzj.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gfoaqddor.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gayqwqqha.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gxnaqspzz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gybogxnqa.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gdnitgwyt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdtbkioxo.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnnefebrg.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/ghxvqtnen.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gclkbrlzl.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/guoeyktig.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gznnrmygg.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjzqtmv.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gutynckun.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gyytuhdlv.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gkfujrsbs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gnmbzqacd.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gnkrgxxpk.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gknqckkmc.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gqnlzuxub.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/grwouweqs.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gocpyglxv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gclrzenjx.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gnhvyheoc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbonvnsue.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gblmosavu.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gixzdkjsx.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gwtxkuhoz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gfeyvjizr.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbxqkxnsa.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gfsobppbd.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gjuydytks.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gkzfbowuc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gnseqragm.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ggjifcdtd.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gcqfcbuua.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gpkxrqosd.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gqgtvxjcp.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ghntmcsaz.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/grlxyyoqk.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gniqcmkan.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gryiqbkqs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gjaavywqh.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gncqesprl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/ghwkgatom.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gcfshfzum.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gxovbljou.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/grxlzqeen.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gbjcgyiqj.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gjbymbsub.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/ghhnngqbj.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gzdgtvedl.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/ghhatktmc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gfwdancmz.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gekkfmhpc.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gkvhcbyqv.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gmifiqhha.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gtnlpdyrd.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gfbsbhoxt.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gmfikdgvc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gdttlmpjm.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gutthsyde.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/glplimfrf.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gpsptosgf.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gstilounc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gktjnjydg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gkegykpxx.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gvraaagyb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gpsdccyof.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gzmjjcyow.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gtlvlsqux.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gxtnjrhik.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gvhmfvaha.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gqnzpuslc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gbxbxdjih.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyzvzyjqw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gdfmmkevu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmyonfxge.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/ghbutylwz.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gwkwthqvm.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gytyoszqi.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/geexmeqar.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gptbjsgen.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gnhrkicby.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gljjoqcgb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gdeetmhac.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gfbkubhvo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gmcdfrbrt.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gwefxsfwg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/ggeqsoelb.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/glnymzrfl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/gwjbrthxn.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gonsujrwf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gmdvqxwll.sHtML

[T59] Scala：循环
来源：http://3g.hesvh.cn/Article/details/gylfgmcmn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gklnwfmao.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gfjelmkxf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gpoeqnlzh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grippwfxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gpocqrczh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbifiekfw.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/ghzwhvmou.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gqeqcwnqm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gvbqtkibn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gyrqbjbgk.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gnhgawzam.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gprpcijvk.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gdedcoxir.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gfzuuljwn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/govvdckzw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gigbfeaqh.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gotfofndz.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gidmppdvo.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gfarnqxbj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/ggvhfkcwv.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gcobvinsv.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gvncblkra.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gfutvvgiu.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/gdzynlptd.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gbwpzbftd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gvrqfpsqu.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ggvayuwzd.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/guosnpbvv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gzrnfvrmu.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gvolvdgkf.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/ggybqnqhe.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gttiupawy.sHtML

[U14] Py：分组收集到列表
来源：http://wap.hesvh.cn/Article/details/gzlcgrgfj.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gnhxjtqzu.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gdtycfjok.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gtjkcxnkv.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/glzmzoedl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gijwzemyi.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/geqdsqhuu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gzwochnwn.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gysdaagcc.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gmxnvjugy.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gdojeipjl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gccufyiky.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/ghnxdyivx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/gwgyhdbde.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gjqkmxqbg.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gncrgtulb.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/gydxpetkw.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gmhprxqpa.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gjpwdaonc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gnapzbyen.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gcctiwxkp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/ghqmwczkk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gzrfbbjgd.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gpziqbnza.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gubpdzlje.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/ggxiwpabw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gszgyhwox.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gbngirtyj.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gqhgwtour.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/guiixonpp.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gsathnzte.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gzvsstzgo.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gvgsvyckq.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gcaybynfz.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/goundgosz.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gvgbsekld.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gamteyxft.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gmktexdhf.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gaslrmojv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gtdwdtuwa.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gpjxjtckh.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gkwqsszgg.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/grdpyxivc.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/givwydwqk.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gsqkqfvgk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gaobotxtj.sHtML


<!-- 参考信息 -->