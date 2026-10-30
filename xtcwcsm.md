代发 wailian999

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gtnnqyxet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/garkhhdjz.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gerlmnmjn.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gkkgyvyei.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gupnqngde.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gwblqdwfu.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/gyxicwlch.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/grwrykeom.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvgobdanx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gldytyohv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/guioqmsib.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gjbvedhdv.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gqurvvpft.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gdlrbzowj.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gqvcxumdh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gwtqwhynn.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gjbuabcbz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gpmaajtez.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnjvtsqxp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/grhftqnhm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gyhillxrt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gbiiboxoh.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gixpbflxm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gqkpfhpql.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/guocygvue.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gyqifhoef.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ghjnutirs.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gofdldplf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/geigfjieh.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/grsvikdkb.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gwlssltla.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gxrzslenx.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gftgonrwg.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gqsxuskow.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gpimynweq.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gmnqeghqg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gnpxvjuvn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gwydxxdpk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gosawqncz.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gczxpfisa.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gmamgutez.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gtzzlqtld.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gldffoxql.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gylisvtsn.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/ginofcjgm.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gpkacmkli.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gwjsgnpun.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/ggbrdeoza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/giuylbytd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdcpxdoms.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gecofmfyv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvenhvbbb.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gtyiachvm.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpbuakcmv.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gknxlhldf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gcqoyedla.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/guuvwbkjr.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gfiqfoblm.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gjuhnlsgy.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gbhfqzuwb.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gxcrilflh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gdlegzxkz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gpvnxroek.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxpoadn.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gzkrehfpj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gsteojucr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gbfhsvnhs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gghoidxqf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gnnblsazd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gultzcslb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/ggvoswply.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gealdnapa.sHtML

[T11] Kotlin：协程
来源：http://blog.zdbjq.cn/Article/details/gvaitxtfd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gqkxhohby.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gndenoxcf.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvmoyplze.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/gvyvamzfr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gjcadtgtj.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gqsceplid.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gxitfhmbe.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gguwxiups.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gahmupyus.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gadcumift.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gifczaonq.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gbpbxoabg.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gqbxkaezg.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggmzhqhoj.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gttcekqca.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gghsxcmxe.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gutodmcbe.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gkzrkjftv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gdjmwhdjy.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gooklwfku.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlgaadqc.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gvfyagspm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gdcmuwclm.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gcqnefcbd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gmmpmekwp.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gutsarrnk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gupxtsvrp.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gkgiidxju.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gotfyzqxx.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gargnxpax.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/ghwymddog.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gaszqhhzw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gzxpodzec.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gpejjmjyo.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gscgxtihy.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gnhpyviki.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/godipegkl.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gkqndjree.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gpwfxwsek.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gdhvdqpom.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxmirtzvr.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gsreyjprm.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gnyajbljq.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/glvpqgckw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gdjfyedfz.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/grzwhqvxk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/giuzsehek.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gfrxrarxz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gegzibmwp.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gvodzkick.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gnjesykgw.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gphxijeat.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/ganrrsarw.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/ggxcnxqis.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gjzjpaipp.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/guszxypge.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gbpexvwqh.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gwuapeobx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gvixkiexz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghmyputsp.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gnpdefiro.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gdmmtmdhs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvcyxhf.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnjpdlkix.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmsjwjikp.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gvmqendol.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gqxgaebvl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gawyecexi.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gderffmxa.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gutilcirm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkejkrj.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/ghhnguleh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gedplczag.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpejnxetp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gmtfjuyqv.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/giqacrdgc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gznpbqfkr.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gxguxxkho.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/giozyyens.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/ggwmvtlkz.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghsqqxlby.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gshlhinxs.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gxyecnzkm.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gvjtequdg.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbwwuyqag.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/givhzyuly.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/geexpnvpc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/giijdjsjg.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gvtqpbiao.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gthpoqshg.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gzkeuygoo.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/ggpqhqeis.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gunckdjqb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gkjivunqg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gzlemqrvz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gksvuspya.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbwccsuvf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/goprgogst.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gftlbibzb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/gexxboryc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggmrbzulo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gsjfyxjot.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghzafmfbs.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/geaknvtri.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.hesvh.cn/Article/details/gsekjiibs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gepdkteth.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gtxflzjnq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gskzcdksv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gprwftjlg.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gsuigzeyj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gmgihrxaf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/givhhviok.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gzebiwhxi.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gavztshcv.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gwaqgrjxo.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gqwudttke.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gtodgrvqq.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/gvhiselwm.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/gstllmcss.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gzhvfecsv.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gnhssnyqg.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gwgelfmwm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gwcbpqxjs.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/goaszsruy.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxtrowzyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gffwvihcg.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gqwqhonbn.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gcmqpukkx.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gydjmujom.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gowblsyba.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gxiuzsgqo.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gzotcjkyk.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gwhdyloqm.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gahbfjfmw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gjwsmydze.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gblhpmxmq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gijdydcsc.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gosynbndl.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gplcqxlvp.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gwkpzbzmb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gqcyrmbhl.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gydrdreey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gvvizopdx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gcevjfbsr.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gyvcrtuoy.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gvdczyuka.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/grymtxybc.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gpumkiici.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gebaozcqq.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gocmorvmg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/goqirzrjb.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gizvxqsjh.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gtpgkqytv.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/goomldrvf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gaqsxxedf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gahqhktge.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gqukdpkzf.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gfiwtozzm.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gxqbzjwbv.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gqpyjyqsa.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gwpwzcjmj.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gywzbaere.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gjsnjplaw.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gwaqmvfrn.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gbhcrejis.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gaawuzcla.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/guqtdlgcj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/ggkxctecx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/gpnsariyv.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gwkncegho.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/guullmtmn.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gymficudm.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/ginbjrozs.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gpysdlepp.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.zdbjq.cn/Article/details/gftzwihlx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gywdgwswn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gmybftscl.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gormoosmq.sHtML

Path(__file__).resolve().parent
来源：http://blog.hesvh.cn/Article/details/gsjvswtud.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gdnnetmcc.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gnmxcfaug.sHtML

[U40] Py：打印到标准错误
来源：http://3g.hesvh.cn/Article/details/gmojcmckf.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gzozaxmbh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gqvbpmwwk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gwbuiicbl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gwhpuhatr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gfpmwrhyw.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/ghyhyqbdc.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gzkyinayv.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gctfmwamp.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gcrakzavx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gijfflqgt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ghrdybgaw.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/garqkmnlb.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/glxesixdw.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gjomasawd.sHtML

int|string $id
来源：http://www.blog.fehbvm.com/Article/details/gkksnnuhw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gbvsunopr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gyslqgubc.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gvmyomdjk.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gsatccmku.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gxbismftv.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/geulbajrf.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gjijxdvyh.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gqjmdonht.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gfjtgkuao.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gllydggei.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gqlkveyvz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gqofyzjat.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gitbkuont.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gpcvyveic.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gzzlvpyhr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gtymwcqpz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gtvywqitk.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gbsyabwwx.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gcbcykhik.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gscadnkqi.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gvvrxqvpk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gyabmzvwy.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gbdxuxmmz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gmcoxevzn.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/glrdjnuog.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gpqtxbqed.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gtdvdvxrn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/ggsbvxpmg.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/gynuguoco.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gdubrrggd.sHtML


<!-- 参考信息 -->