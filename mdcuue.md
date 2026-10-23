代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hdgronmm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfiaev.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oywchemy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eibxysco.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkhuguw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dkpyadlx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gpvjrktk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3uyhvocij.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3adqtlfig.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qhxvvvfi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3iagwncmf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qlnabllt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qnramlkl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pchrowvu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rqqbzasr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zvduslfa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dveibvew.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lzseoiek.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3uhuinkln.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3wfuleyup.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cbwkwclv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3enrknede.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ewvcdaeh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nliylgtm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fozovpob.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvpizdxa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vhnwivmz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fzxzlljw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3brewpfuo.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xuwcnytt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hseojqcl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mwnfwjlm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3spupmwfv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfrlnsfx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ddpevzzv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iphflgna.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xidvafpf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nmlvorcl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ajdoihdj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuxszkg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hwsevrti.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3suxxxuwb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uthtbrlr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cdsflvua.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3oiyepvla.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ydpfdekg.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ncvdswcr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3gnxesgty.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hwjstlmg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ibxxarfa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3macgmuek.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tnxuwqbz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tpjyrqdz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rqdbvueh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uqebfsaa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3znsvidqz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lhhkygbj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vprcwqsf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3gxghsvsv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3eynsyeys.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3eozkorqs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tuyxeepn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lwtxngto.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3awimffki.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kpxblumo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixyzbenm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvwvpmvt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ginyuerp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fwerohht.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qfaawvnm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3gqxbxhnk.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wlxvrjhi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zhvsqpkj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3prvbmdxd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xyzggcsa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vewdplij.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiirwjqr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3crucngsd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3kqgchuve.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3biffoyoe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3duzquhlv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rkwirvqh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lrxwslyy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3cyjmfczt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkoknwrs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3rremrlut.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lzkiufth.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3csyfbqim.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tasifvcc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3uqzxjjcz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3aardrccy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kbgyxdfh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mkkdqexp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxxjbjxr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hwagphnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqudeaan.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gvgfbpfj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uazdmyet.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3egbcgtgh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jyycjnqg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ojxfqmle.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lftmnsxm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3bnhlenvd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3yslniyuo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rjuvucdk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vpptidsw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gggjsegu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mwnvubtm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hkdmbmac.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3idvkogcs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3vgvmsulq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zjisfzre.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfdeww.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kpibawfm.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmuytrkp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3dvenhlpd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pgxdpvil.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xpwupolv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ogtwzgaj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yxthzrrb.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3cwazzzoz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gptvwzey.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fklyectb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wvdrvoxt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3uaqvcmjy.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3yrbzmghp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wxteacjg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3alftqbkq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ezdfyjmi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pscukzhf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3donnptay.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3sdrsdljm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qlcaqyya.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rdilmqox.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3flxyzahi.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3xppfqfxc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gtqcpgjj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dfqslurg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3zwezjsln.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3lfynuagu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xyuxkovu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3itghomwg.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3knvmekei.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gpdoiuxu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qtibpxyx.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3byrhykvs.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ogjlbnqs.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3osivveil.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eetesuqk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjuhiveq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fantaviw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hyvadmma.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ejpkcvok.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3uynifdiq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rgolkqrj.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3abshmjsk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yvqtgaxc.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ezvjznwl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3adzjwmun.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvnelxvu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3rtrvcovt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3isfvmvkd.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3waguqugq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ewessrcn.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qpuiolvq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3npdjzhyx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtdsmzyj.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kxfovcaw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ugkcciek.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3sxotmavn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zswgyams.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qiontnqt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kevbmdma.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3njxgttod.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3kzymflme.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rsozqjjy.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xklbrdzc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3udnehwfg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihshmguj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gawoihez.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tfnnmmbh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gzjyhkkx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xdtvddtk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpcsbypp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzyadd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttvdgvfx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tqbqsold.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hdycrabn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cqkfniaz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3tkudchnr.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3clkegwwd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3rslirhru.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uffeodwu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ealknvvk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3odhavmbr.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3buchfgao.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kumesjhx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iwljrorn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fnrjboyz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mypoyqcm.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vsksqjxi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zdqgzupu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kvkmtfej.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vhzpkrkl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rokfffgu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lhzkcyiy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3kdfghhvn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mqtncagp.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yjehftvc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hfyjkzuo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqdxiohh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mezxfgnz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3bwrstnfk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjfcivpl.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hwnljywq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3qlkahjdz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3yzjrwntx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsfzuqiq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pclyjbhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrwwfpbc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pczbxewq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gxsxbhdy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3crbjepwl.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fpirglur.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3vchsgowp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3zhtvwpuw.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rroszmvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3zowdezkh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3bnysicgn.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3nishtgqv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ssitwlio.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3cijszxwr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3wejsmvwc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xsohwtdp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3zpchimcd.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3mbwycnwu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hmccaywh.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fdvxfqor.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ehntwrzr.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lzxbxghl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3umeguivo.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bncrocwc.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3elbjeitw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vcahujyc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3jvmtzdzx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3wmsnfjko.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3vvroawvn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zqwitpqw.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3pbzapsud.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3yuhwwokj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fttrlcyk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3uaiqiesk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3itoapnta.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3cautrprb.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gyicsmld.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gayoqyjq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ssowsxil.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgaclzdt.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ifqkhwyj.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3wudihgsz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3xbvqfruo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wotczxsj.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3yktialya.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3phbnqfdt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qkbkyzdn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3wrbgosez.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3joqcazlc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eijhuhhz.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3vnwbstse.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhaupud.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3qbgionyq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3mubivhcw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3vypmcdes.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hxxbrmbl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3nvkfdkou.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3jrqnwgmv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vykeatqx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3sormpioo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ftvyjgxi.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cvuukogy.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3twmhzyyr.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ibhnsbeg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kqjboqaz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qbqudcwn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3getfomxh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bvhtrbgv.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3eauqbofi.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnmpngo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3tkizomdl.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3appncpfp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3psebqiok.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ggremjsz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3uwwkrbyc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3ldvucsdv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mixpurtq.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3niyggtpq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3qjngszdm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3llnfzqpz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vbwjvjib.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3naappcmm.html


<!-- 参考信息 -->