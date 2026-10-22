代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mfdkggrd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ttjftcgy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qjurlcem.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ifppnorz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hprlmipr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2wfgkrojj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2oqecdcby.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ypwpzuyk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bhoeczki.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2xlmffpam.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nqctmbqs.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kfoqdtbw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hdpflbnm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxmfwt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fonwewep.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gykxdxlu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2josvlqic.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mxbgnjst.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dienwsti.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pqlbitwa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kseztvkh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2izixpwql.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2btuyewuk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2auurgsgh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gclevmtb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lxtjcdxf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bxywoxfy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oxlkvris.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2twaarnou.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lknfpbum.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kymjvbpn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lestionb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hnipzgvl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uqxbtkpx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2cpnmrijs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlohgxt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ihjoimxy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2syvfgnut.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ycqukziq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dnojcrzs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2nhzgnoxb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ievkuwnq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kentiyvg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iteiznle.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qwwxrhup.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2dwlzkbdj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mwjqlpmw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ryjpnagt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqgpraok.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rrjkopni.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2elssutfj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qurcdnmz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2sxwlzytv.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ivolgdzf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cgucqpxh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqhvfcst.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wrqfwong.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2pwgobvzl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rvxtvrcs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jgttzytl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ddielgla.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ixuiuyqn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2crabfued.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2boqkfjfe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbpjhasp.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bontoxth.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ixxybhrc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2adesopjo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2elinccee.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wtsgrphh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xolycsvq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nalcerbf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxkwcwtf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qmbdfrrr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tpclqckb.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yqzawqes.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2selzyqam.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fpeszgio.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2clwlzhwk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2iazdnmqf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2uxdypfmw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cthskeiu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hbkwuezm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ystxscnd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2psntuzed.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wvjznxro.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2oalafxhq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2lnxvchvv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zzlfhsyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzvsqssj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jeiafjkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbpsmngd.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fircdmjz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hnxbiksd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wekyoiqi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xzejarce.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2rfoonlfj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2uymjenfp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gjssgvsm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xarttvrv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nwduceck.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ctnrhyxb.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2gjugsjbu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2khllavmq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2foixmzop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvkuwtbp.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ygdjbzft.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2vhxgcckd.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2petpxqsi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2treelhpe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2teqolzbj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ubgxjybb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cjtxbdxe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2akqzfzqh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jvrmkclq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sbansuln.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2zamdfaia.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjezueb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebosjbso.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2nubippga.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qevdhsfm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2usgjgbac.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nvliluqf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eqgfwuif.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2baxudglf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2umrtmwcx.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rylzuqbh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2xkapxdnq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xhgtjniw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqvysax.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2wguacgsx.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgwcfvb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lrmpuksa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nhbvxcor.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wocyqltq.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uesunomt.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xyigskpa.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvdetme.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fitufogu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gezpisxw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ytzewxrw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2xwtfjwvt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bxrdpaxo.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2slcmgxmi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kxlbwmyl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwozjnj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zyfvgpgt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2uggkzubi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uijrvuje.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nayhbijc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2kkhhulzk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mfudgjfd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iijfjxxf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2enwybwmk.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2btnmqnuh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zbsdrehl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tammsaeq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jlyrvssf.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2djmjtfqg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2uqbmglyo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2gxsymjhm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2urujcwvj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2eozevqai.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xcnwakmr.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vdwdbnle.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jgnfhnzd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gfzymrzc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xjrizhpl.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgphihxz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ufcmkikt.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qmlrhqku.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2yfdiuunr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2klnhunpv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2topvfjdx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ndnqmghk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hqbhwscs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2etszqkkr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2owjhcprf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jweenzfh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ffqaeiai.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2pddlupbr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2kajyqdjc.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2fpbdafjb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmmmgyf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2brrlfnlq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2papdsysl.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nhsoppog.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2aicnyojo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwhwfyar.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2okxiadtv.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aailrhdl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2ecnjflsj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfxwzzwm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nnkylhqp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xhfgdacp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkyhyfry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lhtwrhub.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gubdlbsg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2trtkhoak.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2eosjuhth.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcvqveyr.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqqulmyb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ppnrjxme.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2rynzqeov.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2olowwdgd.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2louqtpsv.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rwqjlizi.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nsmdijmg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vvgrfagd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2fppvwzth.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wpzqfcsl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xvmwivcp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2jhleszbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxpxmurn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dwtvbqph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtyiabcb.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2fbrrbdrw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2uvzpzkcr.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2dwczpatt.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2heswumrh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2zdlqnbod.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2winarpzf.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2homiyxre.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2geiksirv.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2rtwbzkcj.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tbqpdqtg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wduucblb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2qitlmxmu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2jbyzedqn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2gjiewpgp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2qxxafocn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2tvgkurcw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2btknvrrg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ildbwgkq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2bqkkefxc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2zzyvqhsm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2wwcchzzh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddhtdjgb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2loyvtacz.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ssmrszzj.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ipqezsdb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2jkdikdma.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wvpefhyb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zolkdkpu.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2lzjfxuxh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ofwswenw.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2kyuqkoac.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dryapnzk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2nqiffpuz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fdejdexv.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2kuhcqyab.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wyoxxkfx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2xnwyanre.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bxiyjuqd.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2grgwerbe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ostrjprt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xglhxfji.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ztdmgfxs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2vbknoepk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2tmigeppe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbxwqzhe.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2bpuopzzs.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2hjvpcqsg.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eoymxxci.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fusuyzgy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2uvjxnzbv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2vsrbbqjn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2zytnggpx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2moppwyxl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2eckqsbdk.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2njsjhvwd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2tnwyxcaq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xhssvohv.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2weitbsun.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2cvqxjayb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdfakev.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2shycvfpa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2czqhaahy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2syhdnjzi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wqpguejv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2eqijvfbl.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jpuozmjf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2oqmdzyjs.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xtatyebh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2evynyuuy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2zicgkplk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uuuqcics.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2tsdmxahe.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2slbmbfbn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2utlxgrms.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2yorgfdhv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cekxvllr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2neztlkov.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2znwviyrf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lscpryht.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfcbjipj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fxotjian.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2dfckyidt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2luynyoki.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ocxpstlh.html


<!-- 参考信息 -->