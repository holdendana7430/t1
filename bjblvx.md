代发 wailian999

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dtucfmjk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3tfatbqwt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ztifjxxr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fzjcagmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3djmbwynr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3uuwrdngt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ahputvpx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ijayyiec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3igyxveul.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iothrsva.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dqlegknp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gzbnprjp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3twxzrwgb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3prtzssni.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jmxxmqhe.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pqmwwjpj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wyznyadd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jassnmtv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lnwhomvy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qqwxoyem.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kbdgcsxp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3rmsrlfgq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yyoyrdbo.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3imsjjhdj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mhuywncw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vkjkhydk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sbwipztb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pelkliav.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ucgqkyis.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oklzvujw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ojzroovu.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gsdsmzmy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ooangfni.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eogifdqz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ugrqhsbj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlikhugs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dhlgdryt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rsvpxyzx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3nyzebbmm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3avgotwhr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3aevgwxzg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3annrmzwt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3bviteuqi.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ecdqonih.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3wnimfzxh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mozmqpfz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3tfktsvnw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3dpenyloy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zkkmlsdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3dgfjzobp.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tepqntrx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nspofpwt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3pptrwlfh.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3wlhlhehu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3dstekcko.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3qwoqqqie.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qizptqff.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3joqffvtn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xhpeblox.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kslwcytn.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kjvjwaci.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzujnqtv.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3scznpjge.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zaabkmus.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3tkdlrqhg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3uypaeahr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qjvttfcu.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nljfosnf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bvhrolyl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3svbbiaaf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3xetdueox.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3iyyuxaeg.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3neucnhcu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3xlpozlzx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pldcqvnc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ibwrbgos.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3xlkibczg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3koymtzpw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zqbkinpb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mqebphil.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dsgzblrg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3egjijitp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3icuzbpvp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3dqbbxkxp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3gsarmmlx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3afgaqfag.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3byedbalk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3haymtnjz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vczewxul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvsgdlof.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3smvwgjjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfbqajxy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ppotdyzk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eklfgerk.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpmmqpxl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nwlsqteq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3jnlwdfju.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3rgelsepr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3dbgwwwid.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3aznumbyf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3utivsybh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3woguqjuy.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xzkusyrw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkunbzq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dbpffkzo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3elksfvke.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3earurpmo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3pdkjahob.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqnzxoiz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qcoingse.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mxahragq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gtmztbgk.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uzhvauuo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kbucvqfa.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3qlktkbgu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itnkdzuy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3dzpllcca.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3noajhubh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3lycutcej.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zirbvocz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bipfpuoq.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3myobauvm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nauyxhqs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wydrsunf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mdmvbxwc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3znqkszxx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pqlunhve.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ouqpkcme.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3abqswnvx.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3klyerbon.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ezuyxqgo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3dkrjlxln.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3lncwxuwk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3fgcxkquv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3pgsumzic.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3nxgtgrip.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3saewyynn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lokyuqzo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gpabstuc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3utjirzch.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xnjvbrqp.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qejsslaq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3gckisqdj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3lwnjhgpz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wskztwuv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ufuwirct.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ocqbxsaw.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3allvsnqa.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3fzbqieqi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3heectvta.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3wqdgqjth.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ayyxwlap.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3crceomjq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vblmssta.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3atdeqwwj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qjikgyll.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xpxspojw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3iqntenoj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3slziyfhy.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ihufpqkq.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ktebahit.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmhijvbe.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3peorkrjb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ubbsvyvc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3iiulzlqu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ycbargxm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hrqlligx.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ueucqeyi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bjikmius.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3csgxpzza.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qdqyneyt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bebwlljq.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nohkorla.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zlubnyne.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mernmqbz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3bdhxahan.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zoajouxo.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3gzfykfzb.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rsvoaihc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbflhiax.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zuncpfci.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lbcfllta.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3vpmjkxvy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axqtuyko.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ievmlvjj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3huazymjc.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3uugrtyji.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qpfgktog.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qhntezeg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpchqdwm.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezotvjiq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3hdvgyisk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vncjcdec.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqhdylpu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3joqxbgpe.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cbjulpgj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zdjgzmiz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gsrutchw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3oauzbmvq.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gubdiodt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3raixsoau.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dkjyljqv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ncchfzhk.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3htpqpwxv.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fqbkovyi.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3srarvwgq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmdumcj.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3jocqaqnu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kxhxokhz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3crdtazgn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ctkqeeip.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nvdlwmnc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3uowszoim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxckzvdc.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbddct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpsyyfve.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3kojjslrq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3eavdsgex.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3mbqrxaui.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3prphsfgt.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3maoerkrz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jvgkuhkm.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3emngeulu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3oowdlbaj.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3xacomkne.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cdivubnu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3ynihwtrm.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3kphgcrnn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3xxruhlll.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3yuvzgyns.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3mxgdbkhi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3lymgzoaq.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zscljtst.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3bwesziib.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3deyujsbf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fghzyomu.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3euhrjwml.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qckhntef.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwufvwyd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3rsofwitm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3iongntwk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3lqfvtrgu.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3hpegkjrx.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhbutvl.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3nyhjdbhx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrdziju.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3cmigbscq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rhclyixl.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3emmhvpyw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3kwnorzbg.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3gmirmqrj.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytrclpgt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3iphwcjzh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3owkufhbc.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3rgzsqdvf.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ogrtqwag.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3mdgdyofm.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3phstrmrr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3lyjoxgjq.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3tubeawus.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3yceddfuv.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3ztjtxbky.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ntgvvftj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ukceatpr.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ogbojeng.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlabqdf.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3nmlbwvdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kpkocfxj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3fdmzyaab.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ootafgdl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3pfqxbpcy.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3mrspggvz.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vmznuows.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3ghtguvwy.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3httudbuj.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdmrplv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3irujgwjl.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ejyuctuz.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3zdnedoou.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3ibojlehw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ezctyoms.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vejphout.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gltanoge.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3irqjfpft.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wokslrer.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3heqjknwn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pppzflho.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3axxqlvaz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3htphrluv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fdaodevh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3gzdxvyie.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3kiyddckn.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3lvmaouqb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3rzymfshl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sabmscrj.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gnzstwmv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ixerhyvd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bmfswsnj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vflomejh.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ewxtnaxf.html


<!-- 参考信息 -->