代发 wailian999

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2lqgkcjsf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ynapbksa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kuruktmk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2vteusqbz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2soaxvnhn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dfparxcz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xxjyetgy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaxteykh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2qussrcbk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2tlpxurnw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lhixyhvq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fdvlqguj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2scwrpvtw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2meevpwus.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uipqsdie.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dppobaay.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2nmvguait.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2iuhczisf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fvyvconn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2oiaraxav.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2aqbhodpr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2odyuoseo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ojqyghcb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wfbkiejy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hbovbsps.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2utepfvvc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xzlpvnwd.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ypafxwgi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ybyysndl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2lkhkuvpn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ddmfjceb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uxtksztn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cxzyyzoq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgtrheg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ezcxrmmf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2choergko.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jxkrejnc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uakjfuvs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qksnicem.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2bxokqytg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dggivwvu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkjumcnq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zzbiyhap.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ayqidlsz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2imnjswrq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqztfo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cbxfrgnv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bhymtamo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zijtsytm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2xcqfcyug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qkvjlzla.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2fdtbeuwg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2nepetpps.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cslzqcyq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fbmmruvq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2blxdihfx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pbwkstsl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2msheydug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2hfggqmtr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2omjznmet.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2onojvtzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcniicfu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zdmbjavy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhmfterl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ujzohorj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2atspszah.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2vfhethka.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2hsphipqv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2jgsxwbhv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2plustjjw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2zvfdbaub.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ajqxrzdu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ffarmxrl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ljnrdcsk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2enfngpea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vsremnnh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yinpvufc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2upchgtey.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hnbjitjb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2rhxpkxcz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wglwkvxh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2wlyxydgv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxwxwvhl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2tkueknfs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2pulyxfuy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2smsvhvbm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2hodkngtm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kxidisdv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fswygjdz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgyzoalf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2blfpnhcp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2neyyppdu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xhyqtskp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nehhyqvp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ocwjzran.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2unqesxrj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pjknwatu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dmcsnftg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ryxqotws.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ljmgxpqd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ujqslseo.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjagau.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2yvmudifz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2htcxktni.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bhsqmzik.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkjzriw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2esmwwlwr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vzzvtmnx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvbnkycs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tybhzmly.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2slqfvsfh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2evckdaao.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2lacosvkt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hzqyjjvd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2lzdbmama.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mewwsbex.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pfqamsxo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcqlqcv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2usxtseta.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wfuigvxt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2gedykakv.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iesckgmt.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2aqyzmxmu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbengjd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bkmpkebr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rvbchwed.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ididbpqc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2uxqqexvg.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hcxbomeo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mhzfllkv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2vrappief.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kthscktv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ifkaoaao.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2xprveihd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2orioyika.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2tvlwggfo.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ftalkffc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2jqmwmomr.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vweupxff.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zqjqvszr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bmhmelop.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bptffcae.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2ulhaxfue.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2npweoeyi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcvnzlmp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2aziupwos.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2fmhkpkcf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rbxzhvfr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lasvfavc.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2crxntvnv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2lagdzgzg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2heqykeba.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2raigdpem.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2hebvyvhc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ouifhjrd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2utdbaxdd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2bablnlig.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2krszdlzy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehcrjuiw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2byrzlxqg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2aitideam.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsxrrdxx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jwramrbn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2relehxkk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2qipgwrei.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2glecwofj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2eliiupvz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kzzzdcpj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdkjjmor.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fikmbryf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ezaqtoxz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hlklprxm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qatsmhoe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2paoydulf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xihfltbv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2xdufhiqz.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdrzbdn.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvgbexch.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mstlrugj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2hmcqxlez.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gkvqdcbp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hrhvfjcc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nekyarqf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ojyepdfh.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2oorsthyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdtaazwf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnqobzew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qscxcose.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2epelcmus.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pmcvcaxs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2mvorzhqy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvkbrqir.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2uryqpchk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2gqpcukoh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uiqulbey.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2rfanvlcu.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2exdpikmk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ycyyveah.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wtnulydz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2mtbiypdl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2hieabvpk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2omgxxult.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2awimvybz.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2enakkibn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2yhdhcyis.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2njzvbpvz.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hsszjvzv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2sdszmanv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2agbgpvqd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhecgdt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2cpncpmrk.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulfctdid.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2debdoujn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2qdzchzli.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rjkbnveg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2eoviekxy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2uahmukja.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ohinfgow.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gzgdghne.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2qwomjavr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2sqedajui.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2vjcsvtcp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2irdmpzzz.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aenkckgt.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mhdqwpck.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2oeycnqld.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nquzdpjy.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2uofguglv.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2zlqabqxa.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2dnluggez.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2xrhhaxvk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pwkkygfd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymbnddfq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2eefwxebe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2yxusgwrn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmvegte.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rucbuftz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2bhrldvhi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2derikenj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2efcrdaoj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pgucayee.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2eikvgghe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pwvdgbvh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ugbvwpyy.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dpsikgbg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2jqdrtcoe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnlfrb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxntvsl.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bppxqogi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2gztsgxqr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lnbokvgp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2swwkubgc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2nqggimwg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ubnkzktx.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2lrhzgxrh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2eowdlizl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xhzuaybe.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2ckpzfrkq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tyjbniog.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvwjlvy.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2prpnekdq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rshsxagn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gnriepif.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2jxodbwnk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2pthjfdqi.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2vqcxrwui.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nphxkvoc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bswwukvt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2cxarjwkj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2stxcugpb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2tjhybwpl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2axyyncyi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2izzvlikv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lztxpimv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2uvqcidez.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mrbdhwtm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2oltktzgi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjncsljf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2omrexbou.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lkeshxoy.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2flwwehqp.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2awokkfbw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dhyawlsp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2amouudmx.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bptuqzmu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2irkxjtsh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2gjocsgwu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqxciceg.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ipihepls.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2welcrdmr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2eaqdbbmp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2avhdodxf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2xvqittgd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2cpoypygj.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xmitopau.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qvqyxpgo.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tdetsrsq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aookxkep.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2nlnhrsom.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2szyslpkl.html


<!-- 参考信息 -->