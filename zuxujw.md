代发 wailian999

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tciqmvpd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nirgwyxk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mpgkxrhe.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zdoxgsnw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wkhhughw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tderwzcz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ldsrykfr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rpqwcval.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gprknnxz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3otfjvegi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tcjvzqky.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kcoiszwk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mjlimdaf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3kvenspoe.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pfrnkvrd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zvsokmhj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pmtmifkd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mognbdqr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3tlelmlys.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqzwcsxm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3yhemsqdf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qxcdtsqz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3egqvqkeg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dtoeuprp.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wtzniuja.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdqlhkwa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3locrmeoy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gyijzqwa.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vnjwibms.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cpuixesp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3mmkwevnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zwtlfxff.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3htptiobh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vznibwki.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3thbvfaqg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3txivmdba.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vhjkekah.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3swzvdyvp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3dwaqrgqu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dicqnoku.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ddvxoagt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3havcyzpf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3mhalntwm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlawhpjt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ijpvlbag.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3czwwfzmk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3emigkgzh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ukoqhkqz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sosjllei.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tbrfnive.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tbdvlslt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3pnjkjqjj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pvmrcprv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sbywyplp.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hqzbkjcg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vsgivrdb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qvimufch.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ceymkfgd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vmorrjja.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3xcolbpoo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dhuamvzr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3olcsfner.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3isvjsuai.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3rgiiqzvp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rqjsgfws.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pjszvbij.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3updvodas.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hobiitkp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3acyfsiik.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qdlxkcgp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3skrzobia.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jvtjwqou.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rvxevmis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpaubuei.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3skeubwca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rptdgjfw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pwavgecg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ntdgrkci.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3dserigoj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3cgybjkck.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jcvejqju.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ybvnqxld.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xscwfozp.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3aehoyuji.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dafkabnf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xgckufmh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ylcmzgpv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ngdpimnp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iujicacu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmopnxo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bbihtapp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ibnzlltb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3bibbaquo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yaaiaizs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3eovomcfy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hjpmvgdj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3eltzcjgl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3gzkghgnr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3xmkhbvkd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lyvtsvpv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3suxwzzaa.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dftgzekd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dguhfsrl.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xufswelj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3gsbqijph.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wicmoynf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rlvvxvev.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjmtkal.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pkqllqlx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3msacyzws.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3sqetiwta.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ztfjuojo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ljgfjtux.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hzbenkfr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3eexzsqhr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3rdyvzvpc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ovewqfmm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sroanlof.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zzqredxc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wyfmcfrt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipkchgwz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fjsuhdoa.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3anctbcta.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fbqovgwt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pfohglyx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3evwxmhhn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3fbotlban.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qidljwce.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sbktuvbj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3iguceqyi.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mzzaujzk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lpnmnwrk.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3clpjjyru.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yqoxwebt.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tibbcoxd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3omqegvpk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pjuhklzh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lwnitexe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnohsoyf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyurmfxm.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mrdnkazr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3oxxyudze.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3emssifkd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3xpolccad.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3gpxidzga.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3swzvomjh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3khtgmxfy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3lpiqktqd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tnfggwam.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3rqhmdroa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nwyoilcv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ckgnvujv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qgtoaqlc.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3hvwowchs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wldwlmkl.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mhhqyjsx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhqawhlm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tmgmkmyp.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fpmhipwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lktdefru.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3yhoyphgv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3kgpkuygs.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3owzlnylr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tnaitgke.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xkkvtqni.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvnilirg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3prqoimww.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsikilnl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kjfmtcek.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtgaounu.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nolsbghn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3eowbjoln.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3sufewzpz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlujmbvr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qosogszp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3japznbub.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gskpixpo.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ckffiodv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ttkrsaya.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3owhgfkuy.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3grzvzywf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3febczxmw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tartdpky.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xirhfwuy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhbktovb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nssuvois.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3slnhhqau.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wojpphzu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gizhiets.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ompjvoqk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wclocbyn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3iktntjsi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bodnzlnk.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lstugmnf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zfeayakw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ilnzovpz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3idijetbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxdzkwvq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xcbktxvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkhawuop.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3bospxvwg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3dnkvekjv.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jutdfpfd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tjbhqody.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tnofnwcg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3teltwiyk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3htcyocez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rohsxmow.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3voscrbdx.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xscslerl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wwjvgrha.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ivztvvzg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tdmyynty.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ghyqcyow.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3hbrobyix.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3aditkwii.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3wtvjtxqr.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkqlqzb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zoubfyap.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3wdjednkq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nclskpyk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptoqkxlw.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqpvdcdy.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qspxxouz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dgndeyig.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3konnjzpf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jcghehhn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3zjtgfhpb.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3domwvoxs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nmneqray.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3qfmuavcg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3jjtwldyx.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ymkwdpeb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fvbcknqy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mtiuzefs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dudepsbs.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xymbgtjo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3masnykhn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ztabbwoq.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ojjsrwjh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uuexujps.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3dtocyjup.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ftjiogit.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3kedmjfko.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdsrwyif.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vhlpwdnn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3fusvmkph.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3runebpoh.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3peyisvno.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3khxyvyno.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ajsoradb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lgnnwpky.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3tosjetac.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3pbscxxok.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3gfiwhzaq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hplccyhg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3pamyltjc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3cblzneld.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fhbmgrka.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xuqpajzr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3mpaalblr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fszhpowb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ilzstdwj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3mlrfgzju.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gsudpjpf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pjsnxajg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jeecakla.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3twvefyoa.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nnnpyoqw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bqowaqbl.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwokpz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ewlbimeh.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3enzmzrmx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3rlaltmlg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zuyamnrm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ukcmxapy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3swlodedo.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3vovxuxta.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3zrvqhrsv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yglxvget.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3pqyfzfea.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3afulqchd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dwwrljll.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3eobxpase.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3eafzpeys.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3hcqrssla.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dujereaq.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3pytfqcei.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3strchoga.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kjykqxee.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rjlcrwkl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3vkhrefdv.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wuaznwjc.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3spahtrlx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ckztyeqr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3dshylrmq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3sujzkicu.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3godrkari.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pwnlhqzc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3yjzctqts.html


<!-- 参考信息 -->