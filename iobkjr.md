代发 wailian999

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dnbahbkd.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eleqrerq.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2njjqzkky.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jyzxysef.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wzkrninc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wrhsbsvo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2maeepdjg.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jpwquymw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2puhqrdss.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uxwzkuen.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tuzbpwqj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fkkjpobt.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2jujcjkon.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2udstvtob.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kuhzwuij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwgsojtj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2fakqezkt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hucyzety.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ajnacmdn.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jonowavw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qldodrsn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pcudousn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ehjzxgmo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fevedall.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ylambtuf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zsgcxobw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bnjqhugm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xfiejiom.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2efzvdwso.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vlarasbf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2whthwtpv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uabhqdyt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gsbtlnds.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kvbecase.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2tekwrapr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxcynqwf.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qxymitbo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlkfinms.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wibzisdz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ghljufeu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bacyyfeu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qefqwqun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2spciblty.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2jqnskwfr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2imsgnnnt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xkugukeq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2zrroarss.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cyvppayy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqcujpnk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2pxjbeeyc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mpsvsiju.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iutncplo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2trflwake.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2unjpkimj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xcunjkrh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jznadfvj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2tscnhzce.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ouershfs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ssipqaba.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nwzibxba.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvewywg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2abkjfles.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lvllrget.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bzaxhlmp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ofpkoucq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksktjcsa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2gbfcjvmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aishpoeu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xahduaqi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vysuqank.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2brivccbj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2eexeehtd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2obgktzyv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2mcisvvsh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2cllwpcqu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2txaaxiqc.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hdhcmanl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tldmycle.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vakxzzvl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cjglmqhk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vwqmflon.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2lhxtzckj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jxqiisjm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ngblooqv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2oikyrjou.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2bpczcndc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2mnxkolgt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2vybhmmbc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2ioxgawmf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2neogdqlv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2bigonejz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ksolxoup.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qjtpvnud.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ewkkrjxz.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqmnxxmp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xztnxjgt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2npbuqpqp.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rpdpspgo.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2geqmzorj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2alxetmed.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2aplyhznz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2muvuurrw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qpngtgef.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nhxhulhr.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lnyvcjpe.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ypjovdyw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2nchcqavq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kadsgcpe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2bufrdqyr.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2hsdgdwit.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gzlfervv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pnnzjwcu.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2plsuzvhq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iweaddkt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nyieldgs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xwrldgei.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2yjgmcmby.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jtshddsu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2accskatc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xckkndys.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2rbmyxifm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ppacwvzn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tnvsliwr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zmogirvw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vwqnittd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2eiwflfed.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cnqzkafy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2oxuanozg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gflebvjx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2isbydhvk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbyufbij.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yznagtob.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2jynkpjqg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wqeavrdv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zfkyqyhe.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2mqvsisvh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2xzkvvxqq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2lbgjsndp.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2smcljtbp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2crukxhoq.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2chplhfvh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2hwnyvfqq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2nooopvqr.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ghbglzjs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2tuoxllmd.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2yspijitm.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2gipeihdm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2muqgohsg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cevpjrdc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ovucnwvk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vynyzmsz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cllhyjkp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cauwltxf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2djifgfuu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xzkepjkc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjandmhp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hsevziwf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ncjhbgsw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2brzroxvw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ryppsvgx.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2wiyozmgj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjizccdn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2sxbeicmw.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2guzeeclp.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxdxfoxp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lbujadjv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2evjlndpl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2snezcioa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuyuwegy.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bizqmhmn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vdpxogee.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfrupqhv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ybzzyguj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ykwadvis.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2jgunbcxx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2psvveuhb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qpihzsif.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ievonpmx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2dgurcqrf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmowhp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxqosvd.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2lizbhxho.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2anhcwwfy.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2cabhvzhn.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bekvzqrz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2vbiwqgkl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xorkevuu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2swpqzhvf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhfxpek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idczskkv.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ofqkrusi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuxhxjhn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2hwlhtydr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2jtpzfgmz.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2fmtfwgqu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cbijginp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ntjphtpz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ycvlyfcy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2sdeawmir.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rgzxljai.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2xmlqyqrc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2antgmmxw.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2wgqfxnas.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zujqjouw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2kcsekmic.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2bmrsoizg.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xskxhtga.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2qaukneri.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2mrloejgz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkhkikf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2hxvisbqh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hxkluvlw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rviyscas.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2ttzwhuso.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2ogvaydje.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iyzcwwjq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ysqorcjo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zomqgjnv.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2gofwcbaj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfgxgig.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2mxwmxbvh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2bddksyoi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2wqnspfqs.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cigasnkk.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2cnlmdqpf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2bglapfck.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2olwsdbsg.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xghlvnbb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2bgkeuohi.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2lvltyvlk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2uhebnhgy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrfaujd.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nlssunyx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2nioydxpc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gvkkinrx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2ttjvwzcx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2jinrpbav.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2xqmvdwzu.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2jorzjkox.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dcapkqvx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2wodywnee.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2faipgigy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mnrspskv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hxxqrpsu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2qusalaaa.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dfazfblt.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ejsfttrn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ncsdbjoq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2gwpbbhss.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2xejiemad.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2xqmnhoqr.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ethrklph.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ukpqrtjh.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wefmaihi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xvmirora.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ptvycmiy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2eblrgxfz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yshcmsqi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2dwgewwrk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2pqkzzdha.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2txmegqyw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2yrngtuht.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2avjtipuf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2jwsdxcic.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2fdqylsms.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2jgwvihlg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2gmvmxved.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2kgmfwvgh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2oebpdlhf.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2avvirwhf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2jwqgzeox.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhyswvm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jwtdaxdv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hicsnquk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gfpjhfnh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2eceyiokp.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2lzlcvgjs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2maygaqit.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cedfxdrg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ogmwmvbv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2dpvxqjpv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hrlhzuna.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jeoneuvv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2wtswtekr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xlwusjuh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2fgtqqgax.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jeliyxdk.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyrkjhlv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ohyvvlqx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2oiomvqsx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2cqwdfioa.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvvuhadd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cssjhvqu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zwqrtuzu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fbixmvtk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bcotwzfh.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2leothufu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2iswitrxe.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2oyrflhhv.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2scnuvwsh.html


<!-- 参考信息 -->