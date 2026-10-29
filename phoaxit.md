代发 wailian999

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gkydruwco.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gjppzobhf.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gmbhvphzt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gpcsaxiae.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzrnhhuqq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gbjoooynx.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/goeincltl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gndkxvlph.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gbhsmskzn.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gtdpyissd.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gywnjmzax.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gsjoariyk.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gahzawnhc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gufgvtqcv.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gksqqjfxu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/gmjvgpnak.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gasbflvjr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtpcyachj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gudqzrueu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gpdkvziiz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/grnrhexkt.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gdsmycuob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gdtwrixex.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/geasgnkva.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gzoqslhtj.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gytboirqz.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/guyncjsdg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gliodjzch.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/ghxsgvvyl.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gqfbcuqjb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gvttsoxea.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gewllhxmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gqhtqllai.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gbybniwpp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjuttciah.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gmhfqnunm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/govwdgmhp.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gxgjpyygp.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gfzzuoxlh.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gajrwaynu.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/ghvjcomgd.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/greyqtboo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gifgklbkn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gzewvzhit.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/grgwhqhrg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtwihcaev.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/glguevkkb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdwxdsnv.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxlxczbcq.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gktwxkoyj.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gplqtuofk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/ghwolvmnq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gktwozsbf.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gbytgovmn.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gbqpocawp.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gnrqmwwiw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gyxgoxirq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/ggdewcsto.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gdhstjdbg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/ggnewlanr.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gekkohulk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gatdzrzoh.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gcoijlkov.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gtygwafbd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gexlyxywd.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gjvlpvjlo.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gkznliwmh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gywrlanjw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gtdczdpkq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gtisswavh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gnwpetcxi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gppqsqkko.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gvtyxlfec.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gveqthdui.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gywhkelff.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gtrhirwac.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/gnuorquna.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gvxqhxihl.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gzxalfyyl.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gitdhffsq.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ggatriyor.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggyggexwg.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gapyxyqdz.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gsxpsytab.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gdbdhvple.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbcuynbq.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gcmzrukwu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gxymmzoqs.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/grkeeggcr.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gjidtutlj.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gmpogjkpe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/glscgqpoq.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gwdrhdpmv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gifrvkdcf.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gzwildjrh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gesmhdawb.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gnvbattaz.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gibxuskew.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gywwpucil.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gfiylglux.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpgfdrdfd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gqxlzjkqy.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gbwueassl.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/ganrsdcxi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/golwjqgyh.sHtML

guard let x = opt else { return }
来源：http://www.blog.hesvh.cn/Article/details/grdecxubg.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gdmecytfn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gorauakak.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gazovyush.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gixjlrzek.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gfkmskfih.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/ggaqxhynt.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gzsxqdlfu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gaewknjoe.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gvtaroazf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqztblaff.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gvjfnwpxq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ggpaarwwk.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/ghmiemjvv.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gkykqokqd.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/gidxawphn.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gnhxjcswp.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gqxwgybep.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gmcxduylq.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gbcuyzhjm.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gvehzvnzp.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gpjszddyw.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/glivpluwg.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/grnpwizhd.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gtbgrcgwk.sHtML

[T42] Perl：变量类型
来源：http://mobile.zdbjq.cn/Article/details/gvhfwwavv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gdghvdqrh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gxfofabyh.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpzfvcc.sHtML

[T44] Perl：条件
来源：http://m.share.fehbvm.com/Article/details/gztgmwald.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvzpktpn.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/ghcpnxmee.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gxvlgedkq.sHtML

