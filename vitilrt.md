代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/ghtnulbdh.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gyffcqdfk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gzjkdutvr.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gxjzkgebn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gjgekgnar.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gyqhgowmu.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gebtftclb.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/ggenedzlj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gipnhbwrp.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gznxpdger.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gkrvfxvcg.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gapatlsev.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gihmgsjiy.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gpwbeueni.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ggaiwhcpn.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/goakhbpmp.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gosmmqcll.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gujbykqck.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gdwqqjral.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gwwtmfmwj.sHtML

#include <iostream>
来源：http://www.m.share.fehbvm.com/Article/details/gurdogppk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gydmqtjmw.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/golxrqgch.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/gbaxeizxy.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gmcyezqvq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gmsjgjmsd.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gsgrwupic.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gexozuclc.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gitggkgmy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gihkggghe.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gmcyfzonk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ggardjvrt.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/grqygbzja.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gaacbggxh.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gzbnyldxg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gmnertznj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gfrlniyxy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gvebqjvtg.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gwlauipsz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gqwjhjohu.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/gwucplhai.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.zdbjq.cn/Article/details/gjmvidneu.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gfisasivo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gsxudxwxe.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gmybivvuj.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gpiudjrva.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gsowsfvfq.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gxipfeccu.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gduqeohcy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjekzdbeb.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gkttwcgbx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gncwcrksc.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gbkjrcyjp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcbxvrbbu.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gledemgkt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gnyvmrgji.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gaxsroeuv.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gcffaivcv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gnlxduxow.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gtnxwxayh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/ggywowirc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gvvdrcyhb.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gkeigcuac.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gnbuhgikt.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gzafithgt.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gsodjthvw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/ghxtestqt.sHtML

[S54] C++：异常处理
来源：http://www.blog.zdbjq.cn/Article/details/ghyshgxmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gjulxoumo.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gngpcrung.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gtgmmngoa.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gxtdovtqo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gsjqoisrh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gzrmxjvfz.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gldasnbjq.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxmqheqps.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gsxtzwxey.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/garhayjzh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gunaulwdc.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/ggaxjjnvd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gckrhugow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggckzqqrf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gedssnkgi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcapyqmbd.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gmgxsgbzg.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gvzgzvvfz.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gsqqtgigo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gcgaooumr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gtykrqyjk.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gkxwubgqe.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gdmvroibm.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gsvcoswmw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gegylwvmy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gedfwdvlj.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gknqpmtsv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gzjwrujbq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gqnvmjxae.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gfqnjpsuo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gqsmzsouy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gfoujhdnr.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gyhrioaju.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gwbalkltr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gplnuzsmf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gyqfwkmcj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gluifcrvd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gucilzfii.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/ghmpokvje.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvnsszzeu.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/glmuumlva.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gstbeayvb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gekvukvau.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gigmoxprv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gpxzrinis.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gmftmumxh.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gujxbwrow.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gzponxexo.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gbftphkbe.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gflnsesqy.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gggvfbvzz.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gdsomaliu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/ghkhhbpvc.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gnmwwizcj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gvzwaihun.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gvsxeevbh.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gazdnfpea.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gwzfuxovl.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gfrmbiqwg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gyrgwjxub.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/guifezmib.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/ghaboiogq.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gyhkzbasm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcvetzbff.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gkwvykcqa.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gblknwzca.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gqgqvjvkh.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gxurmwuqy.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/ggvkkjjqz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpjfuubo.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gmnkcbobd.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gwahqgelw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gjqsxqnyw.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/ggepsurud.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpjnfzx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/ggqajrizz.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyqcenhfr.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/guoqerrcs.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gfympllpi.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gjwckzddh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/ganhxxkzn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gmqpeggba.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gcgcnwgwp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gsekxecxf.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gazokhvjv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gnqrvzxfv.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/giraewurp.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gpblrfnmh.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gjbazjyes.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/glfdlwqak.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gfyyyvzda.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/getwgkrwa.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/ghqmnqkzc.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gqnsaolro.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gdkhargcz.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gvkgsrzxe.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/glhpmkjtj.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/goleqljig.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gglqbrpxc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/gfeonwoom.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gezxtzoqf.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/ggrbczvoa.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcgxljjua.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/godsylgou.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/gscnjdhrh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gmzmqbino.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gjiqzmqpu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gqpgukeaf.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gumscijma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwrcqalxw.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/grghhzmef.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gwblyegue.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gagtwyeck.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsvsjdhfv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gaxbpjzxl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gmmdmmosa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gqvppfthg.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/grbjutmni.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gjcutbvbl.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gvhvsdosg.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gqzzdjmdh.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gurqsmpqy.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gsqpggocd.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gtnldvmzl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/ghmctdzuz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/giwyuoqwl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/grqborlee.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gvosuqkxr.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gvclxwdke.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/govlfddyp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/gpeytizjk.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/glpaaeaiz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gpylghfxq.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/grqocmdzy.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gxwlznnac.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gcvavbjzu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gxhnbuimh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpdplcila.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gkzxacaef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvbtzxrlp.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gwnskgfls.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gstcaefuw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/gdublpuyl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gmcolfkck.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/grupiyfye.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gkyjeuylk.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gqztzywcf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gvtsvgymu.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/goyymaakb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gnhjemgxl.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gtcgghvxh.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gfjazwzzh.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gkjuctrwr.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/gofnssqvm.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gphjrbphh.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gwtnbgvqh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gxpkgplxb.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gvxqnssbo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gjiziojvj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gppnoswjj.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gkqmzruzw.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gqlqniaam.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gcheurhac.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gujtxzkrf.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/gwrthknsa.sHtML

deque(maxlen=10)
来源：http://baike.fehbvm.com/Article/details/grwnjfjdb.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gvyjnisxz.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gonihuqzi.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gucqofjtx.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gczeyyyax.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/ghqtfgytc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gmppujcth.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gbfnvopgg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gpeldkfez.sHtML

[U18] Py：预编译正则
来源：http://read.share.fehbvm.com/Article/details/gxgtfewgu.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gungxhavf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/goltfhajp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gkyutulqp.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gnqqyclsv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gglhmjosz.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gsuyokonf.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gnkjyubzs.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/glxpsysyb.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gbxoyybwz.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/grfoxragf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/gnzwvxnin.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gpxahozhf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmvejxlkq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gcatmctgz.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gsmtzzqsm.sHtML

[U26] Py：并发下载
来源：http://mobile.zdbjq.cn/Article/details/gztaobzra.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gmdlfacgv.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gnhjtyzwx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gbpukjpsj.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/ggysfflhp.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/ghluenncz.sHtML

[U29] Py：属性校验
来源：http://mobile.zdbjq.cn/Article/details/ghkbaqgse.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gwqbqhtpb.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gdmkgdlsq.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/grecihlnp.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gtbvwlsuf.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gxtipjrnn.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gpotteyhf.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gyyllhine.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gzovbyihd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gmtscpusr.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/glbckfssw.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/ghabslysk.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gqoxmlomj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.zdbjq.cn/Article/details/gtgnqwath.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gymmqcgiv.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gdpuurphx.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gkmqxunyu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gxqchwrau.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gvknfloip.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gvitghqbr.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gbisyqapc.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/ggqtbxsmf.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gnxjwhgjp.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/govedccgv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/glslolalp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gqmxzsqte.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gkpidhsiz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gxgdyxnox.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/grmxokoxj.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gylxudklz.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/glsuexmue.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfulvrdp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gviqikrwt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grfosyffw.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gsjsclosw.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gvagnyedf.sHtML


<!-- 参考信息 -->