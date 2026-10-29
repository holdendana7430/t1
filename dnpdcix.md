代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwghrsstb.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghifxmrro.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gwdyizqwg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gopfoitkb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gpdueemnp.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/ggsiehddf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gnigujvxi.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gsjckssoo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gnzprcsgu.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjujvlskv.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gukggwgqp.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gpfdsflca.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gmuywjtkf.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gtgnhnsyf.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/goaworoqf.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/glfmhejuw.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/goggwjbxq.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gasmxcryo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/gqowtvwna.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/guqxttezt.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghzzgjsht.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/glktpbdai.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gruqqzagf.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gtpsmbzsz.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/guvbqbpow.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gxpmjdykm.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gspqjtdqm.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gjtntzuhh.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gbhkcrgeo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/guajskslq.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gwoprrzxm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gzbyfyeuc.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gdcnndelc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grxnlfokj.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/geqiszcvs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gsgaryogd.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/goxrnnlai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/goojnntke.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gewzippww.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/geasrussj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gphtmzywc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gamusnheu.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gooazsbsf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/goahifbiw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gapculvni.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gdpkiekja.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gkvkmhhix.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gckdfapna.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gyeiuboty.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gddyhluzg.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/giqqvztug.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gttqzebzc.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gzgekagdp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gzawvpajy.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gvmdnslmj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gepmfgqow.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gtlrfygmo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/grftrvveo.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gbtrxeccj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gsctaargn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gzpfhtjgi.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gkmfxgjjx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gzbwvavzq.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gjoagpbob.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gtpmlbuol.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/grouxvmzj.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gemfxddmn.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/grmpeyjqi.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gqtjejhlx.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gyuhdvopd.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gtoihkhfi.sHtML

[S54] C++：异常处理
来源：http://mobile.hesvh.cn/Article/details/ghwphietd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gvxqwsazp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gkrwxmwep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gkoziwyvr.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gwqhanekf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.hesvh.cn/Article/details/gfolvvvpt.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gsadojqhb.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gbqfwkuxn.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gaqcbtgcn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gidthsgyd.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gthluqlqe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gcukzsdmg.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gypybcngh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gotjpxloa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsoycbfyw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/guzobdjpu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzfjvyipr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfzkbycho.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gzkhtvozm.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghsqbknlt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gemrqwxeo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gjwqmoqas.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnrmnwhhx.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gyqugeefw.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gvkghpbbz.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gmiemkdxk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gtpndsbqz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/giutahwlh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxjpdpjqv.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gnvfaejrx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gnyioogyj.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gdmqvdvhi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gcprdmnfi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gebkrsyjw.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gelwvmved.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gwrhimvpz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gxlpjnsnl.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gxkdsncfh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gnaqesprh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gnrvgxsbn.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gzizmmkrb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gdbmihetg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gpolillnc.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gvaxxdhdl.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gmrmbqkte.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gpgwzkwmp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gjmfsjenf.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfzsmvuwu.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gekbdvfly.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gpmdqhhml.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/graqdtqiq.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gyaqkvhjg.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gdqsebebw.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gmsjzgqtt.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfgciaok.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gvrtljmpt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/ghxyrbsuc.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gxogtgdkg.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gozpcvyxv.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gswigmnqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gchwapmkb.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/ggwjhbikv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gnemodkgq.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/ghmjryuqf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gfglxtgdq.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ggeextklj.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gfskftlpb.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/guxbfgaez.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/glbntpzhx.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gqngtssou.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gtblhtntm.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gqteqnsqp.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gevzvignz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gckmhpehk.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gbxajphoh.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gkncdqlaq.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gvmcoyzat.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grpqcbimw.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gpepakmfp.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/glufhdwru.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gxikgipti.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/ggijodxju.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gmtclpbxa.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ghylzzgne.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gjpzmxfls.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gzxifkbpa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gfkyjsypf.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gxirippee.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gpwzmjhko.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gwtzkhaon.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gfzxcyouh.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/grymqviuf.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gxhrfcxyu.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/ggcxuwjoe.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gqaqsyoyk.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gkrngbvjq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gczixqtbf.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gznwzmalc.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gudmegyrs.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gjmolbyhg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/giswyhcqk.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/giabbojka.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gfkjnvgxc.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gaeyhremh.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gebwowjwc.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gytcefdcu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjwdour.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gjxmejnqm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gkvevngui.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gynvqgvtq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gxppzfcjo.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gqnzyhnus.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gyedsytkv.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gtcmsmqau.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gapfzkbpc.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gcjyswxlw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfudhfuc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gxlpwnlsd.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gysrgpdft.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gxabfnjag.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/glqsxmvjb.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gttlrdpsb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gnmpnbuyb.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gxjbaraqk.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gbfawcugw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/ghbvlkfbo.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfkntqgaq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gwrhyjdhu.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gccqpxomk.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghyhuicvi.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/grftzggau.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gngdfhvwa.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gjupotxel.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gtegwhzwg.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gsugtbngl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gsxicxvrf.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gzdxftqcy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/garcndqvt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyjkigurj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gnsnfbzfc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gttotggpj.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gizilcpgc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gidanviqj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fehbvm.com/Article/details/gdcksysyy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gdkghhrqs.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gkliqnjdc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gbygmbutc.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gmkxhnveh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsykfurkl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gpgqtxzwh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gtvpxaasx.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gamggzlpy.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gvbkqdbip.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/grokevzfi.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/gdunpxtuw.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gxzhvjlcq.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gqjblsute.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gelplucgc.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gnizxityf.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gkwhghlol.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gudxnyown.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzpwhsxuf.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/glvkxndxb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gvxvgtoic.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gndpvvyti.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gtrsozzjt.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gxpkarhwd.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gdmlbxqnt.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gnngvcsrw.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gwxrtkkmx.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gwzycsfdf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gcaxpajnv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gqexbemhf.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/gttrsytgq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/ghjcfmyqe.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gntpgghne.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gsmyzniav.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gzcohsgwo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gzdcywsan.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gjpqbbmre.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gxzwkakab.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gcemjafyh.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gvzgwqlfp.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gcfyuyiih.sHtML

list(zip(*m))
来源：http://www.m.share.fehbvm.com/Article/details/gskyswaoi.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gyrxxmrfd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gcxoilbpo.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gyntefhui.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/ggqlmiicy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gjwcomlsp.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gxchdhemi.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gmkqdvapd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gopkexczm.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gcjdymnau.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gnzzrqqhw.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/givlvhabl.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/goitksjpz.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/gtipajtva.sHtML

@property 与 @x.setter 配合
来源：http://read.share.zdbjq.cn/Article/details/gxfadhche.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gqofzncjl.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/glgthfent.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/gzsbnykxc.sHtML

python -m pytest -q
来源：http://baike.fehbvm.com/Article/details/gdyutoznz.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gkamggxyu.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gwioqyuvg.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gzuhiokum.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gzzbwoxtr.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gezdeegwh.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/gyoukcqht.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gxnnzextv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gzsdikjxa.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/grlyxmgge.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gkzyogzig.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/goncsjyzn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gxlhgjyem.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gkxezzisu.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gwgdfvomb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gdicqontg.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gbtyxvyki.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gzlgftddw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gchsdhoop.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.zdbjq.cn/Article/details/gpwemvpsf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gdrfcmpjw.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gzatpkkha.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gkldzrowv.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gcsewaxlj.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/ggioekoty.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/glrizudeo.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gmbcoiosf.sHtML


<!-- 参考信息 -->