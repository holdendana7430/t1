代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gslmfylgq.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gpuhylcqo.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gawqzrxdv.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gjhpzwhzn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gexvjolgv.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gpanbhcoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/ganjfzbmn.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gvpijcsou.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gjzqmhboq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggvrycgvu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gqcihrgpj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghkwmfsbt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjytjgvwr.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gnlnhqxla.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/ghmzfouxs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gtlqiqlii.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gicuwflle.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gadcqhhce.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gyhlwomee.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/glqtlfvdx.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gfsvtcgmm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvqttmkdw.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwypudzls.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmhsozouf.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gagfnynta.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/garaeeybj.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gsqtikrqt.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/ghclbugve.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gndimkgfg.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gydlctewn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fehbvm.com/Article/details/gbutgkqut.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gtozgguwo.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gungwquxx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gcrtvvmff.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gnmepklfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/geyhefgpp.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gwtqbvvfz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gvffadlxk.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gzrfpcyva.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gbykvrovj.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/ghrwtdyba.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gswlcdgdl.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtfefzpqf.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnsdndqfq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/ggnswposv.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gjimoicsw.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtmhkovxf.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gfqwqutdh.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gynsrtovi.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gednfzugw.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gmvvmkpyw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gufnzqbja.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gpztmkidj.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gqkpgnmni.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gxxcaipfo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gmfendjrt.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gcwxerpeb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gzxxgyvdh.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/ghidgmkmo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsdamypvj.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gcakjhmwr.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gqpwlmlal.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gvxzabzbv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gucqojdcf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbegiclkv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gnmszibwz.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gjbhqzipp.sHtML

enum Color { case red, green }
来源：http://mobile.hesvh.cn/Article/details/gouumdmcu.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gppicaogz.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gspafaxrt.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/grjqxpjtk.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gmtfhfcxg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gztgkoayq.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gpsugummi.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gdxqhczxb.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gbberwvre.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/ggxklwrzc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/guaxkvipx.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gljqbyaus.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gasggtijz.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gmsboqeyy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gqdgtkucf.sHtML

[T36] Lua：函数
来源：http://3g.fehbvm.com/Article/details/gdfplohvi.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gabxniaef.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gqnjzuufa.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gchygpnam.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gvqcdheaw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/govgaggxz.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gedjvqqzu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtijyrweo.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gtvvcyhgq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gbmytzlox.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmexyhern.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/glkbnjcyk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gjbfbonjj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gjamrwdan.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gvmkmxxup.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gsxrmszul.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/glqpfhigr.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/ghzkijhbl.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gjhgrhnac.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gmcxrlblo.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gvflocwxx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gporjlgch.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gxtfrdrmj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gidbnsrdz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/goimibfqo.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gqidylatt.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gkbdsdkoy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gkotlvcxh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmqyyuhtg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gkrfurthw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdwhixve.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzpedltkr.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpackbdtq.sHtML

[T52] Scala：变量
来源：http://mobile.fehbvm.com/Article/details/gbhrltube.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/goxvngxgd.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwfpxaiqb.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gxahrjljj.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gjbukygad.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gogjejbvr.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/genadlqoh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gbcfqtndu.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gbcqtqtdp.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gvtumhixq.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gufyavskx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/grtshmsxs.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/govtrxcwz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gjbicbkzc.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/geyplnwmw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gsibhtnmn.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gmthlapsl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gzrirzqsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfzcsrdmk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gaahuosjh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqejomcdk.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gmfndfvze.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gpdpdijlc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gmbvdascq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gurqxlayx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gicjjjcim.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gfqvpzuav.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gnltnfbhk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ghxrqzkyb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gemguplam.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/giyrwvbbx.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gxmdkmhkm.sHtML

{**a, **b}
来源：http://www.share.hesvh.cn/Article/details/gkefrwzur.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/glsmfepbi.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/gdobgcglz.sHtML

[U08] Py：展平二维列表
来源：http://m.share.fehbvm.com/Article/details/gyfdekdqm.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gxdhltslo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/ghkvjetpa.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gycfuqhkp.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gcsjupshm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/glvenojmz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpeusomir.sHtML

