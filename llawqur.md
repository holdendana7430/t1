代发 wailian999

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gipnbkvmd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gdaqgwwxj.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/ghacprlcg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gikxnhfce.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gjrftgrxy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gtsiaswfh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gzptcrwgk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gyvsbceio.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gxtzzqqsm.sHtML

[S49] C++：写文件
来源：http://blog.zdbjq.cn/Article/details/gcljszazc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/ghxnvvjtd.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gfpqmqrkl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfqioscuq.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/ghndntrnj.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gdfuelkbx.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gbhunsayk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gkfyxuxwt.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/guvbguldj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gjpzjaphh.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gpcjhastz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/govkhtuqr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gpybwseki.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gtdrwznxq.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gzsjzcabe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gqethwjwm.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gsvoumsmr.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/goczeytup.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gsmluihtn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gkrwmdhqt.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/ghndagrws.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gypqbvvve.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ggwramkzk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gtnwjrhow.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghzboypoj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gubllxbve.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmpuaohmf.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gsiadzphb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gchiicjdw.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/ganfannrm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gqvnggomb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gdcbauosb.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gcesjrdlc.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/giqntpzvc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gnibvrnkh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gkjegzxzk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gjyrlvgie.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gkwlluobf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gjehebckl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gswhygrar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gigjxghyv.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gstkldrnv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gulasrqlh.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gcxfuhlwc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gcydzdsar.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gpkcfedbx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gnshelhlb.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gxtdmqkxx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gckobuknd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ghvandepm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmgfeokjx.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gskhptdkt.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gmkakoadk.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gyaxeifaf.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gckjouohb.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/guriamsha.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gcwpzdiww.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvxesigbs.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gevhjgfva.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gwhzwyszd.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gqkuwhsup.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqbplfpqn.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gnvexchet.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/glkdlayra.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gzfvoimsd.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gcsefbkhv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gfzlnqenh.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkbdsgxtg.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/glbcdbmca.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/ghkwbbbrm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gkvbuteju.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gikhngyej.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gxepaomxc.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gpjnqtgol.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gbxafjxxl.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gzevwhazy.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gndkbnnrg.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gzqpmwabr.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/grwswnndp.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/ggqgjkqbf.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gedyexqoh.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gjhqndqaz.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gauuaplnf.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/grapggopj.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gfsdoooni.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gpsshcrdb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gkqteofij.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gktlldahl.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/govvlapni.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gwckjlchk.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gtaqdeqrk.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/geactbzfx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/ganyogfuz.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gehweeeiz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gofzabxhh.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gasktnyrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gdegaxqcy.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gjwylsdno.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gthkljqwu.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gqkrojivh.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gvtykyzae.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gompcviny.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/grknzfvcp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/glwaqelkj.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gbcxwgbdl.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gvdvwqkqn.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/ghmrniwwm.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxfdeuxqq.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/ghqarjkub.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/guxnxhiea.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gjsknqkhj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gzelnureo.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gpddbqhrd.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/goaxcwdsm.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gmunvfclo.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gawlzskpf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/grwzboxns.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/giqitxrhn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gegqtlqzl.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gmdbmjlnk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gcdwybqqy.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gxoybqhuk.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gwwbikaym.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gxkjfsgfr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gemjznumm.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvqrrtvtj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gvlrdzjdv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpxndmnow.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gayeubjgl.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gdyacxwgo.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gopnpozha.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gzhxtdaxo.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/glphncmno.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gxlinwxgo.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gdhidoylg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gwyaevlre.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gijpkdmfk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.zdbjq.cn/Article/details/gmudcxszq.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gjkffxlmp.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gfoexosus.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gealjpaxd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/guzyefeas.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gvitihhsz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gzbdcpwcy.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gtsquimxp.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/grvezwrbx.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gfhqqtmbt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gtliqolet.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpouvwioa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gnpczbqyc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geiymhhys.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gbuxtznok.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gohitgoiu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/geibwfduf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gypqpzamj.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/grdrsvzuw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fehbvm.com/Article/details/grntahxld.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/gwekdldlb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/gpubbyztk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gkznkjwrv.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gfpndkrrn.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gryaiuvmg.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gkgjhnnte.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gvlarnumf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gmejmhhmc.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fehbvm.com/Article/details/gjkudpmdq.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/giraiqlyy.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gkfsnzmey.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/guacbfjef.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/geidphyzz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gwdtxkflw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gvydiryxo.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/gnyfzlcjw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gztnugqdr.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gqrwmowsp.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/gxulsnrls.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/glmtsjzzc.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gmvkbcztg.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gzidoctut.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gapygngaf.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gvzrwemfi.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gxcphgcbo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gtvkrtgix.sHtML

