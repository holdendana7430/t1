代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cfntygvi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3fxyodpsv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3sduwohvq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yyrvgbaz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wyvydxgd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ktapglyt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mtkaajfi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3jcwdllmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ghiutewt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kcxwapyg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lqfevuzo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oefpxjoq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fywjrqni.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lehjkwmt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ioosoglv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3crcjhnww.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ohdffabo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqrnbnui.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ewjwjofp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3zthrgcsv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wkelmddq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3meygogtj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tfltrgym.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jywpxrxe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tudppfry.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkyqloi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjthmeif.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rsvsthoh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lccshmle.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgnreixv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ordmbrgm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3avaumnvn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cpcxpxsp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwsvliag.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3sqearyjv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vvnczdip.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vdelajir.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3jjqlvyks.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3gxvfoyov.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zbkzellv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qeacksyo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3gdormbev.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3raiezczo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3buefywwm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3krxckftn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wjfispya.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mxqusady.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gddgpnud.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kraegctc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bgifnsdn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3bbcccuiu.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxxqda.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3vsfawksv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hgfkhbgh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ifwivpzv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3gkmasbyu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ccbvfavd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fibscmke.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3frkolvvt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3sryimtlc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rzsvhytx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tmcckujf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3fqlrkdum.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3niymcnad.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpzovtp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3msejhmtn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3owspkuqd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3emwgbasi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3rwdhlgtd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zaisiutl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fiqgcock.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ozslshvc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bhzfrbbq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3dwjwriea.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ikzfgduc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3gusvqhae.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ypgwyqrm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qtodqxtu.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kpmoruva.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hcngsnxg.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqfifby.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bbragjak.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ervfdykx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jbokldem.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mtggxved.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxpcihec.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bbezseve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzefjbzf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtkxyyqs.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3buxuivuw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3edthlmgq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3xbwdvliz.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3mhxfnbyq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cuoruuzd.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3rujcdjfr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gknmeart.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lfltzlmq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3cxzfsplm.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ryhrenqv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjicybcz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lairlpse.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3haigtvmo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3hrufcbes.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3ggetjxql.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcfdassy.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3zpiyvdmd.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wotxymgt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jupoxctv.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uuiapetw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lkrelpgz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3usqrgblm.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtddxcxm.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ogpvspal.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dlbbxiru.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jswvtnzr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ayubgswc.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bcidjier.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qiuhdfqd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3clzcppih.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ecagiuym.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bwgscamo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3twwggody.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cjbfugpa.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wmrnbado.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3wibreiwr.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ypivkpvw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ajdfclaj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlwuwwm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zydznsgl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3kavtxurr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3kalwkkif.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzrtccdi.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3xpjzzdkf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xwdqpfmv.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3chuzyqqs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wixumusl.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3woiplarf.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3iffcanne.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3zahgitfl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqiblvp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tdwusxmm.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qestrrdw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tapietiw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rnnfpemk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fehqdcca.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ajpggrjc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3xzlnldwx.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3uxjnabdj.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vkesjtyj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nrbirsap.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3oxowmyhr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jyhyrnhk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ycebzemq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3kkntloql.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hzootpms.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vyrzpfjw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cxoqvgyb.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kyechlrf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgxpmvmf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3scbbjkaf.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rjqjqpjb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gkftzxup.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jtwnxflv.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jlkhuquj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fjsxyknu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qybshdhg.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hgdvfhdv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ukaieucp.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgivimbu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3yvnfhmee.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3twcppnew.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3arodzcdr.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3elijteuo.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3suxkpedk.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3rovpywkg.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gibxpnuk.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pgitahxy.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmuamosg.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3kktntepi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3vlcbaver.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ackyeyru.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hszdtpus.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3iwciyath.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ewxplxly.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgjwjdjs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfbypplq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdjxrxob.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3iuqrgihd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3idlfbxpv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vepwzyho.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xzlhcwal.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mcudptgc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3dgtgzzuy.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zsefddrq.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bfsmvuti.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mxxmifok.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwxsjsb.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fdeiwivd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3jbmoeaar.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3pcccydxi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tlmvkcoz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vhsfrdio.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ogppxuug.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3dadtrogd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3oslipnmv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ioniafeb.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zgmwnewl.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zamejqbm.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlzzsfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qglbcuee.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekxxvkjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jthktixk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ycdmewrz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3yjixmmfk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3flvwaknq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3keazhltc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3onqdrjrc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zdknrdib.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3luebpler.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3iyubyfpq.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3kzhjymhb.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jsbezycr.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3wmqoxrqx.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lovchmeg.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3rvwovosl.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3uxqmkiic.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkafdr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3nbqcikbd.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3imljssyt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3kghjpbzf.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qsfvndxt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3npmoszuo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3aheqvxkf.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ssdnoivb.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3buqmjxxq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hwcuubis.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3bebzhxgj.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qabudbds.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3calajmoh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kuqmrtff.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rmqdilcq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wctrfvkm.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xgccygtd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nvxcfgru.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ydpblxpz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jntezhzn.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3opneubfi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uhxccxsl.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3kdgodvhh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3btqgiocm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3zhkaqkwa.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvdgksm.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3hbeznwkv.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqedld.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3qpvnwwyo.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vrtowdbo.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3obtgpqzl.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3yuckyhdd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3fqdytaft.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3itodlfzb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3mxbteebo.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3dsocgyyf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3mlivfuln.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3sjngzkbf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3yklzcleo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3veoktyfn.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3avatxzmf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3swcfvhwm.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cygxkdds.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3gvdoiota.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3nnafkodv.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rcpjqqnt.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wqxyjbwo.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gaoivjdq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jviujztj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3goyqjpii.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rwboikyy.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3opmaiscl.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3lvbovfhh.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3doewtgrb.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3fljvsuzx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rbkrjugb.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3kidgvkpo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3shbkidyd.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lqamksnn.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qkbvulpw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fxbjmnqx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvfgta.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yopgslnz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ycqqrvbv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ouqmujcq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3taeglpwo.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3otnjjnqr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3ljpluush.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vrshnlpq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3zrvvbhjm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3iintptdg.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qdesncfm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3bvtjflrh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3pknpwoxs.html


<!-- 参考信息 -->