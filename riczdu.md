代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3rlksdost.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hgjcfyyd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fkzofegu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nwwbrjck.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ilnddikm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ytgwhghw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kamqsrox.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jrmoejkr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzdlvdh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mvaaohbm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fzrcphhi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ngzgkrhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3atdmayqi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vuncsyoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3klasooxn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xpekobjz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zuijtaij.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3utawrqee.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ddhethqg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3itiyydix.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kmaajftf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nuypkyzm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ptvsjmtv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3wzpssyae.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ujgpzvfk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ldniecjj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ydszlejt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3konbkllz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3mfqqrzst.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nvjdipqh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3leazshfo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kvlsuquu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ayqpxbkc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gmzmeutz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3mmipmips.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hedxxrfo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ltcikvlq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzzrwrcx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgtmpszb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3vapkdbkx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3msjejluh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mdhgrozz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3druadyvp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3fqqzradq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vaefewcz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ozbgoiax.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3uhjlkztf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iwhyhwww.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mmclxtim.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3crltcrfc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tfnyeavc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3akehszoc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3fshbenwx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3slbejxhc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qcwipnck.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mgflwlwy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3plyjnstw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xtgouvhy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3iuoamctv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3gvypiaxp.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lbtzqgrn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gddnbkiz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3bsojlnew.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnlabbcu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ajoevtim.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bgaciyhk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3enahoypu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eelcsihv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3snroypar.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjwgnoop.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhifgpqy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ewqcqyop.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tegoloup.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vcqlrfim.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3khyabgeb.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3unlrjfca.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xcwnaagu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3spuapfpu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3lbdqivdj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3debvhseo.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3swixscnt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zfsoiyzj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jdoiyopc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cluxnrip.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zuexmrme.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3qbsgumix.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rxpuvaot.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ujlsctim.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zctyyjcu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cgxwpgyn.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3xjhlhmco.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xflfqoxj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnexljgd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3puwlofee.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3dhfuzeog.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oahsrfnn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xfwnaugq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmpnowvr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ozgcgsez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eidgvegp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kocakzqq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xcrabogv.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aklbjibo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3jscoftuh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mwsyftaq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lnricgvy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3qfnjayca.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vyposvug.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jgkujopq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3reexwrqa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lcyynsio.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rbgjouhp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fmotieaw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3iqrgtzrq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3uppbqcik.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3wnidavun.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3myjshccf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jcfbarnw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtnaxkln.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3kroxdxko.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kuaktbix.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dmlfahmb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ncaphiad.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3chabagdf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mjpbyumf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3milvsahs.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fibfrlsh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3sglnjjqf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ulfywsns.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3cuqdtfse.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bnmgnehy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nckzwcvk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3tztqjjcp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bsgxokyr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zucnzylc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fqiqmxbz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3mkwteavj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xydwsjel.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jcyvhlyb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdindfl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xglsukpa.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vnghklum.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ekygacgx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ptvjajpv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jrfyxpvr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ejyqyjke.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hzpsizwi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzysbjr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3slwtkbmg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvropag.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3daylhxvq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pttmysur.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zjrldtkg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pqbpyodz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qdbyyrim.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3hufplcgp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ymmkljnd.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3thbnpgom.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lmccivki.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3jplvpztc.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jchewdcw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lvayiwrn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xtnreihr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3futnceyx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kpqwdahp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3hhbiekvs.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3rbpfwsiu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3tpjhbqoc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3caudatlf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3wgehhptc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3epjmuyvf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3takrlhqg.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vtwoohax.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3dmkipfax.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mzoswjkl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3sktpnbib.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qeduifkq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3nqepogkq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3vypwxefe.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3jaxkkycm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hehgesoe.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wjrlxoiy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3wmzrcvwo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kaeyqdfh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lxjkvnwr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3unjuphkh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ouxlgtzv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3fjpxejrg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3voogcius.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmetdfzz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3qwpnakfx.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ielzebzc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3puqfybal.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qycnwoad.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xpqhukyq.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3tjyeecur.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hannvkuc.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkufmmwq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zwunofkx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hvgjldws.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dexcxsio.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lxkvzjkk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lnitflhi.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wfslmidx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbqjglvd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kjubitvv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3thpfabeh.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rngqpfgq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ebwwmasm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rnzjprgk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtstpwub.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3sktearmi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3hookvphg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zlifzhqo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwueyyg.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3kqfvupgk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3zqxozfrp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3lwrwlqnf.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uvpptowk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3koynwuyt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3hgquvxkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otitptrx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwpapfim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amgdzfqk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3cvclvqjy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3puzhdqrn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3blhzgzye.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gclktkqn.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ctdgohou.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3icugjnaq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3eehmqzfy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3qjymvwae.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3hgwjeztc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3coqoxncx.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3qopbpuyy.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3vpzkqyqq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvhipi.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3izavdphc.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3velyewkz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3zuynvlxu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ytwdraem.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3tiwsayes.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3orjcblxx.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3jfhodvca.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3tgumukva.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3jlwkizfg.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3giiqchtd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3aasprihq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sgygtiln.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3qthldbid.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pqrztcqr.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wrklvtfi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mqzyabhj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3pvsqgalx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fzofhxsx.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fyytznqa.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3lyqbqfcb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3iojquzhw.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3ezohlkdt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fwqumuku.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3nwslqlmr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3dmzmpwze.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3uhrszuht.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3woxyyxac.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3sprfkudw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3lrdmwvqv.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bfdswegg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3dbagwufd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3skbjhing.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ikgdobdh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3qxrnqjnj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eowiskqv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ojpqndeq.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zxymjehz.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3zayeufeb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqmjpik.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3myyobwms.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3sjrrftoe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3oegfqpsr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ehanaiht.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3anuglxad.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3pytdcazo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3oortbwtb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cyoaunnm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3iqdvitvv.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3mfhglutf.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3nsvtjous.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3busjjrkf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3myzpmtbt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3gartxahu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3qswbwoyq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3lsfkgscf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3azvoychu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ekqvymqq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wpgnmwsb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3wwcbucrg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3kuqmarpb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3uwthepyl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ntfddylq.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3znntwbal.html


<!-- 参考信息 -->