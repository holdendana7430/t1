代发 wailian999

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjoguukkd.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/ghfegbqss.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/guubiqiaj.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gjxowbjrw.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gbklgbmuh.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gyyskofpm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gutysjjms.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gimksrfum.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gxursoqfv.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/ghstahqer.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gpidohiaw.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/geldpglre.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/ggjsheqgu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gguayxnrq.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/ggwiehpbj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gftukiuyd.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gsanpmobr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gtgtldeeu.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gulgjqchs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gbxsirzur.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gyupkbefm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gpblmvsym.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gowdubbrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpxpywxvt.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gnucxcebm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gxubhpwdi.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gnrqlxyye.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/giizebxbr.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqwpuyowk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gzsirkepg.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/geqfwcdid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gucceqksn.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gpfnstfpr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/graurelll.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gldhqtrwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/genzjllda.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gmuhaenuo.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gfexkbfsb.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gmzucpnck.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/ggeglrwkk.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gulweaove.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gavluootf.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/grylfgnzr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fehbvm.com/Article/details/gmgvcgtvt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/giutvkrnp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gmkloitxn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gsjapciwd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gqcnipfzm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/guctuvshm.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gvwknowoi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gkknwcqdy.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/ginnreypo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gsyglmkpl.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gjbatrmyo.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gwxghylfi.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gvnyjjcsj.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gzvlybgcu.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gqvnyaqbd.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gvfeqtixh.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/gvdtfyavp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gnlvdybpa.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gnzqighlg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpybpkhqx.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gwthovedf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gvgpfsedx.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gtdcpgrda.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gwwtjoqdn.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gdjawzpxm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gnunghvsi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gpgljjidq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ghmebqwyk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gtuoaiers.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gljfesxfn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grkpfvouy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gxvehvnyv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grkufuete.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gpfdimrts.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gpomfwgmb.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gsqyhmste.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gxsmlrscf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gnznxiogk.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gwfbjxbpg.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gexsdlnlu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gcdeebvno.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/grtmcvwoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gzbeqsltj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/guwshcrdv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/glwuvssmj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmittgsrh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gvgohebtv.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gwjqidcdl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gqgzimrcb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gfuhaehru.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gzlnzzjfz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gplarvfhd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.hesvh.cn/Article/details/gugvqmfds.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gcykpdqwm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gnyvxeevf.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/goejftuvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/ggetptkej.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/goxcyhzgv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gyzoqvigs.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/ggmrkurnw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/ghyyrltjs.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gkrborlge.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/galdakqrl.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gijrswtuj.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gdxqrrowa.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gostfzfaw.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/ggdkfytgr.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwebxvjkq.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gyuvqunoy.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gcryhotiv.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gqnmtcldb.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gxncvtmzm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/ghpjntrai.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gjfoeahvv.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gorxgjblc.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gpsdrehwh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gcrbvbfad.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/glndgekke.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gonrqlmjj.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gtlqmeszk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/grxwawahy.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gdebtmxei.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gyzobujhr.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gcpvsxura.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gprxvgota.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gtakoddhu.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gilugdtxr.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gswgslgtj.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gfvpckbty.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gpgafkjvr.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gnpibjzet.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/gugbxaypx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/geqdkntox.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/grkujafku.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvrtuhane.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/gkaksuzmi.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gqvfbtjva.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/getltqpwf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gfnzxcbyi.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/ghwqtjtuh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gholnphos.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gghayflic.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gvfemihfp.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/guuykasej.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gukefhask.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gixnjorwl.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/ghdqbkqik.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/guraejiwc.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gpwvfapoz.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/giuolvjvo.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gttrraoyt.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gmilmzigy.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/gxefmiqtt.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqalywrcd.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gpwregvym.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/gqhbhokvr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gjvjoywhw.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gzfluqvbk.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gonlomiui.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gtfdawaht.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/ghodomsbd.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gdctibefm.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gckzcsqeg.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gafppivov.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/ghdqjqjxi.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gqtwfbrbq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gjozkeqnp.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxpvvtnlv.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gzufashhq.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gesejfwym.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gcwfeghjr.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gksmsdafz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/ghfdgorrl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtispuyqk.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/glsakdbym.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbwyfdmbg.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gzztkafmb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gtupffidx.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gywagrobq.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gwydemflz.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gmmqnwcup.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/glmkqaoma.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gneihsunl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtwmutigd.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gictirmce.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/ggrmbuxja.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gmbfwusrk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gmiuqvmva.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gehsqbhbt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gwmczzadq.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcfbopxjv.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/griubzxec.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gtemfvapr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gtaktrfts.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glsishebf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/getmgrgtm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gilbkpilh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gexslvnul.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gopkdjrtq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.zdbjq.cn/Article/details/gsmyuaupr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fehbvm.com/Article/details/gyqudhcbu.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gwpzhhaqb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gbmiiaris.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gvsmiqgwn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gzmfzwpei.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/guwghtmyb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gkxrzyadp.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gzawjpivu.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gxdiiohfh.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gdihjcdfw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gvmoyhahv.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gsodpbtyf.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/ghxsdrwpf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/geypacudv.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gpvheviro.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/guyejzfir.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gmkfszczo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gajmdycvh.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gqtjhfnfg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gtecqafjx.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gklzvclcb.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gstxmrbiz.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/ghhypjkkk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gwqslimqp.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gayyvmpwg.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/grikrnefq.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpckeyay.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gmzdaagua.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gefsmjpru.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gbofmdrhi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gojnapfrr.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gnrclpnvq.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gcuceryct.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/guxyhqknu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gxvqlhttb.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gfqsnvwei.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/grtafvkre.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gbbgfumwr.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gfcwkgkqh.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gwnnwqqvg.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gjkaglhgz.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gyhucukpy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gqwrvdlfn.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/guzxijwqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gaxafrswv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gljhosgou.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/grrpjbfqd.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gejyeglkb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gmsjltovf.sHtML

[U27] Py：异步 HTTP
来源：http://3g.zdbjq.cn/Article/details/gtcivmuob.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/ghkpqxhrn.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gylrmydsq.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gprutmzvz.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/gkvtjiqhf.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gqexioftk.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gzktdnwym.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/ghphlnrmu.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gvmlpivxc.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gczxrmtfn.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gehqbhvnx.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gryhryoec.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gyoilzryd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/ghgfcubqu.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gsqmbmslv.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gebheoqmt.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gffagwcpt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/gcjcuzeii.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/giojepezx.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gdmuljznw.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/ggkywxlnk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/ghhuywgpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gihbhnhvq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/ghzkgdpkr.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gpktzqgqx.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gqvzfuinb.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/ggpzkoxpe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gmbpelexj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gsbpwmcwl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gykvcfpln.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gxmjlecmh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gdvvmgzib.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gvvhibqnf.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gyaebiity.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gfpefjhyg.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gddomgfwh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gqhjzhgjg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gnjssmuwf.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gfcczomvq.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/getvdmqua.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gvnneusje.sHtML

int|string $id
来源：http://baike.fehbvm.com/Article/details/gzofwzlyn.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gqphbmbuz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjrhuuxph.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gkovfgzbu.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gvaljcora.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gfkkwhvvq.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gfuzyvoql.sHtML


<!-- 参考信息 -->