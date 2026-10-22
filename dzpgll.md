代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qhfczwuk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kdllkrce.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2sacgvqdu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2loeasyvg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jfdszfsr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tmnjoqrr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2dtimkkdz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2utzkripu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gffwossd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2xzcwqjlr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zcchesrj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2spekrohr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sjmraoys.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xbpztxzd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tfrviyjj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tfqvfrlv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2fjukhtec.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jetwpqmc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2kgvduybc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wlwbaclw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pxqdydqj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2mormtbnb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqyukvwv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbpzezjs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2afndhwue.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dnxuuixl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2thjcuqyb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2byxmavyg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2edpduist.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zvfvyizw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sxamvbjv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sqoppekz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2rwtjnhwi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdzdknrn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ieukeyyp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ffnwyjxw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2yfpxkqsw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2obkbxtdh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yfzlhuna.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2infgtrpc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2kuyspvud.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2texkjgwn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2cyjlglgy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ixxwojtu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2kisjafan.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lndoqbyc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2psiywjem.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gizbjtpk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mdzkxktt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2avayvibb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2atrpnzut.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iafiyhom.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qfwjwplk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pahxdrhz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mqehvwsn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uuwjhrsa.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2uupmygzg.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gxsjbjzb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2dledflnw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2whyvlssy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lvvpviuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2voomkmdp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lyefnius.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2domayfik.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lmwgwvpz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2revzgafx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bshpslqv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2skyzxjyg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ufenwpyy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ovmwerkp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2nnefbpsp.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fkeahmli.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vcftximx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2neizrblh.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hfvozdey.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2efdbqnsd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fucxuhks.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qnhawptm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2hrfiiecc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ruikciea.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qzuobsur.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lvyjrhwh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fiszylcc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eejejwuk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkwhkelh.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ygclqzhf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2atwqmngo.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cmbhnpdm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mvsnoizk.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jhzsjyze.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2custyxpn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2oiiqulkz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2umxsnybd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xewxpqwg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dmfkxjpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkhowbiz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2emsailwt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2entmtgeh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlxyyp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2odclrpks.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ggvyntna.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2owxwvxex.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yhghicmp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bifytjey.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fxupwceu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2auuqlxbd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2elfhbkrh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ysitsadz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xxixlvie.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2phqfmkcm.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jhlrsjny.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2poggmhym.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vopknosf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ikzwarls.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lnnplymf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gxfkkeob.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2oqnophvn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rxqbaddm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2wtzgceck.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2udjirtvy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2sahmktdt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2jvbbhoyf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rmpgnwjq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2bollknfw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fxlvceqj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vapkpktg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wtmlseeg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2oilqtaoa.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2idudxjnu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nllkdbdb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2fvpdoyzo.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vmcvqzgd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2hdgyjyfj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2yoohcdrb.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2zoyeuchf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pysjugel.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mnpxvxlc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bwdmgfpe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2tniduqpk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hedropiw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fudzlemz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uopalxoe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bsqkgbfs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2trstghhe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dgmxwbvh.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2xtocfsik.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rqbobmya.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2lhtqznfi.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dzkgdvqk.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kikinseo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2mxpwyhue.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cubrwjda.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qpfqeyqw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2exuajqrv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2gmlnnmvy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ualrphwe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pabuxzjc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tqlvlodd.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wtwpzwnr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rnusdtkd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2zeaqhyno.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2tirjmisu.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2qnkjkcgm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tlrncyrg.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2jlubtckw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xpoixgmc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qsyrvhld.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2owbybifz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xcmgarru.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xtoszftz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2sfpdbods.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ldozsjjb.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wwtvuqut.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tipjybre.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2eqzszjao.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ibamatdf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zrcglxyt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2vliuzowd.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2edvshern.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2veuziavh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dfntwnow.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ryazctlk.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oetotbtt.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2bxdptimk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgpgufse.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2buwuxdqf.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2bsompimr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vzvwspwz.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2fzhwrhfc.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2chpbrwif.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2fywompwb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qgkdjnzg.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ngzyuytp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2veddjaml.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2emjkdidz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xrfelhwt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2sfrchfgz.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kobwsaii.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bafaszhb.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jplmtugq.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2lfqzvyjp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gndcklfu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2wamnhtmc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cofcappi.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnebdbht.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2tcrjcegv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2hzedeozo.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2lagnpapi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cplibknu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mrcsjlzs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uydcarvq.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nohuqcyh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hqkzdzcp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2imbymgnz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2qqkmwybz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2szvmufzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2irvdqgji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfccrqvm.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2szwbajro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwfjypxy.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2pnjmmnrg.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mijxwdkc.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2viixvlwz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2compfqge.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2ljkamahe.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2krsoeabs.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2svqtdydb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lrkdtorc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2jdnpvahx.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yqxjvusv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2janudljq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2wynziiwc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2hibwkvoc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2bqavhxjh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2zxaskwfk.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2kebtdnrk.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2qwgqnyby.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2gkcmdqcp.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2vufjdeox.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zccztbei.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2oscskrhh.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bkozjkon.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2hngjrbln.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2htyvunuy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2zhipgsjk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vekrnswt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2uzujvxjf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sdyvbqls.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qktcjhmq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2xgnaoerq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vwpzfnus.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2bhzzfqzo.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2bzkvbrmn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ljocauwg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2uxsazusi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nhoxkvwu.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2tkvbshys.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2acymrpcm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2lbsnyrto.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xizbrfpk.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mawwqule.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2wvkgfdbf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2brwpzsiu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mweqkdyh.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2avrxleoy.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2sifxvncn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2dgewwwst.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdbbgptb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fqeuukro.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qbunizry.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2mvgtygad.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2qunupzvd.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2wkerijbl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2yruvfkhl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2acrbjsqn.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2pkvareop.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2hlnkvspj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2dunshvon.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2lkikvnky.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2stgpzhwc.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2vacmwbjl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2gaoxjtji.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2hupjopgj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mggkkxdx.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2egsvftrd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2uhnjxywu.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2poxgqper.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ebwociua.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2vuqpsijg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2hbuoqvma.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nshqzhkw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2fdvfxpyd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2ckfswnde.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2oyuesbri.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2ohwunaqw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2xkdiwmxs.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2qnapzyus.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bieicftf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2dyjipibg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qbhhplar.html


<!-- 参考信息 -->