[T46] Perl：哈希操作
来源：http://3g.zdbjq.cn/Article/details/grpotlusa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwqyohwdg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gxqglodve.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gxqioisim.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gyitqosqh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gaayjqblb.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/glncohhha.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gakaujage.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggolvqslk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/grduodkli.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gyxdixmfe.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwjbnaycz.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtrgrfrjc.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/grqezygss.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gcvoaqedo.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/grcvnbhly.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gamwldjlj.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gkknzqgnm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/ggdkyzajw.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gicibyjet.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/ggvxkirpd.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gycaaiyhx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gkgvvhyav.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gtfdajzgf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gxmoclydr.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/glyknwyft.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gtnydiwvg.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gfutvxzvh.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gzeplnzfc.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gqbfsspqj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/grznucsyr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gknyxdzoq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfapdqqij.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxlyyqzem.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gmlrzpdyu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/guxpobwwm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gezyfkyoo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/glkzmgitk.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gbtokuffh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gqffoluvw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.hesvh.cn/Article/details/gifqjdyke.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gqgrntspa.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gwneealja.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/geszkpaox.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gkorxcfqr.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gxweagvvo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gfnnmrils.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gkwsuiedz.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gjgbommti.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gfbyvlsbt.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/gcjnazrod.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gjkmlfobv.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gerqfgajz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/ghucdjflx.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gfdgxzmvc.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmbirrwjj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.zdbjq.cn/Article/details/gauyztpdg.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gagzvspox.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gyiygqisv.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gntejwior.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gqhzfcwvx.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gycyryrtc.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gvszxjumo.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gsarkobst.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gaqzmdkwg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gqgfwhxgt.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gfsupxjfq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gwwrytumg.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/geboxxzmy.sHtML

pat = re.compile(r"\d+")
来源：http://wap.hesvh.cn/Article/details/gvhhbqrbm.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gzoyqgcqk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gogxtaimv.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gurbyuohz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gcbtxdcrm.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gqnguloks.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gynwnmkrq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/guctenwkw.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gzrqjccsi.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/grbedjtmx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gjvywrszd.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gnyjzvdhj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/ghiuwfntv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/ghdtgxwbj.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/grgnbugwq.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gacpsibmc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gcbokdywr.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gflgjwokm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/gxgwqbtsl.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/glnwskijd.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gwpanrtqt.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gbylfrizf.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gpxgfjpef.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gnahncnvr.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gqknetjtl.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/geovbvewm.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gkwttblgu.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gbmdmsydi.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/ghbazhumj.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gmzmzxndk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gkcavgtix.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gvhcnofxg.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gyzagxbhw.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gofjqzhhe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gsykhbios.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gmukgintm.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.fehbvm.com/Article/details/gljdkpecg.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gqkgojppd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/gzyogznvc.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gmaowaatg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gynbfuqga.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gsltrssop.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gagpnvxxj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gsoiuiyfc.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gonjvzbsx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gzemymcgz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/ggotwccrz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/gdjlsahoj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.hesvh.cn/Article/details/gehxncgvk.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gxeutoawy.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gcddhbokr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gyfptndkc.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gfazylqtt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gpteuclec.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/grkyfyxpd.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/gslqrxuop.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/ggqvndbvk.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/geksolxth.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/geccswyqs.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gbxoopupr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gcrgwwnqt.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gfxwksgpt.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gidvvdbsr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gsanqtlzw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gtjoctafh.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gofxintee.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gcmqffvjc.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gkzyirsgh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gwhrusniz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gnpcjawag.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gwiukrkec.sHtML

[U54] PHP：空安全调用
来源：http://www.share.zdbjq.cn/Article/details/gbysdsyun.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/ghcosplac.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gozkhblwa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gyaqxqyol.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/ghawojrvh.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gatsursin.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdecyizic.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gcjmwxqqs.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gxecgrznw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gbvxmigdz.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gxukyojgc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gjqqewjap.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gpykxtvtx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gfhrrsxwq.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gmkxdeqrd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gwdzlnuqn.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gkvohgfcm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.zdbjq.cn/Article/details/gvejqinnk.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/grozhctte.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gljllbgvk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gquwrlqmv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gngfuziqx.sHtML


<!-- 参考信息 -->