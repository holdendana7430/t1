代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fnrcusgh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zkjnigwa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vdbeddga.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dcionfog.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wxxiavla.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aepfxehe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3lduxlaqa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rojaoiiu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hzyoamss.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cffgybey.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nhhqvutv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ltbysljv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3tvrwdaxp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxtvoo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zibeiiqq.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3pykxhizy.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ksgxxpmy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ddetjfeg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3qrujmwim.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3nzkpgpep.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hwrjrayy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3nyccadol.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ygtfufoy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjikhxum.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gavpctkb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwruqhw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tvipgbrc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3simluwcr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lfdpgjqu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mwbukqkv.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pgqosoko.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3rwbujzcs.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3pxmbxrgy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqnclert.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3hmkxdmvi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nbyuhuvl.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3knrdutwe.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3znfkewvq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ynntsukq.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pyrcmktx.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hrfoacbu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3bqdueuqu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jojyuxwt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3avqllrsb.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkiiodrt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vcpktmlf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3lndhviwg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3loienxjx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3efolqawt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3cejywdcx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3magiphcy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3infjzfuo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lioqbrit.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3goyphcvl.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3eiliipar.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiabzsnr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xrzmktfl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3svedjyje.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zfudzcfs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3iyxakzem.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3azqhhivl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3kapsuapi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3yufpnlpr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3spidyfjl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vypiattm.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3agtufcjj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3uoweenng.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ezkmhfoh.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsfzxzwn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3uzpwwvtf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jbgeijeg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kwdhainf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3huklycbu.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cncfcfdb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3agwotvoc.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ioewnige.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nfyfmirp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nkwhrjpr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yaudqmbn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xkvrench.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxwrlkqd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3gwyyccay.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tlgvvfqf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3hqkapffq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qrukfbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etqcbmzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3otjlzlfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plfgmhof.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mnjyuodx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sghkilfs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ctbiufsk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yatgjmqq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3xcwlkkcv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3oslwgjrm.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pxygxgpy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3kbiisoiu.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qppkozbf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bjfpmicw.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3azhyiobp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cwxleczw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3camvmsnn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3uigzbmjt.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ynjxffhv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwnidwc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrecincj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wnwruudv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nhiwusaw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vdahiwgp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hzsjjppv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qlyziwcl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vxtxnqya.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3plnznrrg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mltdeovq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3avceephn.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3juuxtqdy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bhtsdtis.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3cuphwekc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3omsodabq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3apxsqfit.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tzelsyeg.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvmgdxoi.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3htrafsez.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tbtporck.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3gcyddshx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3lczilhgi.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3kuxftcbz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zcrtugex.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pjitqxnr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kvdlwold.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3joonowqh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3yjznyjuy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jtyttkqx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybmgbutd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qgownxys.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tnvweppw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdspxiax.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3wzpqyowu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3khogebnn.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3wghdjjdt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ajkdvdlz.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sopgleib.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bayrertd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dipqirsv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3puxkinmd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tmuezvni.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kcueicxs.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3xubhfcqc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jhbalqse.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vclenyge.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fexeqsgq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3advdwsxb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3anduqxno.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3nwnovmyh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lohgshky.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3koarvddz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ezltprfp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yvuewglc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tmrjvvxa.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkrhfakk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ifjqnftb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3djlhnggu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3srhetrdt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ysdgvlbd.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3nlwzxrfi.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3rzxajief.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3sojewmap.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3qmiluyde.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3pbblzbnw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3znoqptds.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3zyoaimjy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3oyglmsgx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pzsombgi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vybzpnez.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wxbjmsxo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nhaarvwq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqrhlbi.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ndtpoyeo.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ubuzgfgs.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bycozzbu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhbtburz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sgbrwlhr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mmryoszp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hcoukpuq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3hsuiasra.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vcltsilj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tvczkklu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fzfxerhz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gknoqtly.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcbmfavi.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jclcxnzm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kajogbxh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pchmbkli.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3anflfvoq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wwvncpqs.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3seeumxrj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mrooznla.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yiopeuzs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3xjjxzsgu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3erxqwdnt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3frmoxfpb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3srzcrtcg.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vjkbgyfq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zbqitodg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3dhsqfxea.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ikibuheb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zwoxmucj.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xvhjcwzn.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ktlztpvp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3euqoomwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqzmyxfx.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3inmnpype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyuinyxc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3cckquptx.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3uoqvczmc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3zeeyreig.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fzrdlsmj.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rytqenyz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kyggdecq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3sssoujxl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mkwxvegg.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3tgomxcya.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3upbiwvnj.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3polrescl.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3rqcrwyhd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3mgybhqbb.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nlzxddxp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3iizmglid.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3tygosavm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3varpstpz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oscjdcdq.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nusglckn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3fjtfpvim.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ihcsqtik.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3kuaoiyqt.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3wkylvqhz.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sivehbjp.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3qwhnvqzb.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjiksvc.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3ilwbnfro.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3fghgndxp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3tsxcaydy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cbmixrug.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3peapdyem.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3nxzwfkvg.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3hqptcwrg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbnsfqh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jvznrrdg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lnxkksld.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3baypyabm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gppcmbvq.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3oevjhuss.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3sxiqnziw.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3juybtdtp.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fjovsmqp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3poatscza.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3glxvuoiy.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3odpvmtgi.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3skvirfcj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rmrfuwev.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xlthooto.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xydmljxo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3sdadpqvm.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3batcgvpd.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3lubfnqwk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3rgiqlaxt.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3dsphevtr.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3rxvsvqsk.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rbmhfqys.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ggvucunr.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ikknbadw.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3naxetjan.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3rkcvtbgx.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rjdmfidu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ifsaytqr.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3qbhmyksn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hgmmddcy.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3wpckqyfb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zydcvdgq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3gyhouyxl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3rlbbobip.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pkqdjazn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3deqecfyk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ugmqngrp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3gravhmrq.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3xrstsbym.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3jvxssixs.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qvnwgvfy.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3rbxlupoo.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3nguegxrn.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ygbogtbb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3fpzxhfbp.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3inylndrl.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3rbrssdjo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cwkgllbe.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3zzfowxkl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wkhuxjna.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qyjacxqs.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nrfgxpdl.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hdyecwfh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwcqgd.html


<!-- 参考信息 -->