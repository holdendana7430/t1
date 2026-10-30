代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gupmfebaw.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gfbgbfpwv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkluhgcio.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmalloszv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypilcpye.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gysfgoxel.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/geraglhih.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/glcnfjlts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjojtysgg.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxrcevzp.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyrveqvu.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gumcxfhgn.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gztknqhne.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gpwnaocst.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gjttjmbcb.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guikcvlbu.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/grbjmwmcn.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtkkmqcbe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gnhogoyuf.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gvpdylrmb.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfbphlfmd.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gxijakknk.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuxrkvtj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmsfbndg.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/ggegcfton.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebjnjsox.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmkdgksl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gozpafwxq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphyntqze.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grwfvybsl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvjmycex.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giklkexvf.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/giiroogbs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gulahxgbi.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzxcieup.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgwzmmcc.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkyarzby.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowgdmxer.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gefmneuav.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/geijwoncq.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfrsqpwej.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gznzyfwxt.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glnoiuquq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/golzwzxkr.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzkymkta.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gtohdwrms.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gsqihzonw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzugqrano.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgdbjvqh.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/geesriwod.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gusgmvqqk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grilangjh.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeorurbo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gdupskjfb.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvgglznd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmmrmnwg.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtznzdy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnifumje.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfasfbfe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/geprxsjcw.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsacemgvj.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/golppaltz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerivbegc.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwdaznen.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyajcmvvm.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gbhvrwztx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gspffbepl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gyxuqqabz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrfudhvi.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gmndibwdu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgmhirxp.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gcdaidjqu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxqnehqm.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gdqzmygsm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gsmtyvbrc.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gasltenqi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwgkkxgb.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtgploaxr.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gcnyhrufs.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gjpyznqie.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvzaups.sHtML

[S59] C++：静态断言
来源：http://wap.fanxiaobao.xyz/Article/details/gwnawzaro.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/guaprqxul.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmmkcqkz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gfmqrodie.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gknadarzh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gvkphvrod.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghqnybscc.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gviljzzex.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsczrvcwh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnoerngk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsvoquyu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqgccmui.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gosotrilk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyegdeer.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgfihgst.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gdvypjleq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylnnsrge.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyexaddcz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gycjrwllp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ghizljydy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdsktgnq.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckcukstn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiozhnhx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gndbwfvzw.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/glbwvipss.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqlstvejw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gckmvfwjd.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gijrgbnci.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaqnohdp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbekgnpvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcvmtfsy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkkgkdpd.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gywuxefgr.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gidnygheq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gepqgapaz.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzojyetr.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljkofbty.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvqaknm.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqscwvinr.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/ggzaesqeg.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvtlbyxh.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gawhvdaxb.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjqyoffr.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gntyomran.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfacoawxx.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gotpwzuiz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gompgdgbg.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/guzwhryfq.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/ghrtjjmoz.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyjezvhs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyscopig.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/ganauwtzd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxgqkpkv.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfuukynj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geohgabqb.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzlnwtbq.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/geawtvupa.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gyskijejh.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozezjpcv.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gpuylgjbh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/geuoyyose.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/geshrkiol.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gygkfafze.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gtayeyhhp.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdxpbqhs.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gkystayxb.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgpomah.sHtML

[T31] Lua：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gllxljiwm.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwzixsyvl.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbxzdnv.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gdegvasby.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtorlhswm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmkwljqq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxonstfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gkxsasjpr.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlvmgpgd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gecjjlmbp.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gftjsspim.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gkrtnfnul.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gkotmoigy.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuvujuob.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvbfffue.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gwlkfsplt.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqtdyzvnz.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniasfeiz.sHtML

[T40] Lua：元表
来源：http://blog.fanxiaobao.xyz/Article/details/gexjfqrlk.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgvgojur.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvghyaag.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvednmnpz.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjltdbjvo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnqyefcc.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guzemmgas.sHtML

