代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vzkitblv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pznleaip.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ttqqomtu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rxftqrvz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lwlkbmzs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2rcgriqgs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mblzvwld.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nnzjukmr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lkbmozwv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fnkrwrqp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uzdmxehm.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvsnromj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2ncrnyuct.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxxomghw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fzttmtcr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ykcidgyd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eeigkuyb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vdldjkir.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hudquurf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iwfqvxpb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2nyluxtes.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcjznorv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2mnxsdbla.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hxofrszj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2skcemnth.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzgmbxr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2fwuzkxre.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vvvsnzvc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2wjftndvj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jttywqcb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2qwrwtmzv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hnnpfvhe.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2rnawsvju.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ogakcypv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yfcnjnqz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tfdzfmmn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lgbamhxo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2tvdvgcar.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2vftdhqpn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nypplfzd.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ajcrrdpx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2alwqdiks.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hjacxrlu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ytmbwdaw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2yuqdgeuj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2godawwzq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bcvdapvw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2criozmlg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aikhlmye.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mifklgry.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2hoftmqei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kpfmelbm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2twawzeon.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2svwjotvm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rjgywkcb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2sbfuuoqo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nlcblird.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wicqhknv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2iczzkfyx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jtsjcowq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2edewksfy.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gtqcndou.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nqjcpizc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cvgqqgdx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdyrihdv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2xhovdxsh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2argwgvqq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2urezeqfu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eteypaiu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2rvbmcjqg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wnwuoxdq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2xdzictro.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uvvwasik.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nfgpanyd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2bhsxvnhl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nzygwjzx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qkgbwzga.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2xnzzqzzm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2fkkplhay.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jhfvebvr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qgqariyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajrskdhy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mhjvwnaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmiwvi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wsaaorsl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rmkcvswb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtwrpnmh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yjtfhopo.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2itmxczob.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cigzzylf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ctswlsll.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dtkxjdpg.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgcwtc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2oikitrcr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2snsxyahh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uaumpafr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dtfqjynl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2leilmwbd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jilhzcns.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2adexufur.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2fvmdeqhl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vwtvvchn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ddzzgisd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2azutbwyq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qjdzqdwt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jgngejas.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ronzhfiz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2umqcjxtz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2jnxkqipv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2agvfmifd.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2akkropxj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2oqoapmmy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2wziltpnj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2tpfcdbek.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lzwbpink.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hkozuwqy.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2cmfvvdra.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebvfowdz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2koreiivg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ezkqayrh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pvtdmqne.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wwzjpujq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ewpqeyxw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdewaltc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2otndebfw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lqzeimyv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2nbwlnrvy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2huscuybj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujukwryy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2xztgmxgm.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2aexovnjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lyraaiid.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2diumctcx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ndpyrimn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2hbjwbjhg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tgmuewtx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2zahwxrjl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2cphtwrux.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lerswvii.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nhtttctl.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2liywxgtw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gufloxsv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2acuxhvcf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hyxjlxbr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kqvybmjp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hiswrwdd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgtplsqe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcrhcvos.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2hacttyah.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ldlcuxdh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2fqlybylw.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ykjszzix.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gcjezblr.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xrbcpjjn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2prwsluaf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ggssyibh.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bcnacarx.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lmuvpqys.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2vlhavgud.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2qxeioegu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ltvxigrh.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mwcpwxbx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2zziapvop.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2seyiollh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dkxtdofm.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zqquzwtx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2hyefmens.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mcfgoqwj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2aladrmdn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ixtvnijf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ogepzfgm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdwptfno.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ppbeeruz.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2eltawdww.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2enlxdddj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfojguen.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hlsvwejq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxrbref.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2vokymftl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2yuewljxw.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2rmbtxrcg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrazwpau.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2myuqzbwe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qfwqxsvc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpocrayf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2llwaykun.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vbjfbxjj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfrfueef.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xjketnnf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2evrryeab.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bjhbvqhc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2fnfifyma.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2opblaukk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vlqraysh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvblexdt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2vzfhsebx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmizqdf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tcoafeux.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2stateork.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2jiqwprnp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pdgrnxdp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kwwprcbc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lfbeillp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2rtgbwwac.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2rtjvwavx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtlnoqdu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnlzvjzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkknuggv.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2nsvosuew.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2azuekhok.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2kjokblkd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xmwbsjhw.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2vcpacwlu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2sqequkgl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2nkqxmokg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ldaxxbnl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2giivdwhq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gbqgtnmm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ydxdtyap.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2alkdxont.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2zyqjeukm.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2iduzldnj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2aaclwvwf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2bvsncvoa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2mfsybbln.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2mholyslp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2pvcdtpnm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2fkaehyxu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pfpompnq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gemtihfj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2yltgphbn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2shetxwwg.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zvrcpoxs.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2ahnbvylj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2goizwjbs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2enjiigcr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ychkoqyu.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ifnqnevd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2weiwuttf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2vzpfcdte.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2siljdeis.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fevwsyxi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2jjagfbmt.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gpcnkhwj.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2adotdthh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2xbbgkmax.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2liufoobg.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lgtjqxrr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2jlgvywox.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ptvqstao.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ykylqmtq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2uvmiagul.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikfgltht.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2scylbhpo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wwkxglcd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxyydev.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2dkngnxid.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfjrfif.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2osdrrlhw.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2enjsvqvi.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uupiymoa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2nqqiirpi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ncyerhed.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2lsmgcemk.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2qouiykte.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2fbltsmur.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2glnmwklh.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2dhnztwpi.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2bdinfcqo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2okbuieux.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dyudkjyj.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ugozczsa.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ecqnozit.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vvkqphpd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2gfyqyigp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uftapqgj.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yletdors.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bezeymnn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2giugnhqx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2lozykelz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2omdpoldj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2yujbchvn.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2dosrwmer.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2adhqkrqi.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ixwqplqb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nwgbmzah.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hoerjhgx.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2mbiljleo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ghriyrjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lclzmpjj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2lkftelfw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ubrlpydn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bskgfmvb.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2eetxdyhs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2slatmhde.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2etuoeldx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2glbdckzw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vlqixfbb.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2lakmbkjz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2phsrerea.html


<!-- 参考信息 -->