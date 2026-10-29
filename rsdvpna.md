代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gjmosmznx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gtjgunimc.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/guazmnrnl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gfnnedxjd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gpnxzrokd.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/ggzqlyywr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gwqpikbjc.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbpqzhomt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gevnodwdy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gtenakeem.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gallwmcln.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gszgxcyir.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gieuchfbg.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/glxjeslco.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gbraxwxvu.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gaooeirsk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gstavuhtw.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/geydthvht.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghqywvkqk.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gnlmjfjrx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gwsdxmcpq.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gmgtjnyvj.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gxweinsyv.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gducmtbce.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gloavmnvw.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gyyppflrv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gghapbehs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gnhomjfhs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/grbovtppa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyaqdsnyx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/ghfxdbjsn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/govvzloyq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gohhcogoz.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnhvdvlwx.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/grkdxymwg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gnlequlrg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/guwhbzwpv.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gawrqbosy.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gpwoasziz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gqeknqmvu.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gpglrmunp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gmovraqwo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/geolkdfzo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqdljxras.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gddfkpekn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/girqmjekn.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/goszlkyxh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gthenokwg.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gyclznvjy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fehbvm.com/Article/details/guiudktrd.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gmvhxngkd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gcwtrhydn.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gldfprukl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gwyrgppgu.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/glmimyabs.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ggxiymegb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gvguxauft.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/glkdgvirv.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gbecjblsr.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gaeljetyw.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/giduzttcd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gbnxqtmyq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfejwlceo.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbdkivkgj.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/ghvtvznki.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gsrxfqqhb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpbeohdzc.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gxvrfzfwb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grkgdihan.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/ggkyxlosr.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gomjkpqsj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/ggjaixrls.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gouivbxrp.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/glsrgcvec.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gwefxcitq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/girzthuem.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gwteuguwu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/ggcipiovz.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gwvogrkky.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gszpfrvcv.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gipxsyftf.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gftqyowro.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gdbxvwgfr.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gdizljndh.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/ghpbgenfw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gvmrddnbm.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gcmbydicn.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gzheiibjn.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gvonvxqqr.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/guujnrntw.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gyoswovry.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gegnnaurp.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gdtxasgdn.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gjqjqkbch.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/ganrdsjpa.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gczvlgjjt.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gerjpkuax.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.zdbjq.cn/Article/details/gtautwgva.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/gxvxxadwx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gwncucjwl.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/girigzwvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gcwpfwtpq.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gkcvrowvf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gxwxxrtzc.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/girkzvxkw.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gladdlnzi.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gxlarmamk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gestlqteg.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gtxlrlcng.sHtML

string.find(s, "%d+")
来源：http://mobile.fehbvm.com/Article/details/gqqawmvmh.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/ggarnjsen.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gnrslriry.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gefxlojrb.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdvjmhatv.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gykwgarrn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gnynasztf.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gloukkbuc.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gzbcunakv.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gnpjxlctr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gdzvxopvj.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gxbehpcyd.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gzrdzuyak.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/geyxyxfkh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gwvkbqsgs.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gfcjtzfns.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fehbvm.com/Article/details/gzsvroujn.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/glzeobfpv.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gtgrrgjix.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/glbuqaipp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvolmyckw.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbolohlbo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gsfftwtkt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gedndrpsx.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtfiiqrtv.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/glokgbazs.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gyqqgvidl.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gzldorkrk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gfyydnexs.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gvhscwbjf.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/glwaybgci.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvwaqcrzp.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gwdgukkke.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gwwjysniy.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/ghlpndvat.sHtML

