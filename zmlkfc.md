代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2iqnmlvfs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wdjrbryr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2chrhobfq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2njequlwi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ndlomphx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omlwkchg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mfpaylvs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2goftzgip.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2orbawuom.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qytuidax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sosrgukh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2vbrrjvae.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tlatopgy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rgdfqozj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bjxbdjme.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2btosgzof.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jcjaamwz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2blfdsjsl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rlqgtxcc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2pxcnbmme.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xlcfthpj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cyeikjcf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nxyrndlz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jhlatwcd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vzhsduko.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rudubmnj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gmovhcgx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cuelwoxc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2laegvize.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2seujtehr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2rbksuefb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zdbsncnq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ovwakfvz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2scgzdkjj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eihogsqp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vvuinfgm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wdimhahw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfsytcps.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2tccoemoi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2szhwinqt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2gsaxfhtt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xqsmqpak.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2eyscvhyh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gidjvyse.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cxytrdaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2alvbbspv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2cvbjxmqh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2udnvnexo.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xydirpir.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjlzkwqt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2miwhmjhm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hasjphvf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2rpkeatsa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ngegdeyw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2utivvsiy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2gutbtitr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kuyjrjmd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2axplzxdp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ahrahntc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ilsvrppy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2rxbhldwq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tmknqxjp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ekibhmdg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yimlywec.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mehkujat.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2vowxacbq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2twmakrxb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nnryvtic.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2twieoxwn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjpkgrgm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkayhatb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2liuflgmn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxogki.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2udkeqqvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2njpjfajp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2enubxoby.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2siqigbcq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2zjxaqqeo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xsmipqlj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aqkwukbz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gwabchoz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jbizvjcr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2raydyees.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xqezuqfj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2waxwrzyy.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ddamsxnk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wztxscve.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jwafuvta.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhvkdrhz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2cmbrjqlk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qiumribo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2gvgmzebh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bemwwoqn.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rajsorfx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2opozbahz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aqzqnqmu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rhykbiud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfyadvvf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ignmbiyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubjoewgh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rllnjwkg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jbgutxsy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zndsamjd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2yyqldmdt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qpwjggwi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2uqdbrucu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2tmkdweml.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zuwcchre.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2okcfldce.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vbolirnq.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2padwiann.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fyogckyl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pmohjfem.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wpdtfucx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dxdthuva.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lcwwrqha.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2bjtxrehd.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gmrnklsc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2cfpupiit.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ojotqnmb.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vgqhlvhf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2qjokqsdg.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2efygrjqt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ievqolcz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ehhlphia.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xabeaety.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nimjuclh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzovpam.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2dmyndogr.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bppoajiw.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oqozrmsc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hopkpxtc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ovdnrglh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jphoxpof.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2waposvst.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2ujnxgayq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2faicperj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kksscwuv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2etndisce.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwmetwg.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2quocgjef.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxznplox.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2tmdehtlo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2buovbben.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2uarnwhkw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2abbzjeau.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ayhydywf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wzbpjtok.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hnnplyxd.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gfthrhry.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2vwfjmjiu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vdjiodnv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2crgozjxl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bgwpzkok.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vwdrsanq.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2reiwksro.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wgtrqjpj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2srtzjiee.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iipiiugq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zpmlkzkm.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hizluuvd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lnxujhbe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vfddxjex.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2tctjbyms.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2titlwivf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wjnlhrxi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2oboihdtc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2rjwwcjit.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wppuekbs.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ysegqbjy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2debmhuxu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2wpkknejf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2raiggbvb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2dcpneefg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2cfyhhlro.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2dcreqrai.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2rdgeznvw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2quomeqfj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rnmgpgkn.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qftybsnx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmjflnuc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wqtlkowp.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2rqooeglk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vviclphd.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bgjxduub.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2madfxpxi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjtvzuwr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdiihhpe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tneqpopi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvlmuetq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2blkhifkd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2weskudpr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2ujvnhboe.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2shlpdvbw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jdqyiaqg.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2urlahwpa.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrbrruml.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yljwbpxj.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rifwugmw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2pgltzpnj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2cugdlqzh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bdorqaow.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2upyqrevj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qfubqbjt.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2xslfsphu.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wbekcano.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2krdzyyxw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2oraaichk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlckjrbj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lvmvbdkr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wedwphti.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2tmoofkjm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fdaygwec.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nwherlga.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2dxwlbkwg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2pzoueitx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2jwxbtkbu.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cdlzxnrr.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ensnpsnh.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2rqejhbmp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2zswokhuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvylduvd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qinplqkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxdthvom.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2dwnnhldu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2tsbhmgra.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2aurcycer.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ckotjpdq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2sidosjos.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kkmpgpxk.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2toyotgsl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2mgwywoey.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2zqiymqva.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wmanynjo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2vffbxsql.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2kocohuez.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2apygihtc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2smpuovuu.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2zvzbokjf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2ntlfcgrd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2yapfrdab.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2orqgtgnw.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2hhhcsrmw.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2yrdhjovd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ruwrselz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2tbgxiyti.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2auxvbgdn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zmyzoklt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxxjklqz.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxzeass.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jkjhlzdf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2tsfxrbsn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2cyklmaqg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2ggryawmz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2zepraldx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2dmhourqk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ecauloyc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2isriroio.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2amkqowce.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2voeedceg.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ebqlxlnu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zyziruhh.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2ywjfbxok.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2ncbjlnfr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2xpclgoet.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2jczuwnxs.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2iqmdfxfo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2pbhquxqw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2cerhieiy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2ygafieuy.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zctbtyoo.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mesrozfn.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2izfqnnkq.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzrcxoc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ujxiavyt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gfponzgb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cedrioet.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kbopfgrp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2swkiubhv.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2anfakxzb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2rrkhppvw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2laagdxjr.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2welfkpkv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2bnmezmli.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jmjgwbtj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2satsntio.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kauidnyb.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2aepxliex.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jthfzyds.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sybuqmoy.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2plzfyqmt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2rgxshlet.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ichftozd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2feyjijjd.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lqpiyonb.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2tdaywjff.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2abrzymcg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2satlmrsc.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2imcmjqeq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2nnlkmylm.html


<!-- 参考信息 -->