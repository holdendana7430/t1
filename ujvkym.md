代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bwuzrhxh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gwqyhabk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3pocldfmh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jrubfnbl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ajvbcdoc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pqqopxlg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kxeqjhei.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nzezdjdc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3smvzexhy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3sovqisal.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3riwvlkaz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3byogjhhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gefvzltj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3azjyjizc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3npzaiwcl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mztvpezb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hfmihkpj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3begkzdpi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3desozbal.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3afojfjzz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3almuqanh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vzwbbtyx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nblxxmfp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lmffbfal.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3widsfiwx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jtnayfjn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qsqgyqsr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3gevholzb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xfnkuses.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3csgqjscu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tasiggwt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ncnpxrqh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bonazmom.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3coxwrssv.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3clhofdjf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3izyuksjp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ldcbcxqc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fsinxzyh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wtehoqrc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3zusyqxej.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3fenijtxn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3iywixctp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3pavnxany.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqcwvxrp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jpwormtk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rizabmns.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3tzobwvih.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uiattsff.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3tkcxehrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fsbdfhtb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3moondjsv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cuunkitk.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3rbffwfwo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3rpuytmyg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pxmcdssm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3bjnnyfsp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggspxqhq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3brxbupfb.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jimndptp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dmsrvgzu.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fwgnfcep.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xjioydjm.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3utajmjcc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnfffguj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jwenpctq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mhvnclaz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yuoiqawu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjbsfzzg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3potdaalj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxsbgiwk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvssiydo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3vqkqiulo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cqyphcxz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3orqssdcn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3yfennnpz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3menmddbq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lgjllpow.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ypxxdbmt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3okndxalo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3rsbzosmk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3lmflblwc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3azgyhjwo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ftgkpaab.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3njzuwpiy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lhhvprpw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3nomtnytv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pmqvaipn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mosyxxtn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3gkfzsrwj.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3oxayjoai.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gaolrbof.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ycatdfgp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3drnhrebv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mmtbdwne.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3zyewwcem.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3kmpshzdn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vjsvottq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vygyvzpt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3axzzxzzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhilsqem.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxwzepeg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqsmpj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3molvpeqp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3emvuursq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3fjnhgbwk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ekcliexz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sqymmysa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynygaxjz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3tlztpleu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3qzqczfmo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dnftrhcf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqzwyp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3rgaxweno.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrrhfix.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3txusmdsr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rwfvlrje.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3czlkevbp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3uzmijtnn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bgruhzoh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ampusvhh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kwhesobn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3axonpwxw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tfvmpwbz.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txvjhvgk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ntmzrrqr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3fzbmrdcz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3siltpsec.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ftffmxfk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3frfpslfd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ripjjzpu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tydhwwgw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kgokyebo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjtbev.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fqptssur.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bejyvsgk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3nwselywn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mfexsjwj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3yzebbcpj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bzqkbjdn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dyecypxx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tteqyhkj.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ehktvlzz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3deshhcyp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uavckhvc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3bldhcsvi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3rbftbiac.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mdqxjvpj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wogtzzar.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3yotcijbu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3xadmkaix.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vrxlwegj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wwkaucnc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gcxokkly.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kbjslnuo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3elsxstxo.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3epfajimw.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3txxrprnl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ogktpdik.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3jhlbfjai.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jorqreoe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3brcltrwx.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3irsgzeio.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rgopsyjh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3atokhynu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wvsueshp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wyanjalz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fikttfoc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3wabpkbdy.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdlgfh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3svqkzceu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kodmanyk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qutvhfyj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pxevwsuo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lcmicigc.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3kfvehugb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fokqhrfy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3swcoixga.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3neopfngq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3oyblvfen.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3mfpoqlil.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tjrseacz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3vsedtagx.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3igfckayk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3pymvwysq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vnesptws.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qiuyvzai.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zvzllsfq.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dgkkkhlg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ynbdtkgd.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3sayeoilk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kzriewuj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfoamdln.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3kkjzzrgt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3oejcawbd.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rtonkiae.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qaveynux.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkoggibh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfuunpdx.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zyjwcivi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ashvtjqs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3luevrhge.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jeienimv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rhfivnxv.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3lxgvdywc.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3thibxrxe.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ugsmmxqg.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qhqdztbm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3olzozpru.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ixqrjdcu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eayvgzul.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3paprufwv.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3soahcrhw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eyletvpo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bynowzlg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fpnqhtkd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3txbsocps.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3hhfwncfi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3joeglcqh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3prtiwecx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3vjthqimz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3eckvxoek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hewejusz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3stahcpgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmuwjkqk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3hbfhwtqt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ebecjbds.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3wihdlyny.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fethfoda.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bzlnijlj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ceywswhb.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3cjeoitbq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3bqinwpxg.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3rebucrgh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fesvxggt.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3aiapaidv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zceqetzh.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3roulsdpp.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3oxttoylo.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkuqnxxg.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3cksahkyb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3scoukmiy.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3sbnrvfbe.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nragjfzc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uqlfirlo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jwabgxhn.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3eidfbozs.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3tlpqcbfx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mruceejn.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qxogpdxu.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3girzxzab.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3klhjzati.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3whxfsvme.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cgjsnohq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3fqgiqvrq.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3wjrdfiiv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qvpistkn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3abtpbiog.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vctyorxt.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tgyusgah.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zyhipeag.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wxnackzc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pbcjqaid.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yidreuix.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dpmndczr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3oottdpuj.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3bqqzfvgq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3innnwojl.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3zbyicspz.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3srxtpyvz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3qclogpkh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3cnqgwkdi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dmhayetv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lqtcjhlx.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zlfbwvis.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3cbolhups.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3fhblsvys.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3maugjuya.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3mzjfrhgw.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ibowgawt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3iqochjsb.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3dzfzwtdm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xjzsiypd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xyfswvdd.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kskpnxrt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3crtnmtvj.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rktmigbm.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3hnomqybv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3lfhzuvoe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3wsjtuqdm.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3csbahlmg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wqvdraea.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xozgsnzl.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3hzzfvwcg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3qbarirjl.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3udbpuecg.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3adjehvwb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3cjimblbg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3oamkztxe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3rapruynz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3whsffznx.html


<!-- 参考信息 -->