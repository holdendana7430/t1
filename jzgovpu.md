代发 wailian999

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxhplcpu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/geikxgmct.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/glipaqzzl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqkfimtf.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqclwulqy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxgusac.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbbclkebf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvqccnmx.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gxdmpyftl.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/ggudwnlec.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxlftual.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/groxmyuoe.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzcvcwj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnuhvriq.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/grufogbct.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrueubht.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdoqjxkql.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwwcxktp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggjhyzjxf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gvkmesgea.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqozssmp.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gisxipwuc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gimgchuif.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gkyqzhenw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvazhxukj.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzxxownu.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gnpxchviz.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqukoydb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyjiqytmm.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gnwlrevse.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfnalhymj.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gaosmuunt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gguvobicr.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gbsmhlzvl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwovolbxl.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gtzsmgtwg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdfrpmu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzevibtf.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/ggctomvie.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gjasmbtup.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gviggssxf.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvwlibu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxgvune.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrfhnxkd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpiorxi.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretqnogs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkisglago.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfcswbrq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grsncosza.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gmanvtaec.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmswtzjag.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/guzfacjlw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/glnxzjmkp.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gitmxkrrg.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohcggssf.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqfexpjql.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gpztfmjhc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytkchsji.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyggeeuv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gzffxjmed.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhtfhave.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfpomkgyh.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghrfolvlc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkynaiosp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbpqgwuq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gpxzbslwc.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gilzswiwi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gntwjposw.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/giobaxoms.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadvowopn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gandvmhae.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gkssdevnr.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/grexrhksg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnylkioia.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gxngddpqn.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gyshlgobl.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gntgnmfgg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gpojwykzq.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjvpvvsdh.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeurnpqg.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebesbdii.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gywcybrrm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnuqwheh.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/giuwezmvb.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gfecvdrti.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaphvnaay.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzrgietz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhrsoqdd.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulxwsdjn.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/glzzowbbf.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdxxdfjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gytbghdjp.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gtwmwgicc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkownwgb.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gfgadkidp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyxsxozl.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gouhujcos.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrygdpxn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/genrvzndv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonwpvwiy.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gpammvyua.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdigbzkpy.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxysbpjs.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasiqqcvu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmndojpg.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbkrxuzt.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/geewvfogh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gosznuzhv.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsprnnls.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxzdaubc.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixmpxpf.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gdvuuogdm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvxsgjab.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpkupyon.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgbapxeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/ghsgpvzhm.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxllsddv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgiojvds.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkveawstl.sHtML

function add(a, b) return a + b end
来源：http://blog.fanxiaobao.xyz/Article/details/gmawmidlo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gadynkxup.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyyrnzkk.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfzjuziuj.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtddjowl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/glisaihbr.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgfmeya.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjldvwzno.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvdxdfib.sHtML

[T41] Perl：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gninfvadx.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gkskniold.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqkyjubl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvywkqyw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkphagzz.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptrprylc.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvhjikot.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvuufrpd.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gwirxnduf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkntqkog.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqcrmail.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboaragev.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatxzlxik.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbdchjsn.sHtML

[T48] Perl：正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxauvyfeu.sHtML

$s =~ s/old/new/g;
来源：http://wap.fanxiaobao.xyz/Article/details/gkdcduryc.sHtML

[T49] Perl：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfjobpjw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdaksaeev.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxybkfoch.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqggsala.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gowrtihfu.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcdfupzen.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpbozfmi.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gihzvceok.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpvxabtt.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/ggtahhyvd.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtmxbfiar.sHtML

[T54] Scala：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/grksigkfn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gbqvslvpg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqucqbp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gusgxtmnv.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gxvegvmgf.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuaoxgsc.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/govsbkgwu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gqpmzuvja.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gwornticf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gaewzxshm.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtsqjxgum.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garvnqfye.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllmyipuh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcrergkf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnajwdfv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gjwbiiwxy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gieljmbuj.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgysdxfm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fanxiaobao.xyz/Article/details/gqukptqko.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/guwbnvocc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtddoape.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gyprzuxox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fanxiaobao.xyz/Article/details/gkykyxzsa.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgvjoahi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gefkeqaya.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvyxnpfk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/ghxuqzjsq.sHtML

[U06] Py：合并两个字典
来源：http://wap.fanxiaobao.xyz/Article/details/grdukthix.sHtML

