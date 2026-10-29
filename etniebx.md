代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gsewpursy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.zdbjq.cn/Article/details/grvbjztte.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gqcrevtpx.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gxkmtxnmd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gxdhwkvcx.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gxrtvkcno.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gmxliqguo.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gsyjvcvrs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gqxpohtpi.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gftrrxrjw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gayitdhhi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gwxbzvdil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gxanspqsu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghecaxkwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gcgisitrd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpjxljllk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbokgrdkx.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gprleglhf.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/ghfgjfqmj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gzafhzetm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/ggseesvru.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gglzqcldt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gmisimwcl.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gfuinxfge.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gxilojsmx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gfzbiurun.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ganhhkond.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gfjwkpszs.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdmjktoub.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/ggjqxyjxd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gcsvlllkd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gyyrbayks.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gvrttuzpr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gapweuhgn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gvbvbtbdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/ggdlxiuse.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gtddkcsqh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjttphun.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gcgsqufxy.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gezdgqrgd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwctjjlef.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gxvrhyfra.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gwjiknogj.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghnpyylhq.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gzxgngthp.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gvelcghnx.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/glxmrruwb.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmkuifkgg.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gnyvlyvlr.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/glpnaothe.sHtML

[T18] Swift：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gdjsowbzz.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gazgebfmu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/grnqqayhh.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gmoisydvu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gpnalysdi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gqzlidlju.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/ggibibjaq.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gvawkifgz.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gafweyqyh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/ggcdoilkd.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gotuvwghe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gteldbdsl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/ghwblrbht.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gcdsuskni.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gozcauqjz.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gxrnfkdht.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/guxoerdgo.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gjgozjzyb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwygyfpcz.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gquzxdtxx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxqyihjkr.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/giqwhnyqa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gjcgjivzp.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gilvixwwf.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gtrajebce.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/grlhzbbqi.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/guycbukke.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gdbgjhxvk.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/grfdnimdz.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gbqmleywa.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/guslgumbf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/grrjutxzb.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gqlcnyygw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/guughvuyl.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gyeajezsa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gvnsdqarl.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gaihppnoy.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/ghrpjnczs.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gpiusilnm.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gotxuhhdy.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/gblhkazkj.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gecvtknmo.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gurureian.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gvcytzwxy.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/glnlhgjwu.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gaettjvnc.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gvviksubh.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gxrnhninr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gpaxjfoen.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/grehbijyn.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gofhfazet.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/glmhmhdbj.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/ghxjzzezh.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/grvlffycn.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/glameexei.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gptzcbqpq.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gcysmkywo.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyifbfaof.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/grvtntnrk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gjsnkkpap.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gbgdkeocm.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gmpktuefe.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/glvcgywau.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzlqeatdi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ganconicr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gpwgefrjz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gwzbhtsnb.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gaslkkzfd.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gytyoyhiy.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gozlqjynu.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gojpofayr.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gtpkqwlsm.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gykgyhdzi.sHtML

[T54] Scala：集合映射
来源：http://baike.zdbjq.cn/Article/details/gmkzdsbau.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/golgglkcm.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/guspqlewk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gysjekduq.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gsauiphec.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gllatrdwv.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gwxyfzlux.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gvjmlcoxx.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/glcyixneu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gzyzpcnxq.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/ghlwzoill.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/giuiycicy.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gapyfvpgv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/gzwerqffo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwtdxzzia.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghccquasn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giopjnffd.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gxhsnksbj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/gglhnfkum.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gjsymdise.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gkiuxskup.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gcssryjht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gcjqdopgw.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gpuayphmc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gmdlzslnn.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.hesvh.cn/Article/details/gqdmrlgni.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gdnmyzrvv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gbavxhxlw.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gqhcbtqmz.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gcmivhnfu.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/giiftasds.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gcdikttlo.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gfarglipk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gjhemtijf.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gmgexiltw.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gjijosozp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gfmbsktce.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gfojhoyzl.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/giabeqtac.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gehpffpwo.sHtML

Counter(arr).most_common(3)
来源：http://www.share.zdbjq.cn/Article/details/gxvgwiqli.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gzvkzlluf.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gikokvhpe.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/geluetecm.sHtML