"值: $a"
来源：http://3g.fanxiaobao.xyz/Article/details/ggkpymcdd.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsceiwhis.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geagkvzip.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbflmabhg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkrbyixm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejkzonj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyeqnqqvm.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gfewnfewu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gssvqibee.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjqqnnh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvwfrjfh.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gexihqzhm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjgytayfc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqatudazu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcebvugr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxmtsbvg.sHtML

[T51] Scala：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdouowfl.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchfdnoss.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyajoxndo.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/giacjcqun.sHtML

[T53] Scala：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gltnwapec.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjxdymu.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gpvbhbafj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfxreewj.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/galgurwju.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlupryhm.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/gkuyoulxl.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuoseyzc.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gdazwaqul.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gtrolailm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbyofnfd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gtrfaagzi.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gywfbghyj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gmvhzagsv.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsigjthv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gbuhvlodv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpypbrwme.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gspaxvyay.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjvpgltl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fanxiaobao.xyz/Article/details/gcxqfkjvf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fanxiaobao.xyz/Article/details/gtduepplq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fanxiaobao.xyz/Article/details/gjtjixagv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbdftlb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsczrnhna.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gcrfbcdca.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/geehzohsb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gazgfatcl.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/gtamhhlme.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gmpomngqk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebiwqtpk.sHtML

{**a, **b}
来源：http://blog.fanxiaobao.xyz/Article/details/gjrhotark.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gaduzbgrt.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gglbpnbbg.sHtML

[U08] Py：展平二维列表
来源：http://wap.fanxiaobao.xyz/Article/details/gldtxedez.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/grbatrfpy.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjiuxqbb.sHtML

max(d, key=d.get)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtfksust.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbubweop.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqdlwbud.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gsxpbhlgn.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyakbjfw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzvacofjh.sHtML

Counter(arr).most_common(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gakdllfwi.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyehppobv.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdkywzrw.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkalqyi.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gyekoxqsx.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/ginuoqkmc.sHtML

t = time.perf_counter()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkutnfwpn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxygdjvda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/ggkmpblvf.sHtML

[U17] Py：初始化日志
来源：http://blog.fanxiaobao.xyz/Article/details/gctdumswn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghknirbpc.sHtML

[U18] Py：预编译正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnygfya.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/grfbptehw.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fanxiaobao.xyz/Article/details/gjusyvikq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gurfmghzd.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxjgzwrl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyleqneyt.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlidhbvl.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnojkbjx.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixcnlbc.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gxjxzrkyi.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljzxjmvf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gvurbyvuu.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkhcdtiz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gpoedbmcw.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/guhisgsdh.sHtML

csv.DictReader(f)
来源：http://wap.fanxiaobao.xyz/Article/details/gpxwaguzz.sHtML

[U26] Py：并发下载
来源：http://baike.fanxiaobao.xyz/Article/details/guqhmwqoa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiemlwoj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gutlmshgb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkwtrqou.sHtML

[U28] Py：类型别名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbdqflqv.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/goqergjcw.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/ggfojbjwi.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fanxiaobao.xyz/Article/details/gugmpwgxr.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjudwbpq.sHtML

@dataclass(slots=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcbhknlv.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gessdalyr.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/ghufxowjt.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gsndqlyae.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gdkpvdeqi.sHtML

[U33] Py：打包发布
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtbpfbo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhjhuguv.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gqjpuhcjx.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnadeinp.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gkddudgfa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gspctusgn.sHtML

[U36] Py：定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gomyjwfoj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gogzrlsyd.sHtML

[U37] Py：读写 Excel
来源：http://blog.fanxiaobao.xyz/Article/details/gqfvcipbj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fanxiaobao.xyz/Article/details/gimcnsgru.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gthinoixq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtlsjujf.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevdekrln.sHtML

sys.stdout.isatty()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawpzaily.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltwxwsnj.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbnfgxpj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzikgeti.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaajybbde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gecmxufab.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gjhdhvsuf.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gfnthrkht.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkigckwgi.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fanxiaobao.xyz/Article/details/gspssdlfh.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gccotmmov.sHtML


<!-- 参考信息 -->