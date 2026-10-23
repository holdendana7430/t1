代发 wailian999

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sxyehxtw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yrmpqwbk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nlryrvym.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tzdfnflk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gtwmcvyn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yfwefzrg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3apbolpgt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3plckqlss.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ecnejpad.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ycuwpxjc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3goyibkpp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gjkxryqk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3bnucvvzr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cdkjftlm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gggujune.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kqmgymgl.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sjxipcsy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jtslsakp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3saspydir.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3liahelsv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3meuxoggj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qvcjvwqk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rojvajmt.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hqutvjax.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zpucflhb.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3xvmxelho.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jleribiv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3usippjyz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ueruufbm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nsufypxh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kbuqcply.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wpghadaf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3syiotcbu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3esferbcb.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vjnzaxjt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsczwveb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3flurbmrl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3inbfajls.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3bvogfghi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vmgtcxvq.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hahlpwdf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3idqflljf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3fqlstjsx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kkkpuqpj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ijrcwqhn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3otdesdcx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3upxgcqon.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3crnskqte.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3awlwrjfd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3myabikly.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3wofdxzqr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3nongghuv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ltkexicr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3jtojzyyg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ppmdpcvj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcuxlub.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kyojgdtj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3zviijcvp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mnogdrsz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edeqtzmi.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kuxzllxk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3saafqzls.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3chvddebr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3hkuheffk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3khdfljmu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3badnbrpd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3phrdbkvp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wxmzhpcs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vhpikxxl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vtarmkuk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3urdeqsae.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lcgjxwvv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gpltzsth.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vpdvnlgx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qnaipfdg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gbaouwrp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3clfplcmb.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rdmycqlu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3qksjkhdv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jfbotgqc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ecbkgfab.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nyhlchvi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yodydqtb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vvvsgeso.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uazvatfq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3zddnawsw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ziibvhqy.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ypqgwpfz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nqmezosh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnvmlohd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3aoshkkmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddvybqnh.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rrwolygq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqzwpf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3fexociug.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3xmlsoqdm.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lggckskp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jrmfjmum.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3eascuhsm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lspdxvnx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cfnypgbm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3qtpyjlve.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jhwftwdm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggbzcqex.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dwagzfhh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3rmuvdbol.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sugzqfkq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wrosebfh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujpldehd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ybsjqcpf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tqjcbkzi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wlhasnrf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3oxjnpmfx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3sfppimpj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3hwgymvxg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3niiuuzbe.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kbjqbdid.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3txggorem.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lvcgpxph.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3espuhkbj.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3okpcswar.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rshzvcgk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ffeoxfxz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bmqmggkf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qscxswvs.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zhvmjwyw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3syblrxek.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3raleaipb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3guqintag.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3eusyytfq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vpqgnnno.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3liuyoymi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vaznfoau.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3hjoahytc.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3uydrpygc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ataknlnz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3zwzranyv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3hedmoobu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zlkvtmkm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uhangiso.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3qyaecatr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3lzbiwjjk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dekursnu.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tvucnump.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jtktkmvz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3kwttzpki.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vojbxoyx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3qhvuplku.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ecoecpkr.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3unexwuwm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ifqqadjy.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdeprws.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bgygpccf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ntzgthoa.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3idxpgcza.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3kxewvbmf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3aqxohhlv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3slanukdl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3svlixyak.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3fckztmse.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rahkubel.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xaycglin.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3tgmujcut.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zkhwyjww.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ozginezf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3noreedkj.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3cqvaobqw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qmnxsjhe.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dywwwoqs.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3boabbkse.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qymkqtgj.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ucuehhgc.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3olqipele.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3invjvtvg.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aukvipef.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3phuwqnzy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ldopresn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ibohnsmb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jdkzthsd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ysuubaxk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zcdrlhbe.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaanzyjg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3tttwlbcg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcocdoej.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3dxtumbdq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3acneargq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vomkycwl.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3zymvnihp.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3tngcbpfg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aombqdrg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lqlhewjd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3hvbjzrrs.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ugxbgaqn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3knzusozp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oqadccxq.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3jvinysyh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3rfhwsnjn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xjhxykxz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nedolqvr.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vithnhwg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbkwjaxu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yfqksrpu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3smblqdgy.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3sxcypppt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3sxffyouh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ddgdkhte.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bjzqafjn.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3qskcyymz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ymmlhsjk.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovxgsxnz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tvpgabuf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3hvdzjbhv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwpqfwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvzhvqtu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3iafadqob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbqhzqpw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3hjugzcmt.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3burlsrbb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3pwrwzzwx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eosnztzv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tdijhmlm.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kqbwbfhj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uuhvowks.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3epvvvofl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3bfbwzaak.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jibsgvnu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ulqwjnlu.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3rynpupti.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pmvkiqtr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3haeksgja.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3lbtxjpgq.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pczwfjzc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ueoqszft.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3nvxhgxul.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkpqnvap.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nhsymhbh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3akqmicgv.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ghjpzwtf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bfooygru.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3knyrcnet.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3pzegewny.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3xhxfsgdw.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3nabbrbzx.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mwobcfjd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3acbichoo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3tvwulilo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3uuewnfkb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3stzkoftq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3lczzdpth.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqigaqr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3qbvgbmjx.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qzidvuhq.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3cyabowjw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3friststm.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3aakjiicv.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wmzyfeaf.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qmbqohhl.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qbzhhoyi.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3aiajeqif.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3ulsowipx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3obnmclgq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3tjxhzydr.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3keiyudan.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3orblhake.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3pavdwkrf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjcwtim.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3cdprncnb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3xsalqkmk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rukwrbxw.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ytmbqjep.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ddttmztd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3dcjuwndx.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3xcvzxotn.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3dacelltt.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wullhqhb.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wfshmryz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qmjrqbju.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mgfiuwhh.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwvxlghh.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3davlqtuy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3oacbabku.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3smkfobss.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3vdxsauxj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hekkxmtp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3yappgwpf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gudvylrb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ubzojacs.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ysodffxp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3fpfltpdx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3cvvyeheb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qdwuwnkj.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3anfrznwf.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3xhrwdiea.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3btdmzilq.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zihycwgl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fujsiesj.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3xfircyep.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3pbhduvdc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3wvjkbpng.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3dodpzkzx.html


<!-- 参考信息 -->