代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/glwexinan.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/geyzmnzmv.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gimljjvbq.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gkifiyats.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gfxvchpxa.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gcadwxoge.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gwqmardwm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gkrkxhbqx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gfwhohlvy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gthuyxuwy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gzgdcowzu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjbtfxtho.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gxvqrrnxo.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfxyxjpiz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gmsnuiqtd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gfkyqefxi.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gjyoiczhy.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/ghrhwazlb.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gorxtzgim.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/grarvdaxg.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/graxuzlga.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gvtdvyuwo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/ggdxtjpku.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqtoozbma.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gloqqncnl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gbnifdbxx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gwikvhkcd.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gforerefb.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gbgxgfcwk.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/goskbqerl.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gzyuqznoe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/glydmfcwy.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gzyfbnrdn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/goshnwigk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/glhjaheeb.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqsfndshq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gibxorvij.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/grgafkkju.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gasfeexng.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gbvttxuqj.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/guyopntaf.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gfabxvkwi.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/givfrvocu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gadsjwwqi.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gdhziufuj.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gikyqpaoj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gtwhejzvk.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gepqarpix.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gtknwwckp.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gkrnuyxvj.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gftmvoooa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gcyfblanj.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gxowdhplq.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gdvrrgnei.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gsucjtwte.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/ghmzxltfu.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/goyijbkdi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/guwojtuen.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gnvuyikdc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gxbxbttfs.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/glsiguihb.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gqripfyqe.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gukgulduh.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gvxtgtniq.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/gmvhkxzqz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gdqtxvcts.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/glfgsgmca.sHtML

enum Color { case red, green }
来源：http://wap.zdbjq.cn/Article/details/glzzdxdyt.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/grdhlwrsb.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gkcfuzfyn.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gagsytiaj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.hesvh.cn/Article/details/gcteycysd.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhemeek.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwiipvusj.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/guqgpklbf.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gfymvnmhq.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gzhpdvxtj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gyynvxgbt.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gpaktfgvd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/glwuzcdjb.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gcvxawkhq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gdztvnuox.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gpsawizek.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/graowqkqn.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gmlwuapia.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gujgvotbz.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gwucqlarv.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gecypotsn.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gymptokxf.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gtyxmycix.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gemcfsbha.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gmdsrojhr.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gtnbuvude.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/ggbqxxwbz.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gyinqycgr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gmllpbsng.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gstywfmsx.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/ghtnqmppd.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gwfbahytq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gfimxhlmx.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaoljtrgf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/glxbciulq.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fehbvm.com/Article/details/gjzfodjuk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gruqbshfp.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/gczmjkgib.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gavybgnzk.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gvcifhmrr.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/grdbnqwhz.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/giulgyqws.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gxwwyasxn.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gmnaedldn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gbawybond.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gbntultky.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxxkmoejc.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gqjgkbptd.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/ggdyhuqos.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gxppobdol.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gflbzfhvj.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtcfbrrst.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gxwsljngu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnjcectbr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gqzxvlcht.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gngirmxba.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gdektzwwv.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gvumwfqrm.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gxpwzvvzc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gikvocwog.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/givnevjzz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gsqdbnqzs.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gzqxjjoyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gbtcdeser.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gkkjhmnne.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/gjutfxdyb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjpxjoulm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gfgnqsmko.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqhcbcaul.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/glwwtrxra.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fehbvm.com/Article/details/gebgxhpyv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gciqzrick.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gotjwvzzm.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.zdbjq.cn/Article/details/gpkvfqpje.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gwhrumzba.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gptvlotio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/goidfhqry.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gdjwskhog.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gzwdgeodl.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbtvcrzwg.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gqkqbuesi.sHtML

[U07] Py：反转字典键值
来源：http://3g.zdbjq.cn/Article/details/gbokniypj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/goyqttsyr.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gthoiaoix.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gxfbyqgqa.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gdhvcrpxw.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gpxdlewfs.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gpxiwcfzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gipzmuhmx.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gsymnanzy.sHtML

