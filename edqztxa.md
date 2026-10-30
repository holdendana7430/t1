代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcozivzfp.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/guhbcsgxd.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoonmihz.sHtML

[S58] C++：命名空间
来源：http://baike.fanxiaobao.xyz/Article/details/gcsawtpkw.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gcxasdvpw.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/glppxdmjg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctyopekz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gyqtgucxx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gmimscvar.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxmyvqw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzyzoggk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuyfbrzh.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gakgziwlc.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnzcnmmb.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnoppgscm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gxytfdlkn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gepdfnkrh.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gghzxcspw.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gyckgojst.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gywezsjfz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbegpbyq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gasamtdia.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gookxexth.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/grwqtqadd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gtefobcrv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gogguuuxu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvslhtpoz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gwumpryfv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggtyngsni.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gkvksbpti.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqwugryv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiazybcp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdckesgx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfhjfkcj.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxpnddqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeyolmhg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gnmbvbdni.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxrprvyn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkapfoopg.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqkzhyfx.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbykesyyo.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gflpgwmdn.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrmuejrg.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjcbftjq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqjpeajw.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwoeosag.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gsysajxga.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopjwcech.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gejwchoep.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gwnrlcnoi.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gdjqjdltp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gruoovciz.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwlxfdda.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnigjqzj.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/goldddohx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcufwzpeb.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqcenjamf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqjufquz.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpzrhkzh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkuzuekt.sHtML

[T25] Swift：结构体
来源：http://www.share.fanxiaobao.xyz/Article/details/gctksfqap.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/ghqkchlhx.sHtML

[T26] Swift：类与重写
来源：http://wap.fanxiaobao.xyz/Article/details/gqbxupsfp.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/golfmbuta.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givkjzxqp.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gklogcnpl.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gweyngoca.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gehjksouk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxmjvtj.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gjkvyctce.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijioayq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglxjxuft.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcobnsn.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwznojvg.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyxekizm.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdrdtdiev.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbukvgpe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gsupvbhkq.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/glkqwfims.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/guwthkwkq.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gvovdspyt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwwucuhh.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbayjortd.sHtML

function add(a, b) return a + b end
来源：http://baike.fanxiaobao.xyz/Article/details/gtocgvutz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/grhaxlozg.sHtML

"a" .. "b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwvlasqw.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbmhezgb.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gifqhxywg.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gobqdfber.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzspueylb.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/grbadpurk.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gddiswjjt.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvuvwgwk.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjxpcpv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzzwdwos.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gczlqllne.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guxqlqwyb.sHtML

"值: $a"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkngdergz.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxscfewzj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcykhagf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyncopjtn.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxyvjypr.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gfshkqyrt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glkhauucz.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiubdwng.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goqljxafx.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiemrhsa.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gspgxufck.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheiuvllu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/guarsddwr.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzoozsjv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gilqwmhdd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbobfrqir.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxqtgaac.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gllyrvlla.sHtML

[T52] Scala：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhcedapi.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/grnnxsqqz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gsthznwwl.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxksnvdjn.sHtML

[T54] Scala：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gegddffap.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghonjgvob.sHtML

[T55] Scala：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvcqrcl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/grjvaouqd.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gyyeseasj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfjmiigi.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/grzuwecmk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbdetsve.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcnwchmz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjmdovb.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gzslcvreo.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/guekqemrx.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvoxskmh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gqvvuhxbo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnodpyejf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/grpwaumpn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goknotibd.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fanxiaobao.xyz/Article/details/gtffeyhip.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gbcgaoxag.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/ggnmjznsy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcikmhah.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gbblbbxbj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtgjlgcs.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhdtvvbh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gtihhzglb.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fanxiaobao.xyz/Article/details/gnhuwduwt.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnezrmtwl.sHtML

[U06] Py：合并两个字典
来源：http://baike.fanxiaobao.xyz/Article/details/gnhrmnnlj.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gectxfril.sHtML

[U07] Py：反转字典键值
来源：http://wap.fanxiaobao.xyz/Article/details/gvrqwgklx.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqxgmmtj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwixwgsfm.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/grjmavpge.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/ggizqaxdz.sHtML

max(d, key=d.get)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwvhwawo.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gkimiszax.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gljvkegzr.sHtML

[U11] Py：生成器表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gtayxpmrz.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gfccgrlyk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorttzxql.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxocxfuwk.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaearauls.sHtML

deque(maxlen=10)
来源：http://blog.fanxiaobao.xyz/Article/details/gsreyanyq.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzecasxd.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksphquzg.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvzgrkwl.sHtML

t = time.perf_counter()
来源：http://blog.fanxiaobao.xyz/Article/details/gqdrxybus.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynstltbb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fanxiaobao.xyz/Article/details/gemxvrfvh.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gykmvpznp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggokhgbxy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrsqixlq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnekivdkz.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdexnhjz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnaitjlkl.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfrtlmoh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.fanxiaobao.xyz/Article/details/glyvhpykf.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fanxiaobao.xyz/Article/details/glfrhrmnl.sHtML

