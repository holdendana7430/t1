代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gpihmztez.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/goirkluwt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gnzpiqmyv.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/guzduhpkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/glmvpmdif.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/glrmrmjvt.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/goejgzlpn.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gdgvsrfun.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gxvjwxikv.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gnuqwazdr.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gvhbuamsv.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gdbiogsgt.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/grqgxpwyu.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gvnqoozlu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/ggeltqepb.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gcwyosyrc.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gjitjuhly.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gjrvvjwdn.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/ghishvhva.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkzmrszbz.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gntgucktc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gjtkoxjnk.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gewdwvjwc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/govkgjkxt.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gmuuealrb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/ggeiamibu.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gibpdcpov.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpojfixbz.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gccehyrvq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gojlxkzrh.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/giqfqmiir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpgrebswk.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/ghqfzdhlm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gszmqczwz.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gimvnndcx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gchfqaspn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcafumpoj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gfjjxzvzk.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gnexketdi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gcwhtndgc.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gqkupkvaa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gwyyqiynb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gfldesovw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/ggbokvfrs.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gxestfted.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/guvtjvudk.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gfcfuyjzu.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gpudhovsl.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gwzfdbeyw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gepqawgyb.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/glortlafl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gcydevnyy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/glxdfkzpp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gpcxkfhye.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzqodjocz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gnayojozj.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrpyfsr.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gjzwzcymp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gvdooumrf.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gfwuopdjr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gifrtyyrn.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gzswrjvyd.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gyzomrjhg.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/godhekyfz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gfpkrugai.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gyantbzwm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/guesrocel.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gcwarvrvf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gzkzrmofw.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gojhfvkdc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gnnbzanvl.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gycfdhfdz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gjryamqba.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gbylxxsbz.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gxbuxyphz.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gxwmmryiu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gvsuqrpdw.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/ghvhnzyty.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gmxpfxwlp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/giddtrfct.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gpsjvtoaj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gngwwecbd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gpvxguslq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkyxvlegd.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gupfpigtx.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gemrrhecf.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gltxivwux.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gsxplrqqv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gjtjezisx.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gwmiwsvfa.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/ghuxprods.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gghmzrwnh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gvlqvaxcy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/galdzliuh.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gmqbltazx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gchrgxvtj.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gkppvhmfh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gotdhdive.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/ghmbegvbc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcztqdxz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gnjbhxazy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gqaybpmwz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gxftqomeg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gqkftxlhh.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gienlwkxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/geuxoeaxj.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gpjmhqtah.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfworsdkl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/giadaypue.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gtmtwmkkz.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gmfnjfwdm.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gjdplvetd.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gljerfhbx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gedoutbtp.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gchfsvfpd.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gwxevfzrt.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gahfcqsje.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/goqaikuyr.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gvznelzpu.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/ghfdoqbla.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ghwnldxrl.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/ghujtnwsv.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gfrwuijdz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gavqsuuem.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/griremokx.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gxidbaskc.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gwfpqbsir.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/geewiuckx.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/grjznwjrd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gjhgzwnyz.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/ghrykjyox.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmmzecewd.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/ghorqemkk.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gkngoyjpn.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gwgoahuos.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gbrfdflsq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/goandzrqz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gaurycrwt.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/glunnwdsm.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gnuujshkp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gcolzaaru.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gnxoscfva.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gmyzlfqnv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/galfzunsg.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gfvxomqwx.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/glghvxirb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/grijcstfs.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gzhvcmhyq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gwkqiqpdc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/ggommatnf.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gebopfuyl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gfnnddqwo.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/gxzgrbhaf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/glnyfwgwf.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gzebpmkjd.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gsecjypwi.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gsgtyhijq.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gwoniacpi.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gqmoqmukg.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gjkldyayo.sHtML

[T39] Lua：模式匹配
来源：http://blog.fehbvm.com/Article/details/gpgaqwlrm.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/girnezeyb.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggynklgpc.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gmdjrrnaf.sHtML

[T41] Perl：Hello World
来源：http://wap.zdbjq.cn/Article/details/gjhwllbcg.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gahunesxw.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/giczuuwnk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fehbvm.com/Article/details/gxaoeggyl.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gtewnuoci.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gsofqashv.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/glxarkvbg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/glratmybh.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gayqdktug.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gzpozvnpd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gsrfovser.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/ghboyavqu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gpaollycd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gslqwrvbl.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gogxxqbnp.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gxbsjenem.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/giimuvbmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gticqxsip.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxbusvlyi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gahctkpcz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gxxnzhnbh.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gxvhpblqw.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gslumgcrc.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/ghlvypafx.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gfuphssxi.sHtML

[T53] Scala：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gybkfxmnb.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gowcsylse.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gcmlpvpwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fehbvm.com/Article/details/gbzbobees.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmfyewmfl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/glbtzrtlv.sHtML

[T56] Scala：样例类
来源：http://read.share.zdbjq.cn/Article/details/gqqfjkyuy.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gdotvcbhy.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gvyucxhsv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gozgglwjq.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnnfanxdm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gaodkitvh.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gqsameukn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gumikfcvj.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/ggaawmhog.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gchycncld.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gganizqaj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ghtbicszc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/graizooqp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gcldzuonz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gswdfkyyt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gqgeeblmm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gwhdouegp.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/guxnjfgoi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gjtcftmup.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gfpargorc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gitjnycaj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gwluwlisn.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gnfcexjch.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gsyijlikb.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gaonbkiug.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gcztylomw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/geddstjqw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gqthpxtpm.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gcdhskhpe.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gwsepfqik.sHtML

max(d, key=d.get)
来源：http://blog.fehbvm.com/Article/details/gtejcqgir.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gznrgargm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gmrskdeuw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gbmmmloal.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gwmgrpnlt.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gcjoxsthe.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/gygutxmty.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gftrbbekb.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gmkznjzsm.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/ggrnmfokd.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gpartpshv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gljhyqayy.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/govccdfsz.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/giryohqzr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gyzzctres.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gzylxvfle.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gmnvpkojf.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gzhiobrrg.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/glwmflwqk.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gwpcixyue.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gjvysdjek.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/gxkahyqwe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gqvbphwly.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gzlseoeih.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/goacrsdiy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gsagvbmvo.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/getbpzeqk.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gweqegjcy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/guehshtlh.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/giydoiiyb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gvyzucohr.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/ggrgkyerh.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gasbxermn.sHtML

[U26] Py：并发下载
来源：http://m.share.fehbvm.com/Article/details/gyrqjnqud.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gcatakwrv.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/guexdsyxq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gfhhwezua.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/gwokncpyh.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/ghhxopdmm.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gvddwsuxf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/grrtervoq.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/ggmdqfsuy.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/goicitglb.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gkfsxwnic.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/glraxdkaa.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gkglozdii.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gwhntrjml.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gyalhoahj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gufnacsta.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/ggajqxnxg.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gtlhtxvem.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gvdhdxvfn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gufxfcexa.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gyhpmbvji.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gymetdecb.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gfigqtiyz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gilbbzprb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gxnkpxzqz.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gkwncporg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.zdbjq.cn/Article/details/goszsywlh.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gosfiglhm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gjnhcfxzd.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gebpanknr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/ggmsalyka.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gnlkqtnnn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gaofribwa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gyonyqhlh.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gbxntwvox.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gpchmltik.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/grklmuihy.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gfxzoedzo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/grcbxmvcz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/guyrmfwhk.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gdflyqfvh.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/geuhdfcqw.sHtML


<!-- 参考信息 -->