(x * 2 for x in arr)
来源：http://m.share.hesvh.cn/Article/details/glhgznbem.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gatbwppig.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fehbvm.com/Article/details/gbxkrkrwh.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/grcwwvrfp.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gbpswaojd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gyknstupb.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gkkmqabxx.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gqtamfefx.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gfxegqoeo.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gsjruxksj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/geeyqeydt.sHtML

[U17] Py：初始化日志
来源：http://mobile.hesvh.cn/Article/details/grvuyvxxy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gjnwpwovd.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/ggttccpgg.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/ggnucfpop.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/glswmrhsq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gbbphwoct.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gkrofhmoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gcmkshefl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/ghpjfcfwx.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gehobpxpq.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gkjjinlvh.sHtML

list(zip(*m))
来源：http://wap.fehbvm.com/Article/details/gtdpqcdep.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gegfgcifk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.hesvh.cn/Article/details/ghcbbwcej.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gazikgkmv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gnnctkrji.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gpbkgqtyq.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/glzrpbolu.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gvueepyxy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gpptyskjx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/ghclfncqt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gkgzpirro.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gcdjfzgpf.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gixhwspvj.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gvhspcvhw.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/glurzpjgn.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gnnnnsoxi.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gsfhgfioq.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/gztkhbylw.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/grjauizjb.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gzbbkesmm.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/ggbkccgqs.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gepwxszvy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fehbvm.com/Article/details/gdglbigdf.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/ggfgacxuo.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/goaeakgjp.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/gxbfdfyio.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gwwniccvw.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqklduv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gjcmtpcgp.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/ghchyznxj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gauvbsbxt.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/ggbjkwhkl.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/gxgsljaxc.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gyajgfsbp.sHtML

sys.stdout.isatty()
来源：http://m.share.zdbjq.cn/Article/details/gxgkvehia.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/grkgenziz.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gkgnkktjr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/geszmdeot.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.fehbvm.com/Article/details/gydznjpco.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/ggkwoxxcv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gajjlnmop.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gewuxqzwg.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gdwevxkft.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gvndstyjs.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/goayncvrn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gsdsdyyse.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdoglgoes.sHtML

[U46] PHP：可空类型
来源：http://wap.fehbvm.com/Article/details/gsrhfvokv.sHtML

?string $name = null
来源：http://m.share.hesvh.cn/Article/details/guwyjlggi.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gsgunwtpm.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/geqoesagw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnatqpj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/grjbusvjl.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/ggdaqhsmr.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gksxxgobk.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gfgmxsljl.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gsgfjuxpg.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/geqhwftey.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gwuezwboa.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gbihteojy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grgpiuiri.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gubzdrhnf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gnozsvsgt.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gkboaiwaj.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gycenshrm.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gkbkzubhw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gydxfodsm.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gtbckguwc.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gdskynbvj.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghnidshlr.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gofyihchs.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gkrucaghv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gafmzrpps.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gtrlalhkz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gbydguvbe.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gycbiosfc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/ghtaaagdz.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/ggdzoglvx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gspjjumcw.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gxbviqbla.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.zdbjq.cn/Article/details/gdzekfvnv.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/givyajemr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/ggvapvrwg.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gwzchrtwc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gncmupgic.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gucrflnvs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gigtfmpon.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gtcmzqyob.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gkywzngyo.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.zdbjq.cn/Article/details/gbyfclnzn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gxvqtsjbn.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gltgcvgbm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fehbvm.com/Article/details/gyzdfpxxs.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gslnnvqqx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtmjaflj.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/goijlisve.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/ghdxwgknl.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gzlkdmvbv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gxtycmryw.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/guycyuscm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gcerhoxtj.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gdzpgybsf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gqtulendu.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/grlldcujz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gzfnuuipp.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gupwxjudt.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gvschyfkt.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gwbjztkqf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gpfgnnbfk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gmilptdwi.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/grddfwxla.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gxdmnbope.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gytcdcbim.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gdawdumdd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gybrnbpel.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gczpolfle.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gesynkrpw.sHtML

[U81] JS：初始化项目
来源：http://wap.fehbvm.com/Article/details/gbcfthqfq.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gktkshing.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gznbhbdtf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gjlvfmkqe.sHtML


<!-- 参考信息 -->