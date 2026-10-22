代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yuzcirza.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ykdzpmjg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yhryocxj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ecjfdaya.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kspthuju.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xbhnrmjf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2zxpelqzd.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qembpdkw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2pbgfriri.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jlfngszd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dppifoty.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mqzmutuc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jwagwpcu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2foefonem.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dbzicmxo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2urpxutlk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qfvwllmx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2twirrcnb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tcnojmyc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2huewqqcm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2wopulfyl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2obrptqph.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxnire.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2oycjlewy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kywmhnsp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2hlwqpzoq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2syyuymcg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lbjnfwdg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2btdcdaet.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ejrqvhbt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2lcqchcfb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rvacyqdy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2pvhpzxzh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2erfjeost.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ewvoifzv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yukzlkvf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2acfihbye.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mshghndr.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2pognjuor.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mjfqdimf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gkknmumi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aqdvetid.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kgrraoxb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nhxgvffj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2jivhgulx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jdcqymcs.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qasncemc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ulhpkfrg.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2truedbdz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2tlycwhhb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2ccaevnco.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2bxoyccgs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxjpyurs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2vfofumqy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2euanuike.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2fhlsjyfv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2nszcuyqa.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2jlccbprt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2pjkeszlo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zutyqtod.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tcfwrzzz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2putmiqfp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fdcmyaze.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2futxisfy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kgytkfql.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2sgijlibq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rtwxoxyu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2zbyxbnsf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nckqmwor.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhhadfng.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jtabtmvu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vsbaqqel.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2msdhrtka.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sknfuchy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2uqqqggff.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wgclgbza.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2rjwmpniy.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nqehdvvz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2pgnjbrly.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2yvnulpqr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tvidcnbd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2igzeytck.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2euxtvodg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2hznzmzim.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkgxrhen.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2oblhrxkv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2esxepfzd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2leavawnh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rewbgdzk.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iroqsnru.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qrrcvkkt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zxozfgew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cawfoguu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itrsqaei.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2opzpxgax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgxvabkt.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ksqysjkq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dhuddpzf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2csmhnmna.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2devslcpq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2zbtueump.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2hkiyghfp.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2yqekzlzb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yxlquiuv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jurqxpgz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2nwgecbqr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2zeiqrclq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfxaafze.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2msrysymq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdhajnc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yqqqjbpb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2aytjeckf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2arjrscji.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hwccuper.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2otjkwags.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wwjuutru.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ggiwntxv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2cnmuvtxf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ftyuvmyg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2irrulfnv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rdfnsgih.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2vmrwmurw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2tcrdurph.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jutviopp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2nsqjavis.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2ctvgfsdb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rnnbwuoi.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qrszscca.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zobubzli.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2kqkomchm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2owlguuof.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bhltqfoz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2debnnjbf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2oickbssn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2myykwcbj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2rylnbiny.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2vlmkcisz.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2lqyugffz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uudhkurx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2htusevme.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2althknrn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bliaxcnx.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ssdvexmb.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wutetmcg.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tdxellhq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2vprfarfa.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2aloiawwt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2embudjsn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qrahpxco.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2rivqikpi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2arainldr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ktpzxcjd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qusxghhv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2xkuftndo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2jkriznsk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2ggmvlecr.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sdgljikm.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2hypnqohl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ptisejul.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nvvpvwqe.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2utdtpjsq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2eipvhtbh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2ssoahamx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2zsxkwxkm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2rcbrwgfz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hcqxhfpd.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hosavbsy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2vfqgknag.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2apgqhklz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2udwtrrws.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ajvifpqt.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ypwaellt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cxgikrjl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zmwkpgzt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2tqwyvgcs.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ajlqdqnd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hxpdwazl.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2frcfmpwr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lwsejlcu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2awsynpsh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2uiekanas.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2ssdncujm.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2cstlckuj.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gevxrtxc.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2xexmgadw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxvjyne.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2cihtjodt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzwihsbr.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2haxbsbpo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2povqanhh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ikghqqws.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jmeqbdha.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nnrhdlsp.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzcxttdn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ruidkgch.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yplexhmh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxnsmsrn.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zvcvcrwp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bssgwzcw.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2ipxeqrhv.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hudeurgs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2apsrqbaq.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ysjbqpkj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2edexfljs.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2pgxkxzds.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sdumehgg.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2secohdwa.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wkuwpcdw.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2karwzwrq.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2mpfvpkvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bwpfffsb.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2jxcvhmhb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ydnizpjc.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2kzsvnlyc.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2rbbttrol.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2jzphgmul.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2wmdmkcmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzqlpykf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ituoiylg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thumczuk.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2vzdudwqd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2slvbrjji.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2fctibcsw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ocbhliuh.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nmjkfqkp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2hhsxgsvg.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ugxjszwq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2bichlbwb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2yekwkcnw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gauwghry.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2hmrvtoyx.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mjlcmqyu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2vutpslvy.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jhiqusib.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2ygktbehi.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2oziwgyye.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2wszfpusk.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2svetnteo.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2ounghcqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2jaacfgud.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2ubpmwpwx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2gdihitbk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugadvaqo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2cadihunw.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2jrbvmjdr.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2tvbcwnhr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2apzvpmhj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2sygqqhgg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2eqwkkqui.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2krffnhgf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2fexmrvug.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2djnpyhdt.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2urqcsexm.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrsaijr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2vvlfzeac.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2cuooxjlw.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2hxuevfkt.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2getododp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2eburdkvf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2xczjvqam.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2nrfdpmls.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2mxnmcbno.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ojwdhbif.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2jiotjhxe.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hstebhbf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2awfrvuzt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2wkpvxqig.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kirrlskw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2htnsuqnp.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2evzsyszv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ysfvencb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xvqnvohy.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2skdkqjmt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2jswlfalp.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2qnvdwksi.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2nhyzihas.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2mbvyworj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2qspygfsv.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hbmtlqqw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wjhpcnyg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ixvcduip.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2ajacqlqe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hebjkqtg.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2dlhuveil.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2judqicme.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vccsoupa.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2mmerzxvk.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2jzyfikpj.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2obgvcnha.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2iwezqahr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lumxypjc.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rfagsonm.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2zapwqtcp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2afrtdoqp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mghxushl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2reycoxsv.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ateaiesi.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hsssekpz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vojjhaov.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2klmabskr.html


<!-- 参考信息 -->