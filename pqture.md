代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bzavyvpo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bdmvgdno.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wqaiyshs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bwjjjjvm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2giirwuab.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxmpsstj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kchburzs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2btqqpann.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2mvgejujs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2btfeoxiw.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yakupxju.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqyxeey.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2puoeakjy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhewljyp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ojcceccn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eopiomou.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2gloquqtp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dslilgio.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uswdgotg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vsbhmfhk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2isoltxha.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2incbrofp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tbpqypmp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2slrigync.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2niwcjrpr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2imqkangr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cszsxsbi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2honlsnbn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bkqtbjjc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2eizeidim.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xvuocgvj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2raojwaki.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aqurvczd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2leiitgmg.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2zubdjxsi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lleicvns.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ujdzdpnw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2hjtblkoz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2leffuhaz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gzfvnvso.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2duirmfod.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2yqpeycah.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2agezvfbz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ftbhlpdb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cydxekaq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qqepvffr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2onrwvhql.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rhvtusge.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nricwprc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2sbwtnasi.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2jtpjeolj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2zmdtzaeo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nejktdft.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nmzhdqle.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llmqjyes.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2hfcfdaos.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfthdjjg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2yzckiowq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ewzoofwt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lubpntjg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uzbxvzob.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fzmkkdiv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2csesnavc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2qttmwzst.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tvgbfexk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqsqjsiy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gkfctmhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fevjonoh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqktxcdw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mwnuzaok.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2nddcaptc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2puszrphu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ugqxgrkk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2shbngmyt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hxjyzvgr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ycuzpngx.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2oztncmls.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2grfyrmlg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2azqrzwta.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tyzkrexq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zywpeayb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2jisfbrpf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qvzfszfl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ebfelrzr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2zaxjxknu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lqpcihry.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gzbjvzsr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2fvvkicaq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2rrhxrjxy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2kvoogtoh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbslicpz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rllpziql.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2fiechiid.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kysjlgtu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2brkqtszu.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2etdkglxj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2kdbkvlue.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ogqqibpa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xdqbncgy.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rryxfiei.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tidobmkq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2hhxfzhrq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2nmfkjttm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2upjlbsrb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kcqhizin.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ceqpflxr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wubtqbay.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gksavewe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cgagqtwx.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2zubpgfye.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2bvwlfyoa.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2hskogsih.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2njbxczfs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yzjzzlrf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tzrmycjt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpzgbnqj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2xejqeyda.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2hucfcfbu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ysaykrus.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdyohes.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vnlyxpaz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ehqugiog.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2jzmlenmt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2poeioaig.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wldciuoh.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ahgrfkni.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2jhsevvck.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fdznuaqq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2plkwsfxb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mvyqqzrw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2pbnunuls.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2djiopoyg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yhhioxws.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ethpvcve.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zdbojoxx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2kpzxdrdh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ibhoewzc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wttuogxd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhbqybby.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qoytohlx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cpyjdvvo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2kaavloqa.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2nfcarloc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2wawwshgl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ltbltlpy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2egnyqetr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2gvnsuxpp.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2lqnlujfb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vdzpbyps.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gpfyevbl.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqzjykqa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xtzrjrbx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oovzvjfo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2gojowadz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2pmcgnjfk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2khobnofj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2ikswsoyd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fofzarqx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zimhtgjf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpnhytcz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2opssounr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqxlvbzk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2wyuxitba.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2tcjiuize.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fhsmqaur.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvvjbqnp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vvbydzgc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2xbrhfnyz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxqlxnmt.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kiwvbmbw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ueptwkbk.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2pzzkvazb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bsbfxrna.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jnknspso.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mkipnuvk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2wrnvzqqt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2aqkbnmgd.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wuublybq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2izfkhrpx.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2nozxcdwu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2supzlwdr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vpzcupku.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwmjbrwm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2yucaqskm.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kdyfedhu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qenpettd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2omhdhnmc.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ekedctzn.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjeifkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycudkaku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmqvezwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgabzcpo.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2mqgfhzrm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ehswffje.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tmbbweiv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cihxqyeo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2lpyagirx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2cdrcsfqg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2picevqjn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2bdacimiq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2ybwoigfp.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rrgpxuxj.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2fggkopiu.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2bifnxxol.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2somsyszu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2uhjczqdr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2foqlwhkw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ymhmqctb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2efjpbztl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2xfvxjyyq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2dyzqjkbp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2cutpjgxz.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uxqvvimb.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lbidytss.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2bsittaql.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2alpaujuf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2rercdzfp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xlxzjfji.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2zxdisloe.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2xmoqfoob.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2etubecjh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pdxkzste.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kvrjqkit.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2mkyooykp.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2xmdgrxqk.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ahxcyzqe.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2rqnbrbjs.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ehwecrnl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2joblbmuc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xongopkg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2yqlvpopv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2jqywkhtl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2orognkhe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ohxyfzpd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2exwaugcc.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2efwadevu.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2useyvyen.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2ummuaqxl.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2lmpzuoyy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fdhefphc.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2syqniuic.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2defmeecy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vtllntvc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2vyorgcdh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2jwjyqkpy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2mjzjsjbp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2bxnoifmw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2hwgdzipj.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2nkxagwic.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2dkejevyr.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2vqscxokq.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2okucydpx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sbvivvzp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2synlkkvj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2adgtqrpq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ipiozocg.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2dhsxupwm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2cjpvcujl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2lzjgufcb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rvhakhjt.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xbmqrvqh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2aripqife.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2fdlzboav.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2qemddlgz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2tnqiyiis.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xpakrjhs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tnkznbcg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pkvoyfsz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2stabzenv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2cmnxxjcs.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xovwbair.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ajenmhca.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qzhwiztp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dnoktsfc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2uhjylyib.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gounhgog.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2csmuqfki.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ikmfrvut.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2noburwnc.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2ziuayrkr.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2znhezhvo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itoydoki.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciwgaupi.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2amyvouxz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2kfloibxg.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zrwzvmap.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2ssaaagmv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rptbndsi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2mnmykiqv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2dkvravuk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2wxudvwav.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzgpadfc.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2uuvteysk.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tcigdffa.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mtvqnuhf.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2nllovdnn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hffuvnje.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2lpnkypoz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2qxopnycw.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2xupbeipm.html


<!-- 参考信息 -->