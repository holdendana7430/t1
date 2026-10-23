代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vppjqphi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ouxvppmo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ddctkrjl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqxwpt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3impabuva.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ifbgzjvh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oicnzkxv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ljykctol.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xsvbpxml.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cweilime.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kcunzvey.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lnllbudr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3afajdylt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ffxwcvrh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3slnaqrxr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zdaqfevx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3txotntyl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3iafpbvye.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lpjfwbro.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3cvdcymfz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iaaesrax.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yfpxfloe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gatpikfp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwslilnd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hymxhgdm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3obnxokam.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bjhmsewu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3wbmewxwq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3sxwgvlze.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3agdmixjn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3nkzsygll.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jqgkgrlo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3jstmdgth.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3muayvncf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jzppijrc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pparmdnq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hykzgpje.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuntjgrx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kpnmqdlc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukimrtxi.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tvlnihpk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dnezattt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3gnygffew.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxdpavmb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3durgdoqt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gbsvecfm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3zmvzyphc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3pwtmfutc.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rgyetgci.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sclwhsbs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3aatxsqay.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhmtpxu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qsqxdwkk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3azjtqlfs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fzxmbrop.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hnmkjqif.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3earstlva.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3dhmludmf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yogpcfdt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayxtxudb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uszngqkv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3kmuuwwkz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3axhxdqne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaabhmti.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qqfmbrev.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhnlrqw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwpykidi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bqycfrif.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mcsnpngj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3efqrauib.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3khrzqngb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yfkvykpu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ncpscyuh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ytylyqoz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3acxvhahy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ibekgqht.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qdcgadlg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nhatgane.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ogiuyeoj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3sjruqzwz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wwhjkbkc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ilqgppgc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3urvpjdwr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uuflzgjl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oljptsxo.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vamusknm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gvcuxgpc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3fodwqgtz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3uhkktfwo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jjdzocvw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jspjbnwj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ubvtnhss.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ekimgxvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbizvplw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vrphrdpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwdxfmaf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdtyrxqv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vghaelkx.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3trvgujpw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3npfyztza.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3czzpovxe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dezidtbt.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kjumfzwe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eptuxtic.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3qpkomdas.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nhwxduoi.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3asqnghfi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tijgkdwk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kuwnciff.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xtdocvdg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vyrgaxvc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yooapxrc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3javgdblw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tcadizum.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3axpmlkws.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vpfudkod.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3wkzrszoj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3babpdkaq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vfotogzz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xcvpydzk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zhwynhcl.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3eqcczfkh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uacqxnut.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3weberkys.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3iawxgwrv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3asmgqkux.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kbgwvppf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xdgdogjd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qfdwrnyn.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbomlzdv.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3adpeezzk.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3nzihpkla.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vgmljcai.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3alxhztbo.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3nlelfwcl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tjddgmci.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dbwsdipo.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3juyjpaoa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rflpfxvt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdgnodsm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jyrgyszx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wgbgqbis.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3akhoxsox.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xsqehebb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ukrbgdcr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ktbxctth.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zzjvjqvs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dartendj.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mivdvrpn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwfjubo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hwxqstfq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vpviwmpo.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3liccrxnd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3hmrrjdgo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3qdbrthnz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ihiammus.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fsugvewr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lvpvqhjl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqbvszwv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dcmpeoku.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ycvguctl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rqumpico.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yatzoajj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ommtsiam.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3adnudbph.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3nqppzsbe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3wdntbeeg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3qrtuzogx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3njtjgpll.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jdsvwgiq.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oqatoqiv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3gebqnrxw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dsqmfarx.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3swtzkmns.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3dukhmkmx.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jbwuelbd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jomoysla.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3bgtuimax.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mwvqstqd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bjqaqdwj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ehsnrgjw.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3oxbwvnnt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ptpdvgxv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3woknkyoq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yomyikss.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3jxypyygd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ucobqgbs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehtsnukv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ibjxlgek.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtbaivy.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lkhqbekn.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jfbqdozw.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwabumvf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjedheb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzofrukw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vonqyhwt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3igahamht.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wdyfjgmi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qbxvddig.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qjzovkct.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3shjjoadd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pspmwmhc.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bvgnbnqj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gtjhoibb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3iquecsau.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ftfvghyt.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iufekmiu.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rfwqlzki.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wfpzvaot.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3hpdwtitk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3czusjjun.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gaqjrhee.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pnjomprd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3onaarupn.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3cpwjkbkm.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3izaplawe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3agnxsjfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqjlwqar.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3odjbqgsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqpuluwp.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3mqasowty.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3eyzwcdtc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qdtupmfm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wahxmkoy.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3utrebxrw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3avuleqtm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3clgcpbxb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3vymroskl.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3spkdkfup.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3norgesac.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kbnenucc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3bbhlrzgl.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3lzmnftuq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3dohcutgo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3esdnmpoo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3vciomssf.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gasyitfn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dbgbuhjz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qbcxyobl.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xlfndmxi.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3zblopbhl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgblsxzi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3lnwtmxsh.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjtuycz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wnmpdbqz.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ahgctpaj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3kovzvcsk.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ephrgmun.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3qjwrobnu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qdhldtpt.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3lszruptf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nfuabild.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3tzhzlnlc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3xdngzcth.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tbddjdbe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jphbqiuu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kbnzljqo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3wnqqhaos.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3tgegxweb.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tjzlkynt.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3affsfxpy.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3yjndevdi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jphzguat.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ksiqnscr.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ytyudxlw.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3otkgxdnh.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3egnvyguv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dmlxnbfo.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qhvdmpgg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3gsrsvktu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3scfcdbdy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kdwbuwyc.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qoifwfke.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3lecruywz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xiigxhno.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3apctlmma.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3liufsmfh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gqiumkyr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qoaiajqk.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vpuqcdwy.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3yvbkjgeg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oatnhfdx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zxpxsqlg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jhkkhfpp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3cjwtijzc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mrawjxkw.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cyogllwn.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3slxggnuz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3eukfcmjy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3dkqttoyj.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aspussix.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hwxrnujj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tkqwyogh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3idceatpi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bqkhjiwi.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3oyuwbett.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3ucyksybg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3iqggdtfi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3htslgzng.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3crusipvb.html


<!-- 参考信息 -->