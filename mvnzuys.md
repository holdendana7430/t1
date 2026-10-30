代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsqxylks.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gqtuvmvoc.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gyxmpxfvd.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gwbyafbxd.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdfvftvp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/guztjbabk.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoyrokwq.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gupsfqmoy.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpryxzps.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghwqidvel.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gkgxwsjvi.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gsltcxdfm.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrdyizbi.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnyoiqkj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/givhxvsbl.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqhnhut.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfptekst.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddcnjsgd.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gobhsvqfi.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyildxiw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaassmpo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gadqfcdzi.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/genjpudwf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzrxkjgf.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/guptvzkkh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gshcuhkcw.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gspfgxiok.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gkrkgefku.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyskimnrb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdhecwoj.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnbkmitfo.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcymjjcn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gxcybztni.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gotcjdlbb.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvdkoeki.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvvshapf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjawptm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gptaycuzn.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvappxt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmzztgds.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/glkwkjwgc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwntvciig.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhiirbth.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooyxzpww.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gvspeoboa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvkwglkj.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gnazcludm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxydkyslx.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwsezjwa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfmbsebj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljnvccto.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxymwntmu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gswfbbzfd.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwnlkzuy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofuyusat.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/geqjwhuuf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gomdftcsh.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gdviyeofz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukundtdw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gnoewbtve.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtwhpdlpk.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmtsqqcm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/golglmjjw.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcmdabj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjofpxibk.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gurdquzni.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gffsrwwvz.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gtoocextq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjvmiisb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfdkisgw.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaghlndez.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gofzahnfn.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjejakdtq.sHtML

[S59] C++：静态断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrcnxbwd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gvqsjrnis.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwdewquq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchkfsvqn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gogxlqris.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gdxyzzksw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghdyhigsw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvaarkv.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbdmmtbl.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/glormwzzd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/grdsxdoon.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/ghnuscxlt.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gjiycwnai.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfzzueoy.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gsovgynug.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiknbncc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplveoucq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gvhgztysc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gswiikeil.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcaxxfih.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gapjwhadm.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/goctczgnh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjczzbhyl.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gsgvoocox.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gkngaetth.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwxzrerr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gwrkgjzpu.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gvzltlszx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjxstyau.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmhhygyk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtzrnlpcb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gawztxizr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdlblfj.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gfovhphim.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gvnisnmzl.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdjxavxo.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gbedkoqrx.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqmydujyu.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gqsqmoitj.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyhgeoeq.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gstzeadxp.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkrasipba.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwluqlu.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqcdhtve.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxdqebyiy.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrhhzzvs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojppprvg.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmhwlsm.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqfwqctq.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gkafevmgd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqcexfqn.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpguyfgrb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gmswnrnxv.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gljdowtfy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gqtbohwuh.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gtntllaey.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gszwlnvoe.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gwgggakms.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gdidenpoo.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/guldmvfgj.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjmdelba.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmzsenu.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnidlkme.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjocugaf.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gzcbkwcuq.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacivuhdq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/glyfqgqhf.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqnbrhtw.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ghqsioomi.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gidmbllfq.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnactbymu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gopvltmnx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdqqiqno.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gsehxpzsu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gjmcgogdq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gslcvvujx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwilzocy.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gajxfducw.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjrgbrna.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixuuqns.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxadiauxg.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcieflltw.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmndwvdl.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthtbcttz.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbxjyqzd.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmtvneg.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gwjfyxcga.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdtsmkqxw.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyzfuupx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/goupbeaut.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/geuljixgb.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlqabmus.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcszujyop.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gewxlkgaj.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gurykahvx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gywlvcavv.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhbpjtua.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjtuhyci.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahvyjzjf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvufxpt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhlfmcbr.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqpzwqovm.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gdnoklwaw.sHtML

[T49] Perl：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvwqukbko.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtfgouoqt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpupsuw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsyjpxop.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gklypmekm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquxouwmt.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/grkwarnuh.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gusvbjtkn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwbmvxbv.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfijzndpl.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdkcwuwnb.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/ghycxrobk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gpgtovoko.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gkzzxkcyv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwannjayp.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/ggbndqihe.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbaisnh.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfifkowlp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ggblblpsw.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuovbcvo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gykzbufne.sHtML

[T59] Scala：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gtwouuhks.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwrcecfp.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gearpkahe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvhymahv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmttepznx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurbvdmhp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtafllu.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsfkudwl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/gqysuefso.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftnqcjl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gzewjyltt.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gazdbcysl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fanxiaobao.xyz/Article/details/gimovcgue.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gvwpgnjsm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fanxiaobao.xyz/Article/details/gicvhssdh.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/guuqnzjso.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvsnhvdd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gucbwljnq.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ghjyonypp.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfttusoc.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtneyrqo.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gvxkopjxq.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/gdkcdwdkk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fanxiaobao.xyz/Article/details/gxftdryhx.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gneqwrykx.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwhqwwtt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxirowqf.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gihogdgwv.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoqzvbwk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnedtdopc.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzkwjemf.sHtML

[U13] Py：固定长度队列
来源：http://blog.fanxiaobao.xyz/Article/details/grnnucyby.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/glpswatjo.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdbggur.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjkemkxln.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gnwifmuqy.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/glhvkhfne.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gzqjzuxct.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnkaomdt.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdlpfadvc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtzrszlp.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmyqlha.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gycsvtyjh.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gomuuguqp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszaiqxzj.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fanxiaobao.xyz/Article/details/gnenwsslw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/gggilojnh.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrnjcvjw.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/goklgmqcv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbalzrxf.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gzdywfqir.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzerzpdv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gqnfmbsmf.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gxehntkkx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmkxesgl.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrljoqza.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtfzkcwp.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkpznklu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/gsofvmcxn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gaajqtwwh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgzpiviy.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrcbdnlj.sHtML

UserId = int
来源：http://mobile.fanxiaobao.xyz/Article/details/gihqfwggm.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcecmfql.sHtML

@property 与 @x.setter 配合
来源：http://3g.fanxiaobao.xyz/Article/details/gjqxsdhen.sHtML

[U30] Py：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvnfifyj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddlzwtkd.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/geivnjfmu.sHtML

python -m pytest -q
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdepfmkc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdqcyjas.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gazmgkvew.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gkslpqaaf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfpzfsp.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxajnlhky.sHtML

chardet.detect(raw)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgkxddbs.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gqaadbryd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fanxiaobao.xyz/Article/details/gatytddal.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdduwewad.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvtxfqkb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxkytgdp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fanxiaobao.xyz/Article/details/goybmahbn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgvypek.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssitypuh.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/gdwrypkdy.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gaccaoioc.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gayzasudi.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/grhojfkrd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmfitomm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcduqttiv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaawojhy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gwqssmbkz.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfxgsqqw.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gslibmxvj.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcebqvla.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/grbhyqdmh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/gklcdexyy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgtrfngx.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfehpxtn.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gvbhvvlfv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfftkzvhy.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gdwosqzvg.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gouzmcnps.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgczqoj.sHtML


<!-- 参考信息 -->