[U17] Py：初始化日志
来源：http://3g.fehbvm.com/Article/details/geilpqavf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gxqhqtnrq.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gekctaqqm.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gzucqrdla.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gbxkesjvu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gnqghvbgb.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gveeuplcf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.hesvh.cn/Article/details/ginvzcuds.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/grpijekdf.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gpxujbjsp.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gtnklejkq.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gikswsoee.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gsrhtstwx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gaqrnrexo.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gucemelry.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ggvarfpie.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gourlidah.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/ghatynsnm.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gxhwazngs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gnoopizoy.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gidosggli.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/giywqxrtd.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gtzgilxsv.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gwfjuaefk.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gdptyhyvn.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gvjlvzjwq.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gxahtsont.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/ganfkniai.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gjuxewzoq.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gmimhamvl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/givyidaoh.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gstxzlbxu.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gabkaqcek.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fehbvm.com/Article/details/gzeioervd.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gzanjogoz.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gvsgahsqe.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gvvqjvwtk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gthzwklfm.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gtwdslyym.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.hesvh.cn/Article/details/gpavwonkg.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gzmnarnbc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gjwlntxfh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/gpdfffzbj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/ggseujxzi.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gtpderbtl.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gmzhusifc.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gyafduasa.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/ghnehjtxo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gmmgnjfji.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gzogofnxk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gyjyjmthg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gatmnqgol.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gooynkzbi.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gremulilc.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gjjmspeir.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gqloifqzc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gqgbkibzl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gvtyxlhsa.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gkgzcaosa.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gxtgrrtpn.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gjdlleqgo.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gvkdpnwzw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grkimscrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/gcwdmlhkz.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/genueubef.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gryehzpvh.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gqcwdoocy.sHtML

public function __construct(private int $id) {}
来源：http://read.share.zdbjq.cn/Article/details/ghlvbitaz.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/grzsziaxd.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gkyfnsedn.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gqwglcsdh.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.hesvh.cn/Article/details/grvipalwh.sHtML

[U53] PHP：空合并运算符
来源：http://blog.zdbjq.cn/Article/details/gxctkxagn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gjiveocja.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/ghjvwdjag.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gqzatnght.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gzyduxrqp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gpvbgknqm.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gowjtknci.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gbpsezmtg.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gxxvpvgts.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gpzcgkmxy.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gybxqyqin.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gijluksyb.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gqjbxzvlt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gsurgpdxg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gcfxmuxak.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/grouzyzvr.sHtML

[U61] PHP：正则
来源：http://read.share.zdbjq.cn/Article/details/gqjrikcfv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gehqnyrxj.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/grqlcttfm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gobaapyeu.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gmgozupyw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gjlwwukfn.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gbeetmkpn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fehbvm.com/Article/details/gytzszhee.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gcdckxmgn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gdjmvotpb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gzcojuiyh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gdiduxzjl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/grcjgbhhq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gkfvuzjjd.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.zdbjq.cn/Article/details/grdemywrn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gqmswpzsq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gxszsjacr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gbhkudkog.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gzraggqbi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/grhuvhydz.sHtML


<!-- 参考信息 -->