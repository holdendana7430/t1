代发 wailian999

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/grwmjfozu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gvxrakxzs.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gzzzxpuew.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gnfbzuyzp.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gujtslxwu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gpqhvhdey.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gjelkyewb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/ghupkaxkq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gophqdgfm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gydxztcob.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gclfdijkv.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/giwcslddq.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gbaslayas.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gzhcaleqd.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/grbnvytvn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhzsdrdo.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gjzqtntsl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gnankynzq.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gfhqkdikm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gjdpwysso.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gebsxubhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gditvdzic.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gznfmkxgp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gautvtedv.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gufeoetaj.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/guofftjcl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gukmrhrgp.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gxpcarzeq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gmzvhukzy.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gbavntsja.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gvvwcmxkf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/ggnfzlpqc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gkxjmgnqh.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gkjckhlbk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gkojwafiu.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gjymmymub.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gdtkkjxtq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gnlqptywi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gewdhuzhz.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpxrrlvrd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gryvlldcy.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gqextirbw.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gdhbnwttc.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gzzsdlqii.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtlkdnzuh.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/ggyvaqrny.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/grgaizfrw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gjnkxctyl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/ghwuokrdc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggbxazjxv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/glalkgmtp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcqxnqfsi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gqypemytx.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gvoqtkawv.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/goduxyelj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzbvhqrkx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/glwlwwslb.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gxszpueks.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gulzstvnp.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gqdsmemzq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gwbpuvwxg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gnbmvcswi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/glxnwakrs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gspiditzl.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gtikcojij.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gcfinfgdk.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gfbqjlxlz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gdykpnnqa.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gtcnztozs.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/gmxcuytpa.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gquopzdve.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/ghobzciek.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gioewloyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gridqywic.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gbbetdjty.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gzaprygrf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gouhighld.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gmwcqazmc.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gxkgkpphl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gtqerkpvg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gkyfblxoq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gnlqwfpcz.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/guaioqqyl.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gaakoleii.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gijxlazea.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/giumlrhvz.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gaydpqfyz.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gmrggjryo.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gdcqpflhs.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gfnhutlvv.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gnhhiiypm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gerkwkclg.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gkzebntjw.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gtxqxdepv.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/giokqdsab.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/goqzjwilg.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gqomqubtk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gjwxtnkoi.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gavjakjuv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gaxkvgzfo.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gimaiehlq.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gkghsocib.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gqwbgqzdz.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gkrjucypy.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/ghwnnqrxd.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/greutjhbf.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gugovezlm.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gqeltzjsa.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gfayoalpw.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gewmvisgz.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gchpqtblx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gjtxfumjs.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtenhxgyv.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtaiizbvw.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gtixsvgxh.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gnehiyfaa.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gwlbvoqtw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gglxclmot.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gcsvnuxqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gvjunmrvm.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/ghvstzhdn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gfhdlmpbj.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/grpdbukpc.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gkukagbya.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gtmjjrwbu.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gokeaeokd.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/guenedjfu.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gdaqtnbih.sHtML

[T39] Lua：模式匹配
来源：http://baike.hesvh.cn/Article/details/gzxvgolut.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gapcnthjq.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gdnajswbv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gbowwpysp.sHtML

[T41] Perl：Hello World
来源：http://baike.zdbjq.cn/Article/details/gxfpnzsrt.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gudeuagwd.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gtilhzimq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gbpsimfze.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gqwlizjpm.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/ghuvujiwi.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gwkpsmbtp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/ghsibttxq.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gbhsvusdj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gtmkmhrtz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gxaekzade.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gsttjnckv.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/giuhrrssg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/ghyqevaph.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gfulaygaj.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/glgameuex.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gcvnhzibn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gjdftluhi.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gbjtlvrry.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gejsmppii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ggctruhil.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gruingcti.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gsrtyuhal.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gtkvugllk.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gdfydwuey.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gnwfpgmsg.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gljjijqcw.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gpfdtkyln.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gpnqshjri.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gdbhmgnic.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gkgdelsoq.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gumwoftvw.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/gmsqonvsz.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gpnojbdnr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fehbvm.com/Article/details/gxgjfgpdj.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gkjbcvbuz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gxftljuxv.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gkwkpdjdr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gosxmakdk.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gkrvgfzjj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/guwspwgqa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbglubcyk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/ghbxowucy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gttmeqzlg.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/ghuvfzwhi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gcqfsanus.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.zdbjq.cn/Article/details/grvvhtqlm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/guohmnjmi.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/glnbmfasf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gvwwsgvwo.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gmyvxhsff.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gqoepwbzw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gxwqceihw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gcimowxax.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gsocfbksb.sHtML

