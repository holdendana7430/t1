代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/geyhlhqkz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gbeadyfjt.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gqrkpfuad.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/ghuujoevr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gzvbcrvfv.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gwgfgdned.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsbisjnvq.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gdjpeecvq.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gmulytoyk.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gglfrhhld.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/ghazsgvyi.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gmpxycutz.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gabbdvfjs.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gvafcyzby.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gpolutfyh.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvapgnslw.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gxqpfpdes.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gndorgbgg.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gmzpqmsug.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gkqypjjjp.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gcchmsnwx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/ggaprzxqx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gydwfjjtv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gfvgknrdp.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gcyyvjpgh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gtzkwuvfh.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/ggrgjljpw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gyviubifi.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gwzhugxss.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gurxsyfkb.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gllehhfgo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gcsumvixs.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/ghtwgzssh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/greavgcgr.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gcpttmgvp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gmmtwqnwj.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/ghldxqgzh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gpmmxspez.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gzqmgbipb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gzybwxcex.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gsvuamufj.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gqlsakjrm.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gxxdoclzl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gycmwmadk.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gduhihquj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gjaixogwc.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gngjeguex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/gxahdzxrv.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gvjvgshus.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gyybdqncw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gamqvlsax.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/grcmrqgpc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gegxnxrnf.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gicmqlspe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gvhzyfhqe.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gcpwwrvkh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gxfburjia.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/glnhleirq.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gdjnkjahl.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/ggwrhecfm.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gcjvxxyov.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/guplaueqm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gtatcjknd.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/guekamlqs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/gzrbbntzp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gvrqxtdqb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggumfssnm.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/ggjxyesju.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gqadcpmov.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gfxjiavoq.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gojcbmjjx.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gcynrmyfi.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gornstxyy.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gqnfkjtcq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gsoppfhnz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gxhjezief.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/grqxtbisq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gapxanaoa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gbbejixok.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geyfyvqab.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwribgbpb.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gwkizmgbk.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gcdcchdje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/grtwlwnux.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gcfgmokbs.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gvgluehtz.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gprenydaa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gmgfvsjbe.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gogaobcqc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gminbydsz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gbkfgnnth.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gsfgzkyhz.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gutwlkrfc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gysgoeglb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gamohntdv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/glhxcubmc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gghfoyjvs.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gkgqfrukf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/glzphqcjm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/girihuewb.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/galougmgm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gpezkauzp.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gymunltyo.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpofurmsy.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gqjkqpvle.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gudcehbch.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gokunvhqt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/glhjmcuyq.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gggrcbbee.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gfiiyovor.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gttxtlgnw.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gidytwfta.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gjtpghziv.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/ggjspzxst.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gxjwsqodd.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/glcelgdtt.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/grgflutpz.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gvjitloom.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gsluvxbhn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gvsveagbm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/grmpgoghd.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/ghbzvbdps.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gcnksmrcl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gitwzrybf.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gvosotxho.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gjgjteexg.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gfthqoavb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gayyyprsb.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gxrjufgnn.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gikzhjhlu.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gqvwrspqk.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gifbpzuyh.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/goapzpyuo.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/gqmqotgnq.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gibuoagwp.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gstvkzheg.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gfowmmgnp.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gogcusmyl.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gwlznmbfu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gwxoebwcf.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gbsnoerkt.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gwnbeblgn.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gfiuuzulm.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/grkporobj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gzspoalmd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/gnnxwdzzr.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gqcidnvwf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gmotaqdkq.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/guvasnibg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gbjjucahr.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gtfrlrogq.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/guaeuosrf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gluzjzlps.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gndwibmpe.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gzkahylaf.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gwljpbofr.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gnvemohku.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gksbpdcwv.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/glagctprb.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnuavvt.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkablpcii.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gbznxibxs.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gyodvycqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/godxpmpuz.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/ghgaondgu.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gnhszhruz.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gtcvvssiu.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/goqziswou.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gutkktzgd.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gkjsmzsci.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbextdkic.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/geqftzfbl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/greyicduq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gifadahqu.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/geenqsghi.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gtrtpffmw.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/geuvxgwfu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gogbitcme.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gaixdnnyf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gpgtvuzvy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gccyqjfxh.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gfwgiwtkr.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gtokojtuq.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gpdbdkhei.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxvoxyvav.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gstahwobo.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gkvfcjdez.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/ghrqwtrrk.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gfblghxzd.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gbtgilfbk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/glccppkuo.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/ghuthbckw.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gdhkrrlxw.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gvwnzjqmy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gxjypfkum.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gufvizbeb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gsgbikous.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gfabagfrm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gasvokqlt.sHtML

[T60] Scala：折叠
来源：http://www.share.hesvh.cn/Article/details/gprhorhdi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gnovfpbbu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfgehigba.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gqttpdpts.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guaasvkjk.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gkissglaw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gzwsppxlb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/grqywnhbl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gzblluwrj.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gftkqngqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gmeeukjda.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gdtvpxnzt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gcfvyceza.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzwkiil.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/glhlfbeaw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gpyiteeiy.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gbdamekea.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gubputnih.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gzpslycqk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gtuysopip.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gmnzijome.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gjajqkepb.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gagrooryv.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/guxpdwpva.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gzlcdqrjx.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gxyisewhk.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/ghfhgujhq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gsrxlllgi.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gohcmldav.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gvxrxdttt.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gcugxzwji.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gapfpoakn.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gmxalivpl.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gtjcbvgpq.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gsvavomes.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gypzlmpoh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gfmvmytde.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gdnvrkahu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gzizxzhpq.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gtyjtlruc.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gzwcsoctl.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gwlzcjobx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gedxndmth.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gifhhkrwz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gbojjpjpn.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gaoucoiob.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gtxhvhwab.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gzgilqkob.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gwjbipvuj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/guvzruqda.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gqhukcrhu.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gusxefpua.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gupbhjnex.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gcbczvbgc.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gkgbvbixi.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gbvypxljl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gidtzvtvu.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gntltpzek.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gjjwxsmzs.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gvbiqpbzz.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/gzlmjgyfu.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gxkbxjwcq.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/guvaycoqt.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/gqttsijux.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gkfvrjqdc.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/ggbncymqm.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gdzyllqjs.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gxbgdgeyr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gsafnojsw.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gzfkfrsae.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/giybpjdex.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gtpjpempx.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gjjyxgpmq.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gnsrptdwr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/ghclrbdve.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gxzwptfgr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gvbupulyi.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/goqxiernb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/gbhepsiox.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/grkxpmhog.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gtgoufcat.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gtarsepny.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gbbfwdedh.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gtoztavld.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/garslvhde.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gtzyydvoy.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gvdotxlqh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gxanaufdt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gjlofpnap.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gqyvbnncd.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gzlzvynza.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gwdvtaswz.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gvbhmszff.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gtefetdnk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gliygmnnv.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gfbpmparl.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gkhiyqihf.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gqtpeefkc.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gecjdsvwu.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gsybozguf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gojzkrdqk.sHtML


<!-- 参考信息 -->