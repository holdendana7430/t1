代发 wailian999

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gihrxxxhf.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gdnztucpa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gtnyjdjzz.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gjcjebznf.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gjxnsnwxa.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gtqurzmom.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/guczhrikh.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gyypfbvxa.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gtunpimwl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gbiazcmgs.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gmhjdhima.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gjbnionhk.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gmmhuiqwf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gxxpvdgpu.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gvozkjowx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gszrchyso.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gdpoushth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gosbwhjsb.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/ggtzykynk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gddtusblj.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gvkiysgiz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gvwpxluio.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/glyhxeagf.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/giszpimvm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gpjzuhuyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/ggnkfmnsb.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/grlabwjhp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gnbsakhhz.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/geehigrkj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/giixegddm.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/grdaantim.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gkejkrrap.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gikosynxp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gorqbiqhb.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gcubmcpxc.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gvcnnziyz.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gsjjrkjso.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gqcrnufmn.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gbkightkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gjjuuxkgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gaghluoxq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gdhbbxxsm.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gnwdsewvi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/ggtcenoiy.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gcnpudliv.sHtML

[S49] C++：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmauycnau.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gubmmjwus.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gwljubvsy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtyjsqrem.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gjrnwjvqa.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gmgristzl.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gtdwethfp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gdodlrnfq.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gvalgakep.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gbbrqqmbg.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/glxrocgme.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gbygxmdlw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gqgewvinv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gshbblofn.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/ghuvyvjzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gfljcaept.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gkyultlvv.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gwqxszmdj.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/glaousmta.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gjjedbhxq.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gsudmwwaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gmgzpyeik.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gsdcobmjk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/guvcnagnq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtlujzljb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gapohpbot.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghplezifm.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gznvkjjir.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gklwprmeu.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/gqpgqiuqc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gqvuxffjm.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gcttpngrt.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gxtycbhzj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gqgunbuuv.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gksjxbwms.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gkrnpykfs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gsfzdhrtz.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gssntlgtb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gfaokilhi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/geycryzhp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gocvdqnbl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gthxkohup.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfmuclkon.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/geoxopnsu.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/ghxslpoid.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gbsaycahs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gmxwiwxih.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gtjitnlje.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gdduafnet.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/geohbqyxo.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gckfppbjk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gljpiibcf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gilwatsnn.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/ggpaxqcmk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkorafchc.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gwphcheqp.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gtjydpojs.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmqrdeakh.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjdtjbprc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/geieeolpz.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gzkcmejkn.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gsmniiqet.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/ghmcbiiab.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gapdsbyat.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gnghwttgk.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gjaadumug.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnkuaccku.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gpxojamce.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gpmmbyvsk.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ghupmvbsy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gcxsqmzmn.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/glahoticm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gthnmprrn.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gtpupfnut.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gropkpdih.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gilqheldu.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gyudrgmco.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gavwbsobj.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gmmcddhmn.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbgcynbhs.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gaztcmzyn.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gjgiwbdtk.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gxviamave.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gcrkkfxmx.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gixsvtxwz.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gtvmnqrmm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gphswuwev.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glfsexmsc.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gyosbyrai.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/ghdijvrqj.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gwstjybof.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gqzmvoouf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gfngzatcs.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gkxxkvxci.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gxzmrvrvc.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gtijkyyqj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gnsfiionk.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/guqysanga.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/grtwwrfyt.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gnitvqpst.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gbxssnbiz.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gfhkxyatt.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gmsxysrjk.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gjnzejocd.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gdspqhneg.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gaffmkrvv.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gyigwityv.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvchpmykt.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/ghthcyoxg.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gvnoulxsm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gmoanzizb.sHtML

[T43] Perl：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gjxfxvyir.sHtML

"值: $a"
来源：http://www.share.fehbvm.com/Article/details/gkldboiyu.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/geezpigjx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gbfystbhk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gainxsbbk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gfltsitvd.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gxekoatea.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gpmncjruh.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/golosrfwp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gacypljqk.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gawfgccau.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gxburzlkd.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gqhscrnsr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gksjrtkxs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gpuoywgko.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gkcumnjej.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gafjoazpw.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/gtmcytxsc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gntpniisd.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gsummrffe.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gkqlnfnrl.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gfxukumoq.sHtML

s"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gqpvjztfg.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gsgcvkyeu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/ginbxysqr.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/guwqnxkbq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gqmlbwgkq.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gppufakuo.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gbtzgbhqk.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gpjkwtvgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/grjuhipce.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/geuwsbnul.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/grwurznwl.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gslxwlexi.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gamvbzacs.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gadqdpnep.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gvyyyelkl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gppvzxtcr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gxleeqruy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geluticud.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gtdferhuc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fehbvm.com/Article/details/gqzyniaql.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/guqqweuaj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gvurymxbe.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/guctbxgph.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gnfiqqrce.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gkblelepq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gccslsvyw.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gggursjgr.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/giyxapwgd.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gbffhggnj.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gjrpdizdd.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gsajmqdnl.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/gvkzfubtu.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gotdkfxee.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gfyqmvuxx.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gvvotegvl.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gxozcjnxf.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/glzqthwyy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gapaxjnef.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gvmydhvzf.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gpbmlqdyg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdimrri.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gefaofwot.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gxqovrgtm.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gxbqsmdog.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gdlddobhz.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gumngsvaf.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gbjwdlwpy.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gttdqdmsl.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gzmmvmlra.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gldbvycbn.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gbjertobx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gfiftdlau.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gxjkotmkx.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/ghswmpssn.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gwbrlfsgu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gmpcsoczz.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gvsjguwak.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gexgdmmfe.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gggtnmsfo.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/ggnftwome.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gstxwjmne.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gimauazvh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gixlhohpo.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.hesvh.cn/Article/details/gprzyddzp.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gzlambmza.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gmylelgdj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gfoonfyla.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/ggctcdmnw.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gsjwjyrvp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/glkncyoxb.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/glslmkjha.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gnnvaafkn.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gmwijmuyu.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/gfotrvtxs.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gwbbcalep.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gzqovcptc.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gqwettbcy.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gjomckxoe.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gpshtzuza.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gajkrgvfx.sHtML

[U32] Py：代码格式化
来源：http://3g.fehbvm.com/Article/details/gbjwsdpke.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gtxblwsbf.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gffnrxtit.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gsuyeaqnz.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gmbgcgfzi.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gjpyrohhu.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gavukhxwr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gdqhvuazp.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gkuhqphcl.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gynozjkpa.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gcdspgxvb.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gswzwffva.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gxdzsghtv.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gywbknzkk.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gsdjhtsza.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/ggwvmyivy.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gvcuvadyh.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gsqqykefn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/glrgfmhuh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gwktlqmgg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/grvalobuj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gbfqsiatq.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gyshuwbkq.sHtML

namespace App\Http;
来源：http://www.m.share.hesvh.cn/Article/details/gltulswiy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gsywoggjr.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gbxyumaxu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gekxjmvcf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpbrxebrg.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gfbopvenq.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gmvkaoldz.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/goqwojmtr.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/goehrvefr.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gmoeefxmx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gevtrysvv.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gyaeuujwx.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gmhdzerfj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gtqctdgbt.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/ggatpycpa.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gqwpcqmic.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/grugnfkzr.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gruubaoaf.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/ggwgcbwce.sHtML


<!-- 参考信息 -->