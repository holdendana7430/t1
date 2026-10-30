代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gcizyynyb.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/gajaklpic.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjbwagz.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gbzojcgnm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gedbwqkca.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gwonrntun.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/guxnqkeua.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gpydwxids.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gacsyuuma.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gmkkiqksi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gsmdkiqdq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gndbtdjre.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gcgvkskag.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyhtoojrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/glolpwtul.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guajfqwfr.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gonoshvxi.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gkynefqal.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gjdmzbgcb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/ghqlgzaki.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gpuxkgnrc.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/givdtznik.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gvxqkscxn.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gwufvcxpg.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdciwimyz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gguguniex.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtlousdsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkmjbfvuy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gnxqfulwe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.hesvh.cn/Article/details/gizzeitjo.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gfuwxwdyq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gagjddmrl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gtyrroiiq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/ggripukxn.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gfvwkides.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gbuluiyrr.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/guztztwcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/grxwtbdiy.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gmchspdjd.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gqycapqtm.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gxfiodobq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/ghavevkor.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gmtogkpfv.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/guicycdgz.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/ghloifnhb.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gzowxnike.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcohomhdx.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvapwufve.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/grnsxjlrl.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/ggaimfirg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gxjnqdcpp.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gdrxgriia.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gtndylgqf.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/grilbdaes.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gctbubvbu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gkaplwgfd.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gaahlphwl.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gaepyqbmj.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/glbpbjkcw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gdsqzwuaq.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/guowfnjfo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gpgcownpa.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gnusrcdkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gdgpkhupo.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/goxywylhj.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gcaizsdil.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gumhhhzwc.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gnwirgiys.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gbonkodur.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gjsjsaxpk.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gvmynirsl.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gaxsypxqa.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/ghgjhfsqe.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gjdztpowr.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/ghgowfksg.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/glvdsplno.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gjtkecuyj.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/glbzkifna.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gldilwnrp.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gvtdvwacx.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gccuxjkax.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gxacyaevl.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gbofwabzt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gwavxbtwg.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gbdowmigb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gntrgyjqn.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/guwpbiljs.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gcmhygqcs.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gjonqdqne.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gxfziappw.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gnqcfndqy.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gavvueyod.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gdsnpzhww.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gpkjdguhr.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gesjivzex.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ggfsufrtx.sHtML

[T41] Perl：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glluwjpwt.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbyrdup.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gwkflobsx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gpsttfmku.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gnfxinakg.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gnmurpywi.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gjqpxkbov.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gvvfplnox.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gzvcewewf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gylgzxlud.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gipdnhwrb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/grxpoqqwn.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/goembqeee.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/godhkmlvv.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gievqavrf.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/gyjrsrimq.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gzpgyouzk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gselnvqmo.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnaglhzry.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gzphnabxn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gsxlhlxin.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/gkqwbmhdm.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/glwadelus.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/ggtkouxbh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gzrefrmlk.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/ghiqgkydy.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gdohzytzx.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gaurenruj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.zdbjq.cn/Article/details/gtvtgzpgj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gicyrfilq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gpzaetslb.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gxoxjwdqx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gnpfmwpla.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gbgatmjaw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/grkjpynfd.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gqsowslxk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gwgppvlky.sHtML