@contextlib.contextmanager
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyxitcz.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gzlakxmnf.sHtML

list(zip(*m))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjlratxg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxpvkvlkf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvuxfdug.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gioyypxma.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gqlavetdz.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gcgbhnxwl.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwmilytx.sHtML

[U26] Py：并发下载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwujeykbk.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmdxuyan.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fanxiaobao.xyz/Article/details/gcywqetbl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjuaoqe.sHtML

[U28] Py：类型别名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypnubzjk.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/giilludqc.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrzvbqjn.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gatarlern.sHtML

[U30] Py：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhjzxsyx.sHtML

@dataclass(slots=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/guhbnqxrb.sHtML

[U31] Py：单测
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gindbuqwb.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/geajnzaky.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagzeulbi.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkksifsnr.sHtML

[U33] Py：打包发布
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfpihshp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fanxiaobao.xyz/Article/details/gugpgijlm.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/govtunyjs.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gvmdgfhzm.sHtML

[U35] Py：发送邮件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcryuuqr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwopzedq.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveveriuv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fanxiaobao.xyz/Article/details/gduovplxf.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmdevzpx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiciuxyq.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/gljfznkmj.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fanxiaobao.xyz/Article/details/gaextisxj.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fanxiaobao.xyz/Article/details/gdfkbxwbp.sHtML

sys.stdout.isatty()
来源：http://baike.fanxiaobao.xyz/Article/details/gndclowaa.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/grclvndwz.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjnyicqh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwiscdcj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fanxiaobao.xyz/Article/details/glbotgurq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzyicbji.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfzeasft.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gefenfvcb.sHtML

namespace App\Http;
来源：http://3g.fanxiaobao.xyz/Article/details/gyntsatdy.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghihwyytk.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gimypetfe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghqecizyi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/goeaibgzi.sHtML

[U46] PHP：可空类型
来源：http://3g.fanxiaobao.xyz/Article/details/glhupfuxj.sHtML

?string $name = null
来源：http://read.share.fanxiaobao.xyz/Article/details/gsejqznhy.sHtML

[U47] PHP：联合类型
来源：http://blog.fanxiaobao.xyz/Article/details/grmonwwrl.sHtML

int|string $id
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqxbtku.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhhhjrmo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvhgssk.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukspijxx.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwralqk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/gizgavbrl.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlrcnwai.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwumgwexc.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkimmjfd.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtrxnibux.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fanxiaobao.xyz/Article/details/gzsjkadsh.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuewuvex.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsklqfwwh.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnucbhugx.sHtML

$obj?->method()
来源：http://mobile.fanxiaobao.xyz/Article/details/givbahilc.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyrqwibk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqlskfes.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddsousps.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glqohxnxh.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkakflkx.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcglqhth.sHtML

[U58] PHP：数组三件套
来源：http://3g.fanxiaobao.xyz/Article/details/grsnjxdix.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxntlbgvi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/giihlyfwb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtncjztm.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gtizpqwuo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gkauqyjdj.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbwwgubx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdrmsohe.sHtML

[U62] PHP：日期对象
来源：http://baike.fanxiaobao.xyz/Article/details/ghcjdzznd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjpzoxdk.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtdyqrrb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/glifsndbd.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkftfclt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fanxiaobao.xyz/Article/details/gtazblfhb.sHtML

[U65] PHP：会话
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrgwulcn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gkjpxiwzi.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fanxiaobao.xyz/Article/details/gcxblpkwh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkblpncnb.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkkkkfjq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdobxlvcn.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fanxiaobao.xyz/Article/details/gsasbtixn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fanxiaobao.xyz/Article/details/gqawjgpzk.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fanxiaobao.xyz/Article/details/gopxlhdxh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fanxiaobao.xyz/Article/details/gowiqbbie.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gogvwxxlj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gwjucormo.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrgwflqk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gdvbkzdjx.sHtML

[U72] PHP：写错误日志
来源：http://wap.fanxiaobao.xyz/Article/details/gvcudyvpq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdepaqqcl.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fanxiaobao.xyz/Article/details/gegbheksj.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwxbbno.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqkehgcq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gilcedxwq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbgntid.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgcmtrv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddbtrfps.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/goghjbqoh.sHtML

[U77] PHP：模板渲染
来源：http://baike.fanxiaobao.xyz/Article/details/gezjqsxns.sHtML

composer require twig/twig
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbvbzlmi.sHtML

[U78] PHP：单元测试
来源：http://wap.fanxiaobao.xyz/Article/details/geskfhhqe.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjtbeieo.sHtML

[U79] PHP：静态分析
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjhhwpxz.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpfvpju.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnllswat.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjqqwhzj.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gfipmifrq.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzmjgxdw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gpgaglyhz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegddiejp.sHtML


<!-- 参考信息 -->