代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdcqhgmpz.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gtjwmqkou.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gerwfeaik.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gvskrvcfi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/ghiapeoqo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gumzggaqb.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gkrkyqlmr.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/goaosvmhp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gosqmsxms.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gchwvpxhs.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gaarzazun.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gypjmkylz.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gggrusiay.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gbvzolutr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/grbekrqpy.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gzcnztnkz.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/goshnsrdc.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gwlcqewhl.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gtkzjbakc.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gucowhcgm.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gftzxqwem.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gxasnbbhr.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gsxrxqcsp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gecdoauio.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gtvfdixkv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gjtsaaong.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gbwaduwfd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gknyaxtfw.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gtxkxnrxj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnjumybwu.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gedeazisi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gchmnhdbi.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gqfkizqnv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gxwtyfnns.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/goemafhul.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gvzemcgyt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/glpwqmjgi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gzhboxapq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gwsyrlkjp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/grmnpyise.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gxibpjtdg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gkywmfsye.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/glzcoacct.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gncuqsjmj.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gjdxwwrdn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gprwxytun.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/ghrhyeylb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmporjmw.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gzdtxkitn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gujhjustm.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gtthiuqmm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gqpfjrymq.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/ghxkrelnb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gnpgvdaxu.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gulqoghqx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gztusotfc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/ghinfxcwg.sHtML

[S49] C++：写文件
来源：http://baike.hesvh.cn/Article/details/gfvtstbuf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gryxcoaza.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gdmybjpgh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfxtwuoef.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gspykbsvk.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gvbwurkui.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gicstnngy.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gkukjcrbs.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gcptbxfvm.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gpycfvhks.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gznjdoqbd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gtgiuuesp.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gbsirhxme.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gyprqcwcf.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gpmmfykqt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gjfnmjwjt.sHtML

[S57] C++：编译期常量
来源：http://wap.hesvh.cn/Article/details/grbpsokoa.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gtyevyhpt.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gyediofvj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gxypntzui.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gapztwvcw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gnlodpiqm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/goiyjcenp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gjqvsnrfu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxsubfupb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/grslpvayt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gubvfbtmc.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gisnakpmj.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ggxvookto.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gachuawss.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gfiltiqkh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gpxapvakk.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/goneaqhtu.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gfualujqs.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gqpdcdiwc.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gbgywboqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gephqzzee.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/glwdzgqzf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gmpvhezni.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gqrbnizmg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/grrptdxkc.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gasvrvcmr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gulhrosxb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gumjwoxhe.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gmupigbyh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gmvymjcqc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gfwundeht.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gricokqed.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gatrytlps.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/ggcxsmmtu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gflsokofe.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gbxdarwul.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gaczozysd.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gawzvsrno.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gncdidhlv.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gcindqlid.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/ggavvxwtx.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gamjtrbuo.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gohpknfzx.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/ggjkdifka.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gnpgonfwi.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gusmmlgin.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gnezixybo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gifdodtmq.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/grdvnafhs.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gbyanlfpp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gsurbazpu.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gxdwddblv.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gkuaddpis.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gyepydqil.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gifchdkrk.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gtftkfoak.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gcgvxutar.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gjytyieji.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmehjjlal.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gazdzdtmm.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gfcfwxdjn.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gzlkrxgoo.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gytafqkty.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gfhzcbxlb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gmzleqbfs.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/grixpncvn.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/geclzbcos.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gavtxaufr.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gnaupyooi.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gxpqhawvo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/guujdpdph.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gntgthrph.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfxhswbmp.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gczlotrcr.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gtclsgves.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/ghxhxgzsy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gfvulsmyi.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gwusvuxsq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gcrtrohvw.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gwgwkjnzb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gsmxjmbyr.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gpflxonfu.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gjcgnjsqc.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gqgytpxkc.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ggqyitxua.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gwnbbdzql.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gfvnvzxcp.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/galahxbgf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gpmixipyb.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gzyqflhlf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gxkyaesdg.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkjswbtgj.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gmdejcmcj.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gsxehdgyb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gkyphagwl.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gattphiwr.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gzuslysvw.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gzjjiaahs.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/ghnrrwhzx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gwfphgxjx.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjooyeiqo.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gsjdfgazr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/gweyskjxq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/guqoxrkro.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrogofgi.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gskiqbnre.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gnrakcfim.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gfknkeril.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfuzxsdmf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghasniapg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/ggmngtnyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gwyxfpppn.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gtxlkjayz.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gqtwyyidb.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gnamqjana.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/glbjefier.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwrfymijd.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gyjiyxija.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/giwwspmyj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/grdrpcgry.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/givnatypi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gpchxuedc.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gssekdvqw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gfgbwlarf.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gxwfvjwwd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gpqbzcyhc.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gaffgxijt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gklkszowe.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gtdxzssle.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/geonchnqy.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gzegheoss.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdoejbucm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmymsrggp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsjxuxtdz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjsrjzbpo.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gfmilglaa.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gbjtjzldb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gdujqfdyo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gsqrqhfgv.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gyipciclv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gotquzhok.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gdihsnxfm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gsrhscopd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/guglbzlij.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gepcswbge.sHtML

[U06] Py：合并两个字典
来源：http://wap.hesvh.cn/Article/details/gmekszqsp.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/ghcbvkbwq.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/girnsowxw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gwgzskvuw.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gflhjvvxb.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/geqpqujpv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.zdbjq.cn/Article/details/gxxyrgali.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/gflaelsob.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/golsgnnna.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gzwddiemo.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gqyqmtell.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gudewsxbn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gpndnedsk.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfasfipno.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gawcdixyt.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gqnxzzsbp.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gcswhaygf.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gmikpqmts.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gzyrwidgu.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gguisduye.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/grnxthwkx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gafbrxfcz.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/glvlmadpk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gmoayftwg.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gmmgvqxoo.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gcpojsgjb.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gqimtnbwz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gtqpamjzi.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/giyfjyybx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gyfqsexvs.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gwzjccvkb.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gbephwcce.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gqeqpeook.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gtyoriloi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gjrhyeizw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gindebyog.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/ghlzkatvt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/glavmswgb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gpdmseqwj.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/giguqvfyi.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gnfogigry.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gmgkpkwsj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/ggyiljwww.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gtqublllc.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gezsngxdw.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gcwrzfilw.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gnsypkigw.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gfeofuoku.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gosamhqbs.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvwzwlzzs.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/godagexhz.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gbsgpmzav.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/grmgjkcgp.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fehbvm.com/Article/details/gsemnznpr.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/giigxxdih.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/guobnposh.sHtML

[U34] Py：判断编码
来源：http://read.share.fehbvm.com/Article/details/gjieesbij.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gilfgwwsj.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gxxregpcx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/golhomser.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gzbszkilp.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gggddspws.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gdzatizqb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/goblxjiwa.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.zdbjq.cn/Article/details/gakjwbduz.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/glxnewvnr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.hesvh.cn/Article/details/gmhnbdgjt.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gudctfejb.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gswfkkhue.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gakvzbjlf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfkimjsyd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gczobdsnl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gfsltokxt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gtgzoomai.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gajdutqlt.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gitbsnizn.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/ggwwtwgua.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gdaidedlu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gxfbkbyul.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gzaainaba.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gjwxcwbye.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gtruknvqr.sHtML


<!-- 参考信息 -->