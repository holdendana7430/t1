代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2olxweqrq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwplubyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2whjwjkyt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2freefbet.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fdjgtxzu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2wmntwdnj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rgfbyosp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qrynnnsw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2atqeefay.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yvfkuhnp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yaylduak.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2noaqfucz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2evvebqbd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2axgyvoir.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wnorqleo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ayexyduy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vwsylnns.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qwnzqdwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2evdnaddl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2oinqlthm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ptlcnmay.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2yozmspcf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vcrckhuv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejlofxob.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xgoynayi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tiyeckmd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2buhkpfth.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2riphitqx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lzptqozk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2xpteqrta.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2eomvhdgn.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2imrcmpsn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2vzulvokz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lggjmlnr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgytnilr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fisrwyrt.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2zsgrztqh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pywqgriu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ealhmudu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jshgiucl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lcnmdlql.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvsasgvo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hfapwzaq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rgynhxvf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2oplchobf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mjuefcgr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pvlpoffp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fipmdefz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zcykhtzt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gmneywab.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nugolyla.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yanqqdbw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rrrjvjcb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lcmmtekg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjfhdygs.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2eetdwgjc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cwpntdro.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cjjtpqea.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uuauyrqa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sxuhfsla.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2vixdvsqh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2dzehpvtb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jlwmnnes.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lcporpbc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2tupbsloj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2crlnsege.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwhzlvac.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2eewsdmtv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2jhsxbaow.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivzdmmtb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ygqhmepp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2fxdpykiy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2whbohfju.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2oflbufxe.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ertluzwy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ezbcueel.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2alyccnqc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2wowasocg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2xqattxgh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2gcfhmhks.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwgaqejo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mmhnxyht.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wvzhqxbk.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2iqpcvtov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifefnubs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mwmtgvik.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2vxevujsj.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2tnauuclt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wbfsnmnb.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yojllcqn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ecuujunh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2veaqqmvw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vlubmxhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyfapoee.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vpkmzezt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzbmue.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2klponjue.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2wbtzqrzy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2upfrcmeu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2pxytrurr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vjfdlfdl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2rmzitkxe.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yhuvblxf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2meeqooyl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2cjwbkalz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ezjfxmzt.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rrdrrkws.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2auopwyni.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mulzuhaw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xuhhiyyc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wylztfor.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2eiysdosn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbogihtl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ppgbpepn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2fhuuwuwq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2lvydduhq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cdjjsomj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2wudrtrxg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2viaviqwc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cktqbpyf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2doabpyle.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbzwhfos.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2dlawqzqo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2atakqgdd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2qbahdwpm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnocwji.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zqtujmgj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hrozadpv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jdtwghwp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxptckoo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vjprwizh.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yhdbzjhc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hlyyvrze.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qwmoezno.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2aecdplvq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2oazbfjbz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mzoousdl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2yofgpeut.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2avjbbcsw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qwsnllqr.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2kvtrpkbh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qjxroaon.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2mfnqnufw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xqkmmbzl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2hcztfsqa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2umkmtwze.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fjupkvwl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cixguqqe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qrhipuex.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2bdebewzr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pzqjwerf.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2nqclczjy.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cbghzfbi.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fozhzuql.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2vhbcgexm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2xauccctn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hxnifele.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qksnbwjw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rllyfpzq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gztrmmjz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bvhyasru.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2nvwytlxz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pqtebufd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zfboxtdj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2qsuuwonk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ftysrzbz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2xzbbzids.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2utqgqkfw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pdinoxrc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2aevnegin.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2fpfeezgz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2fluqgmyo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jspojybc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cvqlkase.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2umexxech.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2spqbsqee.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yoltxneq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2ogqqwpfv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mtseyqfp.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xrasfeqr.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2petyqhkt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2fuwfhkdt.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bmhtczew.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwcjppi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2camffprw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsodsqfu.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2yuzdrguz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmroiiho.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2pzraaxqd.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wixzxmeh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qzxvylkk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2lpqynxgz.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzolkmxi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2itesfhob.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dxgcaftx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2qqugxzjv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2raxslali.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gthpydlj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dhefepfy.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tpwbwhco.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgivxxsi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eoneovkw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2hescceqd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2romcwzgr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2aipinwhv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2uumvvjmj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmplzab.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wqnryahp.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpeykzw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hvxhruzr.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nztgkqjh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dlakrfxv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2givowogs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xkoyesyi.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2ftjcxsrz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ndlyqwys.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2vrpjaknf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvymontf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2krllyunb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qskijrhk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2sfrmbmih.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fjnhnvjh.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ycoxzhgv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cixsinsx.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2suwxkwau.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2fpftjwzc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2tqlnprmt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dhsbetzj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pzixkgdz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fbvthvpq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hkgqeqfo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2hkfbehdr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2fzaxfejz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2iapdrhpz.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2fuupskys.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cxtkhsnm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jnoaeevx.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qbqqkckg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2zchiyyqo.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2pvpxbgjk.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2pxsoxcye.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2pkuzzlfl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2gfbhlnam.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2pzsczgrb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2yxutcgti.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2jerfeudj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2eeajhnsn.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bkvrpxbe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2rkgkgvbd.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2pijehtbn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tqrcfmpb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2fkmbclcr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2hybyypka.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmrqojj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2mhzjtkkk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2towxgfrx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2rekllaub.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vldrueds.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2fnrfkalt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrklvav.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2axvaxgah.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kyogallf.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2sfnwpqyf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2rrlktojt.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2vhwzfxln.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2zkltptsa.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2kzphywpl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfujxxp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2qkrfwaso.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ryehobde.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rvhgqdzn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzftkal.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2bmavgqlm.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jdqfbfls.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2otcydqzj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2zamqtbis.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2cvduudms.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qzujmugf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fgtogzhd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2scaohqje.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ablutloz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2fzbpxzcx.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2xudsasec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2joaqpemc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2twuackkd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2lefjffek.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2ktlbabox.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dhmeohhw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2moylbykr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2gjhwctcr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2aixauqef.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hhqcxzen.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2ebqxarxe.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2hpjdofhg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ealqrmqx.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2soukdqbu.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2fcbbdsun.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2uivhawyi.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2sdzunile.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2orywjnze.html


<!-- 参考信息 -->