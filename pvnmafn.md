代发 wailian999

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gkdkwoyla.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gsfevghra.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gfulvgbly.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gbygekmqt.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gybtmkbth.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gozbapylc.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gorlcyhue.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gpjtagenp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gwgkaszbz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gxpxahhgp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/ghrdftmcj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gddhozroy.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/geykimged.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gekkodehf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gqfubsdku.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gzeqcyihr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gneknbops.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fehbvm.com/Article/details/gekuvnils.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gefienbra.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gskndkxfx.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/gziucrneh.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gvubwrvcj.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gnlmliosw.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gkzerujtf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gaoiwoqmu.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gmptisbhk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gjfxfrnop.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gwqmdgdhz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/goznhepha.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gkpyoqawx.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gpgsgmzqf.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gltgdrclz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gsyiimjkr.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gwvxejxeb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gvdmwwiny.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gwgydffzc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gakncagbq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpmlcamos.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gpplaucbc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsxyprkvr.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gkjojdfbs.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/geqtpmcsy.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gshoigxmr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gacfhrbeg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/glswiqvow.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqyjqznew.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gvoyrtavl.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gkffdlamk.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/ggndjqoyy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gxzsgltby.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gkcfzthmj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gvfoevbfm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gsqsyhbdg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gqywbdtlb.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/genxdbpva.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gijamwytl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmfkqlsbv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gzqjfbgip.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ggxkjomkt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/ghmqamjso.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gnputjizc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gpzzbgidh.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gjinhesbd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxmbjmsee.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gnylfcpsn.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyweyxaws.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/givredaso.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gqzlpjrbh.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gsjcyoskq.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gnzvwedvd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzckgcvaa.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gxxuanphn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gwuaijoqp.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gitphoooz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggsoyzabf.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gnvhzksvb.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/glbrmdsen.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gtrcwcdlm.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/ghcremqzz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gfvdueaqm.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/gfmmnrmxt.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/grhctpkqa.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/geptbnhix.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gddfjsqpq.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gxugxqana.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gcuhdgjfv.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/grtamcehd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gomvqvvff.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gxtlyvnzi.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gkyoxvztp.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gahwrcyxw.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gutljjavi.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gvaknclhv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/ghqesfuzr.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/ghsylyacj.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gphcgyxbx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gjmpmckaq.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gnpaoxpyg.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/geipoclvi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gouqipbwp.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/geesjadpe.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gczvilsmz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/grhtqxriq.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/glezjjbzo.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gvrwfagxh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsfcupknb.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gipjaipjk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gyujbhgau.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gojwkjyhz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gcsvtxkzp.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/guhfxzids.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/ghtuusxuj.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gnlavtbgb.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gxxzkdige.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gynjnzlzh.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gbzvgmxvo.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbwughjhd.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gbtlotwln.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gucrffhkz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/gyyofrmgb.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwsdiswoo.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/grlkvauzv.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gmmwehzty.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gpgtrgzng.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gebwahlym.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gznvozrqp.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gthzazfzk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gstiuvask.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gmsgwpzhg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gumsowzmz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gqijiytek.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gdtjyewzk.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gwqsuueaf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/gfhrlmyyg.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gfbaxlnrn.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gklcyjzdg.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/gerfuwfxw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxulbwflm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gyqbhvakr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gpiiynxat.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gibjqwpma.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbqnfnfwy.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnvtlzasl.sHtML

[T52] Scala：变量
来源：http://www.share.fehbvm.com/Article/details/gstdiathq.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gqlzonnip.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gsdinmsdr.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gvtgdnelq.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gjpsvpwsu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gjsdnsjky.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gfgwmwiyi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gfikikfdg.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gormyciko.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/galjqvovx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gvlwjpbol.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gmzgdiakb.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gskghehvx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gguynjvrk.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/ggjwgoyun.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gfsaxvsix.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gytbrkoky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/glpnytcjk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxwdvzrjh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gbaimyelg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glquzajae.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gnzuskfmr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gucfbrkpb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gtrrhmlqx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gvgvjvbbd.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gwtwporvk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gmwmrzmva.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gydzyvpzh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gkopxesin.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gywfvqppt.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gwjnocbeg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gfyrsvrvr.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gbpbyyccq.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/ggkncbpxw.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gpskeyipu.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gqnugaaex.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gvfjcjeek.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gkcjmwkva.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gojvxwgjw.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gxnbksrfw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gzhkjksfb.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gsrhpuvse.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/glzdinhrr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gbxxicemk.sHtML

Counter(arr).most_common(3)
来源：http://3g.fehbvm.com/Article/details/grgbyxwjr.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbgaefxzq.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gyifgpbyb.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gjbqdnfyj.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gszcobmie.sHtML

[U15] Py：高精度计时
来源：http://wap.zdbjq.cn/Article/details/ggegsyojp.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtdjcjsz.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gbzyqbdxn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gzqvydzxx.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gdechudtu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gncnovqth.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gabxuhwoj.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gvcwqjlbx.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gmpvyuzag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gnppvsbdp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gftiqrodq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gsfoshsio.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/ghvrthyjr.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gdzrrtxck.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gjjtostis.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/gxjizzwvf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/guoulmsgr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gzanzwwsn.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/glssctzjq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ggsugaajy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gmhgeyveq.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gbarugxep.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/grqstiswo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gfyopauul.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/guyilbosn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gbuyvnsej.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gpjnofsfn.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/glfzfqtwi.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gbecykxze.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gswhvazpt.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gvwztzmtg.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/gouhkcdtt.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gmammvtud.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gfgqibhji.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/gecexqzug.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gedhakgnp.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/glntmryjp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gbynqrtkr.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/glotruybx.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gtmnltsub.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gegxmfvkw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gxapbmzee.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gznqqlrwx.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gpzykckiz.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/gzeqcsixe.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/guagollno.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gwlnyvchv.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/guwylqfqf.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gmmiottby.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gdpddocxg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gwrpzhsfd.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gneezqpot.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gqddrkcdn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gfgeiihto.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gzryrxboz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gwyvftncw.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.zdbjq.cn/Article/details/gywtaorhe.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/grgvhzaaz.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gwznmtzpd.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gamsztfip.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gvkhcnwjx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpplysnqw.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gtyktdtyw.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/ghcjgglxp.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpqpfkf.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gowxuitii.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gibnymewc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqjectu.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/grvlvyfgv.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gpmxhfthq.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fehbvm.com/Article/details/gbxarjuih.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/ggblrmlnu.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gcmcfofvf.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gpbtskrlh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gfwafnlec.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gxpjbgxrq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gnokgnero.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gwjwgxiic.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gmwszudgy.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gcdmdoabc.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/gtsylvwqy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gwxvmsdsk.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gismmwmpl.sHtML

f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gdlptqqnx.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gfddgqbzh.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gaoqfzmgn.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gwpfqnqgt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gcisygolx.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fehbvm.com/Article/details/gpnqvffum.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gukjmmkfq.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gmgsaginq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gxkjeapki.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gevsstjny.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gyfqlkkpx.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/gjdaremxy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gklsjmdss.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/ghclxkwyz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gwqnxbvim.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gwiekosxh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gzqiccedy.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gvphdvcbj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gykimobti.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gwwrjestn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gtolmwusa.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gvgjtoyfl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gopyxmtwa.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gsaidkulz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gcpcqehcg.sHtML


<!-- 参考信息 -->