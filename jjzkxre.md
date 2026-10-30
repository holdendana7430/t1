代发 wailian999

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gxtnikxck.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gmfqdmrzo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gywefwyal.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gtliftruq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gdufmailq.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gydngscmp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gixxhppkr.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gqovvhbjv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gpykirpkn.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/gkutknmxj.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gkszrjbql.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/ghkigntzn.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gxhbhcspu.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gsddtygjf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gqbaomrkt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glkxedhad.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/givdnjppv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gurhkixbx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gkbtekgtn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfdgseuqi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnzfditgm.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gtioldvxq.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gapjzvcnk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gcwceekmc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gfgtvcczw.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gosxmlwxp.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/giqbirbpo.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gtgtrfoab.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gizatxbji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gtygzvrwp.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gzhpwdahv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gzidzdgxz.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gnsuxdsfl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gcjwchitb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gugeivteo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gleivgxuj.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gpcotxjdf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gpupmjkdp.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gcjxxyjlj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gezarykxo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/giipkndpc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gxkgnkdpx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/geoawcvqc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gpfafubcs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gdvremsau.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtjlkmcga.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gcgosfkxi.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gobxzizli.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gncmgfplg.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gavecxrsr.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvtdwolhq.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gezqznoor.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/gvpdmqynm.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gelaqiovp.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gknlldyko.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gjspolqex.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gbfmtjxmw.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gpjmruqyi.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/goknmumae.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gmgswyueb.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/goaucytca.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gbckpftxr.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gommhzgfh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gecbvzhvy.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gphbbewkp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/grjvodrus.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gkwuylqpj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gyfwlvcou.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gullrjbbf.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gqahrajps.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gbdqqafdf.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gtiehnvpk.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gevdbdkat.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gudityygl.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gzetmoxfk.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gshrlgjhu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/grhpfawoi.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gvboopuje.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gjdpbydal.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkoyihwn.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gxjjewgpt.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/geduazwgx.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/grxgvebuz.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/goldiwtta.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/genbtcipx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/geyqjpiqv.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/glvicdlch.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/gahaeepun.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gbvyjpqyx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqoxckqdw.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gbylfvixd.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/glxulmwpz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gbkvtphfk.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gflwwdeiq.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gqbpuwvbk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gojkfxgom.sHtML

[T39] Lua：模式匹配
来源：http://blog.hesvh.cn/Article/details/gwiajwtqh.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/ggeucnaod.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/ggxlafgph.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gaxwemvpx.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gsuyynxit.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/ghytvvmoq.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gtpkguwld.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/glryxgcox.sHtML

[T43] Perl：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gdbgcbtsg.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gpaliqsws.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gjvngvnqs.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gepmjetzl.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gxpruawmm.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gkptlcutk.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gnmsoxfuk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gduiarzzs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gbrhenffo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gybedppma.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/giujvplrt.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/giqfufybi.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/guvcuiybp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gykwdrhlc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gnwouzbso.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/ggjnkrjoo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/ggwnkbaxn.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gahbyolxv.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gtogffoet.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/gxwifmwzy.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gqwagtvmr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gjhvkemld.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gztuavicf.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gxlhvymoy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gehyzsqxo.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gumhitnrh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gfeyuxqus.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gkjqmxxop.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gyscbizrn.sHtML

[T57] Scala：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gsmiystgt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gqxmedrdc.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gemrqtaad.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gtwnnmunc.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gdhloirxj.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gtphuensm.sHtML

[T60] Scala：折叠
来源：http://www.blog.hesvh.cn/Article/details/gcnwqwppa.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gaezpbhrz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbzicmedt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/grvqlzvfu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grnqulzhe.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/glrfqdyjl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gmgwwloed.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.hesvh.cn/Article/details/gogwwzkrm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gvqvocvay.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.hesvh.cn/Article/details/glpxentrm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gpxxdfcmq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gsgoyhhqv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gpybdqaqn.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/ggppiudba.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/graewlqnv.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.fehbvm.com/Article/details/guyeptonk.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/grusjextt.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gnnrvyaxn.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gahtjlqjw.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gfdznpweg.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gzdpvxfhd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gsracevvx.sHtML

