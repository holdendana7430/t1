代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2uhlhdjpe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2sljubqrd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jfprppfl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2brhddupw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2trsbmoul.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ujkhqlci.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lthmgwbd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mccsqwyp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2gzqizwbm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qzvlbwmt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ddidhltn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hwqgqbxj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tudmpfla.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dshmyjng.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fdzkzkka.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ntbfepop.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2flpmuucx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2uygfzpik.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rtltgddd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kqxjgrdz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2umljtjqu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcftnslr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2oxxnxebz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ziuggniw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2grpmendg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2idkrtvag.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ocoxrrjx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bbtnmuup.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vhppgeep.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zdtmtjkv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ybdxydtk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ogurxsyq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vzgwtrbb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pggdmppu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmteda.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2rzbwwsuf.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zyijoixk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bggvlmal.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bnpmprat.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxolqx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ekumpayl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwcfcjdx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2hhdspgdx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vueoaomc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zodluzaq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rtbofbqo.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mfxlnhwt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zvsbbkre.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wbbedysj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2eovwidwo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvglcvgb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fnbsnyxo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2iszmayxe.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2adrndibk.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cdklbakl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbuozatl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ausuhlgo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yhpvwfkc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2crwndydn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2stadjiig.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ecvhosil.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtukioo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aotmwlbz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2bnahsfcp.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2alrvgzcu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kynvyxdg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mynaopwt.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jgoyjwqq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wveyprxz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uolddtph.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ikograci.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ewdanzxy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2eocgcerz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2uwiiuhxv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cujejujx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2edrvpmzm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lbwahgzl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2hbgopebk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2kmdzokpm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zfksrpqb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tlbgrlvq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ijhrbwde.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wqjjuwoy.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qgmpwwdw.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cdkixlgp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2kfchmdvy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2sroegnvz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ocmjvbmn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lcqvctbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clepmqbv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mnzvygjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohdpxwnn.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ogqokekn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wiiwhmkk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kaeflwrd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2djadtnml.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ovizoqus.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2phkgiqix.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2quzwedfu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vkwmpslt.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fxricxga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ngacekiw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2qafzdfqb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ryjhirvn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hxktekrd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2pggpabdy.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2rflgbhjb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kwhdqdhb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2xdswwscx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gngvlfib.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nupvftuy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2zwqkovbt.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tnjrkhxz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tuvssnpm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2dumnkdxd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjojxvxy.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xqqupzoy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2kkujamhm.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2psxewuzb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dgiuumqv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2gyyhzfpa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2jhpwlueg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xlmqxuzu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2knsnrgsm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eoajpokw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2biaddqwv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dhilrzuk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2zxwnkeii.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2suoqyqdw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2digezplw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ozttrlrc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kkamnnmf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2edczvhyw.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ewmdmcwy.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2aymsgtux.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2izoigagq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iwusmyld.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ufieyavk.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2bldnjsga.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xwrdyilb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2bjsjxygj.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2yiktrlci.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wxuvmvge.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mciqqspn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2whkooayn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2fowrarho.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rpcrpzbu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kdoxwbch.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nyfhhxkg.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ujxpdney.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gyhxzycp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrbokum.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrmowhra.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nvcdwshl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zthiyark.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aktbisit.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zunkndal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pudodyjs.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2iiinmlfz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2knrzskxi.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2aekgclzq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dcarmyur.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2srhqkdfw.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wvzoyklb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xpqtocsq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2bxipijmb.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2waaqqpsf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2melcumcb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rochunbd.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qmezqtig.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ikuakqyq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2nuorkgru.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xuavjivs.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bpkozqee.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2izgorvjs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ptpwzomm.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bnjafzvw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2puiajssu.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2tgsrlvuk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgqotgm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jmvqgjcu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2fdjkmabk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ngokcxua.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2txmwkfps.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wvcvudge.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2mprnmaap.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zafpsdjx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2pvyuxozu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2okhlnhss.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvnkopco.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wfcfstaq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2adyddfed.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2grmucyzr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mezvhlho.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uabpkunv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2mjlojmxw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jaavgzdp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qhedldoy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2yipgiqog.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2yptgwvlp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2alywatrl.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uaflwnnc.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhylhfn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qkspxvyx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2izharcwt.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ihoqbqin.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xzgdyfvx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wymjiivc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xbjagjmz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vhiwvxsn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2abeclgjf.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2xmpgnnaj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2mzobhuab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebosjdai.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xeijlfxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wpuenxny.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2erbhjhsl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vjipbzzf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2rcsdulgk.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2siskmjng.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nwhohjxm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2qhvdpwqd.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2xiuwscjc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oahallyj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2wxdogksj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lcyqtgpl.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2cojtcxvv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2pcgspmvm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2bzazrsmu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2cubshkwu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2novsokko.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2iisxlvvk.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2hcistrnb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrhrskj.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cyibuddt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2isxkytxy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cfquonxz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ufzwbjho.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbwfpltg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yqezavbo.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2bffmazre.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lwjayajk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2rwgeovki.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2roqpgglh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2hsbubmth.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2xguzastj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kbrpffjp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2mespbqqi.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2hwwogual.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2mdwdeurf.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mflhpvla.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aabypxmz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2shcdqghr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2auotlbhm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fmekeolm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ivhelotj.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2aixztpqq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2otzyabas.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sbwvjfrr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2wkhgxxjx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2waktamwg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2wqzueorv.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2shkingkr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ntjahbhg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2spekpvaw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2xdpfuvln.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2blezmhfj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ejftokfb.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2saslpvef.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2kupzfuho.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ivjntuvq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2zsthaaad.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2lbsgdunk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ifektiwg.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lmpcfznk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmaceklp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hptuigzl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wpzpqsdi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dflyrure.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2rwmyqaar.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ggvmrzbp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2tvtpsfak.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2xwdilmaa.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2xswtrhzm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mnfuxqmq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2nndgokto.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kolrxuvx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2drambywl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2xftfuqnv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2bnalvzcp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fqdewpzq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2wezjgtsv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nfsgxmqo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2wefxxhvt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wuejpnwp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yeqytenv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qgjoqjyd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jvbeoblv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2suzyludc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2rlqiygbq.html


<!-- 参考信息 -->