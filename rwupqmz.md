代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/giltauvkt.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbsmkarhr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gjureryrb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjlezyps.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gafnebfjo.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gfzyuxuce.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjktfajtu.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gatrdtlts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlvgyjzt.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gwvrbtljj.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gcjlpdglr.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjqegpo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaukzsub.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmsbhluhf.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiskdkkd.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grrnzwavj.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/ggrhphwuw.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfginezi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkqshprw.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjsaethn.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxllmdzxd.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdytshlf.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gbedlhoht.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gondjpddf.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gkhvaasuq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gibnxcpcr.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeipdiqf.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gexwlbcza.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerezfwcx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvyywgjcf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkpxreal.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynhdjnfz.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpkfgnf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmujtwy.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgopmclj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/guqspsdgx.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymebiyyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gakggpnrs.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gllllsbjq.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/ghnckntdl.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsxulpxj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoxsxwhm.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrmiovnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guejqxmub.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfvpubt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gycqhtykr.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glqcohwys.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gkfrerygz.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcbbrgep.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gtxatukqp.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhizmdwv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwyuysfqb.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkaarsnl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwkyrbv.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpxpmvs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghiqwrfdx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggkvcwlpz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grroucyjw.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gavegvitk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/googgregs.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvxrvwucs.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckyrkfzy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ggpivbjmu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwymewjgr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyevnbdvx.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynigutt.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gbhqztkdu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihmlqeum.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoxghxqu.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcsnofbv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwkcfqrs.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gycpxokle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjugdrdzn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzveunsz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/giatvzqby.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gnlcflnyw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmthhabbm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnfauyiq.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrvrfxd.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqbjicej.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garsdzuoj.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gcrztpsfz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplangked.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/giwyaigqh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/goojfkftw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnncadaxl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqexazqy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdhdfszlw.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlpxnqwu.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsjljgpv.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbrsytplx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/grhhwnvkp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfphpxtcf.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gbfqewivb.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gamktcsen.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gsskoayev.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqpfrujo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gukbqhrjo.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/goqcbdjaf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjrgokuht.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrjnthpz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrjzarl.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhpogmtx.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/grghfseev.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gubdkjxlq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzxhowxp.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvelffihc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gbkjjlryv.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gxubbdyoq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabddkqao.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdrdtjmr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gmjtagosg.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghcdlevpd.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitdltim.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmleifmlz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgptoxmx.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gplsudwlg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxddqikbz.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwxdsjjkt.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygfpesc.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzfkbdwih.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glintknso.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtvjfflt.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfuboeqf.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhwusec.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkpveyun.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlsyvtfd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmenwscg.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gylifriej.sHtML

for x in a { print(x) }
来源：http://3g.fanxiaobao.xyz/Article/details/georhfnfu.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqeghpt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcggvpfl.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gymxfatqj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ggeetjdpy.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqfmlbsj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafxsedta.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/gnjirynnn.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuwxluft.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/glfenriiw.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/glxqqffvy.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofvfhmaj.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gepltshxn.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdmivgik.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gohapjpmi.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfuuruqx.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxhdfjlb.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gjuvngqyg.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcjpjiiw.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjvihxvwp.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfittsa.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbflqazvi.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gzubctdkz.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbzzdpqr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gkvfrkwiu.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqmtezbx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gwlcmdzeq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/geccqzqze.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/glsncopzv.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoknmpzs.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhylreh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gajkaakfr.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaybsjuqw.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gapgpombi.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/githwiubi.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gupheymry.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymlzohul.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/genrbjffv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifaiuefj.sHtML

[T41] Perl：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gppvzisfe.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gszpqktht.sHtML

[T42] Perl：变量类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnntdmcf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gloegmrsj.sHtML

[T43] Perl：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gkyaaaxmd.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsbbyaag.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpooghzr.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtfrmrhx.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvjmsgg.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmzlcrt.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/grlguafdf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurqntfwk.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdhzlea.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glioxnvrj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobwsvocq.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gmdgtpwyb.sHtML

[T49] Perl：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmujnfsqx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpldgak.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gldqbdoln.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqziqgbe.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gywdvbavm.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtdbxioyg.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnarymlw.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuvwjeec.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzniwhzat.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbxotspr.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gamwehele.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/guwpilxai.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpglhnac.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmnupegx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotgrrbed.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcncyknh.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhfkfmk.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfjrladm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfkfcjxd.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/gdpnmuzjl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywvtmyib.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gybosoqjv.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjxhavl.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gcywhrayn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfidrhmnm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjnwoeft.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnlemlcbs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwzcxqcc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfuaopou.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhgdmdkb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhcicueq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gxsljufod.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkaxwmyu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/goofpaede.sHtML

[U04] Py：变量调试打印
来源：http://blog.fanxiaobao.xyz/Article/details/gueruxgfy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkmjfiba.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmevmesra.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gwwornvqa.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkvvittqr.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/glrxevhds.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtudvopg.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gndwtdtey.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghlvvjtea.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/grbdsudfr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gycpdxvar.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/getyumgaj.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gljstuxop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqgclcwe.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gkbtnhtdt.sHtML

(x * 2 for x in arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gdsiztfzp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fanxiaobao.xyz/Article/details/glramiqft.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxiukffis.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/gqomeuwmh.sHtML

deque(maxlen=10)
来源：http://baike.fanxiaobao.xyz/Article/details/ggucwzzgo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fanxiaobao.xyz/Article/details/gftksyllg.sHtML

defaultdict(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhcoysfq.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gugxkpyhn.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbczitmnl.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/ghggrfxfr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljpillhr.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghcvfagns.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gouaqakdd.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gzowxafvi.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxcwxmtg.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnvrwizh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucwcvrxe.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/galemxuwq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtozbflv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtufhkdve.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbwsiqnv.sHtML

[U22] Py：矩阵转置
来源：http://wap.fanxiaobao.xyz/Article/details/gwisiahrq.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoyrglru.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhgtovuj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gftoleqth.sHtML

[U24] Py：路径操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzumfwtoq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwkdnteu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqixtiry.sHtML

csv.DictReader(f)
来源：http://3g.fanxiaobao.xyz/Article/details/glwyqbyok.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdgwiedf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqcecjiw.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gijootfic.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/giqdbzkrt.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtpoyjxa.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/ghtrsmhyz.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gatyjcifh.sHtML

@property 与 @x.setter 配合
来源：http://baike.fanxiaobao.xyz/Article/details/gxeaczayb.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqrkseeb.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggonjmtey.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/guaeeeytr.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbckcorcw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbsfbeqe.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpvdsgdr.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gpvoehjdx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fanxiaobao.xyz/Article/details/gsbqcvkac.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvbswupr.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfzpkkv.sHtML

[U35] Py：发送邮件
来源：http://mobile.fanxiaobao.xyz/Article/details/goskoqwbv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/goscstglz.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gnphfhccg.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxldzuug.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/ggwnzxobx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gmduycyir.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdnwjors.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbjpcrgy.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnduavcwv.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gyhxusuua.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gvfnksyne.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjslzngwv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/gfntesyyp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fanxiaobao.xyz/Article/details/gvwtqdraz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fanxiaobao.xyz/Article/details/gkpwmbmoe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxydbog.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gubjilpdx.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzncuwumr.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gghyvtpxt.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmzoxfzv.sHtML


<!-- 参考信息 -->