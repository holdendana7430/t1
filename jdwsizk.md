代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbljqvjl.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpwbpttqe.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujwrhldd.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gztzkhkhl.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmcsyzix.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ghzqxajoj.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gjxundtfa.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gycrrwvcl.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxikeeuu.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrxkpzfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggruomtds.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gczncztwo.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gtzojldmp.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemwmtgna.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvbtujsx.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgcfrjto.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpgygsnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqvbdfauh.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gulmfukbj.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gefkslrpd.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlisvvkm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfufyimor.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gqrnjjrhr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfclyglf.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvczzgfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdweirnul.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfqgsqxv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfdvhyiw.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gyynunojw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqkutndkx.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvuqeaq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gunpmrqod.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcbussjar.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqgtfklg.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkeeftkf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiifdxiz.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gspheivdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gfffzuhde.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqqrhcyi.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpverei.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/guvumrxaw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/griiekglg.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gxracudbh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaolcrwuj.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gzbtsfhiu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gjpgmmbqj.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gnercecro.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqdzfmaum.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gyomoiwyf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaubdjsne.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glahyozgr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gjnppfvda.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqnimnzj.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gulnenfuh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvreduuj.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggjigszlt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gtohtvdlu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gcmxmjyim.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpknuhtri.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gvzsjaesr.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsvyjenjb.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gywnhyrdo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzjiypfx.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/guexpptrr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzociyden.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxollbsv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlykqftv.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gpjtvbirt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glejoqpxy.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/growublnh.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggzhtfygm.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gpptxtten.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gucronvng.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgiqwirm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjevnqmzt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpnbzurk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/glfvjugzy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grpnyaigu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrmyheki.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghjwjwjxk.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfxacwgqe.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/guemfnieu.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/glyrqshwe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjjvouvb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gxpyprwwm.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghhqzdnxp.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/gesmhhucy.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfigyaym.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gmqfxabwy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gpqiphojl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/goqxvytar.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrfttxoq.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsfdcvof.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjncmofyv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdbahsnz.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/getkoqdst.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwokjbgmp.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrfuznrg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngmdybr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/guilqbfqu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexfftfw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuuxkofq.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqywhcef.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkihfvxrk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqyisjdb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzwbyowo.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvtqeht.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gfnoichci.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdovxqbj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpwfbipb.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmgwbima.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpfnbkvv.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmhukayaz.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbivdfpxo.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gzqrzmntr.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcoxahww.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gedmwpvyl.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/glkiroxhy.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcqodrnd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggublbejc.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgdqxcay.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gkumjbfwn.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshouwuk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbrkltfr.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsnsgmbp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gswtopcgp.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeihxqtd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gatdbwmgp.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvkzbqpi.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgoeqfgz.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gqqdrhxxf.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdibche.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gvalbihlx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gktzdujed.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhzhcsr.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gcvoclhie.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gqcfcxjfz.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscglyjwr.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gofttuxhn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/geuurrsir.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxojbsbqx.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gakbmznbx.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzmjljis.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gttjhmbhq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstnsbcxx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gcppkomwo.sHtML

[T34] Lua：遍历表
来源：http://m.share.fanxiaobao.xyz/Article/details/gyluoakhl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncwcplpz.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gasielbvp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkmgjucz.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgqmsclo.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwbwjnwb.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoloknew.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/guzvbjtqu.sHtML

[T38] Lua：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gthzxkmdj.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqezyjmqz.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrkzcykv.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnwnlvd.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gnuxwywku.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gxlaojkia.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gquqfsvgw.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeslfjbo.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gfekjvnni.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gzknznltk.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gsjieolfn.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gackftasi.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gwhfvyvse.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfaqsnur.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdteckknb.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamqttxlq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghnnylned.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvtpwcqz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/ggxcfxueh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/galvswbvf.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbhvphri.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbomtqsx.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghoflfjgl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtjdbmx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtbdhgkcb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/guhrwcopw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfhszupz.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbienyhhi.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gptyrhuyf.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcagthsui.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gerfryxik.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gczlrbbjd.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gdlvqhqik.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gikfhwgrg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/geieaijll.sHtML

