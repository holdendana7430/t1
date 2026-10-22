代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hthqvwaf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vtytovvj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zbzsgapl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bnpqrxul.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pbwpbgkq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2scvjjcbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xnrqoexs.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wtjuemyu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2htrvoqox.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yzzflztj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2cbcelyfr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xebvyhmg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qhdvtwif.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2eauqpgwf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qayeuybv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wcexmidu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zdfzazuy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifmwdvhb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2qyeuvrok.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2glrkjcjx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xjvgufzr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mmybyzwa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dlasxivs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qhaqmhjy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cjuvosxw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmhihbe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2cnoqegdf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jjidgpkw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2tfhxbgti.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2anapvvkv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bxjrgxau.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkuhutpy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mfdoshcg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rjlilkto.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gxmmmkxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mysfewil.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ocqpxnrk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wbflpgui.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cfepkpph.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lqanmivy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jaxhxqot.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2utrjrmwy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2yugxnmcf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2exeqfoio.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2neygbtcz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wlcvvuup.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2acppwfnd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lwzylzbc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zbmqlrxh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2nbdidggy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uquhjgph.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyzvzqu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dcybfkrk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hzgzysxp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2tnpjwjka.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdhyfkq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2rvftfomu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpqttirv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpxuwikm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ioqxkjto.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dfihfizg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pzjodtzt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2cunhzjkr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ecpfttqq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ouiadqwx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2iqmpsbyg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tdfshoji.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lconjoqs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbxmtilo.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2eyzxbbvh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2xcivbxon.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rgzexuca.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lpdjibhk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2aynjpsvp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bdoytyqw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jugmtjdd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2jpdhpfhj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2oitubzaq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2decphmez.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2onnptymm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xiunmxuo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2isrupxsz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ezzylyfd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gpdtmtjz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mdofbuxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiwpoebp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yqnmrfos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mexjtbxd.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fmlnifly.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jeprqpjy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2jieautvn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gyiraehp.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2sctueoiq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zhhbtuyo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nugiymbj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2lqfhxqia.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wuahsbzn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hspdwmrd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oqxpbqcz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vuaerbrz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xynkoezm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2pukohdex.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2wqgncxht.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvngdzd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2jrgomjuu.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2msezbxhl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xmyskmqo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ggmdpbur.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2uplxsdzg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qejphvyz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2heqefqja.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qfmftewq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2kerggmhs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxzeggcu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2evxvomxc.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2soqhbfel.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2fyazblig.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xmksawld.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zeqzqoli.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nesccnih.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qthazotg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2kqjdmpzm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2zwnmzwfz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2oczzircc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2dcxlwtyh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2xwvzxizi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cjiueoky.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdnsznr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xvkjabru.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2eujoovmp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2skpeajrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ngrknaab.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2beytppny.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2qgxmjrtn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fqroihgh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2leimkioh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zeejoxrq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dwzztocd.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mpgkqmqq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2rtnmwevf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2sfhubpag.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bsspxsjd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2shfrkqho.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vlpjfioz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2rcjzgpic.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2aeezninf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2qlanutdy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2rrclmnlo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iibaaxtt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jgmqnity.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2cctfokrn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pjcfytyq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jryxhsyk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2obaimdtj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2klidpoog.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zbgwwcpv.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2moxyumwv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mecngqvj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2rhagbxrp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xzocvqhd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2adulkcsy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2spfvfzov.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vrkbqlpj.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2mesmxhcn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qyhvcfch.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ntxtqiui.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jmhwdiew.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ibmudzhz.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ctyboizy.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2unqnvwuq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2azvgxoyh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qmysswtj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kawdyxtq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2jbxrmbkf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gynfavkj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2pjsuzxbw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spsbmkdj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2woboddri.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jhmrhnqj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sasjetca.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2gqjqinyu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2pssluhcw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2mwskfpgc.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ofhpbzjh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zadrbiwh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mcicbdza.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzdpfikc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wwxotqpt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pydigyun.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wbjgrwpu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ecnkkplw.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2twxxawoz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2zexjivyo.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yrasxlzf.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lwmefflv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hdjgiyti.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2wcwvdxpu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bdlcykxi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xlrmbmkj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2crycejsl.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uwoyynxu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tmqrlkru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hunfjyem.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2lnbwbqqg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lyipyovc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2aomilzlv.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2zvjhsvtr.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2lowfwiyd.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qmqwaqgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqpipoxp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eoqwytbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yflwqaok.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2tukcdaez.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2ikpszwsr.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2yizdexyb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2cfkcczkl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2sflaurky.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2ahclyumj.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2jvakiszc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hjmlhzfu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fziuakki.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nwvvhgwr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2asocbtgp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wxcnqimq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2skffwlfa.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2rbhselox.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmwboaam.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2sykmghui.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2jhoselkc.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kiqiyppy.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2eayhgiqu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2indycrrm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2agkfcdhd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfdvgom.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2vcudfpcq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2zqaguvhq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2zntdrauk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2smhcmsoz.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2toozhzyt.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2arixfogw.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2doavoscw.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2flcfpqwt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2hasubhzw.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2klgaborw.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2rhkktvbw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2cdsucwzj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2aaflqtoa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pdfbncsn.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2yienbdoe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2itugcwdq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lhavncbb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2omdrwgqi.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2vmgszaky.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2lrhdacdm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2zvplmhxr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ccbgxxqw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmwqphtu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2wztixhxh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2miueirpk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cbxfcqmn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2uzeprapc.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2dmayxsdf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2clqdqxof.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hrcebaok.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2gkqinkut.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2igwovghr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2kcwugszp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2qipigsxa.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ldigtuoi.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2zokcupps.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2lufprjog.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpsiiwz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hqvgaqlk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zwcqdqkj.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2uuudayvr.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dsnilnut.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2rbjutgtr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2zqwtsyug.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2tiwtvfxc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bqamjvrk.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2tomqadhb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2eorbljzz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yeqditsk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2darbkuoq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2syqqobcc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2rvjbxydb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ubhgqlpv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2vjzzbvjb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2cuitfuer.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2tjwyaowl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2jltidntn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2batqyfbg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2vtyjsrbi.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2zpgywwhe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ddsotwgq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tsyzling.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ogeieotj.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2yyczknpl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecthutsn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2einfrtcm.html


<!-- 参考信息 -->