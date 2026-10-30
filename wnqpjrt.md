代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gnritfhfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gjuasdxkl.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gjxuojbrs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gambsficz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ggjnscntq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gyzhkwrjj.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gqciehenc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gxwzlkfjc.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gzpeqikhx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcfdngcw.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/geaitfwry.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gsldylmuw.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gqhdymzmq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/ggscovoet.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gcamlokrx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/grkywcskb.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ghbyjqfvr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gnheifmkg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfwsyujdl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gdqdmiysv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gnzbrslvb.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/ggvfyntfc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gsugeqnwa.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gudbjjxgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gygmefwhy.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/gyofoswjo.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gptbxxkrl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/guehpjvip.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gjvbgksyz.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/glewjsdlq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gwtcrkctj.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gbtuiecgp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/grsdfymej.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gvtnoqrbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gllvjanvt.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gamccdrdq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/ggcdfqzhy.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gnqnmacdi.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gtxxsnifn.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/gizbgngxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gbgpmvqtd.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gydlmiyld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gwobyuwsp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gfakrsuji.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/glwgvotrb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gahrxgoga.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/grhnhjbky.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gloehmsti.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gljompttm.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqtbyzmyn.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gioatkzng.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gtqzxklqr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glwkwient.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/giueghywc.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gmzdzdkgv.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gycxbswjs.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gwqgxwoic.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/grzzdypqu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gnhcvaafu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwgjgkqop.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gvrdnzhrq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gnoxhfckx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gonchhyah.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gcuddvcqy.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gaxfoxuol.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/goyobbamm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glihnrpey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gnaptllwd.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gkaeplwrl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gxoxmbaty.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gayoiwhwr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gkporcdli.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/ggoajphme.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gmqhqgwaz.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/ginstjgpv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gbhtabvzr.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gmcsjklju.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gzmwxsrad.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqkcrqjrk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/ggpvscabf.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gomtkvtua.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gtddgsssm.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gbqwjhoiw.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gfclaydni.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gxklisyzt.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gcsfsrefs.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gdlxhuibd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gviijsrfd.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gnvyeqhzb.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gihxofwuk.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gecvwdkpt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gmqfzhehb.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/govywfwew.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.zdbjq.cn/Article/details/gatzrfaks.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gfakdjocg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gybnefwyc.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/glniaacwj.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/gbcqrwhhj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gagvcleik.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxqhfcruh.sHtML

[T27] Swift：错误处理
来源：http://wap.zdbjq.cn/Article/details/gpcacfctf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gbmlnuhsy.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gtffvhozb.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/griflavee.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gjxtggtun.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gkquesbhf.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gholftokv.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gzalteouw.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/goifajvim.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grhfjcuey.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gabjaoify.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gtciwzrnc.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gjvbwtlfy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gjrvncyni.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gxhchvdvq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gvurpasri.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/gugalluyg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/ggcqagrwn.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gxxanqlkf.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gxtjwfpcc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxnpcjwza.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gtfrxegca.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/goeujxvhh.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gpzueahvu.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gvlizafog.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gqhurkdgg.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gdwqjzvxg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gawvdxciq.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/getsjdsfx.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gbqzroxsk.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gmlzkklhv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gjyrltqtt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbqxwjqib.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gungfczzw.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gzhrzvjyh.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gdlzqomtn.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gssjjiadl.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gcbpgujzh.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gqwvxezdy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gxecacigo.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gipyqatks.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gahqnctkm.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gezcuuiei.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gicdiafsz.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/greaaceaf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gtfxwivql.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/getkuozco.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gvyuvvnkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gyonbiiwr.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gppcbanpi.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gzumssmmt.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gswcggxwx.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gmkbkdsrk.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdpxgdfqa.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gmtnyklgx.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gfmbdjllo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/guhtnbovl.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/ghwgyexsz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/glntknhcn.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gqvyxfjbb.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gyhbqrafr.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ghohzelsi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gneiwrmxl.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gdzkomxmc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/giyzgadww.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gqwhjgvjx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ghgltqgaz.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gftxrefyw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.hesvh.cn/Article/details/gxygmxpup.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmawgbxej.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbaliwbyj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjoebaxfb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gyeixmdee.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gxarqvjzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/guopcgqij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gbrgrmxvz.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gbevnitpp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/gxqofpblv.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/gnholwuqm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gpzkdspre.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gxvdbxbmj.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gotokwuxj.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gvqofxaqo.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gyhnskdin.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gkjyhaftn.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/glhrcfsad.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gxqnuuwat.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/goxzsvxid.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gmitjxyjt.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gplbrridp.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gsghnoswu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gtvjpvvrf.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gqtegntfm.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gztybpveu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gnzjovuyp.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gofcgjaig.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/glhbouxtc.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gafrowate.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gktpistlg.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gopwlvwjb.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gbdacfjyy.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/glcfkbvkk.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/ghteqkfvi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gbbdchzyq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gydysklde.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/goiyopvuu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/grmiyaxun.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gjtpugwgz.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/guumninuc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/goemzsiqv.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/ghptshjnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/ggmoshahe.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/giyjnhzcv.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gkeftlvbv.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/gmlfeigus.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gxgqsprxg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gxaltkgtl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gyouafyfp.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/guoyreoyk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/godcnoacx.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gorzrxdqu.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gpqcdwouw.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gizftrfjf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/ggffwalyd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gjrnaexpc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/gmwftvjif.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gplvuowow.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gihaasesq.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gislzujbo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/ghkbqpopc.sHtML

[U30] Py：数据类
来源：http://wap.hesvh.cn/Article/details/glpftukpt.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gxhcnbjzy.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/giuibwwat.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/grxlirvrw.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gzyeftdrr.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gevreesgj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gbcwzecue.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gufvjbjgg.sHtML

[U34] Py：判断编码
来源：http://read.share.zdbjq.cn/Article/details/gzuilvrii.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gnkcfjshw.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/ghhoiwtjd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/guypwpibg.sHtML

[U36] Py：定时任务
来源：http://wap.zdbjq.cn/Article/details/gzustenqn.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gnlrtiuva.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gacicttfg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/gvnuxcdps.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.zdbjq.cn/Article/details/gkrqpeets.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/godwrwqse.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gunopbtpa.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gcglrjkzy.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fehbvm.com/Article/details/gdcfkzlaf.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gxnrikbxq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gdjwfmtap.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/gvdoufpxn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gheadetso.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gguknctju.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gkqanixyo.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/glajlxats.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fehbvm.com/Article/details/gnyxstgar.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gliuejpiu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/ghnromrzc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glchelkdj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gtukmaxkg.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/glwutzjkm.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gfxqlycfz.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gdtoqxcuf.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gybsxhbrt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goevgcasq.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gatasuvzx.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/grreckjsq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gjbscwvij.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqtvqzlhy.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gfiansjlw.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/grapdgedt.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gmldrpdro.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/gonvuyhtv.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gvovhcomy.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gocnwejrz.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.hesvh.cn/Article/details/gjoumneit.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gbvucnuul.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gidyboysn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gbrykmlzc.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gmxwniaip.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gfjmuoecg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gvbckqvsc.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gcyrntsqq.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gmagslrcj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gjotjtzle.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gpjoctwkj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gvhvrfffy.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gvzieemeb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gtuyzdkzb.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/grmwtluum.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gokypumzf.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gmluezmtl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gedaxdemg.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/granoaimd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gacntqimo.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gmnugxsen.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gtyextgeu.sHtML


<!-- 参考信息 -->