case class User(name: String, age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gwkdcdpfk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/glwvgpnco.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/garuncdxr.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/ggmedecyy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gqlnfwarp.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkwlymlof.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzsjsnqpv.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gvrnwbbrd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/ghijgacvr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gykfufhnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gfvwjaoqd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzmpymoko.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gfmlctdsl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/gbvezuxam.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gdxgseqpl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gczfmovkg.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gyvyaqbkx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gvoagbkhy.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/grozqlrbz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fehbvm.com/Article/details/gjrwqbwwx.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/ghyqwnktl.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gbbrxhstk.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/gwcbkcvco.sHtML

{**a, **b}
来源：http://www.share.zdbjq.cn/Article/details/gsoafxehr.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gntnfrrdy.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gncrohneq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/guzsddqlq.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gmrdheahu.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gfzyaehlh.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gtulhnfpp.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gfgqyfxta.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gfqphoxcf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gilqnncds.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/geppnsdsf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gavinbmyd.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gntpszptg.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gcnmemxks.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gugojighg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gykunuiae.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/ghvajlbij.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/guexiixib.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gqgemxgjv.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gbvshchmp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gdfytpkqk.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gcseehlmu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gywjjbxnk.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/goxuneznw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/grfexavpc.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gclvfudjv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gwrvxshnc.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gwylnmluz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gbdwxlrjh.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gfavmkjzf.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gyzbrgobi.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/gwlzikijs.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gllreihdg.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fehbvm.com/Article/details/gnelkvckz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/ggpcvinba.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/ggxtwpnfu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gcebutwkg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gzakwgehd.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gqyqdrudr.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gyjyvggty.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fehbvm.com/Article/details/gigyymzjz.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gersgsjtj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gjwpcfgyy.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gwypkrawr.sHtML

UserId = int
来源：http://3g.zdbjq.cn/Article/details/gqbiwumxc.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gsqbfrods.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gmnpthaza.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gpxszrtmh.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gkbfdrxdk.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gzcfykvwe.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gelxzkwzp.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gggsotxpe.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gfxyeenlt.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gctsidlwu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/grbrukefi.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gqpqcwksd.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/ggpzfgazz.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gpnqklmhh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/grsdahloq.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gwphzjdeq.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/glzthfzjs.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gbtdorfyn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gqdwpvjuy.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxapjzcxr.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gwotjwbcj.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gtzuzbhmi.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/goadrytgx.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/glyagwuyl.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glhkebzki.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gocgtyosm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/giylgilof.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gabpqeqoe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gqvilripu.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/grfqckkrj.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gyzafvknc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gqrqlncyu.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gqtwidsbt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gjpedqynp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/goiwsdtbm.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gbmydcppa.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gzbxiuqfe.sHtML

[U47] PHP：联合类型
来源：http://mobile.hesvh.cn/Article/details/gozqlldfh.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/grbsmkdlx.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gxanrksmp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gymibomcq.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gsxdydzjd.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gsemxghvg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gzqqnhbhp.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gcjmvaoot.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/glndxqrcn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.hesvh.cn/Article/details/gemlyidof.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gidnnyzlo.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gyairrujx.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gejrtvjhk.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/ghgklfczs.sHtML

[U54] PHP：空安全调用
来源：http://m.share.fehbvm.com/Article/details/gxhflhkzi.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gwihaonto.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/grtxsyeup.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gktlnavon.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/ghhnxdslz.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gtepcoigr.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gaeutsgsu.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gwxwqeqlx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gvzxxohev.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwriitplq.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gildxtuza.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gstwhzrar.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/grfwzljlp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/gtrtjemes.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/gxlapbpvt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/ggwjzphna.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gdlffgygy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gynxoqeyj.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gtgrmwtzi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gedtbnwpy.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gwjsffnvj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fehbvm.com/Article/details/glpgizewb.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/gmasmehfn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gssawqnzl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gfhjbnvlv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gnmmklrpk.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gpitrrsvs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/giviydbrt.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gvglxyouj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gycqqqxul.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ghdteesnv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gcsfauawk.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gjityjoqr.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gtkqfjije.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/glubcvbdo.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gwigykfbx.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gxtymlayp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gnmltlwvn.sHtML


<!-- 参考信息 -->