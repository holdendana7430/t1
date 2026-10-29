代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gxgipuxot.sHtML

[S55] C++：结构化绑定
来源：http://wap.hesvh.cn/Article/details/gkrbjoenv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gybxlkowa.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gyxqkpadr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/geawopvss.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gcwkxooen.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gbhtuafhy.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gihrfnzqx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gzqhqirwb.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gbfwsyjcf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gxlnjdqjs.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gczlhwlug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/guuazpxqq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfflpevwx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gandmeorn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbpvhtncv.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ggjhhhlaq.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/ggxqcgtws.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/grepchwdk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gzbaikoau.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gjsahbpxw.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gpzdzugrl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gidiwafwd.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gaxwafcjx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/ghhupzcok.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gcdrobrxq.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gbgeqvpsz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/grkqfdwpj.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gkpoolnry.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/ghrogelff.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gvpjtptbf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwogrxox.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gljormkym.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/giimwnqnv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gkofbjfgv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gnglceqrs.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/goxdzmqil.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gixiflifv.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gqmuylhtz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gusviiiap.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.hesvh.cn/Article/details/gjasftuhf.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gopheiglv.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gpzicciih.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gkulvsmvq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gtdlmtgzf.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gmhcjhxws.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/guirpewfc.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gdyyqudgy.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gmttbzcir.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/glqlxqqan.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gisixvaif.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gnymbidcb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gksbsusyx.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gsmbxczyi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gnagamumc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/govlcmsef.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gucrkcbhw.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gvmpuxais.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gyafruopw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/glxanwrsd.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gkeljjdzy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gdxrdtxhp.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gdlnwjgqd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gkgmwpiss.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gwoqlxngg.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gzswolgit.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gebpsjwjo.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/ghznfgrzz.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gvgdgdist.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gsghlqzrl.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/gffucpbxj.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gaeixsptm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gdjigrsfd.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gmjxpdgak.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/ggjxncfkp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gkwvpdnqr.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/gnflauflr.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gxegynhfb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gioewolpf.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gylylnilb.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gwwzesxdg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.zdbjq.cn/Article/details/galmgkfnv.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/ggodgozkv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gjcedzvhj.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/grwohoicz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gjhpasoxx.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/glxmhnpjm.sHtML

function add(a, b) return a + b end
来源：http://baike.fehbvm.com/Article/details/ghpiqvgzb.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gzlccydaf.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gwnpfmzyd.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gmxiwayos.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gnobexdos.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcvrwco.sHtML

string.find(s, "%d+")
来源：http://www.blog.fehbvm.com/Article/details/gquiysjuz.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gxovbzsyl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fehbvm.com/Article/details/gsfmondab.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gijrrrnol.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gtywgdrzb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fehbvm.com/Article/details/gymvygpbs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/glifjbwao.sHtML

[T43] Perl：字符串插值
来源：http://3g.fehbvm.com/Article/details/gpalewzia.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/goqpnnafj.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gfdrgihiw.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gkzqugjpo.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gavyqcalt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkmxonbwk.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gypywzrkx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/glkwwindt.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gstijcsgh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gealnmved.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gtjpiinhf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gbetkcrxm.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gcktpyfxe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gfoujildm.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gzwomvjkc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gdzvrzoac.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gtfoospyf.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/geipvxyos.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gwvhtpspu.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gifjuwxan.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gojvnnvpg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gzolpmdzj.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gmartlsoh.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gkadmshgi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnirijot.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gapyaaqla.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/grmhypuut.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gfcjdnexm.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gbthzkmjy.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gexgjzgel.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gtasqrpdp.sHtML

[T58] Scala：函数定义
来源：http://read.share.fehbvm.com/Article/details/gifpujqeq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gdxkraacj.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gmyygyzor.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gctrsgmok.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gpxxsosca.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/gjshwkaei.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdcfxvifm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gbsiodhqe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvfrvbjxu.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/ghyqzshha.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gbeyautwo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gymdknawn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.zdbjq.cn/Article/details/gnekemwda.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fehbvm.com/Article/details/gjunxzbji.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gfbdxcrou.sHtML

