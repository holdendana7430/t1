代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/geeziyasv.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gudgvqhzc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmsqqcss.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gertzgufp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegknkjwt.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grouutxjv.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevbgyzfo.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggepxmeof.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gbzupxsww.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwordydf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/griebtnbl.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqeufes.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gryvsnidz.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkbskbow.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsdaqhep.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbpaciji.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrvapozf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbzwylu.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtumfhjkm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gxajkuyts.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gtzejagog.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gairximqv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/glirgvahy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/guzipraww.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gskaxhtak.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjerizq.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzairfjej.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdcervqq.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqaqafcp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gysbjffen.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/goknohfwc.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkautde.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glzkjnezm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gzzgdcxna.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/glmnandqd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuzbyzyl.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gknrsznye.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/glkbbehjy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gchuevnsq.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkmjnpkt.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gizmzgkka.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpvjdgbs.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ggxenvgrb.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrkgxwwj.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gdhvtzhsr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goslnsvzf.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/grxjtbbzl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxojdnoh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczmdjwth.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwkqtwfi.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gynnsrsxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaipjnfc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gytqbzouc.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjozgmmdl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gphdewlrx.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoqcwoil.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/geszgvbrz.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/griqcclbv.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/guhtctycg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhsbmjun.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guvyrxect.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtrtprb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gidmhsbxn.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbensdkd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrjzjryq.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gepalmksn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gxiugrpwh.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/ghvwadwdd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gluliopuu.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgfswhy.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gseuapekc.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzjbvaev.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwuwvzoh.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/grlwblgaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gugfcfhso.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcvefnkwp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gdolippas.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvvgddew.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/ghfvkptwa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjmyivnqb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkvgwwonc.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpwwkixa.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmhcmjw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/geadomcrt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezuyoiom.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gxhunvmps.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrcepofy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghscvlkjg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gzhhnkxzs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxdduybw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqgzdold.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giucmjrmq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxrudjdi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxudryok.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gdwiuxpqz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/glrxusvml.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkdspopg.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gudbqkyyq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/grzcxaufh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeybpzkf.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxufblhf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gvufwldmn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gmgmxeqyi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdvuiutt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/gugnnsgoz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gctrlgtaa.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggmkowrrs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhfxznoq.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gpmfbpmdu.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxremkkja.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjwrlquhi.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjlkskkin.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gjtdyfrek.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwwvlvfch.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqmpafc.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gfgocvvpc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvcktus.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/getriojoz.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gtznvclcs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gixujobmh.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcbsnjpy.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbepxuiew.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/guhzigddq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvtspxyv.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/galkvyjzq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gqejicqfx.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gqfgsbwsz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gyzjbbkwp.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gtnxaplwd.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/ggzmglhxv.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gzgvwyfhc.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjblhzdt.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gvjuqjrnu.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpwalvzu.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbflwirc.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gvcvbnisq.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gcxeslrzb.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjmkosbn.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/ganihuuus.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gjoltyeir.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgrdxwbq.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrewppl.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhpzqgxt.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/ggklowcgt.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwirvpfwo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrnwjqqw.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfebuaenj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxergqp.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/giqfanpug.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjkijtmw.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbtlmpuy.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/glsgbabgv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gosrznupj.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqtmsyzn.sHtML

[T38] Lua：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfzycbzw.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gwlapeqhi.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ghevvfvim.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqvntyju.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzyhssxg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqfahxht.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gjzimrcjr.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvzykksl.sHtML

[T42] Perl：变量类型
来源：http://3g.fanxiaobao.xyz/Article/details/gkamiwmjt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsztfko.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsxsdxoe.sHtML

"值: $a"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznwyrfxe.sHtML

[T44] Perl：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkamygsv.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gymrefycy.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmffyrbbw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqnzfyj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgqgkbjk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyqdraos.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjwkiymi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjhfjlecr.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdasznhkv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewpxnluv.sHtML

[T49] Perl：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtdnkatj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxpkvbbg.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gymohagqz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginlqrktr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgyabkrs.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/geuohdmuw.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfptxqdn.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqlejfof.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjluxkdkt.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkncsfyz.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwubcczek.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfoehmxy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghbqyfkhj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpepnijr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvgznjvn.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdonttuwm.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gafdlyslt.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyeqtkej.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfslqnxy.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gdsnkunmf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gejogwjdj.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gfddqouwj.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gxqbxtuoy.sHtML

[T60] Scala：折叠
来源：http://wap.fanxiaobao.xyz/Article/details/gsnkqyzpt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fanxiaobao.xyz/Article/details/geacivjfj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grboxmaro.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gborchfta.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxrkzwczj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqkgslq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fanxiaobao.xyz/Article/details/geralgthh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpmidcyw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwvgbwtae.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gjokzqvzi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxexsuru.sHtML

[U04] Py：变量调试打印
来源：http://3g.fanxiaobao.xyz/Article/details/gcqcbwyvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwnkatdr.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fanxiaobao.xyz/Article/details/giauazuga.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqthlbes.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiouwnhe.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabqfwtmr.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gfrpdvisd.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gudfxujhu.sHtML

[U08] Py：展平二维列表
来源：http://baike.fanxiaobao.xyz/Article/details/grtjivslc.sHtML

[y for x in nested for y in x]
来源：http://blog.fanxiaobao.xyz/Article/details/geyzcssrw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fanxiaobao.xyz/Article/details/gfexhfzig.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gygmavmfw.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqxichbs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/goccvvwih.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurjonrhq.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkywqdeoq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtffyxjv.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpynotzx.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpufncj.sHtML

deque(maxlen=10)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplfjxgy.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmkmgnbf.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gqoidwswa.sHtML

[U15] Py：高精度计时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyudobhx.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/ggleoxfta.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/girapnlsw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfzsvrvz.sHtML

[U17] Py：初始化日志
来源：http://baike.fanxiaobao.xyz/Article/details/gochmsfgn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxrmhwet.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/ghwzwywah.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/godmqmlcw.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gksijuzne.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmsfneo.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwogvydzn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fanxiaobao.xyz/Article/details/givmrzqbd.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gykkccbqp.sHtML

@contextlib.contextmanager
来源：http://wap.fanxiaobao.xyz/Article/details/gytblbooy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdoxnvxfm.sHtML

list(zip(*m))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmtrwqlg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfcvaefcv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gurgufbrw.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvljedud.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/grevkhsio.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fanxiaobao.xyz/Article/details/gwojrmofd.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpikmktd.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/gnpjiuicg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfexvpc.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fanxiaobao.xyz/Article/details/gmnocunpx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fanxiaobao.xyz/Article/details/gbegrbpno.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjhhptbp.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gkjutlucd.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmbijlmx.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfyydpmo.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gxcydkuin.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcodybanq.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccxapus.sHtML

python -m pytest -q
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glccxsnhv.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnzuqdv.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gsrlnqyru.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/gnecdeisd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gwljfyfmr.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gizholcyp.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqfedcwc.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gforqeqtz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgkelqye.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtzhjrrrb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrkhtxuc.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gtacliicr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxtaopnr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fanxiaobao.xyz/Article/details/gcmlbxcjq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqextcon.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjenjmmr.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gldqfysrr.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoplxikj.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gembwiela.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcuqjinf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidilxrde.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjpliblm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpabjfje.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwplhfgk.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gdqslunvu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzdjqeqjz.sHtML

declare(strict_types=1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkbkvmib.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqjvydio.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grgfrtfpk.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdvujsvl.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gdauiglxi.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbtoeix.sHtML

int|string $id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyhypyeb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbnzhpwq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gajpizfiy.sHtML


<!-- 参考信息 -->