[T55] Scala：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gepdukoub.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggivagvjo.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/ghjgcxhri.sHtML

case class User(name: String, age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gqnhsckee.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gznvbucsp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzelelqmg.sHtML

[T58] Scala：函数定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gjassrsxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gwqkmixfz.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfyoqauh.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwwdajea.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gnliofadc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fanxiaobao.xyz/Article/details/gizvfblbk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqrsmiyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbexysnzx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghjhpcbex.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltkpfcpj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gfuxiatav.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fanxiaobao.xyz/Article/details/gooakkipi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gozqymqzn.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gjcjymokr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcsrcjzq.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpyvvuxf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gdxpfandp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyzadvn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gorkivafa.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gmkpypmkb.sHtML

{**a, **b}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyrmllgx.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gnhtdjuqb.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fanxiaobao.xyz/Article/details/gikyfplyc.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbfktjrq.sHtML

[y for x in nested for y in x]
来源：http://www.share.fanxiaobao.xyz/Article/details/grdrpncmw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gmbalibpo.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjabtbmzw.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gxvzeyurb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gknyjodhm.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/grnmsffmb.sHtML

(x * 2 for x in arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/guahryjnl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gaypbhlyq.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grknhrmzk.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gacuisoye.sHtML

deque(maxlen=10)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewpkouro.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fanxiaobao.xyz/Article/details/gjneekccc.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnijfnfhw.sHtML

[U15] Py：高精度计时
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrfkhgfp.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/glmyiiygd.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/gncyvxyow.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fanxiaobao.xyz/Article/details/gezswoosy.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjykmyrk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxtlrzfu.sHtML

[U18] Py：预编译正则
来源：http://wap.fanxiaobao.xyz/Article/details/gsdicnxuw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdljrqmpf.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/guwlezdbb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakoxrhro.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxdtxcwf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklzainjl.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fanxiaobao.xyz/Article/details/gptcreqsk.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhcphte.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhjwhxrn.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmkcdlhi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmvbjelrk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fanxiaobao.xyz/Article/details/gkmkhhkuw.sHtML

[U24] Py：路径操作
来源：http://blog.fanxiaobao.xyz/Article/details/ggmbeqnhw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkubzjcx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fanxiaobao.xyz/Article/details/gcyymucyd.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsjrsldo.sHtML

[U26] Py：并发下载
来源：http://3g.fanxiaobao.xyz/Article/details/glhrycyyj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fanxiaobao.xyz/Article/details/gjjkrprts.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajnjijwn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcwpekeq.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzbzddti.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdcvbvf.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtvavgsr.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvfhxox.sHtML

[U30] Py：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpvzxjah.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfjdlsji.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gkwtvibgf.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gexusnswb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuhtdtrx.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gjflqzhvb.sHtML

[U33] Py：打包发布
来源：http://baike.fanxiaobao.xyz/Article/details/glrxrvuzq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvglttla.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gzawbqohm.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmnmnret.sHtML

[U35] Py：发送邮件
来源：http://baike.fanxiaobao.xyz/Article/details/gzrmdbryv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtvdxcxm.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gkrutrjhm.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/grgnwhukg.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gtjbmkjsr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaspaxkyv.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gzogxwewo.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcogeyncj.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzvfrtgw.sHtML

sys.stdout.isatty()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbjenywo.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/guhgqyvjc.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gaxiozgwd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gcowzacyg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxsmhsah.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fanxiaobao.xyz/Article/details/gwxgyqucu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnaszuad.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxroltnrw.sHtML

namespace App\Http;
来源：http://blog.fanxiaobao.xyz/Article/details/getcaroqy.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwhtjrzo.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gscbfczix.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gokgehlyl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gstgrsxbr.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghcepcivm.sHtML

?string $name = null
来源：http://blog.fanxiaobao.xyz/Article/details/grbcvzozd.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrvrtulv.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gtotwrbpd.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/giyrdecub.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfnkprbc.sHtML


<!-- 参考信息 -->