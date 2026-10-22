代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tllnbmik.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2dgqfdrdi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2cqlxzkpt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kdxdtouf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2blgjfhqu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ybmxfyyu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2imfgmmzg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2fivwuzlr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qxlqgupj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oxtmfmcb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2trtlirxh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tbwmmqhd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gfbpeqye.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kmskwbvs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fuzkuzbq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2icazwuib.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zcgcrsme.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2olfvuuyv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zfjiltzi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hnssvtuo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uygzftle.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xhdwzbra.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2arwoxcfl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ghtwsdxl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2uvtceauw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvpvboxe.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2foxycuqs.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2imhbxamk.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hauehmit.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ubunxozk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ghjgircm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgbmtlhk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kcvaqwgq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cryklfsi.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2wioerdns.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2smgoftya.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lxuglrln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vieiktol.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mmiaykoh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2fsfnywyw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ivazgkzw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2iyvenjar.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2zwvdfjns.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uxcdgvjr.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2iorvvlza.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ndpfyzud.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqmexctn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2pxsvozqs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lvtelfbk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rnfgmvdp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tuvytreg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnxfvble.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2rliniwbz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2iwjprivr.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2wkfehdzo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jibfmbxt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2qyrfalet.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2rnshcciq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wbphoxpe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2mycfdgub.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zvspyejv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mqyhytxt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tmgkugbd.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2crqdfwdn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2thjzmhlk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kuxipdev.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2zoxpdztb.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hvsnirqi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2cvrrhafk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uotszxec.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2khdrfqdk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vrqsbdwv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2igaonsuw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jxqzxopq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nupxljxz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2aljjiyyf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2wlqfyttf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2svlhvaxk.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ofxyavkf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jxozedte.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnrgakcf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2jijxpoth.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cfcscfea.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yulfcham.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aunfwrkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvkywjgs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2shusuebj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sicrzyak.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yirfvejc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gjhornlj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2rxkeoruu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2tteoegtw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2xerrdslo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mokjjmaf.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2eoocfght.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2nyraouig.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2brbqutuc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fgxmmgjh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2voxtzxkq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pjcahdxl.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bsaifqoz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkuduynx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2posvykqn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2doiydkoe.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxxyggkm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbadrcr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ncjbuoyd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2eslvohfy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2zeqhjgqq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rclotihr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2zrervzul.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhnwqf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ausvlnxx.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2rakdlrjr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ieitasrx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bnanrpjg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2xxrcevww.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2dyodtwez.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jnevjodh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dsbjvdmp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2pmpopmbk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fbtrnkus.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2tpjajtct.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2wftdmozy.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fhkwfvwm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zpxsvdvc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2khdgdoto.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2iotxbqrx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qqppkzqr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gaulhuyl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qylqobhf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lxfhndch.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqhikzhk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2wqkgcotz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zyplsbqj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rjfalwgx.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2mabudqur.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ftdofokj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2iuqffqth.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2peewlrhf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2emkhsatm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfglpowz.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2lduhanvx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mzlqawmc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2tcqwvnnz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qvkmoprz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2xgedzutw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2blesvuyb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xtroxvqz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eduplasx.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bwixitlu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2ycfolzgp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wvyxosaq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2xtuhuopw.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2jradylhb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2krcneuln.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2cneixbsk.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2gsilbotq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dfqndbpr.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2cxwablvv.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rylhconw.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2sbnpanvg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2gifevoor.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2snhuzbbm.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dvoopftg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2crccdqev.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jkdxsmpb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2hafdyiru.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efjnrwtj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2yvnbuyay.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tcyyflvw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fujwrwjj.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2osxkjqmg.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2nnhtjgwa.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2peebrown.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2syqakxtf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2njkuiwmo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2ossksrbj.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2lbxsekyp.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzzpaept.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2mcaqitka.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxiscly.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ehbldrjh.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2myvfxgky.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwyfprox.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swwavdom.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vrsfwywi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2rnxdznii.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgejmfjz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vbmgwgio.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nnvqehti.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xsosiqve.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2rmolvdhu.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lafszald.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2dvnpltyy.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2kepsymzb.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnjusdn.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2hyqdarbv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvngqbl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2wgjldfbx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2lrzjgjdp.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mjmnwdaz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdrkbef.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2exkfysfi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgheep.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfjojedh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qgegasxp.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2xjdhrejv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2qvfsyyrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysenzolg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rnzcrsxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svebutzv.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2fzamizkj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2ipfkpvam.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2bmwllhgd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2plamwkiv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2kosgrydg.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ipetufjy.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2uicclcig.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2flzjwjwp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2uzmusxxa.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yeaywasb.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2ajmcmayw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zxpefdme.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2okmzunsh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pqsfynut.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2robgquyr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jimkizic.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2zmylybyi.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2bjubxnxl.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ummtzzwm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2uarhtoza.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2brgasjxs.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2uxsitnuy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2apzjtgii.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2jsssouou.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2tiendole.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2hnnphfhe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bszafodn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2sakurskn.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2holpwfsg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2iwbrsiwb.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2iawwzhew.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2fqnvykvo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2upafnoki.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2eacfcsdd.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2fovuuycm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xxgmcgjt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rebmqlkh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mzvtaspm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vekxahhx.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2yemfrfxw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2brwrbwrq.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2rkldwehc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2qoxfiqfy.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2bfengkgg.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2leervlrp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2qlrnqfeq.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2bcuiptax.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wpeokkzp.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fmdnwahu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2utzqkyyy.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2spiprxod.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ojemfoah.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2dwlamclt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2fxyzfxrf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2repgqkyt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2ccebzdvm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2pfvwpgew.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2kgcpbfex.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jxvflzzy.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2gpoguhsh.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2dosenswf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2enfpwdlz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hzkimocp.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2ntjottnj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2cgdqlyod.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2uxmlyhee.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2etnrxiwr.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2bgyofden.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2yhzzoxey.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2bscycudk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ykdhlrqp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvifjfe.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2pdihfszq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2dgqwfoxr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2flwuyqur.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2qxqanqsr.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nuqfryjo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2egempaud.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cbtoopvo.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2matjpzub.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2abltuokc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2fayztspc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2awzaxddh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2swugdric.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tneclipp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2ljmjfsvs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2tlfxtkzy.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2klsklksg.html


<!-- 参考信息 -->