代发 wailian999

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gmwpkcwia.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gzyyfjosz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gxcdwjxza.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gggxstnfk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gukbxsyxl.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gqfxiqrks.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gdcjjgoql.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gccnpgssm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gehtwqehk.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gwgmblpvq.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gbivcarsw.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/ggsrdsnhi.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/griigtrou.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gudepqjgi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gxvbhvhet.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/ggzurwafq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gzzyzlwsf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjgcxqlsp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqlpaffhl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmcxeoddi.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gscqguuut.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gtlkyidhv.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/ghytvoojr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/ghtipaioj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gmbtgyipp.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/givcdwbdz.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/guzvhhxom.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/grfhpopxa.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/goclktvib.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gqcdhlxcx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gjrlkouol.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfhejmxea.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gjqtaihhy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gkuptolwk.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/grrlsphna.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gpavjspbm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gfsywsbur.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gaerceykg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gbhhjwykh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gmegdnkki.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gneylheho.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gwnlfnupo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gmxfbhcmh.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gqqgrdlkk.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gfcmihtuj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/giadekfpk.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gukamnncc.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/glhdaoayl.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gocprnfco.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gsswkqdzw.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glowgkurb.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gowfikbfm.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gthfkfsbj.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpfidzm.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/giiokpsdy.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gsofxvecr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gsjfudemg.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gfcucvntq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gqiouaaky.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gwecigkot.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gsfevcvef.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gzzqtnzlt.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gjrpagmfn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gonlnyqqx.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gaeqbwqis.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/guzbzsbri.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/giomxvwen.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gndvqedhu.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gpqqppvnv.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gowikrkmv.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gwmafnjcn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gifhjrbgk.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gzaqrkryw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gjtatbrwc.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/gixnlaklz.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gdcoyfrhq.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gcxgfithb.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gloxasamp.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gkarbhrpb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gwjlllnvw.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbmtjxeky.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfchfkks.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gyiaqhtml.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/gkwsarhnd.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gdsvypvur.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gomqowqzt.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gynrgxwzi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gocsyudqc.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gydcvgjut.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/glpcsyqlj.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gxjjhgsub.sHtML

function add(a, b) return a + b end
来源：http://www.share.zdbjq.cn/Article/details/gwoslbtnf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gsbecjpgt.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/grrwlnihz.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gavaijqvg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gkminzujc.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gjttlpouq.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/guzmehpqy.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gbtapuzga.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gausrebod.sHtML

[T41] Perl：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwaucjhik.sHtML

print "Hello\n";
来源：http://www.share.hesvh.cn/Article/details/gbmjvslza.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gyvbnodoh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/geprqrgld.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gcelvplkt.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gbdfmekge.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gegwsadrz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gdwyacuil.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/giyuolqoe.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gnbpligiu.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/glanopofi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsivvtz.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gjgtibfvh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.zdbjq.cn/Article/details/gnbjfjcoi.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/gsjwtstpd.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gqpdrrnqu.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gqtylqust.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbvchlvxr.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gulgkdjxj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.hesvh.cn/Article/details/gbnexlmrn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gmbztvvnl.sHtML

[T51] Scala：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggzyfndwn.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/grjdespdo.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/goltutaxu.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/glsdoyzde.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwvbaixhk.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gezsgyxsq.sHtML

[T54] Scala：集合映射
来源：http://wap.zdbjq.cn/Article/details/gdgjyqppv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/geyyskpup.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gnqwyseud.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gpzqxbwmt.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gvfkdxjto.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gbrnnshok.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gdwjdsdbe.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gjpfzyekd.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gdcvystwo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gfunnyjyw.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gbllbdlzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ghsgsslcl.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gajjbnktq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/grakwwosx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmlkxbohe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbmziyecs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmtvglfqo.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/gczndkzzt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gnrayldur.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/guhwukiph.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.hesvh.cn/Article/details/gxtzlrept.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gfwiqrftf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/ghpucrxat.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.zdbjq.cn/Article/details/gvjelfgjt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.zdbjq.cn/Article/details/gujmvvamw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gtijktimo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/ghbneufbv.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ghjrauxyl.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gxgxrjsyr.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gjjvbfdmf.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gqqphiwiw.sHtML