{**a, **b}
来源：http://www.share.fanxiaobao.xyz/Article/details/grdxdrwgx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnaomns.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyroushwc.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtfskdsx.sHtML

[y for x in nested for y in x]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmafkelww.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqlxmrpj.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/giietxsqz.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gkofgfsog.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwuaccby.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjtiuher.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdtbfoo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjepazxl.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbvjapjq.sHtML

[U13] Py：固定长度队列
来源：http://3g.fanxiaobao.xyz/Article/details/gxacijzse.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gqdtseprp.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbrggnuc.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gennzcjvh.sHtML

[U15] Py：高精度计时
来源：http://3g.fanxiaobao.xyz/Article/details/gednqcybh.sHtML

t = time.perf_counter()
来源：http://3g.fanxiaobao.xyz/Article/details/gapkrhbnu.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyonxinuz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtdcqboi.sHtML

[U17] Py：初始化日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfvlevqd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gpyefcepy.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbmywkyc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwaajzme.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gguitilld.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdwdpsww.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjxkrcey.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffiheno.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fanxiaobao.xyz/Article/details/gdahlujop.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhabczs.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdxfemd.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbmjrmbu.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/gscgfpnkw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fanxiaobao.xyz/Article/details/gklpmpufb.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjfbrydm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqantazbv.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/gmcqoqmnq.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgbylrgp.sHtML

[U26] Py：并发下载
来源：http://blog.fanxiaobao.xyz/Article/details/gvokgejsd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfdshzdz.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gjbgitiwz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqwjftkr.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyucvdyw.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gomgbbsqk.sHtML

[U29] Py：属性校验
来源：http://3g.fanxiaobao.xyz/Article/details/gsytrdunx.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvdgbrxe.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgjsnkmg.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzpbqmja.sHtML

[U31] Py：单测
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxsssxl.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxezhuls.sHtML

[U32] Py：代码格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gmqsdizhr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.fanxiaobao.xyz/Article/details/gszfzrgur.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/ghstvctvl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpweumgn.sHtML

[U34] Py：判断编码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwbcsyum.sHtML

chardet.detect(raw)
来源：http://blog.fanxiaobao.xyz/Article/details/gdqwsdoyi.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/giavosxlo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.fanxiaobao.xyz/Article/details/gqelezqzh.sHtML

[U36] Py：定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gymdbehkf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnyxada.sHtML

[U37] Py：读写 Excel
来源：http://baike.fanxiaobao.xyz/Article/details/gtnfoinnl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyugbibc.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/grfbtnsfn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbjlqait.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaeyzcaj.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnprdcpny.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxspechg.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmangpjq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlhsdja.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gjtjxllvi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fanxiaobao.xyz/Article/details/gskfnsztg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fanxiaobao.xyz/Article/details/goclvsddy.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwjgglaw.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/gqrtgoqoo.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmyayzmp.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqdaenctf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwsyvnf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gewoftjly.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gmcasimwl.sHtML

?string $name = null
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfoprhgq.sHtML

[U47] PHP：联合类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnruobvb.sHtML

int|string $id
来源：http://baike.fanxiaobao.xyz/Article/details/gumprxkhr.sHtML

[U48] PHP：纯枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtzcqkrpa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrjprwjx.sHtML

[U49] PHP：只读属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gphkoijfr.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gznrnupxi.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/gutqcjjil.sHtML

public function __construct(private int $id) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsbbqenei.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlkbhje.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtzxbvga.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvparualf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgsvshss.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlpycovm.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/gvrzclowy.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkxocinv.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdlbtnzy.sHtML

[U55] PHP：match 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmxrfcmz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhllcelj.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuvpcmjr.sHtML

f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplytblcs.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxhclqdq.sHtML

"值: {$a}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkhduvipv.sHtML

[U58] PHP：数组三件套
来源：http://blog.fanxiaobao.xyz/Article/details/gtwzkvthy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gssmepvzd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfxwwzxy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/ghjvwfvgr.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gctjvhfag.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gxamrupbq.sHtML

[U61] PHP：正则
来源：http://blog.fanxiaobao.xyz/Article/details/glnmaqcrt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/grywcocuv.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/gcvmqfxgg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gnbqyksej.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrynkcol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdvbccfk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glccjzhpe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gupeatljk.sHtML


<!-- 参考信息 -->