代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2glastimb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yttasdds.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lihannjk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bybxxlpt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ehphfhyn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2icnnmrai.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeemyww.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqcuggiw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qisvilig.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2tewzpsxt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbrhjv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2youehaqv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnfephmw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hxxtfflc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2glpjsddj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hgrnecrf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hmrfoksm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hvjclifu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rhqrspvz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2wxowinrl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dnjodzfm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2bquyjahk.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ogrefmce.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wqadcjlz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2heffezng.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2crjyihhj.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iovwvzvk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2udujakwk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wbtnxfvn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2nsuwcaqv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2aoxnshyi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2xfamilrl.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2mnuccmzh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2nikvhifj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dskhjlyq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjvwrtwl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qramfptr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2lrzevrpf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2toezvcgm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2myglqaxg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2phxrjmrg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jhfqaaoy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sznafolp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdvahvx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2btvipkll.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cpaqyimm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2gnzmrxmu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gfujytka.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bzruqoon.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mslvlhys.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gpvhxtjz.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ajaxmlxj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sttzaupn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kxtxnhww.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pefrkxed.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zrfilnsn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljqqsvxj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2iuqmdiwu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwwpbwrn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kocmyanc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2cufmgbkk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gqtsnhsq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2uxqfhyjb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmaegmkc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fuaydgsd.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2zplrywsu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2grwvmmwt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2kcxuvsjy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gxmuptrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2tkkwknsu.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlqxwscb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wqwyjrop.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tonroaam.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpkcenes.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oayrzzzn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vdgbidel.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2esuqpxwn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gvuiwdik.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gsuagren.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mealghxt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfpnkxgz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jebqyxki.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bcacyovd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2iooeouzj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2czakvlyp.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bsdytgmk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2qftjqlpu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2eukxbkta.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2vignroux.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ielachvd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2thhfrhqv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qukwqaml.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2aquxpryw.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2neluoyhg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2atuvhkcc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2iwdhwdho.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vjlywdbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zirgjcws.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wvwncqvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tehjogzo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wlynjanl.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2veliobff.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bwyiitlu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2uybaogmv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vizkbtny.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2dhrvkjtw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2alvqwxag.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2olyjsqcn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2szppykkh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tvultcxp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lmpvvhni.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kypsmtrt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ktufbulx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2mqjbyjzu.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fhnfbuka.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fxmiuqsv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2byjaeznn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2iadzvqtn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hbkqzbwt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2ekthnlyo.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yahipphu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2zumhgudo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2brexrszt.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzydorwo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2dbabzzgw.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ytrwzlhz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2pfwrulnj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xguzciso.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wippyjjd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bvvykuow.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gnlmtpxy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ehbsquvo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2smsqcrbj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fvliyomz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2khqznyvy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2daynjilp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ahmokwpx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2glwmeupb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2oukquynu.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xugplznp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2joqttrpf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2qlhbkbzh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2srjepvqs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajxnigqw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvmehvbi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2whaeznea.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ipcxiapt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2elizfxvg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ykjcuhpo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gbeuiziq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2prmysigw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mpokqgme.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ydlpefzo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2chtgemex.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dbbnsvjt.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2xblkonmu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ghyhnowo.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zurvfwle.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wthnzvjx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bvojbyhg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qdrdrqng.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2sfynsgxx.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ictmklhf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2wznbtwcb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2wiqrrani.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2isnrkjgn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2tumexahi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2naznfcvz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2swfkqzem.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ijpayvtj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2owbvlvcu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2rbmjsmme.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mahbxzdf.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2wrztcbza.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2yysrxusf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2wyvklozx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evieadso.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wckhuzfa.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2normqsyo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2kijdrbht.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ktblwglh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2qkqahryb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhexqswu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tizksuhw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2umhgwcgj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2txodlczi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ydlagtcd.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onsqfcqk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lepnmlpq.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnbexasa.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2jakugkfq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vxhhbbys.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2iellxwby.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nghfysfe.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pnfjjoht.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bvtequia.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwuqen.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvkxqfk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2owsyucay.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ibzqbhcd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2olvhfynm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lpvnctaj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hryndpmn.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ijnyerjs.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2toromxtj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2modesnac.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2tmwynxys.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vfcpqidc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpcstzpr.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2aqwkokeb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tjrpuimy.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hllxngmx.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2jhyrxhwr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gsgfzckl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qtitqzag.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mjgqlvdk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2upardygk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2txnugcwo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vsfotwdq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dmqujxpr.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvawlxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgkyddft.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2oofgawez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzjaic.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2nurulvfo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2pmxaarbq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ilyrbuzg.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nifosmvz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2bojnrsfo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2totsdtbh.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2mtupjbjc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2yddhkgpl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2ffgshrxi.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gxxizhjh.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hxniogwd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2ujrtmgng.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2swjyppxs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2ztncttzi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2megcpbes.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mptdizpv.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bxrfqldh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmirhkn.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2btdafpss.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pfvvackg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2adnlvpar.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpyclpwf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2arcswkdo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2afigvjbl.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2tgzczewx.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xffvomke.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2hagehjjd.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzlkklj.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2jqyobkjh.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2uzkukirv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2cfdcreda.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cgxngnws.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2nacfdgrc.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2fglpfpge.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2bkiwavqv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ntqpzkwz.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zwvumkqx.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2hntbybyz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jycixrsm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2asrptmjb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jrirpiwe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2miftggkm.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2ctrqhvbn.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2fcmlvnqc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2ollccogx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2uaelfkpf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2juxakglc.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kxagrovd.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2hkvvygns.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2ryuxhswz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2crngwpfe.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2ghlflmai.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvedkj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nrrrkzxj.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ohyecnzw.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2unpyekcq.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2dunuyxjc.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ecgqzpxx.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qsgjjyyv.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zausqner.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2hjgyzpjz.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mnwkauic.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2lgobcfnq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2lvleznpw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2zgwggvxv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2xwkymqyg.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2fsrmgcod.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2fwsxbuxy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ujbijxma.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2jdfsevkc.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2kurvyatw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2hrhbxets.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2frzzskoz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2sxrvnxfm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2luynszpd.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ymtnoigx.html


<!-- 参考信息 -->