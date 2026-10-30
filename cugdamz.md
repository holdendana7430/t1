代发 wailian999

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmrbufmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gadptorts.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkgnozoj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gltgdcrsh.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjyftpdp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlafafyd.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdccvvgn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwttobny.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gddqcqwsm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmebaimu.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gcvyunojm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gqotrtltm.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/goruxhuhf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grxytqezb.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxmdoatz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcvzwnrb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtgigogu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiteevhp.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gkmfdpiqx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gofsxmcnz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guipoctiw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/ghrdiyksi.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxdwkbw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/grvlemcza.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkgnimqi.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gntkkeasb.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/ggetoyara.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdscnmped.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmuptsy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gskxgacsu.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfrxiffg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdbslqml.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/goeawydbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjgeougjw.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/getagzcjw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnbocbir.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxgnuhsey.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwbcxluix.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnymixjbj.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gxeatjdni.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/grkevayoz.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuuoujkp.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gzyihoxhk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjwpghh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcauiwws.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbzcxnl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gpzbsmkem.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfqpmre.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyomckdpl.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjofvyqc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/grpxlvcgc.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/guyxytydh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/goeesqhzl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbofecsz.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmigwogv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glttcojan.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtcxhfbey.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/glvprtudu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gwvvjctuu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpbzkwce.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggqwqvvmo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gezttckvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guncrebzo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqjgbqd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqmgnykf.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gigcvbhoy.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/goytocjrn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gwlwgjgwo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxersnx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gumsdosbh.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvgndrsb.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gktxjfpuz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcvflxad.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibwuknay.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gkssmiwkp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiodixik.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gvcmztcus.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblqnzfci.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gkdbcmams.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gfeafjzif.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwmrruxj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gnurpwbzg.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfymfslr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gzfezgdvw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxcdzbsu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/groxmypee.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/goerjjkrz.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grcafjjta.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gdmhhmcpz.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpitowfdc.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauhhhtat.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gagwggfvb.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjchllsn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gfvgnwsuy.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyvfvuck.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmbztqwt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgiyjul.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ggtawunez.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gonuqtrhp.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/grlvrlcuy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gceljjspa.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glpujecwm.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gxxewneqg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/geidyqslw.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifurcius.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxymzytu.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grkyttqkx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtnweadp.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcjwqdmc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/goerxbynn.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflkdcnxo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjtsexbb.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/grllctkin.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gknucljum.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gsoeteqni.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavlexwgx.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbjvqkk.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/grbslxjuo.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeqbbspg.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/glmpvbruy.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/galrsmyfx.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbtgrzpt.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdfvshll.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gidzauosl.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guapzfvkf.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gucelpvay.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwgwxzug.sHtML

local a = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/guuvkszlc.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvrtnadp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fanxiaobao.xyz/Article/details/gubjycxpr.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gtwjrovue.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gljlbjjwn.sHtML

[T35] Lua：字典表
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjygpfyt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwmokkmg.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbwmgytiu.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gdmprcuvc.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvjbjdvp.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhcciies.sHtML

[T38] Lua：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfbjfid.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gvvkuiryo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/goccmjirh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicrustgo.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gvuwyzvpm.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkdckoyc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrwmbggt.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gellzjzyg.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gzvxvnbec.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gshnwblyq.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/grmtpblho.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gvubfwgey.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggyeywocy.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaerrqxw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfcpkcgn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gogqolldg.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gmfhgjftn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gynmgslht.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjcaeagk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkmkbupti.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmlzbtp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghroxrqag.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqcbylxhm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyuxlnqw.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkkxgesau.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyerrmwu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpukgtzrj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskxpuagy.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzrulbpj.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvzxvevci.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gxoyruzck.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevluozya.sHtML

s"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghonivfie.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxddjnvr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxclvzh.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebwmzna.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnryrnieq.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/glvnuyuqb.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gckvlswah.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gsradmjyd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geewxzdnm.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmqnqxvv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjakufaz.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkamskss.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohkewwuk.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqdstbst.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyigbiyiz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gruvdxaxo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzfzewddw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/godvlgjjn.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiuvqfhq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gbiuocfvh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtacwopdg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvutmrllm.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkmrlnna.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gdahnytrz.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gedsdvusg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdstqxus.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gvonphywg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhwphjcq.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkhcelkt.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gzjybmdgz.sHtML

