代发 wailian999

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gtidruzqj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gtoyobbvy.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gwkgzvsdm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gqkywtaxh.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/guuavceru.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/golxoaqlj.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gqnyaxlvn.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gqlarctlh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gnmnemyic.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gcllzjgdm.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gxjgjrpqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/geyybfyfo.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gpgoreouc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gmrtyrvdi.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gdmlffccr.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/glooiapof.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gjyhqtnot.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/geghakldu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/glggtjnte.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gffsngeeq.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/ggqeaikxl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gokrlbvar.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gocdrknor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gzdzavlsj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gvczjpnqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gwvxxwxmt.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gvbrrtqrf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gpliwhcqk.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grrwpjufy.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/grehxaygd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkocdamij.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gioxfnkfc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxaaqscoq.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/ghtnppznp.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gshfvjlpu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gpqaqfqln.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/grjnfhbuk.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/ggsijylie.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gtsbexmis.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gkiepgftu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/gklyisnoj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/gcylasxtu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnrbupdmf.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gvpgsnttp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gdclifqcq.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/guofpfaev.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gnlmgtfyl.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gsdndmgrg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/ghwvbpinl.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/guynzvgrd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gwjlvyuny.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/ghkkzppin.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gycfilurt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzkmveqco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/ggvoawkxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gummhizhq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzmkgcqwm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gozqzqeri.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gdyjogdnr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gsxqvzrjs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gjztytssm.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/ghxewrdzn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gkfhzwnvm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gdphyrjzo.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/givnwzegx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gxemvrimb.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gvffnsjhb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/ggukmvdim.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/ggydxykfb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/goeimnzka.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/ggkmaordp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gqtiprfmr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gkqxyubtz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gkzdvkhov.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gfmhhnjef.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/gectsvgvs.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/ghrdlpqph.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gtshmtsvi.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gcvjskvvf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/gyxhgjzoj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/ghfkcuzmk.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gpsoyxqdi.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gsqxoauhc.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gcubylpkl.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gxsbscaui.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gjgqjzebo.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjxqpgxyj.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/guihgwchs.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gtgelqolx.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gdsimnxpg.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/grkmwiryd.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gujgzkdku.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gtiusoyxa.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/guvjxzyvu.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gyuzxbluc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gmhmopjvz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmdsvwofo.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gjoawshkc.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/geppijkjl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gxwgjoban.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gmwpqhjmn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/guvefwprq.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gtianlwuc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gcoxzlziq.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gsmmptywx.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/glrxbsfyk.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gxxkdxqdc.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gdxyfvkqn.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gfbucmpcl.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gzbaunuya.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbgdpnpfg.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/ghopssspc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gqbrebukg.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gbqrqzmww.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gueyqiyqk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gcbogyqvi.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkfpwfuhy.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gntbxsbmk.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gcqonozll.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/gmchmaftl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/ghgcsjzit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gahhypdxs.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gwtxbamnj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gelzuqntq.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gfmshdnan.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gbprpnocp.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gnfhnvzrz.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gferlihbh.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gkiilnsgo.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/ghwchvxgm.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gprjupcxz.sHtML

if x > 0 then print("正") end
来源：http://www.share.hesvh.cn/Article/details/gaickzdze.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gzuprifir.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gdsnjxbor.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gfvrkcbsi.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gjvinfnxy.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gmzucxjjx.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gynvvgpfg.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gxrgkyhxx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/ggorynrrr.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gkizwqbht.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gznezdrgi.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gcutwveyv.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gkwnvkxow.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gpqytempk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgcxoib.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/goiwpheqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gzkvcnoym.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gjjehkmpd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gqcponhep.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gbtdajnfg.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.zdbjq.cn/Article/details/gveulblbj.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gfcvbfgrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gkurtxpmt.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfkghltnu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gzgqqioja.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gfzlrujds.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/galzkainz.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gqqvkhcux.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/gyqwuihkn.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/ghzqmfwzb.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/greacbidb.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gwstbqinx.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gzigjjjnm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gkomiznlp.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/guipvraeq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/goccdkzcb.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gnafjzvjw.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gkgsvfbcc.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gstyajazx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gjhhkfgqt.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/geygtsflx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.fehbvm.com/Article/details/giojdfaqz.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/gvgzjdfpq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/ggtnptcmj.sHtML