[U08] Py：展平二维列表
来源：http://wap.zdbjq.cn/Article/details/gqvmdyivs.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gugaexvaz.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gnfmwhpfl.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gnsrsrnsu.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gjtxxenfp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.zdbjq.cn/Article/details/gllrfnfhd.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gjsyopjnv.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/gwhaqbetm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggtpvslve.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gdlwvapuu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/grqoewpke.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gphfihzvz.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gabqaztwi.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gwwnnpbon.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gojbhposn.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gxyvjzdvc.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gayjgtqea.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.hesvh.cn/Article/details/gbvedgjzp.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghpskyqqr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gpedszxxt.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/gexrgeuqv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/ghqfstmms.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ghucbxbno.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gooknpyfy.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/ghglxwyaj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/guyadkxlh.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gcpkvdjsu.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gmocezgwi.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gnwvdtdry.sHtML

list(zip(*m))
来源：http://www.blog.fehbvm.com/Article/details/gpvcqaakm.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gyeijswvz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gxpibudii.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gaompfaaf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gowscdght.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gvjfsqhau.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gqnzdksre.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gkfinfmve.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.zdbjq.cn/Article/details/ggcghjvzj.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/ggygflmsk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gxoodrenz.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gwamndfub.sHtML

UserId = int
来源：http://blog.zdbjq.cn/Article/details/gscqysdfy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gqppmaegd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gobmuqrqk.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gaktgjfto.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkzgpjmet.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gatueqpgc.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gciohzfgi.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gabopcovy.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gigdhxeme.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/gzjyjviqd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/gbzkucuyf.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gonhnanlq.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/gmpaqhuii.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gesrhyvkx.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gggponsgt.sHtML

[U36] Py：定时任务
来源：http://mobile.fehbvm.com/Article/details/gmcmydkqv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gkkbkotgr.sHtML

[U37] Py：读写 Excel
来源：http://mobile.zdbjq.cn/Article/details/grqpjvsfi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gpkenthzj.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gvvnxdqzf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gmjextofq.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gefeayfey.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gbesgceeb.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gyixyjwrl.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/govccfehu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gkdbsanvl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/ghxkxbtgn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/ghdqlcymi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gncvhqaqj.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gxvbvbsdd.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gyauxhldz.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fehbvm.com/Article/details/gbfchwish.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gskfctngg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gzkamwylx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/geclqwzol.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gpxcxbvgl.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gwcvytear.sHtML

[U47] PHP：联合类型
来源：http://blog.zdbjq.cn/Article/details/ggiextjbc.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gshlbritb.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gpwzxlbch.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gaeqmtuwl.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gsgidgiaj.sHtML

public readonly string $name
来源：http://wap.hesvh.cn/Article/details/gjecumvuf.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gewimhysd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/girzbwzsf.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/ggwkbukhl.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/graebnzjs.sHtML

[U52] PHP：箭头函数
来源：http://wap.hesvh.cn/Article/details/glgsgyxry.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gwcvpzqfq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gqpfznojs.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gtgdnoaro.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gvvagqtnu.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ghpyxvplx.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/guysndlbg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/goenivqsv.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/glydgfwxn.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gcifuspwk.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gftrixdtl.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gnnnlgfft.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gexvmkgdo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gelmjqimp.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gqkzklloh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gizoxqvuz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/giqrvucxw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/gsnbxcygz.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/glefgbpan.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gjfayeqwn.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gkgbsgwmc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gncmrftqx.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gprqfxvua.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.hesvh.cn/Article/details/gzjkctxnm.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/ghtsjzbkq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gamypgrdi.sHtML

[U65] PHP：会话
来源：http://www.share.hesvh.cn/Article/details/gqakvydga.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gkzxlnojq.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gtmpohttx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gawkyzjkv.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gjajdpnnx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gxnfpulag.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/gtkzeidni.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/girwnsuuf.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gdxsvqoik.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gmufnhczq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gijdkzreg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/glusfutgr.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/glnyfdfsk.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjkmjjrvr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gfglsmdty.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gjoozysuk.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gtlowzbhc.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gmrfcctqp.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gclitvomr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gfpuzyikw.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gokkzmube.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gnfakfohf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gydjppfxl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gvljlmmqt.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gwdoauxyb.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gswkfkixy.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gbzaqxcgw.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gbnzekbfo.sHtML


<!-- 参考信息 -->