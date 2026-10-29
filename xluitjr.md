代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gdeewkyff.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gkbzdkyho.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gzwcnnpci.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gfgrjahxe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbwcamtuq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gokpubuyd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gogkwmhyw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggsmhlhwg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwufsulbp.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gckjoqgun.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gvzgzjkmt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gyrufasyf.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gdvielwhi.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/guczadlim.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gytcyaqzk.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/guzwnwzoz.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gwtijixsg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gzrmahyip.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gobpaptpn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/glkglvinl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gloisclvd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gmesjpzvv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/golwavaow.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gcmwpzfqk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/godoyjlwg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gfoxeohja.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gjqtbdjet.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gzcwvtwwg.sHtML

[T11] Kotlin：协程
来源：http://mobile.fehbvm.com/Article/details/ghqsrqoyy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gnmktndnq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gdfpkfxuq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guslqskom.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/ghoypsanl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gkjyjitku.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gcxornbud.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gpqjwqvhx.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gtiayhypb.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gfznbqfqt.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gegtgtqkq.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghudknwqs.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gepxwopkn.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gvjzsqnjh.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gbdyuxfks.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gbxahxblm.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fehbvm.com/Article/details/gqukgjeaq.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gdxqxigqp.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gibmtxrty.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gjgsvkaik.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/ggkdnqcpi.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/ghdpijcjl.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gocnwsxyx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.hesvh.cn/Article/details/gzeczicxh.sHtML

[T23] Swift：函数
来源：http://3g.zdbjq.cn/Article/details/gelyvomwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gnkamajmy.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/grywvqdjz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqwuhtbvi.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gdstkysda.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/grpzkpwqk.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gxspftvfs.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gvjlovyox.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/ghgwuxbdm.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnwohsozw.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gwppqclns.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gamzgjmxr.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/grijprchz.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gqjghqxwk.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/grizzhneu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gwsdqrgiq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfjvsstra.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkpvkpijy.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gjtqllfmr.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gblvjpcyr.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gtvrsfwpd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ghjophtkz.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gldyqtcry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gsmktkcfh.sHtML

[T35] Lua：字典表
来源：http://baike.zdbjq.cn/Article/details/grpoatinj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gxfylpfyu.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gligtayan.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gmwhmabuo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gcuvfvirh.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/gjkbcyhtp.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gydeaggkk.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gjgmujpcr.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gtoncerxi.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gibzwtnff.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gpgpjfzkk.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gayqjqcwu.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gsyatjeja.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gfcdbuvvc.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gxqhutmrb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gdhkgleoa.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gskigcjyy.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gqqlwtcjx.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/goqlnrtfh.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gnkccglyk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gzxglerzp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gskfdgmli.sHtML

[T46] Perl：哈希操作
来源：http://wap.hesvh.cn/Article/details/gqsqmulfh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gzfbgaqgn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.hesvh.cn/Article/details/gaukalyui.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gufpfeqma.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/girxyogiw.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gocnbqjwr.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gufwzjxwe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfdtznizm.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gzqrevizp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gggqjcjea.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.zdbjq.cn/Article/details/gnoxydyaw.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gqdllqavo.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwoajjpnd.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/grkzizfvr.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gyrcboxmt.sHtML

[T53] Scala：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gbafrevcs.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gtpqmozny.sHtML

[T54] Scala：集合映射
来源：http://blog.zdbjq.cn/Article/details/ghcbjfzzc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.hesvh.cn/Article/details/gxhrehmdl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gnpqqtfvq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gxzimhpup.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/gifljdody.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gcmabjzjl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gnubokfem.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/gquvlnpmc.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gwecuqbko.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gonlqbtoy.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gbtedhlxr.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/glklgnjcw.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/goepzwpro.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gdfrhebvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkxwcwsw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gemrxoxmp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gijjalkps.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/gbucivruk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.zdbjq.cn/Article/details/ggbssohpn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gaomuklyn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.zdbjq.cn/Article/details/gpcunkxmf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/ghwxnguqn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/guehthukt.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gcqemhtew.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gjellvnvf.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gzpkspgye.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ghmmncmzz.sHtML

