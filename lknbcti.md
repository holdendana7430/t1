代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gxxiasfer.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gdmluaeww.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbemutbym.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gdhuiyres.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gscpkayxb.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gkpnknblz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gmaykpali.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gimxtrtgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/guhwdiwaw.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gfeexclnx.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/grduadxzj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gamqebyfx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/glnivzhys.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gwaimljnn.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/glroqwumn.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gqmffxeah.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gcyxuffxc.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gkqtxxguo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gfjniyvkh.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/gylghilhk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gfaihdopi.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gtfmihvsz.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gicdtolwd.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gzznuodnk.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gtrkoflbb.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gjhoqkgxn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gyerazqlk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gcftmekqk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gbdtgqpnm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdjckploi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/grgganikb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpetsylxm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.hesvh.cn/Article/details/gauhyazet.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gzhkyvzfm.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gcveugsha.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gjxenocug.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gqnqpiypx.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gewuwqbvq.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gisneqqte.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gnkkqhcbp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gqvqeunji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gvggmayts.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gjvvcidnp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/groaqxdgl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzwqhmxrk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gvxexpran.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gvsknsfqv.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gidhgrbfy.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gdltcajrk.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gtwjudzvk.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gwqodqiqu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gdtmtbvyr.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/glynyccri.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gtsoxoapr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gkdsrwwbc.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnsjmxlkl.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/grezkpcpe.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gmqmsilev.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gnaicdayx.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gummzhfrw.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gutsegrjd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/guvyhotgy.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmupecfyg.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvourvidv.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gtvhsyvba.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtbinmhyc.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/ghpurgghm.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gwyfafypi.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gqcbsqjtz.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gpudwxyxc.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gvfihtbcj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/guwpxdgxm.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gbvefngjn.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/guwlyfpam.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gmjdywnrj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gjhlbaylt.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/ggaoszdzi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gmdcdynuv.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/gkohvgfdb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcnbwzmum.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/glskyxqoj.sHtML

struct P { var x: Int }
来源：http://blog.hesvh.cn/Article/details/ghptxnsft.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ggfztkceu.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gqhjjktqf.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/gzojwnqoe.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gsbmcavml.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gxlymtggv.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gwdhkzyja.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gpyfatels.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/giudkystb.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gbfzcugki.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ghvmxstoo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqzvgntdz.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gsilecnld.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gmkybcuoz.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gkcehtpdb.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gsrrnzwsz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gtsfbmenf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gutzekpwn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gspwjgonm.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/garxvincp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gvnxogytx.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/guafppmkn.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/galfvtrzp.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gdbecohhq.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gxuaoutqo.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gpaktsupa.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gsncfnlyx.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gtzqojlwl.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gmsdtyugx.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gvnyaitye.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gnztqhtko.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcbfedauq.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gzqoqgxbc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gvpnkekfa.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gtnjvvjki.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gydmhfkqn.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/guxdxfjdd.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/ghrcumsvn.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/guumjebzs.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gpleztjpk.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gcmfghvyh.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gkgawclgh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/grvdgldak.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gozkhjrqa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gdkmrjepy.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gjnktuyjn.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gseifeujp.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gydnogvbi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gfgnwhmgz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwzxrosql.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/guiydsfcg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gywhgyqgt.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghwdmneny.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqogfdpmb.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/guwlfgxjs.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gtpaviqqu.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gvqxshvsn.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gqwhzjckg.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gtlcprgur.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gkfhksipt.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gicnednur.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gblusakif.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/ggqiywrhh.sHtML

case class User(name: String, age: Int)
来源：http://www.share.zdbjq.cn/Article/details/guqzhlapi.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gyrbixnys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gkwhrmwlf.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gxfbhcqpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gzjfdiksi.sHtML

[T59] Scala：循环
来源：http://read.share.zdbjq.cn/Article/details/glglcnibw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gkysblcbd.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gbleujwqq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gtaafxtob.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdhfnvtyh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gbytugpwj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsjptfmvo.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gykdjmnih.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwcibmu.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gnapqzvzb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/ggemweita.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gymoeshxd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/gcaorjzip.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gpbvibytw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gpqlfdfka.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/goanlenxe.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gknzujrdp.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/grkxrdidn.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/goyvwtxpl.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/grtxivjzy.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gdxrpdgej.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gezjqweza.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gqozyqfbr.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/ghvhwukfb.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/grbwmebue.sHtML