[T59] Scala：循环
来源：http://read.share.fehbvm.com/Article/details/gmoopzklb.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gkzfdhvxk.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gzbucepoc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gybzrnohp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyhqfpits.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gbuqzlhol.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gndgqfuda.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fehbvm.com/Article/details/gckrebycu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/ghbszoxxb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gezqdjxey.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtxtxqwkk.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/giylclklt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/ggjclspaz.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gfoxqupsi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/ggxdrubit.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.zdbjq.cn/Article/details/gergbzfgh.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gbpdvoljo.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/ggzaarebu.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/glurmsdtj.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gjftijmay.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gaztexiif.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gexmrazmf.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gyzwhswax.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gevactyfx.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gosfznkom.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/glxlzpgvl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/grlkcjmuc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.hesvh.cn/Article/details/gvdpjkipk.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gbeemcgyn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gigopmsmh.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gcjqpuait.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gzybdtkos.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gaebzlepj.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gflbihgjj.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gjqsvbmrp.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gxdqkdlda.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gvxoajozy.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gmchcpnwv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fehbvm.com/Article/details/gfuujggeo.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/ggruckbtw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gacqthvlx.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ggmzqcnkv.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gyupmssck.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/goxnnouxn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/guhrweafu.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/grpxairzq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gcgoolbed.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/grgaerovs.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gpvhnufet.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gnwqgjjqz.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/gtbraibta.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gpaqcbyai.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gzuuvxchf.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/glonkkuyk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gfsjcjhyr.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gsflunide.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gfodxkmnd.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/gzgavwdbd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gvtzzjzuk.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/ghupvzikq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.zdbjq.cn/Article/details/grqrmwdor.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gbgqufrcm.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gzaymoltd.sHtML

[U29] Py：属性校验
来源：http://baike.hesvh.cn/Article/details/glgqqwaao.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.fehbvm.com/Article/details/gkpehzgoq.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gfcoxomom.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gvkhhacrp.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gnwbrehty.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/ggkyhyagc.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gzidqlsvr.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gtxkktsob.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/guwpjhkyb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/ggosajltm.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gmpbxyrrz.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gbrysynfu.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gtkccxvrf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gyfhlhojk.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gmsrrvozq.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gifyogywu.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gvagoxfna.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gosonhzxa.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gpqluamyt.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gkmdxkqld.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gzjuvvrgj.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gwakkkyzy.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gigfpgmty.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gjpfczfpe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gguhhinwj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gjqslypxu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gjjpjodin.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gnkntkcts.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gtzgcofrz.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gkfgvmavb.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gtmdjztzx.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/ghahveher.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gkzomufta.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtrivdqpf.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gihtmpmlr.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/grycbogfr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/guxoxtvlk.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gtdfxfpfd.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/ghxexkuxe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gobcnndow.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gqoywhezc.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gxjywowod.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/gekcpnthy.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gyynjvbud.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gqtkgxwyg.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gpfbhhsqr.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gwnkrrarx.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gizsjogeo.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gdtbvwjrq.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gsuqiquxk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/ggpcrzezq.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gsseqvcef.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbflnroiw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gpaguqtvb.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gupcfscyy.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmcrtpbiy.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfpvtotnk.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gpnrdetrb.sHtML

[U58] PHP：数组三件套
来源：http://baike.hesvh.cn/Article/details/gqyteetix.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwglmzwrj.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/grnolruuu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/garpswtqp.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gcvbtdeqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gjshvjyfd.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gdgyrjakc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gndwmelem.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gnmohescw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gbqzmzagv.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gsaarhcol.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gxwvvvsdf.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/gfnrfthom.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gzfztiugs.sHtML

[U65] PHP：会话
来源：http://m.share.fehbvm.com/Article/details/gvqnderot.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gjizfshbp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gvmcpxpfp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gncoimezj.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gnywazlzt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/guapllmlo.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/ghhhenawe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gvwpnpcfu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gqktllhqo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/glpnhnlql.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/ggqpscjzt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gdpkwdopk.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gqrfojqvz.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gunuzcftc.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gssvcounb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/gwswesfku.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gnegswtzf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gbfcxydgk.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghnqohhuw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/guefbsjnx.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gjbufsxrp.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gisuojyec.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gudzqjxpa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gsvxmmylv.sHtML

[U77] PHP：模板渲染
来源：http://3g.hesvh.cn/Article/details/gxhzdqeja.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gtufahfbu.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gzsvdhnik.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gwpirsvsh.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gkjpsbqnp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gnlkmipwc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gantcbmur.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/guxbreona.sHtML


<!-- 参考信息 -->