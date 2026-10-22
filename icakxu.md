代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vthjhhby.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gsfrxpnv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2prroieqy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2iygyvfwq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tyhnqnvx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bohpmvgc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nehakwgt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jjgaycmh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cfumkgto.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ypvenvjs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tvnzabvc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nsvrxlmf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dtioiomm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dbzhzxao.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2taltjfqk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pfesvull.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2wbubphhs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fjcsianv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpixbkug.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2wijxcmmg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2shoxcdsc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kliwfvqf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dmboldgl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2kousbixx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2zwmvbgyj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2nzpvpmpg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wbrqqsft.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2laxojsxk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2irpznbas.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tmlerenx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytqcnhbv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qrznjhod.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2cxjdwnke.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2baqrdkkp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ypcuduxd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhuadxfy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zpoigqdj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lorgkaca.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2krntqjof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rsykxrop.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zdpxiqpj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2siqwwiuf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2rjjohgoo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2iqwlpnzk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dlwflujt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2olgdhehs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2hyissshr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znepkiob.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrkcmvrd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbefkqae.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvhimulu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2wxldgxgz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sjjnjwmm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oesiwdtv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kedztjeb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2nhyrtpwc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cflybthy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kzwxluuv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ltkfdpeq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nulhczbf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wpuvnkzm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wljfeeyj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nysddzcv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2klckbihg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tbhjghsh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bscfocuu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2uidmftcj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2esmckgho.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rgctlsgo.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2txbroiyo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qmmondtp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pcmynxlc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxqgeid.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2njqqsmqy.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lsukmjrq.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2umauffbw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xzykjlkq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jhshweet.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cdvtnvvy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aimttaga.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gvlsytpi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ugruivsx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qkjjudum.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nfmxlswx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tizgrhji.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2frvjdxyt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2svwrtizz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2hqdcvdzt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ukndrokq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvhrclcw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2kovvukyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2muemewes.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqqjsxax.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ydscbptr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiglajac.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2qrjkqnqq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mwtjxjzk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2tzmytkvb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2jnmggbyx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2msnumxci.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ipyjebxi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2uctcpiqv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2aaskphgl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrdbgrow.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tuhzsagf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrbllzz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nhefcpae.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2huiqoahj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhujdexs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dupmbplb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cotvnfnw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jxgokjjb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iykhxhcw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2kvlxyjrd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bbqtdpoo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nabpgzey.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gwgbnesf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpmglqa.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2uajfoamm.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jdytgrhq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dnpbsanx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2izoqmxyl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bgfazgph.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2begyzlwy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ehuizohb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rfvehpmq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yyhrjwhi.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ivokiyus.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yuhsgfsz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2jxtszloy.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2ukfapdzf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2gfqkmkie.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ozbmpfjj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dsptwyyz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tkucklrs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2owjxdwen.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ludyemzb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2bruhmbxs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mmlrkaxb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2badswpgc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2wmarumkm.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tvsgmsik.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2jilwopux.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2vddhpkow.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gruqzuxr.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2peifgqtx.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qkxjrmhq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ilycmnth.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gzfzmjex.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2hgphzuga.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2fnndtnbf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2yufqnjfd.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dxyhflrm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wyqrmowm.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2dbnsvtvk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2otndtdnk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2xfvmyohp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2bmxsfngm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2mbkbqvin.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2guojopxa.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ebuufble.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2wxmewjxz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vkcejuub.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2lctauyev.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zmpwbkfz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2hgigffol.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jvcmbzlj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2eehicmvf.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vxryagvv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wwhjpekr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2hsamofgx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2srdyzhgr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qnxeozbg.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2cjrffdef.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2zhiaazuz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2uaoecqxw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2hrwlwgsk.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2sgkqmhij.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2rnhdcxsj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjvmhtd.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vvchqeki.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2noomgfma.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2nclazqdr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrxjgjv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2onmusrop.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2wgaiqjct.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2zqjvlabx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dopugabj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2yrmyxrbn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gkoencgy.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yfuoutku.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2vkhqjxtu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2aijsmvqq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ntnvjulz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfkjbpo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2zzrsnxhg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2evuotpzc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2pwsbwfif.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xxonuobq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ncctyjar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2ofkhtfqf.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xntdkmpw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2katikzrl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2calufrnn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2kzmbxeir.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ulldvref.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kjmrpmsf.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2glucjdpn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2nyuxocqu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnoqawwf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ohgkknhb.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2uszioflz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rbwativb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrhmggkt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzwnzzpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhmxxzfi.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2gpxaakhk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2iiwryfzu.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2iyuvsiys.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttvdtnhn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2mkmhfoco.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2dnafjaws.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2depfubzn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2juqxrmaf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2gmlwhwel.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sslvjfcm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ljercgvq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2gzaychhp.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xobpjwbv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2tldufwjd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2nebqqjog.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2fpnqlbtg.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kynebbya.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2fxkjllti.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ligdfdqi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2nyrkdkey.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2lmtbvwig.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ytsgyhbf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2xakcoufx.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2rcfbvkog.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2abqsaevb.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2yolpcpog.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ppcyadqt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2lvvoxszm.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mukwyhzu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2hkzxqcde.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2lotskorx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2pssnrgri.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2vmfufoeb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2fmihogkk.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vbamtrmm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xjvkgagp.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2mgrhaqgn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2yylfmald.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2hfqpprcz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2hpspmfjy.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2wuwotfcq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2zjlyiivv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ljoocieb.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ijudhgrk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2fsjmhpec.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2hnikqgyf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tzcnnngq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcfrbzg.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2mfohscfb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcieffc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2chyhxtwb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2mjyboylm.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2uytyufee.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2iofigynl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ipcohwhr.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2edleelog.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2xppidaxy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hhtqfuiy.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sxvhhqug.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2vgezuwaj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2lssucaiz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2wvcufrxp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qlqechqx.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2janpnllk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2krqfcbux.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2keycgjdn.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2kppnulta.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2srzfekpk.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2xxfiwxnl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2txbbfsvn.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2nnpefyse.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kxgpjbjw.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bcaoclmx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2dmziiqxg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ruvcmswk.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2hlpjewlz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2uufrdymc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2banfwthr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2emgdbkns.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2acuxnfol.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2fgcbqntu.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2isnwczct.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2quyqfdha.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vlxelxen.html


<!-- 参考信息 -->