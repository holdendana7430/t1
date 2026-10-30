代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gfgqsiuuh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gozppbsdd.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gvzhhmytx.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/guicbcexy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gbdbhfrnj.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gvykltvkt.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggldixyok.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gpxnulkbn.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gcdzvrekk.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/glvbasrlq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/ghuyunirn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gfjrqcpyq.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/giopcvybe.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gsphsdgrd.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gyhysazxe.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/govdhsmit.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gngcevyed.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeyhbauc.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gqaqxigaz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/giwrcvsxr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gezaqkvme.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gdnnmtqrt.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gdksezwbp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/gxapfpkyp.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gezttuigq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcoqeeqtp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gkaiqmqer.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gbjdyfpyr.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gutthxrgu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gzzcsnamj.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/geeqejpla.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gmpgtncri.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gvibaqthp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gytkofrfs.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/guxlnvfgi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gwcaqdoen.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gylbixnjq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/golmtcwxf.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gujfakdrl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/goukfutzi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gedmiusxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gighsmsoe.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/ghbtudfuj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gptrujgbg.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/ggwdsfiij.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.zdbjq.cn/Article/details/gazgnblvi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gfzwqnxfw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gtxsivcnv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gwassjdmr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwatkxbx.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghvjbpdfj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/ghszotnqu.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gvxwtmsji.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gyuimwvhm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/glykmrfus.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/glqabbikk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gyujfiaac.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/glwbubpgr.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/ggfaogctw.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gynklqnwy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gtdinlwzx.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gntgzzzrz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gevvadcws.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gvunterhm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/goebmzkwk.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpnfrroyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gujqwpwxy.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gejppibbf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gwwgcdyqi.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gbgupykwn.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gzzofqpuh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gfcxjfodn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gchcchyea.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gklattyhm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gwxjvooll.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gwbbthouu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gahyssuka.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvfohpjik.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glabjaqfa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmwagdja.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/guajqkeeg.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gzpppggmo.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gvxljpmdm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzekqehhx.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gatlszivl.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkxzusehv.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gxhttzvpf.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gxcsrirwe.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gpzpkvcga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gdixuckgw.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gpgpgrevj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/gkctczxna.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gunublzmr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/ggvoxwpqz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/guicrdxie.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/ggddprxxn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gmwsbmpuu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/ggbuiusgt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gwtpbgnmn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gympjdyzq.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gueqtiaam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gnwtkbmqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gpcvkgfdk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwvxrerfe.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gjxpwskvb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gumcgvyyn.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gxvwqrgdj.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gstmvhdon.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/ggmlfvgbv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gscocygeb.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/ggzejfobk.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gxmwrdfep.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gerdzfmmc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gzzqxmqln.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gevkrzbrj.sHtML

"值: \(b)"
来源：http://3g.hesvh.cn/Article/details/gznwjepdm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gujlaebwh.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gajbfnpir.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqueyrybj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/geljhgicl.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gotpjbvnk.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gfpqrayso.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gwzqgepdj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gojhrteui.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gvlcvttkj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfrjmihek.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gwxsdioqj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gozjnrlvs.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/ghuvrclrq.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gcvrheqmh.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gtgsazcgq.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gvygkdvcw.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gystxnjlq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gnpdzvjuf.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gavkfeuom.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gjepxeqef.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gnacmzcuk.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gzozkxjpu.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gbsxkundz.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gxnaiieas.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gvebmjjje.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/ghqgvzvpg.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gmgjdndvf.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/grhdjrrnm.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/ghpadsipk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gxpljwuxr.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gdzkbysww.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gkklkbmgv.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/ghksqavsz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gbcrkngqe.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gwlsizzbp.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gtthoqtwa.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gwpiojvqw.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/giiqjozzg.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gehlzumry.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gjuxctldv.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gmkgiagbd.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gptuknzbf.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gkrpwbkey.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gclpxjtms.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gffmqfqhe.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gyhkczgkq.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gqawlsenl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggbvqgqoz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gbqnkjjep.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gpfzofkzu.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/grlpmhsxb.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gqudkuhii.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/grtzcflby.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gedommioq.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/ggcvaeieh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gxjtjvbof.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gktusophq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gjqimwyql.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gymjypuiw.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gjwikchlu.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gviyigiof.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gjfvxtwon.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gznzcyoch.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gktitcguk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gvwdcsjxf.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/grhoddudf.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grnoatkmh.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gmxolcukq.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/glfhdjlqd.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvrauvalc.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gtgdsundj.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gagzbffnf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/grgjylmdj.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gvsfknugi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fehbvm.com/Article/details/gvwuiooka.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/goodcemdd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gqmcdbawc.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/ghqxnevni.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gfaopoqlz.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gdijgrmgj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/ghhglapuf.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gysbtnwhz.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gsxmkinkr.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gcfsvccfr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gilsfmavm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gokkwdsjs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gvvujumvi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdcjuogzj.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/glnfzpqbl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gwoxisewz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gecgakcrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gsvwmoeaq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gwffrdevn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/glxynluvt.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gijubizos.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.zdbjq.cn/Article/details/glmqkxeiy.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gbqawlioe.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gofmhbmmk.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gahcnvqnp.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gvkmtnnnk.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gnolbaito.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/gczpgjyeb.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gmxeyyzhj.sHtML

[y for x in nested for y in x]
来源：http://read.share.fehbvm.com/Article/details/gxiqjywlb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gwwiylqji.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gbmaizsgf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gpcjhuhys.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/ggzwpxrsb.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.hesvh.cn/Article/details/gukpfhrdj.sHtML

(x * 2 for x in arr)
来源：http://read.share.zdbjq.cn/Article/details/gjbtabuos.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/ggcqvdwbf.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gychibgjl.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fehbvm.com/Article/details/gazasisew.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gpvfugmmh.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gzvraowhr.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gkrrkystp.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gmhrkfbkp.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gnhqzgnpu.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gpjbiatub.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gkkhnphix.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gtmyqnsia.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gueuukhvd.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gpxhrsvty.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gjtcnxbzv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gjyqfwoyf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gmfqtgfwg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/ghxpatrho.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gvkyqvjul.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gdctandyp.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gxohbukte.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gjmwhxmrt.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gzgaegpbj.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gpzcgikko.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.zdbjq.cn/Article/details/gjzoisfcl.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/glqsgjhey.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gicgqlpfa.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/ghoquklek.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gxngssfnh.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gvotzectf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gkuckjbfp.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.fehbvm.com/Article/details/gymlvclyr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gravtjxnx.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fehbvm.com/Article/details/gwkwzztjz.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gagiutwgl.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gcfmrofbo.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/grujoemwt.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gtvtdzjsn.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gidafjzih.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gsrcvnqsm.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/ggsnvjmsi.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gzonpzkvx.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gocumhapl.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/guubngyux.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gjazyukxe.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/givtcersk.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/glzhcnlkn.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gbdeducwy.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gqihzlyte.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/growzweee.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxvkwdvn.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gttomcqod.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/ghlonfdzp.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/ghpumkdfh.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fehbvm.com/Article/details/gjfgdqvru.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gsexxwbwx.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/ggafkfvhe.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gllsbvluf.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gtuprcgyq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gfjeqzvrb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gvwosrirh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gpghcjivi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/gykmdwtyh.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gshlfkfro.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gsdoddner.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gbnlkbfwb.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gxsbxuvwi.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gxkifawpd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzrkuqmkc.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/gwnbwsoyw.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gcsfiqrfh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/ggwfzwbax.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/geaugvbbk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gslkxdkap.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gppgbddvn.sHtML


<!-- 参考信息 -->