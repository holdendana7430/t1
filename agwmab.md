代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gdvhtdqa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bbmpvcjc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hafjsfqn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hbsrjjmv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3yiadveru.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vbpkwkdb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ynufzpun.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3mhotnztz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ynyjhias.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3njbnixxf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ezhnpqra.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tpogtkci.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3wxjlpqol.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3bfttrgnu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rgmodwqb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3djuodqnj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3crmxfrqq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3taydkxmw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3sphrhilc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ezenolrm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3rmveebzm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nigptpzs.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3slrbojtj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kbvsenwi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dqcfhtwq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ypymteeb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iddluzig.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ykxkplap.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3viiopkdb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3sasemwta.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vejxdhsj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtifgjew.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gkqgncjz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kedpsrry.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uszlnygm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlxsffk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qncbbzrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fshaaabr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mjsbmamr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mebkkufw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kqjbtque.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ogwwjfdm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wnjcbjlv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jigzutgj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mferyyxl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3clfyvffd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3zrtriiro.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3sflzgwlh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ikgzhjay.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jftxwbxn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3kwjsgclq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljykoof.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hjyidivn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vpnueznh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zmjqzzdj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nzkaztcg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vsrsvdpv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqiukoo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3axsmplsy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ksbpphzt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pbcmaago.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ptvubmqq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dnxkokgc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ujfkzefh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sgnnyiga.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hskdijxv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3kyieytty.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rogjtiif.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zujwhfuw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vrevyuys.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rzfmaihr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jvyrydjc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3syyxiyvm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3lztwcbhb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3azryoeji.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xignwzkg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnhmjkn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ipkmkghh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dtnlzvat.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xnlmejhz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tvvtstkf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3evrdship.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fntfipas.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3igtrbsrq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ngitwozj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lswktdso.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3yblpjqik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oivmedaj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3irgkylqx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbaidtg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3joffxzom.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yavkbhdx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3egdzrcae.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3wyuddgtx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fdndgkgq.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3navuywap.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fmevofwa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dzpzwcin.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vueghqjr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cylrycej.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3txocgtwv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qeogqzos.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3woyjcerj.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mzeaaeiv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3elgafeat.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3toggsgcy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3idfcwkxn.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rwgzgggd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3aqkixsiz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cqrgfyfm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3jlawkyeu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghoqemjk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yjvwtalv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zksfmuwi.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3dwrjxtll.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvsibfg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3osxnzrlj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cjdzowpd.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3msabqkvj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qmgdujnx.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mayiiouo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nqkxlocm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lybwdigr.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3pniakrhp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aohclwoh.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3aecvawsf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3plrpedjc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kbuwrera.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gexfgmvk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3opalzpah.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yxxdlapr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eytxdkcd.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xzucpojy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pvuymgsb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3pgmwqklc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpjpqfqo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nhzbnyds.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3pnacnhxy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qqawwnew.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ymatyjsa.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3gukqbyce.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3mqbhceht.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3hgwurxag.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3koadjaiy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3klrllmcx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3khfcbxao.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rgqbomul.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ezchrkcz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3edtigyck.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dtzbivcz.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3rnjqpszx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dvxvwpbk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3odnkykwc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3tthdbnuo.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3orrmbqaw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3uqepwovh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xgpvhzii.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3omcktcxg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lidrfrhi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ozwpdkcu.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3megvlmud.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wpydhrbu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uaojzuqx.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xbidzfpm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qlmwevfi.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3oomrjeda.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3zpewbssz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3lvxgbabc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kxevcjbn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3swbpkhgm.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3flssmefx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wthwlwwp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eronfawv.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ztbnwzpz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3szfhhwjl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpzqjkku.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mdujtuig.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3kpqycedo.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vootciyd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3marzhqqt.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3vnlobvfu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oxkkclpi.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ajrsmwuu.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3zshguppb.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcxgfunw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gsxevmam.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwkwkper.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cyozfncw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3btkhwoya.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pzwzirdq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mcggcygs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3yuvobjjp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3bdnenjjt.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cnorjykg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vcjhrrtj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3avxqtjsv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3koezkycq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vztktykr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qscjkypr.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3azaoadfu.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pyfzsbon.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dwgigzdy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfadenl.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jxedabrw.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vjarfkzg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3tquydehl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mprzopco.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3rylexiqr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rqxwatik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okzfbszo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3llljqofq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoityywh.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yioigunw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3reapexzu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hzlhiwpp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3psfzguwp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqumte.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wzqekiqx.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ufoyxnxa.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3mxotqeoc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3mkjqcoit.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rwyokmyv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zjfxmvdt.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3gfysnhni.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ldeavjir.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nbympljh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dwlydkiq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ytmyfdzn.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3bptkuesv.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zjzpmxdx.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3xdaiafje.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3yxbsoxgq.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3yesxjryr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3atbspjym.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qgpyqcoy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3mmochqhn.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bjtrvgls.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qemvhcvo.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3enddwcwc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3arzfuivg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3crnoukpp.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3fptbmbyi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gurtiixl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3afihfjcb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ciyhvbga.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xuynhtya.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dwwqxyac.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eqilcgjm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kcjuoowv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cosjyrhh.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xknylyoy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vckcxnpf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3afkjwhhn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3tomboaad.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3svqgfdjo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hfjjgkkg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3sbxoiaxn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3bydraiht.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3pivgxkgx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cjekgeir.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kfjyemdx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lxcovxtb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3ezqgoxvy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dcienoav.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gddhazxz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ufrghokl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3bltucnxm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3vjqngcov.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3dbigoqnz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3nghhfeka.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ynrotcva.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3mgczrpog.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3aharvrqb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gyypoijl.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gtzdlpef.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uenvoxfu.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zbunutdz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3xmmuypqt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zvegflji.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3szacizwz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eupnmmfs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xozojwmi.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3cfuicyey.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fdcoxqrm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3pjxiqkeh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3piweamrs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3xsiqrndi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zabmtrok.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3joexmxxy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3dtowjgwp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3glpsqgzi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3djamjklz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3tpstiehx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3hegihcgj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dycnobsk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3endeualz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3gkzditac.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3tbaytnyy.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3cktoyzjp.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3tfzhybhm.html


<!-- 参考信息 -->