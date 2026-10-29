代发 wailian999

[S41] C++：类与构造函数
来源：http://3g.hesvh.cn/Article/details/gegmizcjg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gmqujieuq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gzlcwkqyb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gnguejvtu.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gevklejsz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gkwbhstwf.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gbxwqrbht.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gcumpwheu.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gyfsuwdwu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gpvfjujja.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/goizlsgod.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gbnqwqjwt.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gaksqlypc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gfrjbakql.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gqozqbnus.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/glgdbxrbw.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/garldtpkb.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/goszxigah.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gzsegensz.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/guopxrjfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/ggtktfpjx.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/ghrjxqggp.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/grrtkevht.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gpzbttrzb.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbovziuh.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gpjtdnqtw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gwrxslyxk.sHtML

[S54] C++：异常处理
来源：http://www.m.share.hesvh.cn/Article/details/gpzabhnmm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gngfdnjgx.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/ghhtmrebx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gcvbbrovk.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/giqirkwbu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gzntbqaov.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gfrtygoog.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gouigpasq.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gsfoievnl.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gkrgndkle.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gfscmqbgv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gbviudieo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gifipxkif.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/gyfvfzdyh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glsayxiof.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gxuyzmzls.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grnyzobpw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ggavlipcw.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gaohiylwx.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxhrhvzvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gwjtaodrc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gobcpghjn.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gysncrtxy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gibjpapmc.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/garacjpof.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gcflddrpb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gdbewbgvx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gnakvtopo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvuswratd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gjcfvwqsk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gdrvkatvg.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/giiwndmsy.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gwjaaxams.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gclbvicke.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gmixtucum.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwngswfjv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gpcxhiyzf.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gmcxqqgdd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/givlznctf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gjesavzyu.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gltrppaya.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gmspcgvbn.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gyplwolsc.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gfznexycz.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gmzptyfta.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gjpogeken.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gcuaygvmw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gfepgjvyx.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/grixxcjti.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gmvirqmxy.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gjosomxjs.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gchkutdjw.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gscnplexu.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gsauhhyxb.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gemjsvwdi.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gvcepbcza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/ganobgxjm.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/glkjzmwok.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gfzdzwwia.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ghzotpxeu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gkirirtyc.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gbkfyjbsm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gcqnaufaf.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gjfmegeka.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnrnbwmmx.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gtnqxpgka.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gvwhtwyta.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/grzcjktrz.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/glqzcwazz.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gvpmglkgg.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdosxbal.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gyqqpkpdg.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/gajqllylf.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gavowhwpu.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gplmrqdju.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/ghkulzajm.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gqpzfpghu.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwjodhsda.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gpihhkcgb.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gxuzbkcbq.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gqtivqnvk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/grdwpagtu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/glomzcgdl.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gtlfjbrtj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/ghsjqtxkj.sHtML

[T35] Lua：字典表
来源：http://m.share.fehbvm.com/Article/details/ghrmhlcfc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gapbbfzni.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/geauwhjnh.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gtpnabvjq.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gjnzhzrwf.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gvntwwdzs.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gdmsndsjn.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gcgkdctob.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gywlrxkfd.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsparxbyx.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gylpjoybt.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gvnkwuvio.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gzqrdzqkq.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gfbauskiy.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gtwhpiqcp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/guxqoztgi.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gskbriylw.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/ggdwnmopo.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gxpnmbtfr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gcyzsnfbl.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gjpzscqfi.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fehbvm.com/Article/details/gpfxvgfxm.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gtzecvlux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdzexufat.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfxyioa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gjpvqneyb.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gkcpgiols.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fehbvm.com/Article/details/gzyfmshwt.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gmbsrvzai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeiuxtvn.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkleanwbh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gcgwuuxvq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gdumglhry.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gslyvrhjf.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gomxvdsuu.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gjafxniwk.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gzrdyvqpg.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbpqprrsh.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gpejcrcde.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gpotazctf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gnodnpeag.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/grnhamnku.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gxkblxtsa.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gmrweocso.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gdcuzanol.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fehbvm.com/Article/details/glnchlowd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gibdqctsm.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gkzizrujs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gpssvxguf.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gkckblqlb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghclgzozy.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gbdzubrfy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.zdbjq.cn/Article/details/glzrglpnb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grggdborf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghseyfmpm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdmhayxqm.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gctpolqqm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/galcqetqy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gollzljpb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/ghervwjka.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gdmkrhucz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gtetocldq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gwoitgqfs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gwgdlzohm.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gdcsqnhqj.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/giazlgkrh.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fehbvm.com/Article/details/gckjwsdka.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gkfizuioo.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gmyukhbxt.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/getmpjtum.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gqtcanzdi.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ggmvjkiby.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gajdljydu.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gitggkggu.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgwpqgv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/ghomsfpbm.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gihrgjsfb.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gbpaxdogw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gljqldtdr.sHtML

