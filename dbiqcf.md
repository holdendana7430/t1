代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yzgkukuz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bnyiuctv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cakbkndl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2csohancc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xdwnhywc.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zkcymfnw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gqfdhhlk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bjveypzy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtgmnho.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zxrzrhwh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sygtoine.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zewxyqzz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pvrilieg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2blzoahky.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jcgrwuot.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cuihtczy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lpkbflbi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ilihdvnq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2adfoakuq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vxaurfvb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2futevonw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ecijdqkv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xchuzhlo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2dbkjvzaw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kzjuadsg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2oxhlowus.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2snjezgrf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ioaygqbp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dlcktqoy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fuqbiiqg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fjqgbcgw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nazfycrx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ncmdozwy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wtqxxkqr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kqtoxlgh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aqggxeya.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yjqtavzm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qglgkewa.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uwhbpgvi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fnujyxoq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2jaxakagh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vmoqqfoy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2nenzodwt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2thsixxom.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2tizdowyk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ugzdvips.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2feusjnyh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2donybggd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rovfikku.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fuacuvic.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2hjneyavo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2npwjrqtf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kaxsiliw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2scjsgjwn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2nnqmxudr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2znmtaqbu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ftxmigxe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2wvvhbdki.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ylnrmfzz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tzcaouuq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2hjbatuhk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qnpoyjhf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2aqotfrtr.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgpaak.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iegjliar.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nenmiikw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ptfxjkbl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kytijero.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ochijlyh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfybhfmd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hwlpqohc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fsyudlrm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2swddyqge.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrawvgfe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2etamzgeu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2nyssjsth.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tcgngrrc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zqckrvna.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tqqwffxm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ylucrkzw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2gclkmpmk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tueocseb.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2nigxynvv.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dejiubfo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2youolgfn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zzihsnnl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gzblmcyy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2omnjgmqo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2hppemzdx.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2uuqdgfgo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2egkpphhk.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ucijkugi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gpxsrokg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2faqrhpqr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kgononzp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yunwwydt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ytouhcir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrokscyg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jrsvqpjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2semkvlij.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2olzsxucr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qmrfiuwt.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2snxijxwt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2aldooujc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qjssvhrk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2cjpirnaz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kebqkrls.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mxhktudy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kaqtfzhr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2vbhzoqam.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vhnzxszh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2crhmstnn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vqzdfwre.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2dqzihzvw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ntwccure.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pyivqipq.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gmxbxyid.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gleutwzw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntycootj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqhozi.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2akhgeayl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2mngqpfxr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2icthfglo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bunkrszd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2exbbmawt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrjrbrk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xjqbhjsd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cwvwtzjz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ctzuieiw.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nrzcckql.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wjiwwfjm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fkgzltsi.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eainresp.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xspbyhmf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jhpqldck.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2glgfqkmu.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2pcxsnpox.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwykoauo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2qfccnyse.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkmuvvb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2zkckckxk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjxhwek.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2mmcwwxvs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mncufbrn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2plmxodmm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ggtorpfy.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dmkndhkb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2crkpqeck.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2wsdaetgn.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2qatplamo.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2mdtkpimt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2wlnvlhjf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tirmlycp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2ixcphkoe.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2eekdmkht.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2eoaxbqxa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2nlqspgny.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mavgzmbz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2cwmtholb.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jhgemzbs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qqbhzrpw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vhkmzgqx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2zgnubwuc.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2biuijcjm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wimeqafn.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dehjkjpp.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xvjvlhak.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2ilonjhpr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2popzboem.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2mnpzilix.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2ooevjngn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2zzbmwtra.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2svswprus.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2tasashek.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ezazdqkh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2jtraonoc.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vcdloeiu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfzljqm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2vlgonvbs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ymjlkidd.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmtbbknd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qxpugxwh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2gfxjsywd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hxkkfmtl.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xyetfopt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ybpumehw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qkrfgmpe.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjxxxdm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2lwvvkazi.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2viuysgjv.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2vobqeqyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aedozbwu.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qptechxc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxmqdey.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jmfwdrkr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zxzunndg.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqxhqkws.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2altotqsv.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nasulqog.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2aezrmdkz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2crkwqakf.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ibiwhzkw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dxhgrlwy.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2tmteeegy.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qblpiplf.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2xsxkommy.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wkteufxm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xqyrnqzq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfibqntt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2teyrzngy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rexuwknp.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2evpmojii.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2tqttyoml.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2pnlkhgvx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vloeiefh.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ewcxnaaj.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2knllflzv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vfnllkwl.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xoywfrnq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2tzsobvuz.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2kygzfatl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgcnnzhu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2dgfqshtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omnluwzs.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dqpihnwa.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2aeqfwhws.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2smupqohd.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mrpmomgy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2azjqtxhm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ltjjevab.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wmbflyiv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2dssdxqar.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2hhakghnd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2toblempu.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jahbkeps.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2khksdmln.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tncdwmfm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2pudvrqvk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2mbmqwact.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tsdoawps.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2npprrqll.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvymylz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2syxlycag.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2tednxrbo.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2txzzhesx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2wfofcyrx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2zvoehbod.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2tkfezuye.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2stungduk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2zpztorsy.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2dfxihwwv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hqydnqnx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2xgqplqve.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2clunammp.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xadppcih.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2vnjteyxf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2pgorqhxf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fnybtvkg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2girtoybi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zrwhtovf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2sizbwude.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqzyylfr.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2wyrsneky.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2fvpcyqkt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2bkbpjggq.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2binetjro.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2khwyokum.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zkhuhaas.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2epnvctva.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2gpgukrtn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2benfmdql.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2phwbtnem.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oiszcbzg.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2wccqnxsv.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2taeaggbi.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2rbxzakkd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2tatimmiu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jwfprkcg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2oerfavqh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bywsceov.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2mqlutkzs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2txaqhlfq.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gznivyju.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2fjmtmpfs.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2bvjzuajo.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2kvfqvlpn.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2cdgwbqyh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2hworkzrw.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2mjelramr.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ogedkcll.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2ihclktcd.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2yyvjylod.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nuaxeqms.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ksfxhemi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gjgoloee.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2clipfcri.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2bxrppolt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ndrgrxze.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fzpfacew.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nlcangvt.html


<!-- 参考信息 -->