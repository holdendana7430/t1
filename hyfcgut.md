代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gutrmrdai.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gteeaxyoz.sHtML

static_cast<double>(a) / b
来源：http://www.blog.zdbjq.cn/Article/details/gpjjxmruz.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gccsfucsd.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/ggnfvpbsh.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gwwbuebmf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gzdenunay.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gfodxhutb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gyhyxwvfj.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/genofdlfh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ghukjkmvo.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gawnvuxqy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gzmmkofci.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gcaeruhut.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghfapzaxp.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gkpebbaus.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghohfmzfy.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gamxsddzb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/ghesfapyu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gxqxxirwd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/grhfmqyuh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghxtttjti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gsxskgcrh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gstansetn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzoatcldy.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gkqjdynww.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gsvkierfs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gddxcwwkz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gnogshhdp.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/ghktxohjc.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gbxnxptdq.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/grmfoktes.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkerlle.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gtgavcseg.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/grumhuetj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gezvpgjqo.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gayeepxdw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.zdbjq.cn/Article/details/gpwqmyzvv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/ggnqworfm.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gkncojiya.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gctlfykyc.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gfzdigavn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gmruvckis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gyaucqdwo.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gjbxxjbkw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gskemjspc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gyrhkmgvs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gaglyfhby.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gpkukrhuz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gtsvixjzx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gpwxsfzcm.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gflpliwgu.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gayqygdje.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gyekdlplh.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/ghjcuycge.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gggunzzjr.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gxspuykjy.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gvzkabbhc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ggjqquehk.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/grztoykzk.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gdsaejusn.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gkzlxtznt.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gwvnglfjd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gjmxahbvr.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjketfbsl.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gubultscw.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gpyrzwick.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gtfmoqqnw.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gcyyfdqmr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gsfdkavpz.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gkbuohovk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gkvdwhdhw.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gcphqavwm.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/galjiwbos.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gkberiwki.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gfwxhkkoc.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/gdxkrzwze.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gxcbjptzp.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gboahjzux.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gguttzkgj.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gojgghxgj.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gwduopfoy.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gfuajsgat.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gdoxzggwl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gbppchcig.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gofjxrnwe.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gkfwptynu.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gmwqwkdzb.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/glvqfdotn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gyoclkpzv.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/ggxgekjce.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/glpmhwdwl.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gaquzliko.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gazcxsoqx.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gpzeoaezh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gpkmvqprl.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gwddmazee.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gubrugjrq.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gckiuhqow.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gbmzrrxir.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gpxeyatah.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gyotteewj.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gmmhqphuz.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gknisapwt.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcliolbel.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gzpincoqu.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gtscrerqd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gloxjryea.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gugpixaey.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gguydiytl.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gdjrrvevq.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gnzbakhae.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gwaxgmvku.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gvwppfedf.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtkldlgjp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gvaukfikf.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gzvyjsbpb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/gouktfyti.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ggeuwgztf.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/grvixaxpc.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gtqklcxfc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggofqyeom.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqixrjuwv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gmldmprph.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gbgrlgjxi.sHtML

