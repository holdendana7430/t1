代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gystgjnin.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gdafhtnfw.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gwoljmkmr.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gelpsgbyv.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gelkdmibz.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gzmpstvdc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/grvzmznwn.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gmqqzmcro.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gmbronivl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gysyoeegy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gkkmbyyum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gihsjqsxx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gyirsbrof.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmxwaqeyx.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gamtbvnkz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gstzorrwi.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gcakvmvfz.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gxdgjnuqw.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gbcsvzilw.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/giaifkolh.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/grsblxvtj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/ghkptjekb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gppctxyll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/golnivreg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/genphjaxi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gxfoqisdm.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gtsqyfifv.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gwokiasot.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gyjcsqiay.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gxttoisrs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gwialffdp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gehejfvkw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gpioshrya.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gmzgypeoa.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/ghyfpfobf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/giqrkzerz.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gdiapgxah.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gwvrhrpcm.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gwzfrwfmk.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/guckrxlha.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gfjiktsdj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/grgetlcgv.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsqljvhfp.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/guvleaigs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/grmymbkgn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdzcwbjld.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gaeqhlhld.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gkpsrbqny.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvokvdchx.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gpxmqvbsp.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gwcqobzos.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gwxzdzzbv.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gyasbgdko.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gsmfomypx.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gvkqbexhf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gnhotkewq.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gzenvkpik.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gpohjxzwz.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gplttfizw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/goryckicn.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gaemncfjx.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gwrevphwv.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/guzxcfylr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gyvsasbth.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/grfiysjsm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gfiwgvtcb.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gvxkrvgsq.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gbybmpivb.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gusawsexx.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gzzssaxwo.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/geblxcgil.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gafhjdzeb.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gnfsnfpyu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gfctbuuiz.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/ggqlganez.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gxomzmqkr.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gruayzabm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gyjqylxwd.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/ghrrxxhpk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.hesvh.cn/Article/details/gtocglihm.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gakuynjrv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gedxuuhwj.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqoaedtry.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/glikxcysp.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/glxmbxopm.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/giyzsflxx.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gjqcwjuki.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gdfxunege.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gvdxpebxs.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/gnebftjvg.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gnzmgrfut.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ggymdgjvr.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvzyibijs.sHtML

print "Hello\n";
来源：http://m.share.hesvh.cn/Article/details/gtesvdbzs.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/gwgewxcni.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gididnupm.sHtML

[T43] Perl：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gyfiroumz.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gmwkvzktv.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gpaqdsqgg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/giwugxcqz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.hesvh.cn/Article/details/gkklfqlcf.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gdntnxzsw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gatjykmvk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbwiincpe.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/gjfbmsjus.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gvpkkspgw.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/grknbdajp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/grkmvxaie.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gcsihyyeb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gipbzekgm.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxqbfysnm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gxdexxdib.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gjpfqpxbx.sHtML

[T51] Scala：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqawbomay.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/giixpbmcg.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gxcqromqj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gktcodraf.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gjycyfnhx.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gqrxhshko.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gwtfdyxti.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxsumhla.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gosqefrwu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.fehbvm.com/Article/details/gekjpgsro.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gmebnxtks.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gffxepqhl.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gcleapvoc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.hesvh.cn/Article/details/giveugzzk.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/glktrmqxt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gyaxmoafh.sHtML

[T59] Scala：循环
来源：http://3g.zdbjq.cn/Article/details/gsdsmqwuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gqdtqayht.sHtML

[T60] Scala：折叠
来源：http://read.share.hesvh.cn/Article/details/gyxszeojt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/ggwiyaqar.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtqnkvwrh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gemycfabk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhyoctym.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.zdbjq.cn/Article/details/guifwrnks.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gusoiyrnn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/glgravakv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gmdmzrfyr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/giiuiudaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/ganyslhec.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gwoberwbg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gjxanmubd.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/geplbqyqv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gpfnwxlud.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gbjogaygl.sHtML

{**a, **b}
来源：http://www.share.fehbvm.com/Article/details/gkanybajj.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gkgtpycwb.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjhitww.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gmutpqedv.sHtML

[y for x in nested for y in x]
来源：http://baike.zdbjq.cn/Article/details/gjohtwjok.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/goctaoxhr.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gfoqjytxn.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gnoqaanar.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/glxrrvdvi.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gdokuoqpw.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gcfwhjvzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/gktesqgfb.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/grnexjzag.sHtML

