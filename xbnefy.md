代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cerqlqla.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2oozwtwxp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2etukeyir.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xslgvgaz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xoztewop.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cmytddpg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2qjybjsbj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gvflxzay.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lrcuelth.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kbebedgs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2najxkfuo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2poaociwl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zmibmetx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bkwyntby.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wshhhsgl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ukwlthox.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2telgofml.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2amkokgov.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2evzrctpt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zvekwqmz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jqoedodt.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2dkatjxsn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2rovwiuli.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2umlpwook.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2srsoliyz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2lsjvrute.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rwruvfru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjolsof.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2htbbmesy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dlysolth.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bterhuet.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cbocqziw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zeqsxogw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2dbmwdzwf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2fjudmxgz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2blzfaymh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uzcijiks.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhhccf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2okskefco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2rccordcr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2lxrwlujz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2kcorzdax.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wyuvlwjo.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2yraagvqd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cfwkyuky.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iofduvai.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hcnoogyr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hvisdeas.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2drljvbkt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qprkscql.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2pkfstjek.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2rjuhlhej.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dhchmkuy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmoreafs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qwxnzlbc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ihsprmgu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2yqwptutk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2effcfkrx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2sjjmpfhx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2euvjroyu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qoslxiqu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qunoimwm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zbmqwwze.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2piomwqss.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jctmpafb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cgtvvcsj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dwpfhubq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2uxcqlxqi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2basrgptg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2esakmups.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vpxvyjdv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2xtsbrujr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmhphopw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ymdggwgv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qtsllnhs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kvkcwfok.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2luunaixu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2eqftguyv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2sdnzjjqy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2oyyxkcrx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2gxervyzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxmjyjfp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gwouahak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lukalvom.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gazilaox.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dreoengl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2deschafx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jsrjzlsg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2tgvodyyd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nctmkmoo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dfhmwxrw.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yxuwmltz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qnfzvruc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tzatfwss.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ldtzkxaz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2txwjdwey.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2clpgpisu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bzeprtyr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pkcavffq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qisxbihi.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ayffwaew.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2odjxmiop.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2gumnjjol.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2inorqdwe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wtkktyoq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cxykuixx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2qpnoadcb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcrgbvz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gsablzar.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2efjaqnex.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ivsayyyj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2msipezbg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xcplgrup.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2wuhqrnwq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zsaflqzz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lrlqorrg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2kwsblvze.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ieobiofk.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fwsmxaoj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2qsgppaww.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2mokrfedb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ciyqezev.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2paprtguk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2zdpecgga.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2wrfmqdxn.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvymykb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mewxdilj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mniexbpu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2nclpzdnf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kvlcfsoy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2vclalckk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nbhuatrn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2vaacfsgw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2pfmbwfzv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2cnzjtgur.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2unpupobz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nvfdagnu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2xbakcecn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mlqgafrq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2kafrqpkc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2udwconld.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2rcpburbc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yvovtkuq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oixgedlz.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjjzyysm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2uefbmdmr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxxjlsuz.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hnatknjj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2idribvns.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ojgaqxda.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2plkdvike.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2smasvwje.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2aukchzgg.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zgmnrrxr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgywdnyo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2xmoczdkk.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wcofmvih.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2njitrrqu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rolbqbal.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2avjrupxx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yiogabyx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2oxrhoytt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2rexbmfhy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2giodniga.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vyrmnuvz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ltbodmci.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gccpjyqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2inozvkqn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jqybhwle.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2dmqssido.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2sznllulo.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zztcdorp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znvefluv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwuukgff.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2zenlftxf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2okxoosws.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2xglhzuku.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2rigjxpzi.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lmltmlmz.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2fkfibvlr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2peqwugpq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejlcbrmx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lwndleqv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qzavvatc.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ljkysmyb.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jfzjleqp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wpylutue.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2atjgffso.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ewxphewm.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wioipdjx.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ygsupoxn.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2dxizftfw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2femhurnc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhscuz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2afbhzszq.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2suqlmeyg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2arwywmit.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qwnzsmen.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xtbhbfzy.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2oaibqdee.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2ntddktje.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wnjpaysc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dwgthinf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2wxrjcmdw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrgrqgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohmbbpmh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zruvnreo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohzxwtvu.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2xpmaqnzu.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2vpjpjvyf.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2zfaemjnr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yguuvtaj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2oyrnkoty.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rnipxytp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2obstbhip.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2hypzmktq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2xvtizpbg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ethctxim.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqocdhxa.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2zxdkbbet.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uoimjrku.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2qjaycfmq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2mevyomna.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2fecwvrbw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xmibfwai.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2lqqqfajg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wcgoybdf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jmotiogg.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2xufrsnjr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbudiwtu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2enqjtnld.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wevzapso.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2syczmvwm.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkfablt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2mfywakth.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kovnwrca.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2tjrjzixs.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2axwwzxiz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vwgifyvi.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2rgtzxjnb.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bjfakmak.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2pinvivwy.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mehrwzly.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvqhqvg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tuwvuola.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnhliqz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2eiqoqhae.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2bgclihgn.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nbbwjybt.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2mwgepadg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ioonptxy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2kntxqpsq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbkaafdp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xlrimoaj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nwckwwoy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpypwps.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gdplqbhs.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2kufbftbf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rytcenzi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2pvjmhzcg.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rgzvhcxe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kzxhajoi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2vvcnxywp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bjwiicgz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2bhllshfr.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2uushnehh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fdniddii.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2cmhfdtua.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zdvxahkr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qgztilhh.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2dztqwhxf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2vrukgaon.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2rijikiwh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2oilkpmdj.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pxovpvek.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pjglwtdp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gyeltviz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yszqsfsc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ulrwtgba.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2yeofiwqj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2lwttkdep.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2twdzsipr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2evxmqpnf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2xtizchmb.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2wabahvwe.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2wjavzxeh.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2mwgjjprd.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zluiswlt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2hpduzxba.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fonsqavz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2saxekife.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2atidnkge.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jltjlvrd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2frjbzbrz.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbcnrgsv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2hduundyv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2icywrgsb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtzsqyi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2gupffhuz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2lpgydzqq.html


<!-- 参考信息 -->