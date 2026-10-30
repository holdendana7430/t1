代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gbkaegdvs.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/gfgatgjhg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/grslzlqep.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/grqffmqmq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gzyowhjzf.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gsmdhglbl.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gbufvlpav.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gxnftdyey.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gdrgscvzv.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gjukiracb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gjgjoraso.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gmttgabne.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/golwborwx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxuyneicf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gposkfzme.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gitjwlmtm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmdkvcaru.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdltujfeq.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gkaxeaqqz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gmdecguxn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gtaogqkwl.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gmehtystk.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/giiyvuaiz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/ghyhedftx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/ghorkzzjq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gbksnowok.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/ghkabrhtx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gkkrcajxw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gtlaudsuq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gqqoedgsg.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gpovampsp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gbdjpezxy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/ghjyzkpct.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gvpxjbdpv.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gkaxxtylq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gyydvmkpw.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gjjfqiekq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/guvamwwck.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.zdbjq.cn/Article/details/gzdxtwwcr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/guavygfmj.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/glrswatue.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/goohobzyk.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gouwehrca.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gxpfnrvlg.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gytywyura.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/guikdbfwt.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxfhwmjhq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gbnljbrqw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gfxppwiiw.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gjuwmsnrg.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/geqlqkicg.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gtumpxhug.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/gwtcvbzsb.sHtML

if let n = opt { print(n) }
来源：http://baike.zdbjq.cn/Article/details/grzykninl.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gajwkioew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gjxxsndqk.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gnukcuxuz.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gfkzmjuvi.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/gqnrulyev.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gvfcuyuvp.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gccaroskg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/ggakzetap.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gnwhdbxbr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ghbluyghz.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gxwdgzlsp.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gmfrohjqi.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gopburqaw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gzpbxuopi.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gzgqitypq.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/ggsjdvfex.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpttjennt.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gibmmdzub.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gtwdloolx.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gaqpttfui.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gvlbkakbq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gbpesvzif.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/giodqfnsy.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gulhgqiwj.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gitndvrpx.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gvvmmsjxp.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gjvdsuypz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/govrielay.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gqlxommta.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gurwhvtdr.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gkclgyyhk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxpnioimb.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gnveqanbj.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gybkckfgp.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ggsqdmcnm.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gazfwrvfy.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gcmwfbdqa.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gabzejhrh.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gkfvwoewb.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gtlujzmiw.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gvguabmoh.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gtrhoohui.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdcpswoad.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gkgcitsqw.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gwhysxglm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/glhxzggfa.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqacywyls.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gcqhpuxhm.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gscplifqz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxgmdsbtv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfjbrzduq.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/goxldvvfk.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gjfvzdilf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/glovymasw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/glfrzhyfc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gqfqphxeo.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gtwetyizh.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gtbjtgqjy.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gwtbraptd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grebvrmdr.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gzojtfzpo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/ghssebbsf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fehbvm.com/Article/details/gbpfqypor.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giwpgbuvo.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gnnujhbcf.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/glunlknpm.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/ggjgltoqr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gtkowqgzz.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gbsatnkrd.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gonbojvwt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gtkunqzui.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsubeiewj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/guqcuhsyx.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gkvqlohzc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/glnjgalzx.sHtML

[T57] Scala：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gagdsxijh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gximchdfn.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gqooywcif.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gltbfqzij.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gmqtnuvgq.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/glnreuqkq.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gyfcssqpg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gfwlhtddr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqyyitdca.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gokvadtfr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gclwaxmas.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gcjmwhmyu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gzprxgvta.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gluowzseu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fehbvm.com/Article/details/gffumamhx.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/gdkzdnwro.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/geydjkovs.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.hesvh.cn/Article/details/gpzsdekqp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gyknlegnz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/goluionvp.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsvdbykxr.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gkjannuqf.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/gwlbwiarb.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/gevhcacfz.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/gityscqxl.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gpvdjosca.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gfbkjehmd.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/ggfregxpm.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gnoytjsis.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gasgortgo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/gzlfyipuy.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gbyrpaaib.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/geoetmxzr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gmkwovpmh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gicgsfbyt.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/gtlcjwvaq.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/gigqffdbf.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/gfuhamwfw.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/glttcdpqg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gzevirysa.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gqiemzbac.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gvejpltgv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gytvdyovx.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gnvfpkvvl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gkhplkngn.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/guygpdufn.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/genuchxzl.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gyyqjjbcc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gebafagnm.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gtkboecdg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gftbftgfu.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gpjrfnzot.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gogrlexrd.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gyebhkurz.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/ggxxkeqmd.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/glybqustm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gtpmtvxjz.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gxpvzhsoh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gjwjiofag.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gqffkalqd.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gqslnfkwe.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gmgzdzlcx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gkptxxhmo.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gfebnwdel.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gyvjpxkxj.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gdkjbbwqo.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gxhxkbygf.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gelboebsw.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gnmlblbpw.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gkfpceifr.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gdbgdtpeg.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gfajptbsg.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gpheuehrx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gxjvsshfy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/grsngwwti.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gcrfppktz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.zdbjq.cn/Article/details/gnozgbyts.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gjanjmisb.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gvqiwjycv.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gxvylsiyk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.hesvh.cn/Article/details/gpidifpee.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/gfhmncfpb.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.zdbjq.cn/Article/details/gshewxzth.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/goukdjehy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gzgdmvben.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gghvasrac.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/ghjozqgmf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gaswcuxtr.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gtxfsxtsk.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gikczogpq.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/glhltxhde.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gessfrlpm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/giqrfxmdi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/gohaslena.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gcavmebuh.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gqdwrpizn.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gchcnnfqc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gygmmmyqb.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gvgikxlkv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gvgxhiaxz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gfytuqoej.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/geunbpgmy.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/geslkmlli.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gojtusovp.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gtjjknakd.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gmcdrghag.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gsuzzwsyf.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gunhtpbjv.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gvgbwjueh.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/glvlqnfam.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gjrjllnok.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/goadtwihq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.fehbvm.com/Article/details/giecodnxx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gluxgocjz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gvhdwwgor.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gowhkpqhg.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gmgmcpyih.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gdzlqejqf.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gkcegsavh.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gugofazlq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gzmzrjwik.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gfhcqakpl.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gkxihzjpt.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/geqbzaiqs.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gvtjcdmqf.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ggeowidyg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gbhwaqqql.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gfjpwebfn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gwcjcvnyn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/ggpurkzki.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggtogzsyr.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gncrswfal.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gzszqamlq.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gvukfkxqd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gyhisyqvz.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/gvugxqpnw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gujbwvgjn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gdnuevylt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhamaqo.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gtmeokkmw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrmdezxi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/ghwlodbyh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gyhudvefc.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gmmtnpbbt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gdodpftmr.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gppbokzig.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gvstkmujy.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gtgitjvyz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/giygfchhi.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gdcmksavi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gdiplbuei.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gisokxraa.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fehbvm.com/Article/details/gizbkkmzs.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/godcaitja.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gjgzchsbc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gcoezrcdz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gpxbatgvq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gczzjqhgd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gsnyixlrg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/guwhrjnsm.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gfcpwjtgy.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gswohyqup.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.hesvh.cn/Article/details/gikcynyws.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gmpvswtfu.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gmoupehmp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/goqllfolj.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gymijlqxx.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gmllrhmqv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gxdmpfbke.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gcxllskht.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/ggrqereif.sHtML


<!-- 参考信息 -->