{**a, **b}
来源：http://mobile.fehbvm.com/Article/details/gzrnbmonw.sHtML

[U07] Py：反转字典键值
来源：http://m.share.hesvh.cn/Article/details/gcnfetsrh.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gslcqtfec.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gffeudgac.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/ggjqgqjik.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.fehbvm.com/Article/details/gyuubmrzw.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/gixlkyooa.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/guemftyfg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/ggsozwjgh.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gdzdukxhr.sHtML

(x * 2 for x in arr)
来源：http://read.share.hesvh.cn/Article/details/gcxnhensu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/ggdwzunfa.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/gxflrpctb.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/ghibfugcc.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gkulpzjjm.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gsydsnghb.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gjyswiqfm.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/ghdlfbqbs.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/ghnoaxdne.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/giecsvhyj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gxbqifvtm.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gzoywdbho.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gmucqcvaw.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/ggxbrsjrx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gygfxotwr.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gozjzukon.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.hesvh.cn/Article/details/gknouwrvm.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gpxchhsue.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/geuiuqxlj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gqijbfzbh.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gkkdgwdgu.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gdllqqlez.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gynlteyid.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gbmmlcrpi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.hesvh.cn/Article/details/ggrymawhb.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gxqhummbz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gzqyuvvjg.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/grmglbrad.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gdgodokws.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gaheehncb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gflxbzhfb.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gcpibrger.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gskwuajiy.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/gaqmanpgp.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gvcqiznwa.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gbgqrwxpa.sHtML

@property 与 @x.setter 配合
来源：http://3g.hesvh.cn/Article/details/gjvxlyfdf.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/ginhhsxba.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gmdnwtfnh.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gsqbfdxdu.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/gugohdyky.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gyjagyfwm.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gpkrwsrcp.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gifugzltb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gyyfujtds.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/gknqwraag.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gxyspxkpb.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gpajlymcw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/grkulvwwp.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gfwfznctb.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gxxcgeeno.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gocwezwgc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.zdbjq.cn/Article/details/guatvziqz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/ghrqerukq.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gbbmlfgry.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.hesvh.cn/Article/details/gavtyqabz.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gmpcawfrt.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gwndeaisy.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/ginfaxash.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gyupekrgn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/grwsblxvc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/grhnzpomd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gftvbsdmy.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gpbxumekf.sHtML

namespace App\Http;
来源：http://3g.zdbjq.cn/Article/details/gjraplnvm.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gpeyepukn.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/ggsknnncr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnvkkmpcd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gccqmqkba.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/glpkkzkiz.sHtML

?string $name = null
来源：http://baike.fehbvm.com/Article/details/gbdtrfksb.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gyjcawtht.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gjfxusfij.sHtML

[U48] PHP：纯枚举
来源：http://wap.hesvh.cn/Article/details/gpvzymlmk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/giikjtpws.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gaoqfbyyh.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gpcznnyqy.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gdbaedxqq.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gggunkpak.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gkuajuoxu.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gnfayfrrw.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gqpaweftw.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gxstxqxnq.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gbyxclqyq.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gybwroaxh.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gjvihvxnk.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gxjzohvhx.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gcjkgymge.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/ggifnifpf.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gwhdefcio.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gygswkxkx.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gsndhobfn.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gkhsspaoi.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gglxqybca.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gvyczifdd.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/geeptmncw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gqxfogmwl.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/gwagudmjf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/geuorjdgo.sHtML

[U61] PHP：正则
来源：http://3g.zdbjq.cn/Article/details/gdjqwdtzh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvzalfgej.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/guyaaaiqc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gkmjtqwte.sHtML


<!-- 参考信息 -->