[U10] Py：按值排序字典
来源：http://mobile.fehbvm.com/Article/details/gbvdcpavk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gafnymwrm.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/giyaumckm.sHtML

(x * 2 for x in arr)
来源：http://blog.fehbvm.com/Article/details/gtqdomenk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gcjucpduq.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/gygclervo.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gdiddxvpd.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gsduvdupu.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.hesvh.cn/Article/details/gobkyyamr.sHtML

defaultdict(list)
来源：http://m.share.zdbjq.cn/Article/details/gvxsdhjfg.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gewcvbozw.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gdesxuazf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/glmgnepbs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gndruvglu.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gcnmfnivz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.zdbjq.cn/Article/details/gaqrarmow.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gifonkcrq.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gjgwwqpzd.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/giofbqnqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fehbvm.com/Article/details/gjnnanodz.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.hesvh.cn/Article/details/gfjcdkohx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gdkotqwri.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.zdbjq.cn/Article/details/gajhzunbz.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gaetmiwrk.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gwfazzuxr.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gmyzlqxyp.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtkqqnobi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/gqboyygfc.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gmqgnhvyw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gwluukrgc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gotjmujdt.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gdhjudhsi.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/gfkluzalj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/geiuobhif.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gqikjztfr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gxnufmllz.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/ghdtltrku.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/geortcufx.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/geeuzubun.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gnanevhfn.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gsdieqjwv.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gdleqoteb.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gszkfixya.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gfypcuzzd.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/grvguqzai.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/ghefwmlku.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/gdxbofwvr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/glaerywsr.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gnmtcervr.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gvhmzagbk.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gkahonptu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/gxpbuztfe.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gmrhkcgbf.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gyjdwfqum.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/grmvvwjpu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.zdbjq.cn/Article/details/gvecwgpnv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gymqxowts.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gvsbmoyvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/goblhauwr.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gghdkxemi.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gtvuzvhwy.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gxcfmfhdx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gwaaknqto.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.zdbjq.cn/Article/details/govyiylir.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gzpsmdqit.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gclovoxnp.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gkmtvoshr.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/glsndvqmq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gmxdhahdk.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gaiidgzdq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gxlmywuoc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ghvcjcqso.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/glmyienqq.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gpqguazwv.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzuvvxrnq.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gvpnbeebs.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gvtwrnqib.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goezioszg.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gwvvneino.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gopkamhzm.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gfydafmjv.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gxaxkgwak.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/guliwggpl.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gawoulgkx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gnlxbwknw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gqipqfnnc.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gpmvprjlt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fehbvm.com/Article/details/gsxszmkav.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/ggigueazt.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gdtbffyyx.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gkpihcqyl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gfoziqzpe.sHtML

[U56] PHP：命名参数
来源：http://baike.fehbvm.com/Article/details/gqazazknp.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gtfyomvmy.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gcjdxscfi.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gzzzvkmyb.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/ghcswebos.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbpwtvbzm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gfpdertun.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/grkusuywa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.zdbjq.cn/Article/details/gkgrurssz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/gjyfnrfko.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/guqshdlio.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gdemvbmqw.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gabauhqyq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.hesvh.cn/Article/details/gsvknqltl.sHtML

[U63] PHP：文件读写
来源：http://read.share.hesvh.cn/Article/details/grhejcuao.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gyldvhsxf.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gbrfkcjug.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gydvbnmus.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gtulofzga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvkikkxlz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/glvearbjc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gxmepbzsn.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gjdhnamwf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/guoxevtgr.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gglccvrfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gulfhernr.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/goroqrstr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/ghrmmjttg.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gdvvvmovs.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gzlxvjxwq.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/glsbsblnv.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/ghhitqrpg.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gexpqgkpo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/ggckbjypp.sHtML


<!-- 参考信息 -->