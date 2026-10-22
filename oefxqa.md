代发 wailian999

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yexlluxz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bubermhs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vpcewmaf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2llpcqxoz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2llwlpnqa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yplhyvds.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xkrtaopi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dkimldtw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lsgbgcqc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2haeqmfro.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dsktjbfq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ihzxacql.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vygtkmop.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kfetilbk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2yrlrkwkn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zltplbed.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zgpcmozx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2oybjfubh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2grushqac.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cdxgktwg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2aunqdswd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bmwdccfu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hqyxzcmj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2liefeklh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ehofstae.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2upalmvzh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fvkalrpd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2pwtreqyf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nyxpmkky.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2uyvqnroy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pdrarwfm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tnundeiz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2aoiztzvu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wykjwwpq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwflumlu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2epkicbrp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2roarizeg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2soaozaqd.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qbtprzcb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2qorkkkzj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ixbbcyon.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vxljlvwv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hhxrplys.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vylzirsc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2iatculdz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dltijqcd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2cgxyhjxg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2alwivdde.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zdqcbwgy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2qlokvgas.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wtdvntpb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vxveehkq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kxmfbuzi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2sunlzgbz.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2upcmwkqk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hrfmcrbi.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hzrneofd.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ewhejusn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ivmtmuhn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2cywggjza.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ukxqhnre.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gquokdvx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2rrlhacdz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2tszvicyu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ilsipdze.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbhwzkce.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmrsqsdr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ngsswesi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tnvnmquv.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsszjuyz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2gcwkiazs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hgvyaciy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jtelqrro.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jookzcbd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vpbvmsvn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2sdejuqob.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2imjzemet.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2knxftbql.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2bfweknae.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2iqsfjcki.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2yyaaxawv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2taiqhwpp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fgveixdo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ksytruba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnngycqm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zdtpssok.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ugthihsi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nknsftri.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gvlvxwun.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2cfctzban.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wovayqrf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2zwecvnqy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2spbflqfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqnitypy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2feuaaifa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ycslxdui.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jczonbld.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2shqelzqi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqnpkskl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ksbciyyy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dspdosri.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2zaunnwup.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nhydhfmq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2uvizhhux.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sypwxkna.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2qienmphc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nxqhlhsq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rnvugfox.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qphfealj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rqsrhnnf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wpzbrhrz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lmtugtdc.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gqizcagp.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2pzrrxvcs.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nomajwhj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ijpgytne.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2isgokmbc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2nqhtrucd.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2qbtktqbm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlmkwcv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dguprhfy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2qkckxkdr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vyyyjopl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tuggshvc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2hwqbmagk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2tdsenjun.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xkhcppmi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qxoxylgh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jeejcqbx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ouamaltg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ffmxclaa.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ccbwzagp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2peelgzqo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2zrkiateq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2zzvqgxhf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2krxgsixu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gegvlzde.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2nohaynro.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2etjjxxlw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2sfkaexpm.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2xezncbna.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sfswvxkf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hkjxgzit.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2acstorgs.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dgxmhyur.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2wdxkmbzv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ztcquedi.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2extwssif.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hjskuycz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzrywbpf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qzsslfkd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2vcnhyupa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2eybdaujj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2qakqxguy.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2nawjzkwx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2laulhber.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wcvwqwrl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nfusnuwf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2vkqjewcv.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2phgiprva.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2keyjagwz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2qskxxnwk.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2hqyqlcbm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2bdirxrue.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zzwiotrn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2slvxjutc.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsneggro.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2behetzgj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xmanymaj.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2owoyjcrt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ulizmbti.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2zvxaqtvk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ewwqihuz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbejmkx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2tmamcquh.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2cvenmgcm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2znafkcvr.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ikamfbyy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2eygtgdsi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2harztorq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jcaxyuda.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qmbztqzq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2vufjrjtk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvzvrkes.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzplnmfr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2whcwhbfe.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gtwdxosd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2wzuxtwbm.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rixeqjja.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2icyiahvl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yqnzfvrk.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2tgvckhjh.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2ayfuysvv.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ygirnmwp.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dggoemhe.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2arqnihkd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2jpvqplvg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2oohlaayu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pkncpqrn.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hfhaqbnw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2irsnuwam.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mxwspahg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2kedpjrnl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lwxtixgh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbhhrzh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ajldiesv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2uqhyaeoc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2imtgpodi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ekpqzvjm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ptginzww.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2skkkwtjh.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2lhzhjtcx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tarxiego.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dxbfzifo.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2jdszovus.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2dlwpirdy.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xfykbkdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxepsfyl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xucfkadx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otzbmehu.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2dutzrahj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2knwdkbfn.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2lzcaejux.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2morqhpvp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nvmzwihp.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2eqqyjign.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2cqdzkicl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2lqajwmqo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pfvwtbqs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tohdkwmm.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rdcshvuc.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2jwnrgdjw.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2eanvqlqs.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2zczopzqn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2iylsscam.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2cvbnklei.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2phbdmecm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2jqiqbjgd.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2taydwyxb.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2hfynakoe.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fktdjiua.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2vjaazlht.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2jkumrwed.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ajyqeswy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2ckyihbft.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2xpxbjjsf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2idbgexpc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mssxxgup.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2zervbeea.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2subpqtkq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2vmgfputc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2npcmghkn.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2rdoycenf.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2ravhgcju.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2gqvhipgm.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2slbtctvv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2zctinoen.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtrtrcq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2zkdbkztp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxgjdrr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2uyfvkbdn.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2vbcodgig.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2rszycrwx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2idzhysgm.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2daolkdoj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pejlawcg.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2blklttvx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bdxxbbtx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2fpjwbpdt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2alsmwyho.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2pnomduex.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2wqcxqtvr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2gcytxdsk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zpkrjnod.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2peibwubl.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2idtmwfzm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2omqkisxc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2efmsssas.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2uyaapqiu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqulqgf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ggpfeqsf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2sfevhigu.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tcjrxzgz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lycfymli.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2azkoziwu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2jhuygbsu.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2wtlwubix.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ivcrboof.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2kleetzdn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2asmjwbke.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hgmjadhx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqsatbs.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2bbttljnd.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nuyvbtlk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2qdthwubk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2fxrhdupe.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2nbbqfmyl.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2hujarovg.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2qpeuhtjp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2npkuwdil.html


<!-- 参考信息 -->