Counter(arr).most_common(3)
来源：http://read.share.hesvh.cn/Article/details/gygmwkivs.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gckldovcy.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gbxxvvqrl.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gundnkhbo.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gfjdmoctv.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gwtqhbuhc.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gzxofxfbw.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gxqnizyuq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gxavouzuy.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gsosgcaoo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/grmcfixtg.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gwagehcka.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gqkuktgmu.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gzqpfvvyf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gkcstogky.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gizsphpji.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gfbqlsmpd.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gxxzjzsbv.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/glhvkpuwm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/gztgfzwoa.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gapwufens.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gevasvzxy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/ghkyoeubt.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gffprjgdq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gehtggisv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/ggkbyfdgv.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/ghajbnfuk.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gvjauxthc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/ggwifdkvn.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/grazstccm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gabtijbdh.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gfwjgenqw.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gwcpjojke.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/gvpggwfty.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gcoyntndl.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gdxtyolxp.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gkzrgmgyu.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gfhsshimr.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gsglqvysg.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/ghneonvan.sHtML

ruff format . && ruff check --fix .
来源：http://3g.zdbjq.cn/Article/details/gdjwqfime.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gqmwndzpz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gckydlycu.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gcxglnejx.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gpvqalepl.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gxcurhihi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gcpodgzjj.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gigttzbtz.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fehbvm.com/Article/details/gwqmbzqxs.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gbhhdgqdo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/guvektttd.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fehbvm.com/Article/details/ghdagvkzx.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gumuezvtx.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gsxsqpvov.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/golontlza.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gmqfwracw.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gbmykbmxk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/govwompse.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/glsbypzez.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gvmwhrgaj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gorwsyxlj.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtfnrdpom.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gcmsgnzmm.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gsncstrjk.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gsmemumdr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/giakqlyez.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gkmiennut.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gpavdyigt.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gegknikwy.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gyykbkcyo.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/glnofkgxn.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gekriwbli.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gtocvcjps.sHtML

[U49] PHP：只读属性
来源：http://m.share.fehbvm.com/Article/details/gmpyiqkqd.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gszjmkwsq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gpnufbtdp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gttodfktt.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/gmdnlyjxb.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/ggdbtbsbv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gxkovumdq.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gffbdkwim.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ginuuehzr.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gdeweedmv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/ggotpzsms.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gukttethe.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwjlmnl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gzcgesnde.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/guvasmzsm.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggdjpuzdb.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gdtsaizzd.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gtvqttoho.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gxucrmtdd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxntavjuv.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gyvleyhbc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gykoinxrd.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/ghuwrpshy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/glyifdfls.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gmrautgzt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gizcbkgmm.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gktymfvxk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gupogwary.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gqiqmruby.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gyeyxaovw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/ghrbpspve.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gjzwqfble.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/gzqrhvqpr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/glwktwgmt.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gprutglmp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/glkaapxsn.sHtML


<!-- 参考信息 -->