[U07] Py：反转字典键值
来源：http://baike.fanxiaobao.xyz/Article/details/gmydxjhiz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fanxiaobao.xyz/Article/details/gbqnyitgn.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxuxvrbh.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/ggyprcjxe.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtmstfub.sHtML

max(d, key=d.get)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhroovzw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyufylss.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fanxiaobao.xyz/Article/details/gthgaqmki.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkedoeiyi.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbsdvgyl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fanxiaobao.xyz/Article/details/gcoxgvkcf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvtjtvmd.sHtML

[U13] Py：固定长度队列
来源：http://baike.fanxiaobao.xyz/Article/details/guyiaowng.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gnoppiyqi.sHtML

[U14] Py：分组收集到列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghchfbwdl.sHtML

defaultdict(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gexnqmpve.sHtML

[U15] Py：高精度计时
来源：http://baike.fanxiaobao.xyz/Article/details/gcbltyinp.sHtML

t = time.perf_counter()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawhhklwe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fanxiaobao.xyz/Article/details/goznwhtdm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gqbnaxvny.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbeyxlgh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxjhffqm.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gjljjrrcw.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gigsrcozt.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fanxiaobao.xyz/Article/details/gphyekajy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmoktmwzr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gbjaujmsq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxahwere.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxghlan.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgwfrnzq.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwbdtvro.sHtML

list(zip(*m))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggsnnjdx.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvzqdavp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fanxiaobao.xyz/Article/details/gycfzisky.sHtML

[U24] Py：路径操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuuyqptq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganwxbccp.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/grwdixuhf.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gzgebwfjh.sHtML

[U26] Py：并发下载
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlzfxyd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzndeshrh.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fanxiaobao.xyz/Article/details/gqwgvjvzg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtzjidrj.sHtML

[U28] Py：类型别名
来源：http://read.share.fanxiaobao.xyz/Article/details/gozhaqtdl.sHtML

UserId = int
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnvnbklv.sHtML

[U29] Py：属性校验
来源：http://baike.fanxiaobao.xyz/Article/details/gyaeuyzay.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltyyhved.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwlustww.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycnfapwl.sHtML

[U31] Py：单测
来源：http://m.share.fanxiaobao.xyz/Article/details/gxevtztuh.sHtML

python -m pytest -q
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdiffdgp.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzfeubtf.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhxqhyg.sHtML

[U33] Py：打包发布
来源：http://read.share.fanxiaobao.xyz/Article/details/gyikkcegx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbnghvr.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/guagbmgjd.sHtML

chardet.detect(raw)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhtdjpca.sHtML

[U35] Py：发送邮件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmpfxqxp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fanxiaobao.xyz/Article/details/gvaamavtm.sHtML

[U36] Py：定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gqegsupss.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gzlbyacez.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzfcopue.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fanxiaobao.xyz/Article/details/gdfoxiokx.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fanxiaobao.xyz/Article/details/guxqjijpg.sHtML

Path(__file__).resolve().parent
来源：http://3g.fanxiaobao.xyz/Article/details/gxgakkaru.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdamtdri.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/guiipqnej.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/gczjqprgd.sHtML

print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gclhxitoy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fanxiaobao.xyz/Article/details/gpdijlzgz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqxczvfp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghywqzdow.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.fanxiaobao.xyz/Article/details/gspvcghxi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssmwofou.sHtML

namespace App\Http;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlvagtnz.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fanxiaobao.xyz/Article/details/gsjjkbhzx.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gerzgimvi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gokiguctm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtnhlqaom.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/gurwvtgge.sHtML

?string $name = null
来源：http://baike.fanxiaobao.xyz/Article/details/galeranhx.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfqbnfbog.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gqzmoflgn.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsemzrdb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gailpxzwp.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelnpaflp.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfwrztmv.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/goepcblcu.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwxqgvqzd.sHtML

[U51] PHP：数组解构
来源：http://read.share.fanxiaobao.xyz/Article/details/grtajlcqv.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/ghiebbddy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeuynnbd.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gzbgucpjb.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexpvrys.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpnesgae.sHtML

[U54] PHP：空安全调用
来源：http://baike.fanxiaobao.xyz/Article/details/gjizrsirb.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarlaliv.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ggmlbewfl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gauefvhfv.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyezrslo.sHtML

f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwxodeyl.sHtML


<!-- 参考信息 -->