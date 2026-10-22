代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xdtqjvab.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pxfanqmi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2grzlxvkk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2adgpfkjy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dmndwsud.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ludgrzpg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xdgpkjvq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ftqpewls.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jqvzpkgs.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zqcjudfn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lrjmdqwu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2onqxctlm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mnjwjmyv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xittrxhf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pmswclwj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nkqcitpf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2foaldufd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2juakzrvb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ljejlaka.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qtabfceu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2nnwydjfi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2prgvcklv.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aairoqwr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2idsoczep.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zfswnkxr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uqjldhgq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cjrfqeec.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bahqycrj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2havyvesw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dwrozoaf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fcammqak.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2brxduyvi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cczwizlg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcwcmiek.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lurodiyi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2qqybpgmv.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xvdostzk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2njiceebg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2rmwyplfy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2aochsxvh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2qkzjtpjk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ftyfoxmg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ezbyytht.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ladmhrmk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2wjyonfnz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2pwyzdkko.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lnfawhbf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nhitdloq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jgqwfray.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2zdxthfkf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2atfwvnak.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kcbktpau.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2becbchlq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jglfqarz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2zddhxacw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tuzdmmkv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2oxgruutq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2tnykssmt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2mrdbqdmj.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2bbyxutga.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jjcqdvwq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2zwmgpens.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qsbwbxsc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crowwdmt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cjgmldtg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcckcwmm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2signocnu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qbazctuv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2womgnrlm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wvjfnxwe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dmjlmljj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2usopjspa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zosybuiw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2balfylpg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uzqiccoz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wpheiuaf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2yavspkzc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nujyeidi.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2grlkyuyj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xgixbxoc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ksdbadaf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iqlrasfo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixsoqfqu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qqcvwaun.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fsbgimvr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gkhpcmsg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tpkwodcl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bcyrgtjv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2tdyorysx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mazcdeuy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2vbkdodwx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jcmwgkvc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qhwkaneb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlykronb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2oqbkgwij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmoqabsi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dfipjkrq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2rfnyairs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2wqiplvka.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rvqcbsah.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2qhjrmevp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xsbklzno.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2etlmhadc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2tormhykc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ibninqyz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2cxruurcn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jlayfyir.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkteagay.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ebwfrkvu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qucbtmdw.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2synfmqhx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zqbthknh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2poewmxyd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2jwgaxawu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2txumpcru.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2xhturwss.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2wzqvkvkv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mmwvzgnu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xostddzn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zbtvzvbj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jhkzguwm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkibtzfh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2xaurfwlh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2akmlomvr.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2oukqasak.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2abrnpuni.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nrgyfsyz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cbjpjhzb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2tpemllxv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vzdxxcjn.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2euzgkgjf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nrexvuuo.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wzyybuhl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2twxoowoo.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pxxjglrr.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrkevz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gbouvwjd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ipltvwge.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2eyximolr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xtzhqpay.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2luicbljr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2skuctwdf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hvggildi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gqhlfsgs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2joddvzya.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2tdyzbhvd.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2uhltsuqf.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2bswpfrne.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2boknoqoo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2botxnpuv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ofjcrgtv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2zwtqwfmi.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bdvdbyzf.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvptrlu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2uwviaqub.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mxpoxhgb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vmrkpedm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ksaszesy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2fmjpsnxd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2yjkmjymb.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2uxxyxbbz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zomhhzsr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2fmoijhtq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2efjnghsp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2yjsrcteg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hwmnlwev.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2awlismgk.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2zfpyvhyw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pvailrxv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2imhhxfww.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrwkvkal.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2gxqloiee.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eplcwaon.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2lzgqazdg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ipeqrkdu.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2nwtjfpbp.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2igirtlch.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2tomipewl.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2wktejujg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2cmcaowyn.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2bkcdmlli.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2rgcsfjri.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cxfwwyqg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gmnlbdcj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2emyfkqwd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwoqfvca.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gvxvhuws.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcnoeswd.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2afpwapot.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2hdexwjek.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dggsdmau.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2mcxmbkqx.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2lqixfrpu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2otkdvoku.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwsbdboc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2qxuzydmn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2buymyepd.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zzmkdoib.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pjhtdbyz.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2lvicglmw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qykbfmmi.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ceqounrs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2oyosnzrl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2vzzmmumk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqszlxav.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2mhflnnri.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2tnjnifxf.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2tuuiehzi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2uouhvifu.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2icyhqxog.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2egadlocb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2avkzczvb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bgvluxgn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2bsvgfgpy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2eauavwls.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2oxzihgmw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2ttxlrmgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewhjvzpw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iauabdkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cenasorl.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eyzzwryy.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2audvqvwd.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ewjumccp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vnvrmeru.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2wfhawnsp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2yxgejshc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2rzqjbqdn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2tppsvsyr.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2znmqlyjo.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ihfqzlhv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2vznugvuf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2trhdalei.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2idzjfxhn.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2lvekhylz.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2cfdbblab.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2tzolkoro.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bfnlmieu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2qukzpuyq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2alnchbmu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2kpvhgnkf.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qzgiqaqc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bznnhxqv.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2gjsbqdup.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhxonaue.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wabmzeut.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2dxcxvoor.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2uwghzvlf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmsefqh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qimlipgb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2admtptag.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2tpknowgb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2kurjicvs.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ofarcbvt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2bkmecujg.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2mypjhrnp.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hzxfqend.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2ksketowd.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2mdwgkyej.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ifgzdsfz.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2amsjhync.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2qdwqkxel.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2gvhdnroy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2dnjifsxd.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zjluhiax.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2sscojxnq.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2vnsgwecu.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2mjgxowhj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2pkbduair.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rolwjrft.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2gqqjwuom.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2lnpfzccc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2satgruum.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2ctlraecq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2wwcerwaq.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2dtmyolnw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2negytdmt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ksdevecw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2oxjftufa.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2gpkqqanz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ctotmrvd.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2sdubykyy.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2uqqjkhjb.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xjleznzh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2mxhlpbsg.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2ushmhnky.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2btwnqqkm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2sfhbwgoq.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2dtdamdhb.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ftzdsgef.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2xqyuxpah.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2pkfgrclt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jvegatks.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2xtsomftl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2zkujegnq.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2nenelynh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2movhnlbf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2axndjgeq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2bnifjncq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2fnhugfri.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kutlwwsg.html


<!-- 参考信息 -->