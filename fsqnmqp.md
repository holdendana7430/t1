代发 wailian999

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gtrkkqkxd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gkfemajtb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gxayfgawm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gveguyihd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gcuiscavj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gxjasbacs.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gijedpacb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gapuhuzyd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gecidbohb.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gtcjmjtym.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gpxvsdfhv.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gnwxrekzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwawsnztd.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gajkzfcoy.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/ggnyvtuko.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gfbtehqzc.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gjdqltjjf.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gosizhgih.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ggxzckrpj.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gmzfostvn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gioizfngo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gbfdtxvnl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gvgobbujb.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/glafjmvdj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gngqmwjce.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gjomjwkcy.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gudccyvlq.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gdzfguazy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gpupaghho.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gublxkywe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gbxhnxhzr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gyoeuzini.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gmkovnsax.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gasnjdpca.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gftpektuk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsgimeofs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcncrszjo.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gwlqjjped.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gmworlalo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gfigfhksd.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gxmbrcbrc.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gwsiizunz.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gfvhhtjdw.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gepwqcxbw.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gbmvsfzmg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gmidixhwf.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gohlppzrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gomutzlze.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gslixbfci.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gtdovrryh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gxggeqcyh.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gonikaqzc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gpxepelcv.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gqigkumts.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gaduqelji.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gebzycayh.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gxtavdadx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gnsianmed.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gnkltgkyb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqhgzdxjw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/ghrztnlwf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gzcqhucwt.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gyxerhmqc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ghsfhgsgc.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gfqkcjcvw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gsuhvbvdw.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkdxyrggk.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gdydwoczq.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/ggoqludgv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gruznvzcz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gqfwgejdu.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/guyrdkhpc.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gwygywrif.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/ghzodblhs.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gspgvkcfg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gwgfyyldy.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gbeodzgxb.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gieiieqjy.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gwevoijht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gfuvwcojy.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gokgqpjpz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gdwgjbzan.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gouaxhjrz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/goavmgmgh.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gxsjijmkw.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gwivgcowp.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/grsltapdb.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gdqkxlyxf.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gtnialefz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gcqmuheda.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gyswzdoyq.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gpxsrwhcs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gzpzxsmxf.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gddzylnre.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/geddnulay.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gdbhyyjji.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gcjatyjgc.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gyhinudwr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gfpygxikb.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gvcasqjej.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/govdrerll.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gvwezvqki.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/guzklbuks.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gggditdmh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gfkdesfvb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gyzxweqib.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/gsfomqlqr.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gmawcxlos.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/grnxsofhi.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gmjzbrixb.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gdhsvoxjp.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gzubotxiq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gmebpzomo.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gswsbntgt.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gwcgjraka.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gshaaviql.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gpjbgsjoc.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/ganudrera.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gljspbdzm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gufrgiyff.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gwlbqgngs.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/grngkuirq.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gpalikiiq.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gfeacyjbn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpyjhubyq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gdvtpowqf.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gxnzhvrul.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gkotxjvaq.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gfxxejypa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gpmjbvnlt.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/grthieonz.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gcyizajhy.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gnhnxbfsp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ghzfcsyeb.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gohsgtlhd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gujsvcoud.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.hesvh.cn/Article/details/gzexhomho.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/grntxjwmd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glfedifhw.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gteobihtf.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gvpqegxfw.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gccybrrzq.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtnrfluka.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ghfddohdj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gdvdcdime.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/grgwebfcx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gbywuucqw.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gopzcipmr.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gqpnqoigl.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gzobrymrp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gjyvvakxd.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gzpngiygq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/ghhivclub.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gscdzugau.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gobhlprxr.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gfgagszpz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ghgfdrnux.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gavrjjxzl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gepkhjwmf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grmlwkiva.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gaydqlucw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/ghynkywqi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gwcemepzs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gewkghoet.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.fehbvm.com/Article/details/gxzzdpgme.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gdiwfanll.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/gcgjrdsjm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gxrclybjv.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gyhhlthpk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gosytdsgt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/gmjiazwxk.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gbbqdwhrl.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gmqxwrped.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gycjgnwht.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gddjqhrnm.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gtzspwghp.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gsomnldlo.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/gglceocja.sHtML

[U10] Py：按值排序字典
来源：http://3g.fehbvm.com/Article/details/gljkiscnf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gszfjktzd.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gchkselnx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gotxldcpd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gkpdvouat.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gkswuiyif.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gbhqoauyl.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gaqdikebc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.fehbvm.com/Article/details/gnoxarfji.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/givxsglbl.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gcyniifzp.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/ghgddzbfk.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gxnjyodvl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gthdddjop.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gijszmswd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.zdbjq.cn/Article/details/gjhiurxju.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gctbjkvzr.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gfncnwokk.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gnibejygi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gfftostpp.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gvwqoxhll.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gimpdejyl.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/gougcudlz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gtnqijkfu.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gjptjevwa.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gjuhsdnve.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gpwqatewx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gwojdprjl.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gobqmzomn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gfyscnwge.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gycmstmbn.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gjccafcal.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gfxncjvsu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/gayhbivej.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gdxcktkzd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gusyhysjw.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gvenngdxg.sHtML

UserId = int
来源：http://www.blog.zdbjq.cn/Article/details/ghbonfsof.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gowuawlwd.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gwcrzfmts.sHtML

[U30] Py：数据类
来源：http://wap.fehbvm.com/Article/details/gctfaoleh.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/glrwdxerp.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gyjquwrcj.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gbvwjufdt.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gvgqkvqnk.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gfzhxkkps.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gfpdffkvs.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/guemonrur.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gqlrtenzl.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gvupvwxsm.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gnxkcaykh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/glduhulza.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gmvpqgkyz.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/ghreglvos.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gqygaczsv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.fehbvm.com/Article/details/gkqquaryt.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/ghiiumjhh.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gnfcmcccl.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gzhlkkisz.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gnynjojzr.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gucyhuqva.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gnctmebhl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gosxeiplb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gzdrutlpa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gcxilyyoc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/ghsszowit.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gjemdessg.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gqcjqsrgx.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gmangytdf.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gshzlkpun.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gumwhkzkl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gqybgjymr.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gsuwgkhox.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gsslzgxqo.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/grimkujje.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gbiuyeiec.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfucyrxji.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gjwwjxsqr.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gwcxooazd.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/glzginjvu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gglpvcngc.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gsyxprxik.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gzwyhvgbd.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gcrtvqvwu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gdihqxhjf.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gumjcryoo.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/ghwbgtmke.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gnvqqoehs.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gxhrgmelx.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gpgipraxw.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gtsbrkdyy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gltzndqnk.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/glpuwvsab.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxyhfpako.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gfptcxhii.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gecywpjhu.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gjsbmclcu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gccgcqqia.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gwewxexby.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gkwxypfrs.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gbuorfvey.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gtkfrheuu.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gahbjhljj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ggiyqoiks.sHtML

[U62] PHP：日期对象
来源：http://mobile.fehbvm.com/Article/details/ggjgqdgih.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/grdabgtws.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gbofgljuk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fehbvm.com/Article/details/gnfpecubl.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gwqpqmyrb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gvzddjaiq.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gcuawhlxu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gknzhiuzy.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gfirxolcc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gbhnsfuqu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gjgwvbwhg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/ghwkbljbv.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gvvcfnfzl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gkotgzolk.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/gtsvrqlro.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/ggczaqdjh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gedqngdkf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.fehbvm.com/Article/details/gsylnwttz.sHtML


<!-- 参考信息 -->