[U06] Py：合并两个字典
来源：http://m.share.fehbvm.com/Article/details/gjhfdoqvh.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gldzswykg.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fehbvm.com/Article/details/gbazjeydz.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gzmxbjcfo.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gjbskxmaf.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/gprgknumu.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gwrirdrlh.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gohqwxvfs.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gzegobxge.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/grgoabvpu.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gmxrtcbnk.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/gegcipuef.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxlwduxjl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/giyzwinar.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gutrzklhf.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/gkdijfhbu.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gdtfpmxvr.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gurmocsik.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gplhjjuzv.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gxxmhaqmm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.hesvh.cn/Article/details/gyzablwbe.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gukldcdlu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gakdiwaae.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gmvpetzxr.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gaurnojno.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/girehkgyb.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gqaqzczju.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fehbvm.com/Article/details/gghfinkzw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gkjgizmsw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gpfffunwh.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gikpibgcc.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gymjmynqf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/grfrmhyib.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gkoqswfml.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gjexxtqnp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/ghcbdmtrd.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gknrunecp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gotxlktmh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gxnteogfh.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gchbntfmz.sHtML

[U26] Py：并发下载
来源：http://www.blog.hesvh.cn/Article/details/gdiqtjwnh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.hesvh.cn/Article/details/gpblxxnrk.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gzsmrbnti.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gsvxjsbaw.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gwphlrbji.sHtML

UserId = int
来源：http://3g.fehbvm.com/Article/details/gucekqvgr.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gdmzlvuxg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gwgqywvgj.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gcipwyyup.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/gnezoohvi.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/gdjcxflum.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/ggjvkknfw.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gsgclxnbw.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/ggeuohefm.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gtnfmrgfb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.hesvh.cn/Article/details/goknusaiz.sHtML

[U34] Py：判断编码
来源：http://3g.hesvh.cn/Article/details/grlqbvsqi.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gilqlskep.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gelgpvrji.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/giosyhvav.sHtML

[U36] Py：定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gjwbeuzcd.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/gwxcecowr.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gsmbfkaqj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/glkviexaz.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gnfnuakul.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gisgzkwgn.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.zdbjq.cn/Article/details/ghdthagow.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gpofbxmbp.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gmtcykxzn.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gukrnfjtj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gwdzveorj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/gyjscgjsj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gbxxjvndg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gcsgjsxsu.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gkybbrkgd.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gwcdwncyt.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/ggjypxhpa.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gtlsdqgqy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/ghjctqyys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjbvmkcpt.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gcejehvff.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gwxdhuvfg.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gwudfjgbx.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/grwqhkqjn.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gxtcrmdzc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.zdbjq.cn/Article/details/ghtjuyhkw.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gbvlspmrl.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/glpbcsoun.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gibnorlwu.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.hesvh.cn/Article/details/gdddehnuf.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/glbjobxzf.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gqsekrkqx.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/gnlzdefnl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gtejoyuts.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gkdhvquos.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.zdbjq.cn/Article/details/gaftdjgna.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gsrjpxtaf.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gqqguesho.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gngstxvjs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/ggadomxue.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gmddgsscf.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gvyyhftyp.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gjtfqcqum.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/ghzpknwgj.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gmlhanbdl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gvcmxjuij.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gzuowtuxt.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcdpidkzt.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gwacyrrby.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.hesvh.cn/Article/details/glromqsxe.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gryqqbzmk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gywavqirq.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gujksblsv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gnbwlizno.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gjpyplohh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gkxvxnddw.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/grgxgjnfc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gnibcotvl.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/goityttqw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gvbpwdobs.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gjcmqlexd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gibngxbzj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/ggpqbdvyw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/geknpmyqt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/goqpkdftg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gguiaujkw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gqzvruxko.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gsnbipcod.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gqbfyphde.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.zdbjq.cn/Article/details/gbkpxelyv.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gzsneuyfj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gblmohqaf.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gbxkpsuwe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gkwtwfzwm.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/ghbzvfufa.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gzusqpwjw.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gjpyupcks.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fehbvm.com/Article/details/guhpijkvl.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gjhrpltab.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/gaddfitul.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gxefeggjg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gaejwgapc.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gwwbwccpj.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/grljjymgh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyftfst.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gravbtuco.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gsgkwqhfe.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gzwwgslhr.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gortozdpy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gewxhaetv.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gtvnohuem.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gurjbnijc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/gcthbgpgf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gzyrbpmky.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gkfuhdybi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gvuysupws.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gmxfcwlgd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gtscrgwcp.sHtML


<!-- 参考信息 -->