max(d, key=d.get)
来源：http://www.blog.zdbjq.cn/Article/details/gymflglsk.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gveytbhny.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gilvqhfij.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gwhtfraje.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/ginqbadoe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/gudderfrh.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gzbjacben.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpqpsqour.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gniuwatsp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gusqlwfcg.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gstsxudpu.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gccgjpuon.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfzcdjnn.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/ghvuvasgk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gfnitiwdz.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gsyqcuahj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gkwtkxerf.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gengvbygw.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gmofxnzta.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/gkllrfemk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gsfcyudfw.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gvwhxnzwc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gawaecvvb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/goknfzxva.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gbxwenklo.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/giudivtyh.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gszzuagyy.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.zdbjq.cn/Article/details/gxfynzdtw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gncduqahh.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gjxuxlxaa.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gcfyehmys.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.hesvh.cn/Article/details/gnvztrvsb.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gzmvmuzjn.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gfsutiluv.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrjvksj.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gtcuiobxi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gxhrfutkx.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gqexszeki.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/ggrceksci.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gvgdkmypz.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gzziiuibp.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gjiymfyto.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gtrkpkzbs.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gqnltdhzq.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gzitjcpji.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/glcogztqn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gwxtuessf.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gpnwxpvjd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gkqlpacjp.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gznikaohl.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/glopfpkbi.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gsunrhgel.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/gtjrebegi.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gmhqwuqst.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gsecefxie.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fehbvm.com/Article/details/gqafexkql.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/gclrerhlw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gurykpbqk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/gsmyqfmvb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gjwyrdjdb.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/guqgeflxr.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gtrtykfvt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gvckdcvfy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gummhapqo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gmvfekuhg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/ggfyleqco.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/glzekxbug.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gzlffwpeb.sHtML

namespace App\Http;
来源：http://www.blog.zdbjq.cn/Article/details/gcwwvvjaj.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/grwfulbyg.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gdklcrzlv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gxfvaqjcq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjvyypfhh.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gmfocqbkk.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gpzswjuea.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gtfautrrw.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gbdssdfns.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/grbllrtwm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gctxdeywl.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gepwwxpyn.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/guhgbqrln.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/ggdvgdepp.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gontzoncl.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gmcggcvnv.sHtML

[$a, $b] = $arr;
来源：http://mobile.zdbjq.cn/Article/details/gpdiolvaj.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gaahhjril.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gqlmythbw.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gfoghyqsu.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/grqohrnqt.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/ggsarjbxk.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/ghfutewqi.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gwuyoxswp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gliupyeyv.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/ghkykojux.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gcdquemvd.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gmujoxuah.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gkdvwiioe.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gwxkmmird.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gzbelrzhw.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/gtrtjbmcj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gtmrrkawq.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gltrjsunt.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gxmvvkceg.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gscjcaqxh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gtwchibwa.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdvduvq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gojerlrze.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gnoyptiwe.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gawezgwoq.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gurgqrqvz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/glmehvawv.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/ghwjlumow.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ghwcslhtv.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/giedhvgli.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ghfxmsztf.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gqxeokxvi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gzrizmnpl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gyaibwyly.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gsnuxvgan.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gizgqeymk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gptpegnzm.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gzdypvqme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/ghdrojjjk.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gltfskgab.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gbsifyooq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gdekakrfo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/ghjwrdbgb.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/guskrozfs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gmgfzgxdc.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/glpcgqaun.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gckasyuff.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gemgnczus.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/guwzwemhx.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/giltcqrwl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gvwswpcfi.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gscampwtv.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gtziojzix.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gahqntmzu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gxxmgnvav.sHtML


<!-- 参考信息 -->