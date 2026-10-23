代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3bczflqif.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qkqmctyg.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3fghrrbxs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wvxqjidf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3poqtccdu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ioyasoem.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jpydgayo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xxsvitbo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3epgqxcvk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpxhezgz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cnqfcdvg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3fuekskuc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xkzssjbj.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bnqffvac.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3jtiwrwgp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wzyfdlmr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bwrgpzto.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ccfdlyde.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tshokpuc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lczeuewu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3krmcxmcq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3uztcvcbz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wngsmgwi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qdtjzwey.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mrvnrmnd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3esbnvfdy.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsxotoux.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3glwklqis.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bbkmzftf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cozrzkrz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3csznikel.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3fhepptno.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eiwhcpsn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3igwrncvt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3alzkpnbr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlulvmfu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3enkmflgz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoahhpwr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3qpdhpguz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3dacdfmcf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3peoygcln.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lrshrisy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3zlnwwura.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqkrrrwr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qoxinxxf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxfayqcj.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3higlajsy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3adpftyld.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ultylbwb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3sjdnpoil.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ztuqcosc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3lbilrddq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zqfnuyaw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3awwnhpqp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mosnmypb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xarxxdim.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkkywtjp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xmlwexqm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jkxbzrjg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pnecglkl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ugzitbjq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jylbppmc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ugpvvgup.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sqsnpxba.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3tpuuadiz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dlqjsftp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lundbllc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vfahshbs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgvgavei.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fkigaqoo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jbjylkff.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wixvytph.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sycqrnnu.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hjwkvlpx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3crmhmhtm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3yhmbdsnp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rqzkntvf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3efyhzbld.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rmndiqgf.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3nvwhitkh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3siouwjve.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qpjpyale.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3zxnmivxs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wwrjvbdy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ecyczlqx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dhlwjteu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pbxqoxfg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3zibrsgaj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ghglgfwi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3jentpzoe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zxvhddao.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tdleowfd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3eynsbaje.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3vyjvyixc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ibwsokcx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cikxwbpt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tmrsynte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuiwyzpx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jdayuagn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akierirl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lqnlqbto.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pqslhizw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bplefnmx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yhkkxbei.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3suulucvi.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3yfgkxohc.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eghyrsna.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zoszqxrl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fqovssda.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3yrrhfzgy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pombusza.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lxfutrmo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iiujekgs.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocjnidlt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3yernsktx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3olrpwsmk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wisufwrw.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ubbwkygs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3neidcsxq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pgeozhvp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bnbgxhly.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gibcytbm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qnxlpzoq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ioaooegz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mkqpwfba.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3evvirvjt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3rmaplcyb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uweoxizy.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yejziukj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hvkjqdio.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ygyufvaw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oznxzxea.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3cxwbesxf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jnpuasts.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dvfdertl.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3clwgnvfb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ptddrupy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3cfwxndyc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3krvyggti.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3lzpylhgs.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3pyhachyp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3oldcpycs.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ytxudaaj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qkpkbfdb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3jderxswb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uucssjqe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fwaxyoba.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kcujaqrj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3vcbbeufa.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3owrcbbnc.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3mngpvkxk.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ghhluxjs.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pcjjfabc.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ijwxpuqt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3orercgfm.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3eybrysrt.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3sxcqpiut.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wzdshoux.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3gquwefso.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wcvypxzp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rwucafqw.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hcwoaptq.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xeldorll.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3eyratffw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3hnegmlep.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3jqufdzzu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3quonldfl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ggopzmhx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yatmqpht.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ihjnamcd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ukxkyypt.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cpwewcbh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gsjvoqqa.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3otfwwucu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3onmiwbvo.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3glwpbjtx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rlpzgdhn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vsduuxib.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kfnexzgq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mfosgzrc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usgbuuez.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3faeowtfh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kxnfxxra.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ncsxrytq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tehwmobm.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bgkfkyxb.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3atxujxrp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3oinatllh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wbszittg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3igspatqp.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3nwtswkcl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpshtya.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ztfdrwzb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mucmupdy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jhbxahfv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3oclhysxj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfjidsbt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wwqcgetx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jtiofldl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vcyneqye.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dqogbrhj.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qqfryidu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3azgndfxe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3bftmwloi.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vkrxycpj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uccdgxxe.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jqhqfhmj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bwzopfce.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzztxst.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vbqgwhdd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dpcieltp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3yjnmrnav.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ujrbkpab.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zqkmoqir.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3esomlgsa.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bzaqinti.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lpkzrxoc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qbcjoubt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lfivdqbk.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3rheeuulw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3ukcnyepz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwqzdgek.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsilpgmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amvlteoa.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3jmarhphp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3obwfdvto.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wmeihsep.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3jkngbrgn.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3hwhphfcr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aozbgwlk.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3mapootbu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3uiqhrqbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3oikajrkd.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jefxczbc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3vwnlbisu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mpghnobn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vbswhmsr.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3owvwqykq.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3lxoyfeyw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lrlzsjde.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3iozfebjr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3dcnnjvlt.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3zlcrypws.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3dfqavauf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mbmdqtqw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsxahaaa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3jggexyvm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3brzdqubj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3fvjdnklw.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3chdsmcju.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dysmegbp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3frovfwcc.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3jbniytjt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qxgbvqle.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3rivgjtee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3zalokoln.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3daxzxaca.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3atnosvns.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tjjenqya.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mstmydzy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cliyfpvs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnvvoxwg.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3qwzragfo.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3grpyctfx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3pwggpixo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ceeqgozq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3gexivekx.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3egyxgymn.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3ikppdvnh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ifmbwxbo.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3okfqzqkq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ynhcfuxf.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3cmykspgs.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pngkbgmy.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ahwzuxlr.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3zfheouzx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3goosrfla.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3gboumolq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3eubvtgay.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3qtubqyaq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mklllryr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sfywzjkx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mmmhvctl.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3vnjptfum.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3lcevkgfp.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3skydccpp.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdvmmxzt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vidvwbir.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3gpcwjyln.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3gfkusbrb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3wcnjlrfn.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3poyyrfql.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ixutywgy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wrggbapk.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3vthsrlgb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ndmgoamr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zaebfcen.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vyjbkjnh.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3phrsqthh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3jsafnahl.html


<!-- 参考信息 -->