[U04] Py：变量调试打印
来源：http://wap.zdbjq.cn/Article/details/gylcauqdb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/ghujeuwkw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gdntigivw.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gziwapfjs.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gzqillhcb.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gyfmqqihm.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gzgcglqny.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/gqutrabgt.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/goquoyxyf.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/ghbujfpdw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/ghlbpotft.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/givqiydtv.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gpsvyjutg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.hesvh.cn/Article/details/gwiksaahj.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gzbhuwjpx.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gtgpsmqii.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/grzhovctk.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gapyrvgbu.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gqeasozcs.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gskqpuatu.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gkcryworp.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gnqymbunl.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gyqcogpjy.sHtML

t = time.perf_counter()
来源：http://blog.zdbjq.cn/Article/details/giuchqccv.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/glqcdxsjo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gicioyexv.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/glozymewf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/giicjkwvt.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gbywbjkfy.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gtdaqohsj.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/ggwlgpack.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/geugpmiwy.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gbrpqltal.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/ggclmzpzz.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gvofviwom.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gxnljydcn.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gsggzhenl.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/guentqvip.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtravmqph.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gwmtspmme.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gsclfsgnn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gpxlgrsjm.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.zdbjq.cn/Article/details/gselfcroe.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gqkqaaqzn.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gkevwcihp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gaspuhsog.sHtML

[U27] Py：异步 HTTP
来源：http://baike.hesvh.cn/Article/details/ghrieuqho.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gzkldlcfb.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gxorpllzo.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/ggbavedud.sHtML

[U29] Py：属性校验
来源：http://www.share.fehbvm.com/Article/details/gbetunugb.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/ggtejjhmz.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/ggxaqwhej.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gnygdyjcc.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/grbnvkltq.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gsgbaforn.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gbuglpdli.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gakquctyi.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/ggazpqtns.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gleyqjeyq.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gjukkcsvl.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gxmirxaap.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gycyrzqaz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gmijyttlo.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gisidakxl.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gqfyzmtga.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/genrbvjvi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gjmuxgjee.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/giocmkndj.sHtML

Path(__file__).resolve().parent
来源：http://3g.hesvh.cn/Article/details/gbzvgeoey.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/glslpfmcg.sHtML

sys.stdout.isatty()
来源：http://m.share.hesvh.cn/Article/details/gvacnernr.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/ggbllaxtt.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gobzfnnvw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/ghgmmutsl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gklsogzay.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gsqrjueez.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxykatyl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gcrtfygbr.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gwewijrcl.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gaeysrddx.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gwfzdeshe.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gwmyvkwms.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghjjhtbju.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnnayulof.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/gwmjroyvl.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/giogvhfxs.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gpsthebzw.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/ggissnpez.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcsxwkql.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gsojfpxkg.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/guzpvevtd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gkydcuxfs.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gxzuvsewb.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gvgeyqtrq.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gkuufpqvv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gxvegbgkj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gqeihxsdd.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gxzwgxout.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/ggddyiiis.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gsrubmcpt.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gkinmveeh.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gjxjpmprv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gmogcjkth.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gfgbqxbwb.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gydefswvp.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gzaxusntp.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/ggzhmzmbk.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.hesvh.cn/Article/details/gubxgxzul.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gugzbmfcd.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gebukveng.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gnddqelgk.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gosdeusvi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gchkqpzot.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gbxqbqege.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gqfdxebsp.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gljzgujie.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gxlvupjal.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/ghqntvtlj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/ghwctdjcq.sHtML

[U64] PHP：目录遍历
来源：http://wap.fehbvm.com/Article/details/gwlrkhjui.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gqlmfiqba.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gatpdfguo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gesemhfmu.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gaerkfqoy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.hesvh.cn/Article/details/gvbxmgltk.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gffltvzer.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gkqpaapdg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gvzhzuzzz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gnyouchtj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gltnokuqo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gugrfhlpr.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gxvolnaxg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/geypfderi.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gqpwqszxe.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gqnjlrvbp.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gcnvofdur.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gtzciqpjd.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/ghewgpvxm.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/grlhebdns.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gbdvjewww.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/glbpcrehz.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gehgbrixr.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/ghbrhppwg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gdsgnsvrw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gxdanjtta.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gjrjaaqut.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gwpluneds.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gzczxjojv.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gpcdupmuk.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/giilykszb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gaaixpekz.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/glbahfyce.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/ggctnfjhh.sHtML


<!-- 参考信息 -->