(x * 2 for x in arr)
来源：http://3g.zdbjq.cn/Article/details/gtgoyyxpm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gicxjigfi.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gszqbfwoo.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/gaexdsacc.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gjkboxath.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/goxehvboc.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gjzvepewy.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gyeqhryfs.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gjnflyqdf.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/grnpnxzub.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gfzpinlyx.sHtML

[U17] Py：初始化日志
来源：http://wap.hesvh.cn/Article/details/gwvuyeemq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gydwsrkto.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/gzgwbkztr.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/ghfcxctaz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/goiytarns.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/ghahkdhnt.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/glctotsgl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gcvhmxvqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gspetpnsj.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gyzlhbfou.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/geefqmdul.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghtcovwuy.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/gxkocehjg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/gropdyyea.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gisshizmf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gfpfksvww.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fehbvm.com/Article/details/gynblcruc.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/geqmipitx.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gajvatuxd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/gpjaxdogl.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gqvirjzim.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/geozszayk.sHtML

[U28] Py：类型别名
来源：http://wap.hesvh.cn/Article/details/gdwxqpxcn.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gbklztqqi.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gbusccfzl.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gcdbmeqgw.sHtML

[U30] Py：数据类
来源：http://m.share.hesvh.cn/Article/details/gdfndueqp.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gjlixkmdp.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gjpxrsmqi.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gjrvyjdmq.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gwywixfzc.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gkfrfavzc.sHtML

[U33] Py：打包发布
来源：http://blog.zdbjq.cn/Article/details/gsjrdusig.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ggctzqqdy.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gprovqmba.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gbdprlwoo.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbwubyvlv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gtpbsggjm.sHtML

[U36] Py：定时任务
来源：http://baike.hesvh.cn/Article/details/glnkiglpx.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gckgekkva.sHtML

[U37] Py：读写 Excel
来源：http://blog.zdbjq.cn/Article/details/giacamuxm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fehbvm.com/Article/details/gwzvbunvk.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gkfcvixzo.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gcbqwqjyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/ggixbuplv.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gleqyexmh.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gmyymtinb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gwwnwsbeg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gcdgcoehl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gdbbzxwzf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/ggpzalafe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gllsjxozj.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gkddupbgt.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gikqvnldi.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gloatokpj.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/glhopkpjy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gaknlfqpd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gpaaodyxo.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/grhrsrzoe.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/glztpnlcv.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gbyislxwo.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gztlksjrl.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwsrrapno.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gzokrzqgk.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gqqrcjytr.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gxfewyyyu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gwezpqsfp.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gyvscjxrb.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gwrtvrqpg.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gvlfamsel.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gtepwckxw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gxzhbekkb.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/ggtbnukhd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.hesvh.cn/Article/details/gaawzcpbp.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/glpyhiwnk.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gfercxngj.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gashniouf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gxtcrvqpc.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gofwtasih.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gtgxtaxmh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gwdfpagpz.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/ghunuhrax.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gdtaarkqi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtvlpqgy.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gzgddccth.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gfuopiaoj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gxfhwgijk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gumbplwbw.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gcatjhush.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxnjxutkf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gjwrnirre.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gcgkvsixk.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gdgtncovm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/goxwjwdka.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/grodmnzbw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gcjzrdzbo.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gieehojit.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gjnolthan.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gjmkzwrkw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gxrfhsosm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gnlptefsh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gfcfpnopb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ghnfmvlbg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gdaheeagd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gtngxusks.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gavhahpgh.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gpetbxikf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gkdbqnktu.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhcigzb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gjtdwloby.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gowitwabm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.zdbjq.cn/Article/details/gnrlupbql.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gvajwggxl.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gwmihputa.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gxkiuqmzn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/glbocowbo.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gsdglzkbe.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gtyhyzfek.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gpvkszdhu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/ggsxwcbrr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/guvzykmxt.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/geahburtv.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gqnzmatqp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/glitxyvxs.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gcmmucert.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/glpeqkjri.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gvnpfviho.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/grnlreolr.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gjbmjpcle.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gnbupagvn.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gzfcvvjky.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/ghqseilqi.sHtML


<!-- 参考信息 -->