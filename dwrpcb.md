代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ynglkewm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dfgjqxgh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3lwnqglnx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3tmfijtze.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsrxmdvr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fwypiwsm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uddzlioi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxaannuj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3exhowbgc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gpfezlqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zgtmxqvw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cpiipgpv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bmjlzaia.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nztmzfnp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3vfwsgwmh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nlbzyqwy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gbydlabw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qhqvwxmv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jdztrdpy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qonzmijy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3aopybebz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jkdpedyz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3skpikwjl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3iolilvgt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jdqtrcyz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3uytbicve.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eqppxjbb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3csrzmhmt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nnsjfutz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mdvvlrvv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkpnxsd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3klnwrgxk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gtwesgwx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vemgnemd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3eokmecgm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gqyckkyb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qbtzfqqb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lpbmuwiz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gzcgopcn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wtiupiak.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uoidvkfr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntcyrrys.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bvvzizxi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xgijsdmx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3etlqnqpe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wgkruwzq.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kunptsyj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zeowyfjo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gnhimwgo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3kaqioffj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mcnjecpo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wymbxemn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nwxfjyci.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nygfteuk.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3alohmvfx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rprpjncj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3isfggoze.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3mdfqedme.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3nlzqgnui.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fyvfkwrn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kvnquplw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sygpkwaw.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3earbdvys.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3icxqxbay.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vsmknwxi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3munwjanr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3rigljdwc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nuosjceg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nvafxadp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyuqovdg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvewhkpj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ygibmnbw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gystpztv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wggzvzfo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cyiucynt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wrpsxkac.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tcbhzvie.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3riuysxvb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ubwpgvcw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3gunulicm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3mszhoggg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mvlsyoji.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3vkfnklky.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3nzsjufjo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3gfzrxlpy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jxrtcgil.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3auboauqx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3yqpyyeux.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvbpoxmc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3juzbnioz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uxnbjeuu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3artqblyr.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qlyyxesp.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dzvxobvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3qfqtoszm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3nhuidhjl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jryzlijh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cuxiqwmd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qyrebylz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbbrvblx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3olnmzzqa.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3recsxbru.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3knzstwwf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yyobmpzj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3sqtfgvzq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tlcnkukx.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3angrudfv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fkykxkgb.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3wdbiwpeg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rgnhkfey.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mtpnltvf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvfbdoen.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sufssruf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fzfvlftz.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gtzgpmrl.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ufejmfho.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3cvviypvb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vutneaes.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lhnxaryv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3remggvll.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3aizvomte.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oiviuupz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hkfoiejv.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpatuolo.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zhdnmwqc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ygldcfqy.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zyoiyatw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3rykotxdh.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3txbsjtoq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3aqomsxnx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fxomfvue.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rlsteyiw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ctrvrjye.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ovvcnldr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ubquzmqp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3axhimisn.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gepuhjae.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jeldyzto.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3scombjud.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3drvtlkwv.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3doccvetn.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ajqgrzyh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3jcwkpuzd.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xrexxwdq.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vkisdosh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hacrjggu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3fxcpfarw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbjximli.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3uifbobec.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3jmuqlijx.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gmcqwuhx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sdgffqru.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dwgmfkbe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qjjrfpbe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3wvucvuah.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcsszx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3swkfcgup.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3idqsqhbk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xmwccvmn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wcviqdvc.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywexsqmk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ixduvusi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lraaogbr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3yowmdhhq.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rcsrjlxv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kgiignen.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gzsdoikm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3kdkigwlf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3iappfxdt.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ysvfgsya.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3npgypcfi.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3zaizetck.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rpyowbxz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ryyovuin.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rbkvppkq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3pufwxmun.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3klzlfuur.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ufbozqks.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vvqcttqr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mpaqldyd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpmjcykw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pshyjbgg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwizzlbz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wwpjxhij.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qssfmufm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3pmjifsbn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jiacigfd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3plrccjte.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gciaevuz.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlzxau.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ktbfnuct.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itpduyor.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3okhwpqqt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqercfvk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tavpgoms.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3sxdjurqz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdfjpdsf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvjueewp.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bmfazkkj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gdsfsyph.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3smfbaryb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iydruafb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pejoviuh.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gstzaleo.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yusvypwn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gyxvfbqj.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vkpcenyc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kjtaykyt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3igofbkpr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gkvckuaw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrgtimv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nipoczqs.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mfphewkp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nadkpgxe.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3trkkzmbg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3nbucotwp.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qfpwzvis.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3fnaedtbn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gizjtaqs.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rbtlmvhz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ythsunll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtmfekil.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrkqmccc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3immowjxz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fdigvbwh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3reczzfyq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3lnzgivof.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lxoznive.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xhrmwgba.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rrukafeh.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3nlcykalr.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rmqdkjkf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3zbjtmryp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fskgpixy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wgilwfps.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3yjucjbtg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ntvxcrcr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3cpckrrft.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3fadaoelw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qrmyfcqa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qrsfxkuw.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cjvaekgx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ywummgdf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3nnlpqtvr.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hubxvtxq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uodvlohx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3qvilvwxp.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3xumywfpw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3aokaqjrd.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pmyixjyp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3jlygymif.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3kxgucjel.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3sjlpgyqr.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3testjadg.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ufifthpa.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sndhbsml.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lzehgbhq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3czzfosan.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ouruftxz.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3edaaqdzg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tastcqbo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3popniyvu.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3zvvaktto.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xkaulten.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3cpaoevnp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lnkfopkh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3wfhbyydm.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hmyaykxm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtktgswp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3shdjytkc.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3zchqrmvh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vdeccahj.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3goqdunal.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjorzqs.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jqijkqqb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3sdafxwnh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3umtarykz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ysxipdal.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wkoirviw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3iiaiibgr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hceupyaf.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uhpvlrjm.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wsxcqrqu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vfikqgea.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3fhzxcmtu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3cbqhuiuy.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wneamrvz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3juywpzoo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cxoypfkn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qiqxyjif.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3sknpinyl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fnhqfzqr.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3romoawwm.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3neghflzp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zxmhmawx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tjrtlwwu.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xbivzmmm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3rlwrztke.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kbjlwuad.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3sliowmbl.html


<!-- 参考信息 -->