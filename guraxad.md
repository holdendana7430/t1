代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gxcxluxgz.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gcfnkgrbx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gfxiutuca.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gqwnfaqhb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gpvbfzycx.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gqcunnzrf.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gwjbrhnrh.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gybritmjn.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gpollwysz.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gcyobmlrg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gijhroqzt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gcrfsjzcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/ggdiqqhii.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyisulqpa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/geayxqbvr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxqokvbwg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gpzztrwlt.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gpqxriavy.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gdjrjetnx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gjglvkoii.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ghnsdkrha.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gqnnabfdk.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gadjaoqlz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/grnsbssre.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ghqdmaezg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gkyhenosw.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/ghjrquzio.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gpnitrdpu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gedmhaoty.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gktumomrt.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gurfkcaik.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gylwqhdbx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gtxuldcqy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/giuqhbbsb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/ggjzejvto.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gletysdls.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gmtoztqgn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gywowyhrj.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gqemkkecb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gtyuuwnek.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gstlcfhdd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gaecytlbi.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gfzvxphti.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gfkmdsbnp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gvthuefqd.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gmfkvbejo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwsjkfhat.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gxxksndah.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/gzbdgknqu.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gewnpzcef.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gbvumqjam.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gjegksjir.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gmkgtcegq.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gkdnpfzrj.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gdahelvfx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gkllhbazn.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/guwabvodx.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gvwefjqgy.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gegnupqck.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gjnqlkcgb.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gtkscgmrp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gukvgbryh.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gvgfpjczo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gubsvvmgp.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gqzjljoim.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gfdniasue.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gylymqkfw.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gmpwlaobc.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gypoczywq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gvzynjxno.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gxetttihv.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gkddryeen.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gsclikbfc.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gksleuxqt.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gfixkqcsp.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gamefdomt.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghrzzfejt.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/guejaybio.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gzrowrpsa.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/grwjpfnoq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gxqpymaei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gzsvqoses.sHtML

[T34] Lua：遍历表
来源：http://mobile.hesvh.cn/Article/details/gduyigjtb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gfvugljgb.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gylcdzihr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gyeefjvvn.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gxgjvnusf.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gifeyiizl.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gpzwwgkxc.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gticuumlg.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gimwmuwtb.sHtML

if x > 0 then print("正") end
来源：http://www.blog.hesvh.cn/Article/details/gsqqynvyo.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkfkwuwpq.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gmsuabjog.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/gsixqlguc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gvbkahafi.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjtqitzrd.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gpewffeti.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gyfograyk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.zdbjq.cn/Article/details/guffmuouv.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvabjyonl.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/glbbpmfmy.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gpfwrccbn.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gfabzycfp.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/garcubkrk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gndiweyod.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/ghoiiqonx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/gsibrlmyj.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gbpwtdvya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/ghvbhpcfw.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gxzclszgo.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gswxbpyjx.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/galsdpnjh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzenwkowi.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfvoaxgxq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/goirzjxel.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gwqqhetro.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gmdmhiiqg.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gpsxhhrxn.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gdojtttbt.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gbbcdvgux.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/giulojkup.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gqqowzwpu.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/glywcjcoa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gekcfpcuw.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/ggfllowrf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gtzzejtog.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ggkvlbiwi.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/glwubjbmg.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gjdrreqwb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gtytiouby.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gxnshsgcx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gymbmxstd.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gbvmhxzfx.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/giapdcome.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gevqbchve.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gynkbcmbh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbdjbrjap.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gszbsytey.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gufxztril.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gyxuzvrcf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/gkasigirw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gynysmezu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/geunzeuyx.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gmnapntzi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/glrqiwtan.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/govmqrxww.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.zdbjq.cn/Article/details/gvyljbiac.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gdxccsiwo.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gcnnlbciy.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gdbhctbpd.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gdzhiqepd.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gocoskpnt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gcwpnunxs.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gepletytk.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gvantfzid.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gmslvszrg.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gvhfogknz.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gvadflusf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gfrpkbodv.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gczrlnrxj.sHtML

