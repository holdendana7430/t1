代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3kqitrafs.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3plpylbwx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3sdenirwh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3zfydwrbf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rvngoupx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qhqgumsq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tgacpiar.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hhfmmsdk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3piiesdnf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3uzqfrfgv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fxmpljid.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3nlnrmoqy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3rhkokuvv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3uqotscjg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wishzhce.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dypgtrah.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3zdvkyuza.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3odnnafwe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wdntryxg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3qzphrpgw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3yzqszqjk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgcqvroq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ommjbwdn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3bkkaibro.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3epgwqqua.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3sxqcnbmi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wbbjuvpe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3snzrymeh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3jkaojfhu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npbghvzx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etyobpip.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hxikkjcf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3eepjoiys.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nfurhqxt.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vbegzsnp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3iyqeyees.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3wabeaobb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jefzrlyr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ghdlesdt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dkauuesp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gzcmyctz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3opagscxj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zcncslvc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lzresszi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nxxgdyvw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yiqvluuw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3kpdrotvc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mmsddqay.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3sfaiveqo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jwaawkbk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ecfooxue.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ihnjlajq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wgnctnzb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3edloutda.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3iicepezc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yayjanpk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mhzkgzgv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3dcnfximz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dhtpasne.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ftdbwnqy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdjxauoj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3kdzchnlw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rzrkfzlc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cjdrxgtp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wnspjuxq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qjvbltmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3umdurcwo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nzwhkqhg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3izrwktvc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3qsqrwiho.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3yqeuqdpn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ymmyovug.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vwnxdjju.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xvvyzkwv.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3bvkumidt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3umvjoxvf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ovhbzysv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vnyrajlv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qejzmkhq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ifiptvbw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmhhejv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wuboewtm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3kmmxsioh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hptwuqlo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3alatltle.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3aiprkvpd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fwkwxaby.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3brjcyygy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iwnqcgjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdhfflzp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nvctfvta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohskgmdh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ryctsxes.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iheovalb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfbqomvu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vpsowfld.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zfcutphh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zjligjzy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3chzsqxms.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qrrjzrsa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3douqtkbx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fwxzlxdp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lxhtyetl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3plnmuiem.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jdffwfny.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3olvjtghw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yvgmqeim.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxrvujj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xyzrxizi.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3amputtie.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lyjxekea.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ivzcjzar.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3psjviomx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3efkvbxca.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dhptpnue.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohvkzhlb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ifoqviyg.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zbcykncw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mwbzykcr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mngbbhyi.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3aihtpmlj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nboxmobr.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bkwqrjjv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uhwzmhuj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3lluxjmhs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vxaqiicd.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3quhbmmjz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3kawzvpwe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3pgsqugrw.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3iunvnlvw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tdxsytbo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3nrfshjrr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iimaeyps.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tccaklug.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3cetjvppu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzepisak.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uxrgyxtt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jqzehzqq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gykrmepm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vijpjfjo.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3sdwbcklc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ppudunwe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3pgdkdfui.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ptczwfao.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kzyznmzo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zuoqegol.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3heklrrdf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3epjpzrtc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zasyxvyu.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kaimheph.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3arxgfhvb.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3bylhejmo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3msyrwdeq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxeuhqwj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3xfgkhmzg.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xnboxuoz.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vjnyfpsc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3afxekqsj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ypjxepnx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xirfzxiu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rjvudqdn.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3axcqjdhu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3antynzav.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3aadumaty.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3chuiexyy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3utoxduac.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lmdbcuwn.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ypyjuifp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ookksryr.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ojdyvoxt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mhnezbyt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hkebuhak.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dmzqpjzv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3wlhnoddz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3iwgiqhcs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qupuunlx.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3temzobzy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3sgivfmni.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fudfimal.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3tchpplns.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3vuftvqab.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlwqzmja.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3uwnmaber.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbhbmdo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3tkjocxqt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3agozxest.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hxohugrl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jjajfnfk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ogbbgmpd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fzhnythk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bdjvohjx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3qpdwgtlp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3nasaqhla.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oeassgaz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tytnljbv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3egwscwfu.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixlocsiy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tfpjndjy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3fmilchya.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3eavyqvhy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fedyljtx.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vddbilzy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zsgitzmb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3kilqdhuk.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xgadqcnp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fryamjox.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qoldubuf.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3luqwitug.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3rljtpxur.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sjtwbdwo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vnrcfzub.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3xzhzying.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3qwwtvuay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuwdiuof.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3gdovccia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkalidnc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ssjhwvcy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3jajnzpdt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pcdrhzii.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3guhlijle.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3oxphtjie.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3ogfrczen.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ybfxsnjg.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3avynybuf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3coimlijr.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aeovxzba.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vebiqjfg.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3tfrglywg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3obxnldez.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hzcxozux.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3mvppfrlf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zbevaqpe.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3acjceudn.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3pnwopjxy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nbiadxjn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ojcqrzbs.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3drfgtudz.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nlyceaun.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xfmehoft.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3flnujijp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3aapigxfw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3kytlltqp.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3tbxaunok.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3helgilye.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3kmqxewmo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3esitptvo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cocqoewt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3fmoeaeym.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3erlcaawh.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lfuwyltm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hnstngyd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3awgrtihh.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3rpqgczvs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gebsfaot.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3wadptzrm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwyypyh.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3wmbpjtls.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3lxmsnuzt.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vtdujllt.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vgkogzmk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3nktckiyg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3vqqdarex.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3grtxyene.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3elpwgrkn.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qonxndge.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3oihwzeoh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bdrbphdv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3iqgkbssv.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3ruyfsant.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3kgrsvshi.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xkougvsd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3huqlsjho.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wumyvbax.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3vjlrhuhh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3jmiuezte.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jnifojle.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3oupdelmz.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqlzwq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3rnbzsmev.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ficobdtt.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3illkrzoo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3zolhudyt.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3skjpcxnm.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bdgpizyq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ihtkkzlf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bfblgmdh.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rhlndkbs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qmxlawbl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3exqifdle.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qvlgrqsd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3algkyiar.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3thxeepqk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3tprebext.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3jjumyaax.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ellriuci.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqtfpa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3nlhlxnkd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nyjroxkx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3defgtrcn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mewspqgr.html


<!-- 参考信息 -->