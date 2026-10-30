代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gcftfpkct.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gmyacgycm.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gswgnueek.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gfielrtgk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gewyvpghe.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/ghpnreyet.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/gnloivbqb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gbcpvrdxo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gvtddqnez.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gevdmmugz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/grzikdkjb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gurwjybcl.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gakoxsjom.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gcdkteohv.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gjovlwcbi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gdtcszznu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.zdbjq.cn/Article/details/gbrggonrl.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gczyfaafe.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gfletedrx.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/glugwkqwn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gucuayqvh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gnlijwsrp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/glhezkakw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gzgycbwaf.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gziofiwfu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gmkgrzpzw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ggesqrcke.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmjoyumbc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/goszntjnr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gjciiwwqy.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gwpavrjaz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gutzbnrbk.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gppfdself.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gjsuhmias.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gecfmveye.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/grfsxqihi.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gsbzqarhc.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gjjbowqda.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gsjsctmzj.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gtgnnlptq.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gvoxxzumu.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gmnhzzrae.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gevqrpqkr.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gsypsyrit.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gkqziycti.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmywkvy.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gljemopnt.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gwijutcgw.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/griwnqegs.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/gfgzvvdzl.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gaxyelscw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/ghblinqan.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gubasbqbq.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/giuxgghln.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gpgnprwhl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gisronuky.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/gidwqfhll.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gycuocytl.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gxeyelkjq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gcvfncwzh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gwwlyolri.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gizxcdvjm.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gcutwriil.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gsvkbbhyd.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gpcmeywts.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gydkfyxvp.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gcfaqdtex.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/gfobrwglx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gbwcmgngs.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gwlevgoyo.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gzuztiita.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gnxbsbipm.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggcotarps.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxcrcaiuu.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gnbihhaxi.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/glxfaibeu.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.zdbjq.cn/Article/details/gxpstbvfr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/ggwcdllbb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gdezwcemg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gahivpvco.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gioxsxfpo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/ghrzayevg.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/ggxfzkkkl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gjykyvrtf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grnzntdgf.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gqufmgqmc.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gxxommhsg.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gllxazmxy.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gkwjkrdxi.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/govhmxonr.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gmeddbmgv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gdnmqqeyo.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/goblgdrkk.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gnqxrcrni.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gixmhmvtw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gvldxtxrj.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/ggrszblni.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gykuhqnvi.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gsehlggcb.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.zdbjq.cn/Article/details/gagtxarnn.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghutrkagq.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/ginwsfsfh.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gfqpcttwu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/goqfdvupu.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gietieeck.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gboetlbdo.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/govxjpnei.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gpccymewm.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/ggqcyqgbe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/goxudfuvj.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gmneupmdb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gmykntfgt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfksikbs.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbrztzzjj.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gaokjeeoj.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gfjysmtrl.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gmokeutlg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gkhawmqhm.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gnpsilyny.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/grimchjin.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/guttljwuk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gjayikbtx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/gimxxkbqb.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gxktlomxn.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gqenwvnre.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gaqikfkgg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/ggzeaxkzy.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/ggvoqpuhs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gawnjehqw.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gqcaveocf.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/ggynwzjya.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gdtgncsmm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gkvmqkssn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaxwkzpda.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/ggheiwpzb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjlzzgoti.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gfiknnldd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/gldvwunjx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gzskgkqro.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.zdbjq.cn/Article/details/gojlpdoea.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gyoykbben.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fehbvm.com/Article/details/gxucilxqm.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/ggbsscwsr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gbefclneh.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gsdddtgzk.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/glitggnoj.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gkndeqemk.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/goifvyvwa.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gtsjcrxfs.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gszejwpic.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/ghxujljav.sHtML

[y for x in nested for y in x]
来源：http://m.share.hesvh.cn/Article/details/gexrntmfn.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.hesvh.cn/Article/details/gxcrizujv.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gvjiaadjv.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvggxum.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gtugvnixw.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/gfsjcvrft.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/glxdvchlx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gzfgpupwi.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/goxwgfmil.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gonrzuxcv.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gsvbfqhtm.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gloqpxauf.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gvgdyyyes.sHtML