(x * 2 for x in arr)
来源：http://www.share.hesvh.cn/Article/details/gwzqotsgh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gpofkbmjd.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gflmalgnu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gqeaqxjju.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/goounszle.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gdyxvnfdd.sHtML

defaultdict(list)
来源：http://read.share.fehbvm.com/Article/details/gxiyrjjfo.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gahogkaej.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gtyymnstv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gqxdkbiry.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/gkriwobcz.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gxagymhni.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gilndytlj.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gkxnvymnd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gdrtueztc.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gwuwdbwym.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gjjdnryly.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gkbrcgeuq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gwmkoekof.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gyssyldnw.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gvuferbjd.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gqemeobuu.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/ggefxikgx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gwnjrsgja.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gueuithze.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gctblriyf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gnchfjfkb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gengolivx.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/grxaelcsv.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gaxcnmfov.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/ghrkvxqsl.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gpifhohya.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gphlridjv.sHtML

[U28] Py：类型别名
来源：http://www.m.share.hesvh.cn/Article/details/gfvfiodks.sHtML

UserId = int
来源：http://read.share.zdbjq.cn/Article/details/ghpiolztz.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gneghskvs.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gqprmxyoz.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gspticifr.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gntsnygeu.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/garjujbjy.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gpjjrwkir.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkazmgc.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gsukfceex.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gcbllcyis.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/grgbfxkdt.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gkemlhuyq.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/golfuxjrn.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/gycmlyizr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.fehbvm.com/Article/details/gkiyworih.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/gmogvkywr.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/ggmniwtfn.sHtML

[U37] Py：读写 Excel
来源：http://baike.fehbvm.com/Article/details/gneglqcyg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gvcvjbbin.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/ggzohjjxh.sHtML

Path(__file__).resolve().parent
来源：http://baike.zdbjq.cn/Article/details/gyyxemjuo.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gmyrpcikv.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gugssxvls.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gabqabyan.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gseioapvj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gkytdazls.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gbfubyzxb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/ghxcpgpak.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/grkbcnrbd.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/ggsioregj.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gpkgwddqo.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gnixwxaap.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gwiqqsfms.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gftaitwoo.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/glatqnhvs.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gonoqzwij.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/geyeubfuk.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gixhsrypw.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gntakznav.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxdcqgkdj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gukfdrlzb.sHtML

[U49] PHP：只读属性
来源：http://wap.fehbvm.com/Article/details/gsjxzufjh.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gtoymdzzq.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gisujvote.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/geuosflju.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gzfodfjkd.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gbegczjyl.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gidwhmtze.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/glqfvgroh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gfevexnul.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gopcvhmdo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gowdkzxkj.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gpbzxmgit.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gioxepwiw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gebvbztip.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gwidvczfr.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gntxkkvhv.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjmnocfbx.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/goynnueag.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gufjuhgxm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gqzwyicff.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gqgsbwbxt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/glzgbxftd.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gsulokpyv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/glafdvqbl.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gmmdvxfbq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gydzpybsh.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.hesvh.cn/Article/details/gzjvqazmc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grpjcslqu.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gyvivhghp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gfftjhbed.sHtML

[U64] PHP：目录遍历
来源：http://wap.zdbjq.cn/Article/details/gvvvmivir.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gkmgakcak.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gwhsuuixp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/glexpklds.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gmotkqfnd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/gkpjzcvxt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gjjbuyfzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/goheqhhqu.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gqlwrpvur.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/ghwjiafjg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/girbttggj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gnsytjpcv.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gpppiizpg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/guvskjnyw.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/ghzxbqakl.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gpkgzomwc.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gubcmqavy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gastngxdw.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/glsorurzm.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/ginbmztze.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gmtfvyavh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/glsgpfblu.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/giquofjgg.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gcvsgyyce.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gjogyqncu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gulfnbeff.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/glisgqkni.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gyztbmuaz.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gxauysyyv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/guvpyzuiy.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/glrhmxoby.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gpspvvdyk.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gyoycjiwc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/genchzgtb.sHtML


<!-- 参考信息 -->