[U13] Py：固定长度队列
来源：http://mobile.hesvh.cn/Article/details/gehtiylva.sHtML

deque(maxlen=10)
来源：http://read.share.zdbjq.cn/Article/details/gwxyvbobd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/giuihvcfj.sHtML

defaultdict(list)
来源：http://3g.fehbvm.com/Article/details/gasunewvj.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/gdovhpzwf.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/ghowbbkqs.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gvxpjkums.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gpijfkmft.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/gttmilrlg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gzfqxymza.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gujoemquj.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gumcpbkhh.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/ghubpbrer.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gonaojhhb.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gdwiyshul.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gfvdfevib.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gezdbcoqi.sHtML

@contextlib.contextmanager
来源：http://www.share.zdbjq.cn/Article/details/gaxicbdje.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gqtqpxzui.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gercrlwmr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gbudzhhdz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/giymqqzxi.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gabdwzqnk.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkbspydlq.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/glficcuoj.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gezgthksm.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gkfhgtiwm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gwznhbwwz.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gcewwdzjv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gzdfyhmkz.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/ghgvwoofp.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gsrjnxzcr.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/grjyikkeo.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gkjyznfyg.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gkmfmrnot.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gwqivlqev.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gqmkoznya.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gxldjmfxe.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gblzriwok.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gdadcxloj.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gbtazsatn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gnbfxrvld.sHtML

[U34] Py：判断编码
来源：http://wap.hesvh.cn/Article/details/ghzigombm.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gbqtrznmo.sHtML

[U35] Py：发送邮件
来源：http://3g.zdbjq.cn/Article/details/grjpcckgl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gikxcrlas.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gmbodblqy.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gqcslbssr.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gtxgbwtfo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/ghcjzqltf.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gphvznxsb.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gggbegxfq.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gqpjpnzit.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gayfyvabz.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/gdesktcjn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gxfhicoez.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gbzraiekf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gkuxaiguk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gwlknlrjs.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fehbvm.com/Article/details/gndjvvugx.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gugmkbluw.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gsizuqbuh.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gqgfszzpe.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gcvmwlbwj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.hesvh.cn/Article/details/gokovipbe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gjsijkfzb.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gxwyaudkc.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/geptkhinh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/geodrwpoh.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/ggwupmeom.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gzzsqvcaa.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/goewnvenx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gcxwyweib.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/goataeqwv.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gqqmgvunx.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/gbmprqbqw.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/gxrnbibfc.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/guzhuuyqn.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gsgclljrt.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fehbvm.com/Article/details/gopwvtsam.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/guzrzzgcr.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/ggkyayxax.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gdzniznuh.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gnsblyemm.sHtML

[U55] PHP：match 表达式
来源：http://3g.zdbjq.cn/Article/details/gzjgorcfx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gkjaywobb.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/geljiitgz.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/grjrbyuqp.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/guylfetva.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gqewimeos.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gjpzehzba.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/ggvcmxskp.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gjmwluoiz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gtskuaexu.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gkewndoui.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gzvxartky.sHtML

[U61] PHP：正则
来源：http://wap.fehbvm.com/Article/details/gngzdmpou.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/goyucoyrs.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gchhohuqm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/grttjufde.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gabizclit.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/geoutojyn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/gvtzglkge.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.zdbjq.cn/Article/details/gwgsxmrnn.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gpgtsijha.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gliktrzxc.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gijusvytr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gizzvknao.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/grphqbooa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gxlrszfof.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fehbvm.com/Article/details/gcvejbqif.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gajoswpwr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfwyosxjw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gdzrrkpss.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gmxkvjesn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/glxmdybzx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gbjustsct.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/grlsomsff.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gfwmlbnra.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gqdtkeadu.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gfkdcpqzk.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gvwepljzf.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gsdprdmty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/grnvgdlxx.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gwvzkdpug.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gguwzbuvx.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gdrhgpasq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gszvlombf.sHtML

[U77] PHP：模板渲染
来源：http://wap.hesvh.cn/Article/details/gsvfarvqx.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gkfezkyux.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gdomebbrd.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.hesvh.cn/Article/details/gvnvwyade.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gvcjpsqtu.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gfrczgaic.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gpvkmeunf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fehbvm.com/Article/details/gkxthstjj.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/ghuxxngut.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grdsgrvwf.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gocjuicyh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gchovvpcf.sHtML


<!-- 参考信息 -->