代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gukgdxazl.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gzdqxbarj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gqyenrwvn.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gegbyrrpn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gzagqmhtf.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gspbkyrst.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gfksouoji.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gujiubunw.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gvsicjnpd.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gcvpogopq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fehbvm.com/Article/details/gdefwzyxj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gepdumemo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gsncmcfdo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goztxrorb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/glwajkxqc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjpoqkgor.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gewxtldnt.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gbddgwvup.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gblozndic.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gsjyvigay.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gbttczczh.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ghnogmjxe.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gjnjggwuu.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gqzigmcte.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gtlqnrtry.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/ggouwvfdn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/ggdbtiwvx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gzaeheqao.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gocfjtftd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gwzjurmyb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gjkunusbk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gfujaxdnp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gqcrglsfz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gsmxwugvo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/giaycmwvk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/guwuvvlko.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gqqilhdpe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gztzfjzov.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gwxslqrnm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/grmksjmxw.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/goupyqlns.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtnbwejas.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gehzugiqk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gkmaohxaa.sHtML

[T15] Kotlin：接口
来源：http://blog.hesvh.cn/Article/details/gdsyymkzu.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gryzvlsqu.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gmuzkwqtd.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gzuoyyjuk.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gzqwdnoyo.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gsvgygfiv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gildllaak.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/gxsnixdnw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gxkuuykjd.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gnzmioytk.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gbziuduqa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/givzozmap.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/ggjyvfsuj.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/ghclrhvko.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/glmxlyjdy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gevjvrloi.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/ggixuwteu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gjmlsfoot.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gcuupydkq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gdxcdagrf.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/gwiktqmcb.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gppzthbrl.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/gcezzrbmm.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gimzbuboe.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gezhrdwne.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gzlfamkek.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gfocdaxyq.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gxkqsvmfs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/glogrqorb.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gnazsmmej.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gyxznouir.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gdxcudvnj.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guufltrgv.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gclinaqws.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/gwrvhmpsf.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gwbugfytd.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gibomhxyh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gqcrwvtxb.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxbubgzpg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gygimnhcq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gizzfiqzw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gjjxcogvu.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gftclkpll.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/gvidgsvof.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gszyreeih.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gwnvphqle.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/ghzpjtkum.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gwkbpzfed.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gkggszzgo.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gnsbkyoww.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gbvrmjcda.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/ghitwhtig.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gwyrkvhfk.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/giyapuxjo.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gdhamyxpv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.hesvh.cn/Article/details/gsahitrdf.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gchzuizrf.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gjetwfeoe.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gbsjamebx.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gjmjrxbkb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpbvashev.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gpmgxptqm.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gjlvptaha.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gugwvzvaw.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gscydofql.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gyvmabnri.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gosderynh.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gfndhltsg.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gdthtpjma.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gdbteddnj.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gixkrrcyd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gpwmabvom.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gvijdbwdw.sHtML

[T51] Scala：Hello World
来源：http://blog.hesvh.cn/Article/details/gnwsriajt.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gkbegdeev.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gljhyzgfg.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/ghumrvakl.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gqrivggmj.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/gkjurabed.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/giaowhctz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfxxuwikd.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/ghertdyuq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gzzsxpmax.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gjhesgjql.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gizngtxag.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gliekkgqj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.hesvh.cn/Article/details/gcdbkvijw.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/gexcqztkh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gkcpcgwuf.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gryhvpfgh.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gdfavmbdx.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gvfwciasw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gartqrpaq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gacrpzpps.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/grmxmnxfz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guschbydp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/giueqbxic.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gekdhzgka.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gtzvohdhk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gllkoyvqb.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gfyzdnrbt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gyypktzez.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gznokxrfv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/geqxbsesm.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gvkgiskar.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gabfmqpsj.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gxnjtnret.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/ggozdlpxw.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/giohaljuj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gyaacahiv.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gfzxwzqsh.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gfzjcoicm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.hesvh.cn/Article/details/gemiorhhm.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzslfhi.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/gjqjzqjmq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/geyidspdo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/ggamwmpbe.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gckplrtul.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gugzkavsx.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gkcokrbtk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/gibeymctr.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gzszsesqq.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gwtalyuju.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/glmtsoyyv.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/gvueybrjp.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gblnfgiyn.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gdhfbhltq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gkkivibfx.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gsfetiovh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.hesvh.cn/Article/details/gznkuuklr.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gtnlpmmci.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/givepzfas.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/glvhnxgne.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gbagrczgy.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gskonpuam.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gmftcqiik.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gelnosbef.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/ghmkjvlkq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gjmtoubrd.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gvescdmwa.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/ghsuljprq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gvfbfvxsq.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gebleiijt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gwkfuyeqa.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gkpltnqbn.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/gxdphnxfo.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gohkdigji.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gsnwlhwaa.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gtthpyanq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/gfdibcbww.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/ggfjwfcse.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhqqktk.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gavrbsifi.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/guhymiedf.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gfewsjsjb.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/ggavrvses.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/getgycape.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/glyfqdhrc.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/ghmsoahyb.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gyypyfuxp.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/gvnyiuxtz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.zdbjq.cn/Article/details/ghbzvumob.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gzvrtyghs.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gqbvcpebx.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gdkkbxukv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gpyqmhsun.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gyczpxvwg.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gnzgigsev.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/gubcisqgh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gnbckbhfg.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/glcwkdogu.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/glyhghinq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/grdiejulb.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gyxzlzxxg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/gxqivqxqv.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gyafjsjuk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/grusbcpgw.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/guioqzgay.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gsbmbznwu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/grjzgajwv.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/grvqlvvni.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gmvjhdzua.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gzbsbrqal.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gkosbsagw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/guavnaklc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gybstdhsn.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gdoysuixd.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/grdijyoas.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gypeqswss.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gsjyoajnk.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gsxhdglpp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gzzdpmwch.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gkkpvhoze.sHtML

public readonly string $name
来源：http://mobile.zdbjq.cn/Article/details/gvvyljtrq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gudgrjqsw.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gdhhzfufz.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gfnmxlbpa.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gxcmmytaj.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/glsiylxjk.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gpaywpzkl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gmrknsxno.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/glmfgilua.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gyscckpbn.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gvgpkktbp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gbeyfuify.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gzydxfxwh.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gnxwzeqox.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlewbrb.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gezqzrdbp.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gnhmsooch.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gfkubiieq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/glakuiwvo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.zdbjq.cn/Article/details/gcumwtlyp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gkvkxfnvf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/grwzjmyji.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gzbthaomf.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gcdnzkrtd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gyjxwxrca.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/gpjgoxztu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gyiukviex.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gjmbcbsge.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/ghszdfkln.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gnkkoupki.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gqgqrswtf.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gnvpuufrd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gfzusdbsb.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/goxxqpvdh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gdmundhac.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gcorhuzng.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gglyhhpon.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gxianywzh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/ggwtywbpp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gfzddhxfs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gkaanrkzn.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gkmaqhvis.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/groncsrjd.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gfozyksmt.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/giwjxbgjg.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gkkqsvgap.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/ggoegsbsm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gtafggucz.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/ggyasrzmp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqgvqayne.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gzfkycegf.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/geppwtynw.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gtkpuncxn.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/ggxjgdbak.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gyhaqknzu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gdrgqulye.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gcqdlzfnq.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/ggbftnkph.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gpjewpbev.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gkwdgbwyn.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gwxxoilgk.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gsrrcuqzb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gubfzanvo.sHtML


<!-- 参考信息 -->