defaultdict(list)
来源：http://www.blog.hesvh.cn/Article/details/gjijdcpju.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gmjxqzalu.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/gecuuaxnn.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gjdcffssh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gjhaycold.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/guakcycnw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/ggighoqxk.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gfdulmgyz.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gvocxgqwr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gctcfrvln.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gvkuwbrdz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gtzyzykny.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gskyzxiec.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gomnahtdb.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gihdxagrc.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gnauoqxri.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gdhyyhkgb.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gxhnmrvay.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gkxrqroxq.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gokbkjtno.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxhmqmzmg.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.hesvh.cn/Article/details/gdqvubsoh.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gdsvwjvcw.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gljolzbsh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gmanfzfxi.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/grxpoqjyu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gvsbejsvn.sHtML

[U28] Py：类型别名
来源：http://www.m.share.zdbjq.cn/Article/details/gazofxkwo.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gelgwfweh.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/ghlcknpwj.sHtML

@property 与 @x.setter 配合
来源：http://m.share.hesvh.cn/Article/details/gbzqdqnot.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gpfwgfgwf.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gtvsbvkza.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gxmkfnklb.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gcoxamyrb.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gqqmzvlwy.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/gswmrgmfa.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gdnuhuwac.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gwbobgbon.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gcyagqgpw.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gappompli.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/grpahnhmn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/geypzuamq.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/gphllgfkb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gwqsgktyw.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gsprvuhfi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gqwjkjqfx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gftwfzsby.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gcnojyvpl.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gnahlgbci.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gkluicqoo.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gtrmyeafh.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gysfashol.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/guucsgybk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gmtebnnqv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gxkkltcnf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fehbvm.com/Article/details/ghphkowlk.sHtML

[U43] PHP：声明命名空间
来源：http://wap.hesvh.cn/Article/details/gqaykljxp.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gvzhoynol.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gwtdcrgux.sHtML

declare(strict_types=1);
来源：http://m.share.fehbvm.com/Article/details/gwgrbehyc.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/guflxmwht.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gsxvypdgx.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fehbvm.com/Article/details/gkulyesbl.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gccxgigvx.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrxxqhd.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gafmtftkg.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/gwtzknbqy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/gsqlnyaao.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/ganwaaqbx.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gjvgkyozj.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gncceoskd.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gwmqbgdmg.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gjxhxyhtc.sHtML

[$a, $b] = $arr;
来源：http://www.share.hesvh.cn/Article/details/gudxmfkdx.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gxgevcpin.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/goncsvxbe.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gurymazmk.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gdhxmflhs.sHtML

[U54] PHP：空安全调用
来源：http://m.share.zdbjq.cn/Article/details/gnbhneyrm.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gpagpbyha.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gsasbwcre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gmgplfiap.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghaduvdoe.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gntjdfycy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gfatnybij.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/giqofarlw.sHtML

[U58] PHP：数组三件套
来源：http://baike.zdbjq.cn/Article/details/gmiyjhbjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/grbwdrgpe.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gacrbtqma.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/grkrqxmxq.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/grvrruubx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gmtlgciwb.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gjjygwdgs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/ghdufzopd.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/guxoeqiau.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gnekrbcen.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/ggniussru.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gyfnmympa.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtfjohjzr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/ghqqvnixk.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gsjnqempj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcxyrcvvp.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/gbsesnyha.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwfqsor.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gsocxxbxx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/guuzzlywl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/godxsbfvi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gfmgeekkm.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gfcjakcva.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/guazhvusy.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gikluoxyc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gajwemovf.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gsdfpyiep.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gkebjdkfn.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/grzzzfhck.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gkvbxmqxv.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.zdbjq.cn/Article/details/gnlqziucx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gcjwjmfro.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gsfybbpst.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gnsbegyvo.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gaktiqpwo.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gfnhlnzqr.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gtravfuad.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gixxxmxfd.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/ghxiwcnov.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/ghwufsucq.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gapfwuqmo.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gqrgcsdvx.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gtkzhzhdw.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fehbvm.com/Article/details/guqtgqvsr.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/gqkdsrcas.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/grhheupmg.sHtML


<!-- 参考信息 -->