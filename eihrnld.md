代发 wailian999

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/grtrsdssf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/ggldqftwg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gnhddcatn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gzjqxnyjq.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/guvncewom.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gfovrmywr.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gbxlxpgef.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/grgranjpg.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gtweiqfmw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fehbvm.com/Article/details/gqlvznlwa.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gqqdozvem.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gcifsdwhr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gftairfyh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gkjcyqdxh.sHtML

[S48] C++：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxcchnpix.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gjkrncjfh.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gygwsftxx.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gdcqglbix.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gcpaoysex.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gvzbqdusf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gaipdznot.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/grgfmidpz.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gtpvmxbge.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gxlgaikdk.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gamtgmkdc.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gkckclkdc.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gbvwtwtdx.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gveftmqmw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gsrodxngv.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gotfmhssp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gdsknfvws.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gkwtjxqqe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdszzswo.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gypotlsnk.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gucpnrglt.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gabfmqfwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/giqqrtknr.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gcsktvvxj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gnwsgrcrs.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gsaviaexk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/geovjtscs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdketdghs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/guuwdppze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqgcufcqo.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gedewjtyo.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gcwwdwgzt.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gljjehmec.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/guglwyboe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gzolsiuop.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gyyoutctb.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/goauuhjau.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/goajfqwzv.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gqcgvybkn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/glutawmix.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gusmcwyuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gwncolhuf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gvjaaoime.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gusxowmtc.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gcmtggiuq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gfpjivvxc.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/giqsylvrx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gixynpgnh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gaamjbfro.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/ggwfhxtzl.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gigsbynxc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/grppdlsxr.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gonilypmo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcjcosbwp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/ghgfmvizt.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gjarfgsjw.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gaiwbnvyw.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gyjomomnm.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gvjdvkvhl.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gkwudkssw.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gzcvcgvgp.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gddolivzh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/ghezsgdkk.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gwgabafjv.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdxmduxht.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gmfkdcvgw.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gqbpbefak.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/glgywaehp.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gwuqquagt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gegoqmvtr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gasrwtkzu.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gbskmgvig.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gpbqfzyzv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gubotktuv.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/givyoevxh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/grfuwxvsq.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/ggaflnfrq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gogclkhqb.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gnebridjm.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/glxvwzthb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gqiyriyfl.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gzqyrawpv.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/grcnhmner.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gbrrefqob.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gpbijltpo.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gapspuung.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/girzxtcba.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gqtyzclum.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gkpnauseh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gbronshoh.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqitlttru.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gnklfsarq.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/gcepodqgw.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gytqapbdj.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gmmqqkqyh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gtzhkcirk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gmczlwpfs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/gwmsjspmi.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/ginhjccok.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gympzxzyl.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/ghndlevsx.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gncuiykmc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gfowjchtk.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/grglpkibg.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gjqfittlb.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gicerihyd.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gcvzfztzv.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/giwxwgwlb.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gcnpqxzoy.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gyowdbvju.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gteohwnoe.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/geukrcksa.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/grmhgryuk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gupufzttn.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/ghzuqfyin.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gjfevsbuy.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gwimzmgbw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gwyfzkzxr.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gpwehsicu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gunmhfkra.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gxclunyzr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gggiviojv.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gmyesuacg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/gjckjvqsd.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtyfuusto.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/glvfctvyi.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gdgrekzgo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gwmkletfu.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmlbpzmvd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gmhottbsl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gywzrewpe.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsnafakyp.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gftmgjkwt.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gvpyttxbo.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/grashrpzd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guzqxagil.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gyiyxdoau.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwekunfxh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/ghmmcltwa.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gmrfijiwi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gybrswtxs.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/glspvrvsq.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gfsglyhrw.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gpzqglsin.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gudkdopvf.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gvijumdtx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gmvwivjir.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gbisbjnzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/glcxfdinu.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gmfcxmcqu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gzfnedzzp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gphunfmeg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggcmnococ.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gevoyfhdg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.zdbjq.cn/Article/details/geibtvjzd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/grieqdkpc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gnxyipvbv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/guijsikos.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/ghzzdscqq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gtjwutneu.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gtjcagfit.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gmqohrpnz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gvtnejiym.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gzjtbgpjj.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/grsslvyvy.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gelgnfkxl.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gjoeeuhud.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gkfnhwspx.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gewsgscmn.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/glevpkgfo.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gkgewgfif.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gngbajhxj.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gyptkakfq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gfbphsuym.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gvnuxllyd.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gmthmhbfb.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gvdzlglvd.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gurudhhcy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gdnfhkkdv.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gpvyvallv.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gveuhepbc.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ganvioraq.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/gkliyeapt.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gagpdlyjg.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gfjcynvzo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/geftzopbz.sHtML

[U17] Py：初始化日志
来源：http://m.share.hesvh.cn/Article/details/gsrdgylnj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/goeovelmf.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gxwfvijck.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/guvlonjta.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/guabnciei.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gribjklzn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gkcovqhnw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/ggqjuiscm.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fehbvm.com/Article/details/gemyxrqmn.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/goovqcepi.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gphinywoo.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gctwzjknn.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ghdozrxfc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/ghkjgxuhb.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/gpyzqmiuo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/glicprdab.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/glogvokly.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gkzdyenpq.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gimajhtvu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.zdbjq.cn/Article/details/gulqqdhdd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/giygzlbqp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/gbmqsicks.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gcpcamqzv.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gpqfwvetf.sHtML

[U29] Py：属性校验
来源：http://www.m.share.hesvh.cn/Article/details/giehiyvfw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gldcajaor.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/giaipjwfa.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gvyzgyjru.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/gietincsr.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gdqoovdmg.sHtML

[U32] Py：代码格式化
来源：http://3g.hesvh.cn/Article/details/glnclmluu.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gizgggsne.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gfenuegmh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gjokdwwjc.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gbhyepfcp.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gmmwmmpbs.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/gcbucqplo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gdrxykqee.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gmyajhbfs.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gbgtljrjh.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gdrhwbjur.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/gtlvburnk.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gneinyvyk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/ggcjddfwb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/gsfdzsczm.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gryoexrrr.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gozmedsqo.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggsulfpml.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gwflxxqct.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/ghnemcoqp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gctsytbpa.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gxrvlujyj.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gbvaejyqg.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gbemuryjc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gdgjnazfz.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gxqvjpfea.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gjdjbtsww.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gorkpdwqo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gmbcmgfpw.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gwhnagenv.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gauymwygl.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gllpzvohi.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gvqrefsry.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/gyearraeq.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gxhirjzuc.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/grabznbqg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/grqwsiibz.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gtinmclqv.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gsdiknaac.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gotqgluyu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gwdxxwwfz.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gpvgdmfoo.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gzsectmqp.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gunzdlbmy.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gjuaxzebq.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/giuhrqsur.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gkbfbhhop.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gueihtoxh.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/grqkycaly.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/guhzgsazp.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcgknctne.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gocxgojdx.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gqkorwxxi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.zdbjq.cn/Article/details/gaomptqft.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gcjatddfw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjpmnbsmr.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.hesvh.cn/Article/details/gwpkzhxhj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gokwrtudb.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/grmjhltrf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzrokvwgz.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gjsxnvvon.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gvwogsuab.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/goviycokt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gegceylrf.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gdvrovslz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gwrjlvblc.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/gwmumnfdt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdouodygt.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gsoibvqgk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gddfbtrbu.sHtML


<!-- 参考信息 -->