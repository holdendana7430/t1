代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aexftgnt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zmfflmbk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dwbsbpbb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2atztxgtw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2efolhkwi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xscjbdit.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2rizqnxhd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kdfvysvu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vbuudlbr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rahxrszm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kzhzhgnx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gutncdzx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2oehegqfk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2eorqpjgw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2bmguxqhp.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2yeymcldy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2oylwcuzw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pwdctkmw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ntsgjito.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2azwdvymc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2gdggykoc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzcbivnf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ecdjnjxo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2nmfjoiny.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ynxoavep.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pauaukxt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fmkhsadf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mvluuxhs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2bbtqjtoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2loktlphi.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2vmadhrdq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hfniesln.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ojfksrsw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uuckrxpi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mojkbdqz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2moagejin.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wkmypfsh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vntnhswu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ichfjxvz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xgsmivlc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ojgbiwbx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lomxriwx.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ojvwurcg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rsihhvsh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2gwfeyojx.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cdokjemf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hllfaevn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2goirfaxh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2coddxslf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qibqcvfh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ejensejg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olaiaqyx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ctajhwkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkiqiag.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcgakawg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vflmjxfv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yhagqtku.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2londersw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mwxdtpci.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jipiergc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jkdikflk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2lvfidfgt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hanhxuet.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2busmjmzg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwwuryyi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2wrlorrwf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2cyhhjtte.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjcyjerg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oomgrujs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2vrjsncxi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2brtfuxee.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2votllgad.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2olwtdwvd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dvowjqbm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xowerpcp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pcpyzdhi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jtdizhyy.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xswaheqw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ngdgpfxu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kcgsptph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2exmajvit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tayqgcdy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vsngpeun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnsakgyy.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ymhuuaon.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2umpbxfpy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2kseauwth.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2oypivfuo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ysvufosi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ywfpbivp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pqwzgzkm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2eaubnoiq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jbkpeqxm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xscuraxb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mdjqopqd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qzdtpnty.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dgqzzecp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gzbrxdhu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2bolzudeo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2pycsyhoz.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2eguszzlb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2lowckojh.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2htvlinjk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2gtvcgcyr.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2rkmnbhmt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2pzrmahrk.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2gfnycwli.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohaujeyw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ljpptqrm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sppxbrqf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpjeknbm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ewxthrrj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2mecdmyal.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxvaulj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfsrsftv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2swjaqksv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2cvspbltc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xxbmhygb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yphqiice.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pdqjnydw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2kuuajkme.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2knhxjrvi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ljdnrxgi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2myhvcmwe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2odubhygg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tpxqfoip.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kcrvmphi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ashaugrh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cakakscd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2fyedzuys.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zyjwfpwh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnpcamsq.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2txtiodex.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwiuohg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kyigfbvs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2eukrkrfn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cgcqoboy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2tradnasz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2koyckqhl.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2svjgorjz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2fcqjaxes.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjmrzas.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2fjcbstwq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2orbcijuh.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tesspfph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lratryeo.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2jlnbkomm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rehcdrxd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2lqutstan.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2kjcqmkys.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2rxaqditt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2htmjlvvn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2oumrblfg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykafyimt.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cicufhgk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2symkxbpp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rptbfpuz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lciebxqb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ggwswtdh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2yvfrduto.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dxklehhp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zllballm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tzcazpdi.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hdwoqggz.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ocogmryb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cnijnzbq.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2aomvbfbb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nmponphl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yfrxvvhb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fntloviy.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2honejyfl.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzebrku.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qsqylynn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlcbbrkb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2wvpbfxzt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljsizopo.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2kxykvrtg.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjpigpfv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2tscbdcpm.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2ngcslrbh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qprzgcvf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2goboitzt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2axfrsfnr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2uaiuujnb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2yccoesah.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2suapzcha.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ciiqsxgg.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfeupwle.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2cmljvdhb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lvydkrcc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zrdqbuyl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ymtydlih.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmjbfbmk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uvwuljtx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwyalkx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2oyzdvzpt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2homdekbl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mawpogyb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2swsnrpkw.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2hgxlejlg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2maguiqjr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ngadpqqf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lvtbxayw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2wjbaihso.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2myihgwjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvvalppo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mdbeonse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxcorzgt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2cjdsqwnk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pxoorinq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2nabnwzzp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ukmlnttw.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2rlgbwniv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2gmyunvqi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2nlswccib.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2zadqfukg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2kyqzqhgb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qffnhnvd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2auuxcoxb.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2dermoctd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kvyezqcz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jefrtljs.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zuznvusv.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2sjpswude.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2lepchyrf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2otzsgrib.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2iofwujbq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qwuolydd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2vambkomh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2resacnfa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hdkfjjvw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qyfvcibj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zohkhhfc.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jopiaylp.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gwvyendl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsulmkc.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2njmpkdum.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bzxogjmr.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2rarltetu.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rsytuewu.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2awrnfgmr.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2iacjwgqx.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kfilqztf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vklputpf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bmxnprfc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouejnrdr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ryrhwcce.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2krrkzegy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jigzvobt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2awexxics.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2wkjjjsdm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2cyrwjzck.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsfczhtr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hgwuxhmb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bripwzck.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhdldkn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2bilwscwd.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2hlalgkob.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbyrjp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2gikwakog.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2jukmpuof.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2fyxgzmtr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2zbrpvfbq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dzkmozzn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mbuedlyr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2mzruqytb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2pgiihlzs.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2flpyrggp.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ousrfgld.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rscilzcd.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bysxugxg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2cikvipew.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wzfcphfv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2aeilbtih.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2feryhlip.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2mpbfmuks.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bnmafmxd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2otirjsqh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2xrktddua.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2bjefghrc.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ijlrksgz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2eoagwtxa.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2zwrgptpp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2pmgcogne.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jzpkzhte.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ypobjzdj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2gtyecpuu.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zyajcgym.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qwojqjll.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2bljjxazl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hgylprhu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qghbqltx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2fwxoryok.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vvnomtsp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2ykpvkmqg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2dclnourn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjssfjab.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocgnvctr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsckxzzh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2fzpeaswv.html


<!-- 参考信息 -->