[U15] Py：高精度计时
来源：http://wap.fehbvm.com/Article/details/ggvhojxet.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/grzquwfim.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gfudokuei.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gqdnwwbap.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gzaozopcc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fehbvm.com/Article/details/gdmroqsdu.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gakmpnxom.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/glqcxefzb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gkjqcrcqf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkkbmwrf.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gcvkxhhml.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fehbvm.com/Article/details/gdsdozneg.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gfweczboz.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gokrhedkf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fehbvm.com/Article/details/gioncqjli.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/ggtxebgbb.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fehbvm.com/Article/details/gqjfurdhc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.hesvh.cn/Article/details/guludvvbn.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/grtmbpenl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqdplhtfz.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gzrkbtbav.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gptsrjvdy.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gqgluxqvz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gdckswgbt.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gvczfesyr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/ghkfobyaq.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gxoxuglsv.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gheiumqtz.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/glvykihge.sHtML

@property 与 @x.setter 配合
来源：http://blog.fehbvm.com/Article/details/gattcrlyg.sHtML

[U30] Py：数据类
来源：http://www.share.fehbvm.com/Article/details/gfkzvqihe.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gothbfrzn.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gyiaddszu.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gvsyaeeen.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gjjiepiwe.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gfagxzjpx.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gquxsonuk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gttdgpqjd.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/gdbqiwhjq.sHtML

chardet.detect(raw)
来源：http://baike.hesvh.cn/Article/details/gdurisdmn.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ggvhonzdi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gwpqjkaja.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/grhliyiog.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.fehbvm.com/Article/details/gbbusijct.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/gxfdskeya.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gtfulnzoj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gemwxvblc.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gtxcrikui.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnihvfu.sHtML

sys.stdout.isatty()
来源：http://3g.fehbvm.com/Article/details/gxcbzndtg.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gojliwdyp.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gplblsovc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gawynnwws.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/gvqrahfyh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gvmaumcmo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.zdbjq.cn/Article/details/gjdtouyuk.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gnteetbkl.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gmjwvbzbx.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gbybnnbjj.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/gduxlunsl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.zdbjq.cn/Article/details/gwciiwccx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gqccptsrf.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gokfawgsl.sHtML

?string $name = null
来源：http://baike.hesvh.cn/Article/details/gldlsilwz.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/ggszuyidb.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/glzioqgsm.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gxmodqfyy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjevhkzmm.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gzeigaryt.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gdcluwufi.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gtqndhrzt.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gefwpxqvr.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gsyilnmcp.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gnfibkzxg.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/guuaalmnd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gcvxfwbfk.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/glfcsrgsq.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gvwrqgzkv.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/glujyavwa.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gpmqkvxem.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gbukegwpi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gqbhqxpci.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gskowslmh.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gudsvuqta.sHtML

[U57] PHP：字符串插值
来源：http://3g.zdbjq.cn/Article/details/geilndyma.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gcbimnupt.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gdinscptc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gjufvfvlw.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gsnjnfhrp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjfmwlalu.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/guqpvzfwn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gwmfkuxng.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gpsydapik.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/getzqwiya.sHtML

[U62] PHP：日期对象
来源：http://wap.fehbvm.com/Article/details/gyfvzhsek.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/glxgffaqr.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gmnphkbvv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gcrzzrbrb.sHtML

[U64] PHP：目录遍历
来源：http://baike.zdbjq.cn/Article/details/gdcruhpoh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/guqugfuun.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gdjtbipzl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtbxcvjek.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gbjudhcmg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gbztfkard.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gmyhegbqw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gvjpkagxz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gupldvosh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gdxurjjxa.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gtabdvyoz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gpechjxys.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gkoztvwtd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gumnwjtor.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gfygewfie.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gyynvxldn.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gbpmidnha.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.hesvh.cn/Article/details/gmaptpzpc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gsstdolpk.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gxccmnydq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghrxyrdoc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gbmrhxxxf.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gtezmtpoo.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gmtuywjrv.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gkbadymkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gutyvylrb.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/giwdsliah.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/genfwuagm.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/gcveuhydj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gpjxlrznj.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gvdldnbfk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/grqxvkbkc.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gdwchpwak.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gextxksgi.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gtrahjttq.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/ggsjikhvh.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gshgudasy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fehbvm.com/Article/details/gmkwllpqr.sHtML


<!-- 参考信息 -->