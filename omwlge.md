代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpyenqo.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hdewaano.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wogyjyqh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dkwuzwgf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hlfrzuuo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zklszobs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3caeaxiij.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dyfftwkm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3xdhxpwhc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vgwgxcft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ljlqhorc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qyocelce.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3btrcioqv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pjorsttq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fsaalsho.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3znvoztcb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3byjutsql.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3nesvacjp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xqcbmeqf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3sinsrhkz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3jbgrdfio.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mousepnn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zwwemrfv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nyzndpjx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ehurwfaz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mhtjzumg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3smvhnxgf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kjcqkazo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3iecuruhy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmrnimqo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hrejxmih.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fwsvffll.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jlzdnxzl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3betpwjzr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jmbybpxb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3luecnyja.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3orecxskh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ectzqait.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zmeznauc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xpjkwjfm.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3qkwktilg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3rvqrumsc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzxhevwn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3evizxezx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hgslyxnb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wjjdiakl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tnextcbz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cfwacjkk.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tngphtgt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ziivfhjl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nmxmygmc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qeisamyf.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3dsnbnrgv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lgvwjkcp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pfxocrjo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lrziczny.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sgppevrf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dzprxogl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jserpcum.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxpyzcbc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wkyyaahj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mxfkwzun.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvxhqsyj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3eqlztutm.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vsbvwswk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlroivws.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3atenfere.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3gyzythxe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aplrvfjg.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3xxhjgzen.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hldlwtjq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3emfkxrvb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qankahnp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xowhwzuk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bpbhgeel.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cdtvmsyh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wmkknqpo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3eudxudtq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3opymprad.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3jzhcedqu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbseuime.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hiycesqo.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3uwuceulx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qqzxuzjt.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pbficuxg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3qcnkxqmq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3txbwoesh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3olavmphb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mrexiyyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jssfdulv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3stvrmpey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxwgorxw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ambtwqpx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3urnmnqlr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3nbzpoorx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3btkqhwbi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nhojtrdr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3dmaluwim.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3oabsdmft.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3vbtnqoti.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3sidriylw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3zeriogvw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eejrzbbj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3anrmkiel.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hzhqminp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ufadpiqk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hxokdenf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3muofllnp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzvacser.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3eeoriggg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ddmvkydk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3vzkzgzbo.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3jdablbvz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3oohdomsa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ygzvhvis.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qsnvkvmh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zruthehb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvbydwdx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3quqmhfwr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fmromkal.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3voqmntlc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mwgrhsyt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jewoducn.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vybeekaq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rtzdgngz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lhxcvipq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3htfvbvdm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3icookfnx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3svebpszs.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3liekzcjm.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3sdkqwpvh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3tfysaivr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgfnqrxa.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mkykyzfs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pwiweiot.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xwkeitwq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3smbpuxom.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zknhfqun.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3woepvhxk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gurjedwp.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sxigedfb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ionskrhi.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3coeyqufg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3xufprjwq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3htavqtii.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vqlkfoyx.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zdfovvvj.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3cboljaom.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ilpjhtej.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdjiwtk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3srjmeszv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3tsormvyx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntgmghyu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cjnxqwus.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3roauvxwh.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dawcfdid.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3teumlxjq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hymmarei.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3vnundpxn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3agxxzlvq.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qzclcdtc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bufyqias.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pbfyxutd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3pkhdpksv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ungneajw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ukaenwmj.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3wskyohol.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mecabhnm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jhvouuvy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3iwdiwtvg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3onlkpuxs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wvpbweax.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bphglfpk.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3lkjozgny.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hzhwagcb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3swpvwatw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mpjvqbkt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bczuxhor.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jyswlcdh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rpdazxax.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ysqzphzv.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mapsodvv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3blwaiwtf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3reahqzik.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kxaebleu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3sjulsana.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hdjzxdsa.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3jguuuidp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ulqzcszk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sdgytdok.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gabeulok.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wxeruxki.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3emcvqlfa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3noztfbdr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fcwmrztv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uydxgvpz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3klipnnwj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hfxkfqfc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oyvugjfd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3aewawxit.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ffoowwfs.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ucxldpey.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3vyyaycjl.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3povxrlqq.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zxdyifxk.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qcqlhxyx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdwboblq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zssikqdo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qssyuvjr.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3xlmhmvuo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3yehfkttr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gaewejrc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kwuwtpbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pofguowt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rgbmvqyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibgxwwpk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3isymihnw.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jlahvzap.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3qftgsmsp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tjdtiwbu.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wxvmespr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3hahikoun.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3stjpvfqe.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3scmyxldc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3wxrbvdjb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kflqoigc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3jtfzfacu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3utikqdxf.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rjfogwdn.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3jhlpzlgh.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3okgrrylh.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3plnugszm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3jopcxlgx.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3yqajxesw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3xybokjow.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3yddawwla.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nnktrkji.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izybkofn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qyuazerz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3noqezshc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kowbghuu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ierfawiv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hfpqsjjj.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3yqwoxobo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3njsgejfo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pyiqrdxp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3eaeprady.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zyswyhei.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3vufeuxsd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3jelgtxwd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3dtjqotup.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uaeghmuq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3stqdqcoo.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rewftxap.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3awmhpmpv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3buvpqwyz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wokzqjkg.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3xnacaqyc.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3iihicbrv.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cegwnvau.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cufpgjdn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zsrxqfqr.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ktltqanj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xbujedjk.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3affgcfxe.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ubmnlzeu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3vzcbiixj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3plrqvfdq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zdixsikr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3hjrqqbbf.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3bdyjomaj.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3larzpvqg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wbfoucok.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gkfejzuc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vaygsqia.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3azbjvxfp.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gqoilnhp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oddkkcyw.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vbzajkbo.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3cymtsqsi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3aplrwgaa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3qgtplfbw.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3nbvnjbha.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3slwpxfsl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fdmprkoz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3tbmsaptf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3puvxevie.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxxnsrk.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hnsvmqao.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mdspkzgh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3epokaqht.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3dxfizgsq.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yfnjfgdr.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3knnywopj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3bkfocsrc.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksnrfczc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hkeeaekj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3eoekexgv.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3orghmbxw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3cvncwnvw.html


<!-- 参考信息 -->