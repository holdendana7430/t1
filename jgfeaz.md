代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zjqopqhz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rzxdtmjl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3msvodhxj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3wycxoyky.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kyrmsitp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nzadxxis.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3joaytldh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3txjotjij.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3tfddwfuy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yobdliix.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jhqordjg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3crgnrwgf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jwyiljdc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zxndrplj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ypgzzktr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3cdmkjibw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wituprpx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vmgqguvm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3erjkokku.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aqbdgfeh.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qazkgtgm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmaggjop.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jwmhgjxv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3chphpraq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rperjofl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xadybqwc.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3iswoweip.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlttyyov.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ffrszhtp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aneifhhr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gqufficx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3khsbsprk.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hgxypvdq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsrxtuws.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mievrjkb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3irjtopnm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3winijiuc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xwbnrqjb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rjayccex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zzttwdcb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3acqjxmfo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3uggkhync.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3iudbyufc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tjcmmvrl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3enocvrcz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gbhinymp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3oujkctwx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyusiwwu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ouuycwub.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tpvlncta.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zvgzypnk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ncfoxwmp.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yqlyierj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwfjvuy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ixvafgjq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3rjrknjvw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3yhufgfcx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dgjcdxpb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eqgryetp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3aopueyhx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pdpwijvp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kevnfgjh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3foohvpik.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3awlrgpkf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vghjnemq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3oibuxycb.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wsajvjhw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hgyxcofw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bkofbwit.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3jrozzkrl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3gcxuejzi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zedippus.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywuzdhpv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dodukciz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rxfwuoes.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cfdjpslz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ihjffcxz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mhrfutei.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ucwdeuca.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cfggpybm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ckebdwde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqqalu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jxgpgnpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyeujszz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ncmqqynh.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eppmczlx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kzkockvz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3oxyyoqhf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3pfwbgcwk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3axmrffop.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3zwxeofij.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dxvfygjz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wrmtrnds.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3chgtztjg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3edorvurp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cyduiosd.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zovtlzpf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhhlxop.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qqgsfifr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mlhtzfql.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nplpmuzh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3cyzqtgtn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3sfqulkoo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3qfgroxmr.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gmvvroda.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oafhmvjh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rbbakmza.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcapdgba.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qikxqwzz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3uzzqdumf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbhraxgd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3gzroddsy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3nnavvlzx.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hjribneq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rmqpgqor.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gzbdwudm.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3wljqeths.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ohtkvahc.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lxxxmbcu.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kpyxbrzy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ptgvkzzw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3iimdfskw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3mpwqvkyv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bcreshju.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3whebsysk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3owbzrojv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3xbimojtu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lasxepwm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jzaokwvr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pcriwlxi.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3opnnceig.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aovxvxlb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pzwoioba.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvvsydy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3umhhpwqt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ptitnnim.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oskjqbsc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pjbhnxlj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sjdftkxi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kxuyiwdg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fqrunhla.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3evsibcau.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3zgvxmbxl.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3uxjaptva.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyqyuyul.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dkpkdmqp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gcvcvzdc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3bvfrvdjt.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pbqgltbx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3gjumqanu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3obpssbsg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3orqysncp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3bzziwcgb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3urexiamd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fmxtyedc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3xxxpdqcx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pnwjvjwb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3buntxbtv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zatlicfj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bqojdfol.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3dzihhcvj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jopdgpnm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3danyjfbq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3qrrpwnbs.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjcrxslr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fjxfwiuu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3vxjtcrpt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3tnylshnk.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ymnthrhc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3orjykdyz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fcsyptcv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tinapjxi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fggzjmzl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyvrljx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3oxqovusg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dufxxprh.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nvusqsgh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvppcti.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3koridjed.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tdtdfpzz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kodjbnas.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ublhctix.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uzkvlhnw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3dqffcxdq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3jrkiyiph.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvmebbcs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3edpqhfqp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xqkilhjb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3xnhcobkt.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rauffuth.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qgwmytjv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ezoxwkmp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3kqqfhswn.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ivhurmbd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cjsyonpx.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kmwvktrq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gqtlhnsx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yjkbrtjt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bznixdbf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3mtemvxhz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3jjcohvdd.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3muoejzon.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fluierti.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3etshmbso.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ytudjkpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tewbimrp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ymspmrph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqmzzmih.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3osrxzjpr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lpyuoshd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3hnmpsymd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kheosqby.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ccjduzfq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3swiqoqgl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3yyyhbovd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3pgcxmiox.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gsqyvher.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wobvqgmy.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3gmlclewu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3dhgfzwsb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3sswtdrqm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dfmpiamd.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mkkgyyem.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3eqtapuce.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3enpxyzji.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtrxtcb.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3diknsmat.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qtzbuqxu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3jtypcpoo.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3ykxduzzs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xframchv.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cvazadgy.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3gvrnvwxw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3oawusdml.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ipinpfym.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3giqkqndo.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jplogogc.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rynyuymc.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3beghcvgm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3wsttiijg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lrmsqpyh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3txofsyxb.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3vayatobn.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjjnyqe.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3nzmninre.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpcfpuie.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3trazhxck.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ugqgglxz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3junkewut.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3wtihkzgh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kclpqaht.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3vsqjwkpr.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ycyhpoym.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3trmvsqva.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3bklpggin.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mpgmircg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uiiegkpa.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3komvqole.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3arhfqgmm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwkdlmr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ybdnsytg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ivjzmmum.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3rqicjiqw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3hyxqhbjs.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ayclnztq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hyceyxsd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wjbpjwat.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3isuphjpl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cbbmgpxv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rtokhibe.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3duageebs.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3tsjligek.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3fiwqnynx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3bvmpvvhf.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3drzotzxj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qsaoqrgp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qzulbtxz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ubvffeic.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3wdmgbknp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3fazfpqaz.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3azsatlea.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3eoawwgri.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3kjlhalrq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3tpwfisph.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3hqglqlab.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jztfoblq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mxcypjqt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kerzovib.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3bpiftglg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3yoclbqjx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3opcevbwa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jmcnazri.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lkcsfcih.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ftfntmdn.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3xgoypsff.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3rvzxlhhg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvlntzoh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ztoohlbs.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3dumcbemw.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3aclrhben.html


<!-- 参考信息 -->