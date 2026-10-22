代发 wailian999

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ahzifivu.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2chfxxxrk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2vbtfoayr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipcfcyzd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2lahxfhem.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofbthkdw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhtmcezc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2inlyoyqx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xyiunzop.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2udqpoars.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sqmusquu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sueaigrk.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2aemajnan.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gkhmzwri.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2buppiccv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2alhiwavx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2awekpwmf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbpfnoar.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2sqtinwxd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2featcqwd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yprskeft.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2jdumclol.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wvjetkyp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2insyyxff.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvwqkobk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ccbmrxji.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2fsroycga.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2lbocnctc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2zcfqulsm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dcuzaaup.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xjwecftx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uygddjxw.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2twwxepsg.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2uprlhykz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rbmdkkya.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2litzzpta.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxvwaohr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfunllyr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwyvpjyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ogjrryec.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ubvwzoqc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rzsrmglz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hioeqslx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2aprgeffy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ojjgyzny.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ajfpjmnx.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2qlajlsoq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2lipeinby.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2agpcdpjh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tjybrvwm.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2slojqymg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2bvsidlqa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lslfhohk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bnccrlvm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lgighmih.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zxqtdeng.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2awshsnbo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mmjxnise.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2scmrgchv.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qmusgjji.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2zfaklgii.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2seikjnvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2okxwiwwo.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2cywxlzom.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qadnplum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dubzsowh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sztzdxpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bceuoskx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sfmhgulj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qwjfejcs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zfslwdwm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zeglpcfy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ynordasn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2leixzmdy.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bbesvcqn.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ksauwlwi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2zultbcpa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hotdukxw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2msxfkrbl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oqyrytzl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pbhejdqk.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2msymuttw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dgvnwczm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zwjbzjmr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nbrzlbix.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2inivjkrs.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2erqywwgq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zbhawgua.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2gbocowhf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2qgltynxx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2esyywwcg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2efcdcirg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qsklobto.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2xqcarggy.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2dxcdghdz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2dsacmdkk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2hojspzid.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2hzmkwfxu.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rhxasmmo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2pvodgfjo.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2bhujsfdg.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dmkntqmo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mynneeqz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2pgsytovc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2tvuypwqy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zdieymbl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qqtaxbbk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2wxsgeuxf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2mycgjscs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyzcmpr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2kkxgtgvj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2nsthkpzt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcuhpjto.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhcbqor.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hvpyogbf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfoxzorc.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2nxpftwsy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2aoxxyvwk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ihoqfszm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hfiwwlgb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2cynnrwkx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvujpyp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2kpvyvlrk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2wixtkbys.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kelepbgj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2fyipkwyx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2gfgcgosz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kcpcaizx.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uavczcnp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2neeyfsjd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2nrwivwdm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2cafoglpg.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xviflswx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2vlhczugm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ekszpylp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2glcjyuut.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rvtykyjl.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2legetgxu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kxcjttsc.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2nxdbeoig.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2agwxqkjg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2loeikcma.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qlvyniae.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ktidkyhp.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qenpwyfp.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gobrzemr.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2jzreywst.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2cbcfsxow.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gdgechzt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2kkxklwle.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ncfsygsx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2rgcznrib.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2geuztfua.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2onwckqnv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tvmladdz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgrybyhf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2vpnenshh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjgdrxq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2wttycomc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vebdmucy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2kwotepsi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2uvmdyvsq.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zoiqxfug.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2xitivrxn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2jyqblxri.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2evhyvivk.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqgdjylc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2nqyyxxfj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwpjxbes.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kthuxdrb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gqilahnq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2xjiaimeg.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zciulwlo.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2oinxetbr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2lpnejldi.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2qyiozbkf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqtsimrs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2pobruzvk.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lipubnki.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jvzortrg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xkeazdva.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2xwterhkb.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bvasvace.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2xafaaiup.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2bzppbuxy.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2clkwfqbf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfptpud.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2qdvatael.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2dorplsmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cimwvolp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bezzuakk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iftazomj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mmqxkwfl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2fmbtblfp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2feakozja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iyrxqfpm.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2qoljlmjs.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2zgcuitsp.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ramvaurv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2iocnyxkb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2nofrfmcc.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hrayqiaa.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hjmzrkrm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2uhrxwtpq.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2lhejzmjk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2rxipiudy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kyzbrloo.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jfypqyvu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kgknnjwm.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2ogueybmm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nqapvaac.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zwuohxxa.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rcqjfatk.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vyrhkdzm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2hxqvcsue.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbqgrgj.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2ueuvzewa.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2xcijrlra.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2ogoolbak.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2dcjmnkob.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2wfjgcneu.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2cikoralo.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2ymnhfmhf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2nbgnwdnd.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2svwywttw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2dwbuhqht.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mwenadic.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2krculnax.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2ximiirpp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2uuxossir.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2fpzlzkzh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fivhizse.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2mxpuadkv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vawhwmvo.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2zgriruin.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2xpsotmhm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2gxbwdyhq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2poqmurcp.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2qjzztoqr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2biqrjoyw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2yhotizbw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2ivyfayxm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2ndgopiqh.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2gvdbfikb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2pzsfuedq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2bvcncezi.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2ndvcaaqz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2dyprmnbc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ddmagcav.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2iiogtnuk.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2sffbiprn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtcuihs.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jaqruzpn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zlxocvll.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jhypdnjq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2touacadb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2hrrzbqww.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2yciojncr.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2awasyvox.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2hgiomqaf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gccvgxrv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2mkwdwllv.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kzfpcrqc.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2rqopszat.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjvaam.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ugkmwibb.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2niyzvews.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tqjumqgc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ukznxjpr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2vxtnibbl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ebtnhlox.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jiajdrmu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2inutarel.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yjpngnnb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2aprwbtws.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2wubxhcwd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bvmbvsdo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdnxvzx.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ernmuuqn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxlgje.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2gurxaovn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ncuiqbhx.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2yhbtxnty.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2enuxhove.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2tzgpzwyh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2ufddjldl.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ouoftipl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2riurozkj.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ihynfkfg.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2nvvcfpvc.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qbtdjcng.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnkksxfp.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2iyaorqbm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2nudtyuft.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xykbwcpb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gssplhyn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2alsplqea.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2olmamsfx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2xenfcznd.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ddshnxjw.html


<!-- 参考信息 -->