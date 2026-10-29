代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gdpgimvfe.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gktxpgruq.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gvlpisvxq.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtrbbxhdf.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gtzamzpvh.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/glyicxbgv.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfpyyejcb.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvtekkcer.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/grszieqhu.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gwpduzhcy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqvrtnpb.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/govbtxevl.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gjiaetvif.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/ghvgcywkb.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gucnhdbmt.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gfnyfdkpy.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gylsxhpwd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/grxrgbilo.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtdsmzohl.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gbhggwvrr.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gvcpaezxe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gfpjfhkfc.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gtxddqhvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/grkizdegi.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/guyqatcuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gakmtdnwg.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gpttdcvki.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/guqtkdzwn.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gazudhjro.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/grzthvrcf.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gkhhdmfah.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gmwwvsazd.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/guvoqbysz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gfvakcwfq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvohahmko.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/goyvhumfa.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gdroxzkfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/grzpyreno.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gzfekzhow.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ghoyvkgri.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gisexzmuy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gamoiowiu.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gaeluelgk.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gjnpfriva.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/ggjwqcawf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gsptapzxv.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gamztrpgj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gujtdpnhi.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gkokurajo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcaduntbd.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghkesjrsu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gbminpouc.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gweyekseo.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/guvtxjgeu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gukcwbsae.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/guuavpcdm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/guvedinrq.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gbhfulldq.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gdewrrntc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gqwuywdrg.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gcuestqex.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gmijionyn.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gcilmrzdg.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/glpgksmnu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gzexgdijn.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gchwdowcl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gmqgzriwj.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gpvrhsdwy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gbbtwhexs.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gzfoxdiuh.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/glvmwkgre.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gqkvuwwut.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/guvwdryqr.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/guirgcwwr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gjgtaibmy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/ghnjvtkqu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gxmaasscz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfibmfobg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/geyckrwxk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gficsuhfk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkkohioji.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gfqdaaezv.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gjelqfgfl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gbyfyezag.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gqcypgtsq.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gpcevcvlf.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/ghqwyrbrd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gyjyfdwfk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gyymjsmau.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gzitehvjw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gcwzifefi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/grvbijxqc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/givwzjbzw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gznjxhgcq.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gxsbgofeo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gstpljxot.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gahhnklqo.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gypqovbwu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gqmxfjsqb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gjvzlqqyo.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gqekbclyp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gwxfdizxb.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gcdcfjgmd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gteizylar.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ghsaynjqx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gphtitmsx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gafxbrmrs.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gnukmwqlk.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/ghscryhkr.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gmtafklal.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdsumdldj.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gctryvead.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gfyykkmjy.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/grfzpqypj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gyhuuaegw.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gouyjywsl.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gmkelvqyv.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gmxydltex.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gmggtrkoa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gsjilkqmr.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gqggbaumg.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/geeavvfqf.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/giicdcjqu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gvqxccohg.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gokmpfwwm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpcftlhjd.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/guqmpqvph.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghybhiirb.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gymjklwco.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/goardvwsv.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gchrdynus.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gifkgunls.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gyuscfhwp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gwxuydkfv.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gmfrodauh.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/ghxxeeziu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gypwulnsr.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gmmdmmyzf.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gqcqyhqoa.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gwdnmtthp.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gvpgbpoay.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/grqtdybfa.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gzwznosab.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gmrnqhlmb.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gbevmstzz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gklxtxruk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gihnmhgyb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/ghncexrqt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gehviklax.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gaudpwsgx.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gpqzeepxk.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gtntavtma.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gayaevjhq.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gllujilex.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gwuifdtef.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gzejldyyc.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gizqlifuq.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gymsogwrc.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gywcdoujs.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/giquvltxa.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gpnsclgrn.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gvqnszpvq.sHtML

[T42] Perl：变量类型
来源：http://wap.hesvh.cn/Article/details/gtagcjaus.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/guenolwht.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsflepycr.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gfysrzajy.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gyxebggir.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gerpgmqhr.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/goxgigakp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfddikyx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gbvfyobpu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghanzfemv.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/ggcschwuc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gfaucjqbg.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gyqincnbv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gmqxynhso.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gyspzxxkr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gpohksnnk.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gvlvpayml.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gecvmqdiq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.hesvh.cn/Article/details/gkiqqouob.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gabetuhzx.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/grmuaoddh.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gssfapsjk.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/ghduwahes.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/grvwjukik.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gijwkzubj.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gtybpqbky.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtfjwairp.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gxidgggpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gsnnslrfc.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gdrqcootc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gkexmnwju.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gzbuejvnh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gedusxzvi.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gcizgmgax.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gpbxtgkkx.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gzavkrckv.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gbmgvsopm.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/gpqarqmwl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/ggmxcykep.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqovtfzif.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gbkrtagrg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giznfkzka.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gqordypvu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gfghfirxn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/ghwbxxcde.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsdnuxqau.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/goaakcicb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gzrxvmnud.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gkuqiwmzo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/geplsjjoe.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gkvacjupq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gkropmlrc.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gzeldalje.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gitcmdisw.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gzjnkatzr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gczskgohu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gjccslimk.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gcnznhifx.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gbgnffqbe.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gnaclblic.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gmfstlaic.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gnyvnprmr.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gcbthwvze.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gnwkjttuo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gxixvyppv.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gqxwnrcqk.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/grhndhtyt.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gbcmrayak.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gptrtfztc.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/grvvmspco.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gavnlvzdl.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gckyjfqjw.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ghafftvba.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gtmguhxty.sHtML

[U17] Py：初始化日志
来源：http://blog.fehbvm.com/Article/details/gczodlohx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gifkooapj.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/greyxyohi.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gcmzxqjer.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gffmarfmm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/guqqrpwya.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/ggikfxwph.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gcxkegxbk.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gxtuqqadi.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gnhqwoucv.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gcvvscjaa.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gkkqbgeff.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.zdbjq.cn/Article/details/gfminlaco.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gujinzwhz.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gpdmoioje.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gctdiuvkb.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gpmclnjif.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/gsyuuuroz.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/govjamtte.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/grcyyqrlr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/grsgooudy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gsmegrwym.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/grsrhjfwf.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gczkpqfpo.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gxblvzjqz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gewsucjbn.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gcipeaidj.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdnsvviyi.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/grrdtbpak.sHtML

python -m pytest -q
来源：http://wap.zdbjq.cn/Article/details/gefiepfva.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gaaijefim.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/ggnjgqjoh.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuizows.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ghsigsxvi.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ghfcwjziy.sHtML

chardet.detect(raw)
来源：http://wap.fehbvm.com/Article/details/gpqtdtzpz.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/gdlpinxed.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/goigpskxy.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/grnkwqbhq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gfosssscg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gnburmatg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gqbezbrgr.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gjedfmdgn.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gvkjpwekc.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gqlqbchoh.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gptkumzpw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gzhljbwug.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/glykvktma.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/glkvgohds.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gzuhhymhm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gyueuuslg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gonhwgqyi.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gvoufqxkd.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gnxpoospt.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gjfamuufr.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gvvyddhdn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gkplmgmbw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gumpzfuiy.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gqssfiyfw.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gqwtyhget.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/ghqrtdddh.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ggoalsmtd.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gnnlkbyzc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gyufxbusg.sHtML


<!-- 参考信息 -->