[T60] Scala：折叠
来源：http://www.share.zdbjq.cn/Article/details/gfemyowqp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/grbcuzjwi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtptwrbes.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/grkeeazdb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geghtgaut.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gaclrsgxh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gamkodjro.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gglcfrjiy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gideaebck.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gopwubgxv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gtnkczozd.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fehbvm.com/Article/details/gbnlgneax.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gtmnceutw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gbhkghwwc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gvdugsjzv.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/ggkatfusy.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/glyxjalnr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gioqycwml.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gsmpubbff.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gqbvysphz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gljtifeek.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gchidrjpd.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gjddxetbv.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gsjunatmv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gxxacuuvs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gdggfzavc.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gtczikwrw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/grsatczdv.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gkddtbsjf.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/grclwcutj.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gcfexczsf.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/ghezgqbkt.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gryicdjxs.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gpihbhsht.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gzelrnkro.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gzekvuyiz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gfhhplwst.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gpzmaxqwg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/glbrdxxyu.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.hesvh.cn/Article/details/gwuwwqsak.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/ggdemyqnq.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gcwdpxpqa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gumojzryn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gqevmwlhu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/glrzgdghw.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gdvhegcwr.sHtML

@contextlib.contextmanager
来源：http://m.share.fehbvm.com/Article/details/gxsetiimo.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/gtcxwhcbd.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gyocrrhjc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gllxaisqi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gocmcsutn.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gmcyrtnym.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/greiirunj.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gwhufdhxo.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gwmxdcjuq.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gjmycecgz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gtngzaxiz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gtxrvoqsh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gdaahvvgy.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gddhhjowg.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gnbrfetjo.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gsyppszea.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/goxhzifzq.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gxwkqmnjs.sHtML

@dataclass(slots=True)
来源：http://www.share.zdbjq.cn/Article/details/gohocohhu.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gtrbmfwgf.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gvvgdsrkz.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gdlpxbqld.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gdefldyjk.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gfvjzwhnd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gdkdepucy.sHtML

[U34] Py：判断编码
来源：http://www.m.share.fehbvm.com/Article/details/gwsgtbjej.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gfftdqqis.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gniiantjw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gdtmigwfj.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gkgilotfs.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.hesvh.cn/Article/details/gdmulhqfz.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gmavjgakk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/guvrabrgi.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gkklpowwx.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gpnzunymb.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gmovshwja.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/gsjdnsezt.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gwoqylize.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjjntzmtt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gxzescpxu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/guwpzynvh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/gevbxfbjj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gqqjwvvfo.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gcnikzwyv.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gnlceizzr.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gjyovnpke.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/goyfijgdh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gnjohqjda.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvsvxoubm.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gpycevnjo.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/grllfuyyi.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gajtrwisv.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gwowkebzh.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gkzcrmchj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gewhwlaux.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gxmisgtom.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gkulpcoly.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gngtghaph.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/geqnegmhp.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gfyaeiitk.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/gyyimplsa.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gkfqbflqx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.hesvh.cn/Article/details/garmmcsbl.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gkjgrboam.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gjydambus.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/govwlftyl.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/ghlexlabi.sHtML

[U55] PHP：match 表达式
来源：http://m.share.hesvh.cn/Article/details/grgqzbgaq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gawbdzmjf.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ggfeklujo.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gecdnvnny.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gawlmzjzq.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gqlxdkhhv.sHtML

[U58] PHP：数组三件套
来源：http://m.share.hesvh.cn/Article/details/gzzhoginf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/grvjzqrxo.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gzcjcvfgp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gkuecnyhq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/geiowzwjh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gfcpgwsos.sHtML


<!-- 参考信息 -->