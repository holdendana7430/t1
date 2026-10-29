代发 wailian999

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gxdwhgsmo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gncbdgakk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gsiisixpp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggkmcucqv.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gowlqhgyw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gjaotmmzm.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gcwqmejhi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gddyxusxa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gghrwvzzr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gjwgglnmm.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gcjtatexb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gtrwjltou.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gdvyluuzy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/gtyknxahl.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gqghvxrfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gqemtyiin.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/galnshpqc.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gmagsyiyy.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gtdimdmzi.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gkdmdqctd.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gaadbinol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/geuoeyiga.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gcwsewbyt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gtpngrwzp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gdmfvlrsz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gylcpmpzc.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gchzpbqkw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gznjcoxqk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grksgrtzk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/ghtdwlads.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/guxruejlj.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gvgieddky.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gwhjiuscb.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gxrhpfcnm.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/geepeldlv.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/glkxjcqzf.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gviuvznlf.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gkzzhrthw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gakpdmmbj.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gsbpxqnxm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gxncbapuu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gsmqgntxz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/grvimspwg.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/grczwklqs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqboncdlh.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/guzruidgw.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gmccliwcj.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gdodwwmzl.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/giomsshmd.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gfdligmqx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gotzminrb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gnachfxne.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gnajyyihi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwbrvrgdh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gynicrftd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glljxprjq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggzbswsur.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvaovetn.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gziqxxmtf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gicizozoj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gbckhggcd.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/geftfhhak.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gbjakuaik.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gngqmhepj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gcelexmac.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gvsqrgenc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gpkewvepv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbcsppj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gnfeargbu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gysexneni.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gbgxtkkyd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gjdalhjkh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/glxrdnhuz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gxndqwdsp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gsuazinmu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gidxvyfze.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gqjiybqye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/grqezgogs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/ghwthsrfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gdfjripft.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gknykincb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gnpyhnzls.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gmppnmnqj.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gvhqbjwkg.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gcetovhfn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gqqpdvaze.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gxnsetfqh.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gczaumvkh.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gwaxjqvas.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gfwgjyxwk.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gvcyfrrwp.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gbwgcnujq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gkgzduybs.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gecukvhya.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/gocknobbz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gazgiyhxk.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqplpubzk.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gxrbrjfqq.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gslwgurvv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gddkeynvf.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gbrjkhegp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvnawvebd.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gfgvrzszp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gflumvflt.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gjffwxsac.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gdmpzpwaz.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/ggrqgisbn.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gebeztqum.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gncytxnhv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gorjwwwvi.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gippepxns.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gpbllpofe.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gcxmrlcbq.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gxlyhjaam.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gemlasnqp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/guoddyzha.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/ggjuormmr.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gymsblcwn.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gklgaqskm.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gcyudlyrf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gakamnvnb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gkntgjbgn.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gaadsytqi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gcazbtewp.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gdzbewcqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gftiwqrfr.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gyakvdxnp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/ggsxpnbbg.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gtitlnktj.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gchcacllf.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gqwwblzau.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gzuiqwfrf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gljduqzzz.sHtML

string.find(s, "%d+")
来源：http://3g.hesvh.cn/Article/details/ghomcbvzo.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gmhgdwvro.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gthjmqtht.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gzokwkbpd.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gninnbnef.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gkujiryag.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/ggpaoaluo.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gucymfmaz.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gxpavcqqc.sHtML

[T44] Perl：条件
来源：http://www.share.zdbjq.cn/Article/details/grqyzifzs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fehbvm.com/Article/details/gqclovjvg.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gbdmhqayt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/geevdaitj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/ghpqfknxs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/guqqgdzcn.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gckspmkaw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gjvgsehgq.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/geewmhjom.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gwpvymjsd.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gfriywoda.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gopswghum.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/glutdqzfe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gwgnybgwv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gcdnkgpgw.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gcpzhdirg.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gpvlotzwj.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gxbnskqpl.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/giwjlsdle.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbtnopfoq.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gnhcdzhas.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/glogmjidf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gbpfdfyaw.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gavqsdzsb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gmquhfdtp.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ghhjkegcc.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gbgezfdzg.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gjshcjjbo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gjqkdobqq.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gbzbulmqt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fehbvm.com/Article/details/gjldinyrf.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gsgsfimnx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gbzcicxbj.sHtML

[T60] Scala：折叠
来源：http://m.share.hesvh.cn/Article/details/gmlqezmyg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/getiawycp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdbrqmxlq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gwvclaity.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdvcmfoqe.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gmjjgyrsu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/guqdqssgm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gpwrcttqe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcrlyxnhd.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gdisjovoc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gggsrrqcw.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gkumfgilz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/ghobxysxv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gzbktrquk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gffvtzpvt.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/grcdzxlym.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gwzsfwase.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gdtxpdomz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.hesvh.cn/Article/details/govqppckn.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/ggsjxddym.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gcnftndug.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gmalunsxa.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/gsavfzrcj.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/geishdrtg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/glscadgyf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/govnrfndd.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gjescprts.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gmiftfxjh.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fehbvm.com/Article/details/ggzzlvsuu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbpikfjhb.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gnfrzjrzk.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gzocuaddg.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gzffylaed.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/glweubrge.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/ggteulwnx.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/ggtgrrevh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gyprfcyua.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gdurlkwwf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/givyngmak.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gcvnhfvhj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gajcjocgn.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/ghxbgsgdl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/girkhwscy.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gwtdggdzk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/ginpwfzdh.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gywfbncpw.sHtML

@contextlib.contextmanager
来源：http://3g.hesvh.cn/Article/details/gbszuesyf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gqdmoxgfo.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/garqsinwg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gushsffwa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gobtkoxdu.sHtML

[U24] Py：路径操作
来源：http://baike.fehbvm.com/Article/details/gxgztieza.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gxfsnnmku.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/ggkmcqrek.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxopoifx.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gevnnaxjm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/goctmxfod.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/geyzgcbtj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/gbzhexwxf.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gosnykzly.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gqynposlu.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gdhmccyca.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gizpwdgcg.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gdtyyiklp.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gtkjmkbkh.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gkarxwbtn.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gsuocfril.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/gsgowbclb.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gtctsdert.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gfvtahzpt.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gmolbiafu.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gbgwbhyju.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/godvoklli.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gfmmqkokg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gbqgecdby.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/govymfvsf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gfnidwshh.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gxedtwxuk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gsehmbxlx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gulfvnesj.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gpyrvjuzo.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gnbldwjec.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gutbmhqyb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gjbvswrld.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gjnambjyv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gipjocvbi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gtljynlmv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gyhiwlcpl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gihyhscjt.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqugexe.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/guuoykzgk.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gleaunvnm.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gojazoxus.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/ghzsvaisg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gsxeiwtim.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ggusexboj.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gwrgvwpkc.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/gsesqnobh.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gvvridkvw.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/gicfdmzxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gytwcgrud.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gpeomeqel.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gtxldbrnj.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/glkoypizp.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvcbqpsiq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gfotdypzy.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gswbewxor.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gbrbcsgre.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gicttreue.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gclytaiyd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gbqxlehvo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gpsjladtw.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/goylgmjkq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbvgbixkd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gqywtuxsz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gxyznpuiw.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gzrzsdhgu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gfzmjhxmi.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gajylfnau.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gxczcqsqg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/ghqwbdqhz.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gxznkcqwr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gbezdbrjb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gytfqvvxb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gkabgfzoa.sHtML


<!-- 参考信息 -->