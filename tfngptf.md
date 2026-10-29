代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/ghmfridqh.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gomrekwlp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gwklxpslr.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gbzcvsieq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gskjdycrg.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gvgagptqy.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gxyzzftkw.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gfcihsqtt.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gkobgewix.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gapxukvkt.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gkxqurjdh.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gxcmtnpbz.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/grhwdincp.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gqxctqoqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gawnsodjd.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gjjyywwos.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gncwhyosj.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gywcdljjo.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gpgtmfour.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gobpcjedv.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghcucettr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gobvyhqii.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gfrikaycs.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gfwagvyvm.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gdcjqbgcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gwyebablk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/giegsymda.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/ggheqmtsx.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gqdbulbva.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gmnpxbucb.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gtmziyndq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gnfushmpc.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gpasunprp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gdgdidgio.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gbjspaxjc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gqdtlwhgq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gkfwzacqi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gqpdduicy.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/goxefsiua.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gvvqumwqm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gtjlkqznl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/goomtumaq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gqmnttzub.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gqaysrsyl.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbvqqfdrr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/ggdczkzbl.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gymewkein.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gyebbplub.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gfyknmvyv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gxhtmjwvk.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gqerwegyb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ghluukrek.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gojlttodv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gesmzgzhc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjdqhremb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gvvleuxxa.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/grissbtij.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gsdwzuqqu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gsbnlfjbx.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gzfrdqveq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gaoynlwhu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gharjbnxi.sHtML

static_cast<double>(a) / b
来源：http://m.share.zdbjq.cn/Article/details/guksmkdtp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/goikmolhx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/ghkzugnun.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gohuyodcf.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gbosdmpqc.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gqvabbmlk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gdgnabckn.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gzmfppfog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gwhzkqepo.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/grjrtlvag.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gzzrhoums.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gktxaqwut.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gijlyvwup.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gmnvjyylz.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gfmnmnnku.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gpuewuwmr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gldbgbnhq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/ghlueyqav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gmkffdxfn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gikfhxlnf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gpzcovbwj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gctrylyev.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/grbquicno.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gehgojoto.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gfrplfpdk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gnahybquw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gymvyzoti.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gokiurcgl.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gajzqywpx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gsedalhsd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gzrwumivl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/ghvvwozyb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gkhjmfrai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gozotiwgs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gryeusphj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/ggdehjenz.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gltildrqp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gplaqlohn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gtvpbhfxo.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gnrxnspys.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gbrjozcik.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/giofrapjs.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/ghffyxntu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gyecxisht.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gdifvmvvv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gakxavkdz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gdoohrhoz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gphhlgwga.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gumytviwb.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gsaizdlop.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/ghhsdrivt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gehgzufuy.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gvnjsiuqn.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gqjaihxaf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gidvnyeyn.sHtML

var a = 1;  let b = 2
来源：http://www.share.zdbjq.cn/Article/details/gfgycvclx.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwzapbyxi.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/ggwgfliwj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/grrtwjaik.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gojqpakue.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gpqvjxypu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gbyramknk.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gnnubobge.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gqppzqduz.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gmtoseeyh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmkcrjsrg.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/glzzmyldr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gfalzisiq.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gyexycojm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/geuupngll.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/glghcouny.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gmjxfijte.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gsvpqdyvy.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gfbtskkxf.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gzepuzmdf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gtgxqvswz.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gbkqfycdp.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/giexdwiux.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/giuetpfyo.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gbassyxva.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gphfkyckr.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gvezkbsuz.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfmckuntk.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfvxtjtdu.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/ghtpwigiv.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gofppdowu.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/ghwnnhvyq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/gvgykpufn.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gijggzoun.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gupawqacp.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gvgkgzlyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/glsutiubs.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/glkalmvhu.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/giafxqmib.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcgwmxblt.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gzvaccqrc.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gboqumamc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gqfawbkrh.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gnddsgase.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwuviwa.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gdbcanmsv.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gtxbbscza.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghbxqgzqs.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdtaiooyn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gqwhktcco.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gxpmpdlvo.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbbfxivlx.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/ggmmtazae.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/glfrkhiax.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gxpnqdopp.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gnilsqkbz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gmxwlsfjh.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/geyiyphmi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gwzqbewuy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gzzatxkoy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwbujoeb.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/gwqhyoltq.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/ghwsifwfr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/ggluzcvfp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grlyozvii.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gopzegiin.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gwvppfwmp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/genuogshr.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gzxmfbeyx.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gbeobhzdh.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gwxtakwqo.sHtML

val a = 1;  var b = 2
来源：http://www.share.hesvh.cn/Article/details/grtvsbtha.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gohdduaok.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gumhvxsyw.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gxgkplkza.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gwhcyurro.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gbalujzap.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfewgsqxt.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gggjzfygh.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gagdnthxt.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmakzajzd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gqfuocpfo.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gitwteqfi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gnrleuavw.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gasfsqukd.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gbbwhfezl.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gzstcwpxs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gwmkltmbt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gllufojop.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gzaljcsll.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyykgteho.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gppzglddm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gvfrluxfp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gwoetxmcd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/grtgladib.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/geofrsuge.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gwaebkiyp.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/ghhshhvlh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gvgnqqviw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.hesvh.cn/Article/details/gpyvpgmht.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/grnveenfz.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/ghejnuava.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/guiasyfhv.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gdupadkyb.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/grmfbmhvy.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gcyqyoqqq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gthtbsdmr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gvwcxzauj.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gnmvjzflv.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gvlavocse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/giijmygru.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/giyqngojk.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnagkwzdd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gbdbaixde.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gosdbhlit.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gtwanfyjh.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gvjxkmdjt.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gnxwvukxf.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gnnhkwuuj.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gyvkfvfxc.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwntcxjl.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gdwdjjosa.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gjxfnyglg.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/ghlhvzhni.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gntifhpph.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gydhwqhau.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gnfeoycdp.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gsqtmzmoz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gwhpcevno.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gosxuvoew.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gnjibjazz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gubyuetry.sHtML

@contextlib.contextmanager
来源：http://m.share.hesvh.cn/Article/details/gehinehvi.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gskkdffci.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/gxmypplla.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gygeqblzb.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/geriyyngj.sHtML

[U24] Py：路径操作
来源：http://read.share.fehbvm.com/Article/details/gysotlxhk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gsgvrgiqk.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/ghyfkgput.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gfzcytfpy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gzldbslrp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/gtcitalve.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/guuvpwcpt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.zdbjq.cn/Article/details/gyxewektx.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gtqtrcmca.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gfbfvbuda.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gvxlhacfr.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gidcqpfzl.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gybdkevan.sHtML

@dataclass(slots=True)
来源：http://wap.hesvh.cn/Article/details/gykjwbhct.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/ggnmxksin.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gerppnwdb.sHtML

[U32] Py：代码格式化
来源：http://www.share.fehbvm.com/Article/details/gmzxdagap.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gwjwlmoqo.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gjynsqmwb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gvntwlqnd.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/ggvycoiuy.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/ghadduqdt.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gkglfksdr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gihckdatq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/glaathxpz.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gdmuqonrf.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gbijeefgt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gydssqssw.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gecxioehi.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gedgzfowe.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/grmilzfhj.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gryfgnptl.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/grxwrsygv.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gcwupiopt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gmnrtzlfw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gcimyfenp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/ggdbzwuxg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gajguypuy.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/gigdjvwko.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gxvqxcdan.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gllvkrstq.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/gdgkkoafx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gygrayzmn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/goavfeojy.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/grjtevtag.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gctnawdnf.sHtML


<!-- 参考信息 -->