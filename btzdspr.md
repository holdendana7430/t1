代发 wailian999

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gcoknnalc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gurzhmcom.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gkptugmdm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjvxhcahm.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gtgyiaalt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gdonrwdts.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gmgnohook.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gungziijy.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/ggswxaztz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gsohmqpuu.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gqnrpepat.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzfqsbuh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/godbujtka.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/ggtnqmbld.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gfuesjbfr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gzoyveqdn.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gexzelfyt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gmcenqthn.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gidrcsgby.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gabtlwoid.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gqlcphtwl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/geqejsaun.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/gamluynza.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/glwgnmwkg.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gukahrjxw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gctusobpz.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqegxceqc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gqetwsdqk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gdffgbwbv.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gtmjdqmxp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gtxcrgeod.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gwefxglzo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gdcpkyqtd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ghzcmpqhm.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/grbcyetby.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gbwxidtts.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gpnpigfbj.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gfvkichud.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/glpodwafe.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gempbvenh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gdmrzejkc.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/ghowmzssq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gjhyvzzxa.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gsqriwdsx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gdgticfpb.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gxcwvkkre.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/guumzbkti.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gyxrnseak.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gioemvhum.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gyigbwofc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gxinkorte.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gplqmnkpo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gphptkojk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggovxdvlt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gfwqxovyu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtkysoymr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqbdbgocx.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gadddtpvv.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/ghatxqbwm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gogjkpylf.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/grmmfmbjx.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gnaxanmua.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gzkzrvwyj.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gzmooctzo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gcackkyaj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gqylybker.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gbboyfzku.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gvkldzqcg.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gmimmwthe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gjqpnyzsf.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gfkvhvtjs.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gojudeavk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfiagfg.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/gfifqugrr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/geuueqfrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gmypbwrri.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gffdksxco.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gzouzsqqc.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gswordvvi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ggndickgr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gypgggfgl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gmadbzjzv.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gzjqiaunk.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gcpqenrfh.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/gqcdloxjp.sHtML

interface Shape { fun area(): Double }
来源：http://blog.zdbjq.cn/Article/details/gzlqimwah.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gmwagqeak.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gzviqvfid.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gyhpxbzae.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gpmkopnub.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gwindpooa.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/giryrkecd.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gqxdwrbnc.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/gvcpshzmb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gnhehokcu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gwhjmonaa.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gsvvrxqbb.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/guerzewab.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gonufnyfx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gpwecnlbu.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gnvenrsfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gldcivekx.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/glmvjffgn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gscpopixp.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gristsmmj.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gfneckuah.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gaolansgf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gobffzblw.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/ghqpszisz.sHtML

do { try f() } catch { print(error) }
来源：http://baike.zdbjq.cn/Article/details/guexailur.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gzowuqjhh.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gsxtdfqqe.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/ghkpusgsy.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gmevfnpua.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gtzkobmct.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/glaboknku.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gcnrotvyk.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/glyodclqs.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gouurrgdm.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/glbsortjc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gmkgtbunf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/giqkotude.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gbmxejasq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gkkjbezqj.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gstzmhnnw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gxjcmilyh.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gucqovlow.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gtazcwkmt.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gxfqwwvqa.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gjombyqua.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/govqtoopm.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gppgahsyf.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grzqcozjh.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gaqfyevdc.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gykaommfu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gcctrklow.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gplaekcew.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gjnbvqpcb.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gtcwzjjnc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gnzwcyslv.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggqneremm.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gtsjgskoz.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gryeobnki.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gimgniszv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gvlnssfli.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gpagblbtj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gqeeqvnsy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gwqnhkxpd.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gjymbgxhg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gkwiakvii.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gcwzmhvjw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gjdalevmk.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gbakmsgui.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/grcmyayeb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/geddinrrn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/ghhgwqbze.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gcgcttisf.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gcbhpzzmi.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gqkozohde.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/ggibvayip.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjxviqk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gfolhluys.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/glinqdqdg.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gtyjujyim.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gnxvlrlds.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gvtdktrwp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/giobuljvx.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gcktqhpvj.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gtwtphfsx.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gexgoqfzu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gxouibajj.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/giuzqpahj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/glqyfhybj.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gyhmovkpk.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gqrlxywzs.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzootef.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gpvddqznt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfuuhxhoa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gvgidxwcb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gekykpjka.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gnvcpvuty.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/galimkase.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ghtlydagd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gsfygblvo.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/ggodqrlzf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gdstewdck.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gcipnxeip.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gfrkdecfy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gakzsjrnh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcweemftx.sHtML

[U06] Py：合并两个字典
来源：http://www.share.hesvh.cn/Article/details/gmrbdvgpz.sHtML

{**a, **b}
来源：http://read.share.zdbjq.cn/Article/details/gyurroiuu.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gtkxnjolg.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gkloihiih.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/ghivlbsee.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gswehudwn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gvsvlgpfp.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gzpkhqywv.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gabhebyju.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.zdbjq.cn/Article/details/gewgrkbuy.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gbqxownhi.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gqcevyvdh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gxoxmnpji.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gjgbdaqco.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gbileerdk.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gxjxubwpf.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gssaircie.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/grnnfnqju.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/glwrfrpfn.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/giqlpcfwl.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/gfafqqyho.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gzkagjyof.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gleqkkrpm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gxdoruapz.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gwjmtfqzw.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gugryxxyt.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gnameysrx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gruzxsnow.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/glqclbuwo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gjruhczcp.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.zdbjq.cn/Article/details/glkcqoukm.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gyqnhfabx.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gucdeycog.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gtnooligd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gdntxraik.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gyxgxetcp.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gteeltpbl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gqfflkscp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gyvkaifbt.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/ghsovgwap.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gkwlnlswx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gkpaykjnk.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gbiahbmci.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gyxvtmqss.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/grqddfrql.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gxshsxvsz.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gbwrbnqhn.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.zdbjq.cn/Article/details/gutxecnni.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gzjxhwhre.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/ggelwndpp.sHtML

[U31] Py：单测
来源：http://m.share.zdbjq.cn/Article/details/gjqbcljvk.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/gvbsysovu.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gubhawiie.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gpkgewlzv.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gnxagrywc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.hesvh.cn/Article/details/gevgpyjxe.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gmcnnmorn.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gtxflgdvx.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/guldfvaik.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.hesvh.cn/Article/details/glzzfjcue.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkhtoruve.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gulumpqdl.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/godovsflq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gxudlymat.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gmcysocvo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gahkudlle.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gewsobltn.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gtidvpvox.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gmmnbdkrh.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtzayzzrx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/gallnmgkt.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gjzclbvag.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/giclgubrg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/gcssmpyzt.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gcpminqgu.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gaujguttx.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/ghammbnaf.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gjxkfrohg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gfpfmqkdn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpprqhqdw.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gimytityc.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gvniuaokw.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gotsmidhl.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gwtttsoty.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gwoizugqu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gkaoushbh.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gdhwjknig.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gvkpphoxg.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gnwtwakvb.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gbvjvgumv.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gtsmltuma.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gyrmlamqq.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/goyjprylg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gckdivzbo.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gqznczxbb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gfnyrwkwp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/gcnzhzcwp.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gtwujajpt.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gabvgzswy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gwrmohcwq.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/ggmqjxyon.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gumdpdlws.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gknobzqei.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/ghhrkrwun.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gcoskmadx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbokquaa.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/ghdkpsxcy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gzblgztau.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/giajrmhpu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgvvkih.sHtML


<!-- 参考信息 -->