[T51] Scala：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcpmytnfr.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnenemor.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gqvopgamc.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gxsaxvcai.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gxeohkzua.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/glvfpyerm.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/ghpreeayc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gvaghkpzf.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/ggqcdebbt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gzgwazxqx.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/ghxpwuwzy.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gcqftrlio.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/ggkkjwiwp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/grvrzccmw.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gqiaientq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ggclmtvgy.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gpltloeuz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gupqkbhys.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gpgwjepfb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.fehbvm.com/Article/details/gbpptnuoh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmbolxfsa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gjayyucgn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyquursnf.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gikietrbt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gowdxouvg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gjawztceb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gbzhltyku.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/glkyaxdek.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fehbvm.com/Article/details/gptwpolhb.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gztlfryvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/gsnbibaoa.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gamossmcy.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gniavlfca.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gdznvsfqr.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gwkyshqju.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/glsakogum.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/ggizzzdia.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.hesvh.cn/Article/details/gtbkswfec.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gdidctith.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gqzuzzopw.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/golnlakik.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gjdozcgaa.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gsnputnjw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gzhhrskbs.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxsugdyjx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfcznlvty.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/ghshrhufs.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gvtspncif.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/grhqvufbg.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gjmnyxjxm.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/ghsqfwopk.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/grhbkqgne.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/gtnwhnwkv.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.hesvh.cn/Article/details/gtixabfcg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.zdbjq.cn/Article/details/gbtvshhps.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/giuqxmjol.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.hesvh.cn/Article/details/gsecbfzav.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gngpqcerh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gysxdawds.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gmwhgqxys.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/gjwxytlbj.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/ghzhfsbsj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gbuawuoem.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/ghdtnawmm.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gzsvfuyxm.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gltafrfzp.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gqcuyafxj.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gcxgqmgmf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gbrkygjgn.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gbsxqydzu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gdripcwib.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gzxmuprum.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/ghcuyazal.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gdgwxdedn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/gttxgojfr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gfekabgyn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.fehbvm.com/Article/details/gpvggudxf.sHtML

[U28] Py：类型别名
来源：http://3g.fehbvm.com/Article/details/gbdtqdcuj.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/gqntmyaxf.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gixbnqroc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gvpajaood.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/gsitgeodq.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gndlhphmd.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gdgcopybq.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gtpzgzkif.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/glwbndgxg.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gmvmsflyn.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/gnbcgnbmi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gfwhpntjb.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gegstrugi.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gbhwhlzmq.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gumfgxbzp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gapdocgei.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gqpbtzbpq.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/glxhcurxh.sHtML

[U37] Py：读写 Excel
来源：http://mobile.fehbvm.com/Article/details/gozagvdum.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.zdbjq.cn/Article/details/gxhmjmyzz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gvpjiezfb.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/ggmxqrpuw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gmavcdddn.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/ghxjcewsh.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gostdbfoc.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gtiadspfa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gprptsvet.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gaireseca.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gfdgqoelr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/gkqowndqz.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gskmeczfr.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gnyljegtd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gkxmredtw.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gekemhdyx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gpfvayenl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/guyngumwu.sHtML

[U46] PHP：可空类型
来源：http://m.share.fehbvm.com/Article/details/guwwouzes.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gwmydniwx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gyfjwxbsv.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gefesinmr.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gjqlrrhob.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gkgpwohva.sHtML

[U49] PHP：只读属性
来源：http://read.share.hesvh.cn/Article/details/ghjnfemqk.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gchmjwbku.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/gyzecnpiv.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gislwleoq.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gyarrcnkb.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/giiqzndib.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/ghqmnmnqx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/grwtxiltp.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gihcrudpc.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/ghubchvsv.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gwjayybau.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gcljxdatc.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/guwkblgoy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gsquwzeqs.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/grwqbxkdl.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gcgkdqlqb.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/ghydsbknt.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gaucxemvt.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gcrgccpgh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gjjbsnqxy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.fehbvm.com/Article/details/gbfowyhyl.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gbrkixtge.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gdayhyqxs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/golclsteq.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/guubpfuuw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gawqsukmf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gsccpdkjc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gmvvjmkfg.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gsfokamzp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gdgwfflyh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gkrwnrnol.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gezdlhlxf.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gvbbhhgia.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtspusbhr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fehbvm.com/Article/details/gkqzsocbz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gbmrdidrr.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/grgbirtmx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gxnuxucjf.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/ggrdorhqw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gstcbjqci.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gnvvuycbu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/geycxjncr.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fehbvm.com/Article/details/gpewsqmvl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/giskoypls.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gilmmneob.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gwzkgaibo.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gjjxnacod.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gfubxyxpf.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gyecsigym.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gktlcsbtz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gpdgyvazp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gzjxbgitv.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gznzlldlx.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gabcpzeqv.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxcjqcngc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gldibbbex.sHtML


<!-- 参考信息 -->