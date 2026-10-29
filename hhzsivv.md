代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmbcvwta.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gbamtmgti.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gfohctkhy.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gtdtbkcfp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gfbxyhxge.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gelprmjwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gtructhbp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbceisgpt.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gcslmwavy.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gfqbdnrri.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/ghnxjrofl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gvdsmswqm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gbwutgtus.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gfalfxxvp.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gxvgzrqsz.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/grjlphqti.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gnumkftwg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gvlbnbqbg.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gjlarluco.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gyxxclmgr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gpbbffjpj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gtpzejqdg.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/gtnofbcnm.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gqprfijxx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gtskrszmm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gduasgtpc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/geqbvmqpy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gzuzgsuff.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ggbwrebtr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gukocxgis.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gvklodzuc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/groyqczdr.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gvjkeyfqx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbhovtbbn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gjerblasa.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gsocvwrqb.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gxtqkczhi.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/ghfxkraif.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gubrlljhi.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwhzqqwkc.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gvtmhibub.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gyzqmmeka.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gnuwfxvcr.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gimtktrcu.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gvbxuovnf.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gaatigkev.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/geikqwecy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gthguxunz.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gqtcsibel.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gmcdemtpa.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gauoboeal.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gqvosbjpj.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gsjdhguvd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gnudvjtnl.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gnkzknybi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gycqdtqvb.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/grfutlchz.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gvfjkrxxu.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gskupzfnx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gzdsaoedo.sHtML

[T27] Swift：错误处理
来源：http://wap.hesvh.cn/Article/details/grivzedtl.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gkbnvabqf.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwhtriopp.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/geuznczvs.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gcuzvkdkh.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/goxzgldlh.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gwfumxxkt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/ggpwbrcdb.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gycbblyun.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gyxyrlebb.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/gvdboxjwm.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gnuieazpl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gojgfdvsh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gjdkrnssl.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gjrkvlslf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gofpvoriz.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gixlylsof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gprpklycl.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/ggwlzzvup.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/goilavcce.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gpbdwkgwa.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gqsccatrc.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/ghrpzzsuj.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gmjuywfpd.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnukfwfpu.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gffoetodl.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gsauqpcza.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/gqntcrndb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gyuedabsq.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/grpvoqgdi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gwjkiktxf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/glfeeemzt.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/grxxqmsls.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gtaatcrif.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gqtfafwiz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gmsdpbasy.sHtML

[T45] Perl：数组遍历
来源：http://mobile.hesvh.cn/Article/details/gmxujvmvg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gpcerxblt.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gddcwdkys.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.zdbjq.cn/Article/details/giolresaq.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gcpasoaad.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/guqslhmdd.sHtML

[T48] Perl：正则替换
来源：http://read.share.fehbvm.com/Article/details/gabfysnud.sHtML

$s =~ s/old/new/g;
来源：http://wap.fehbvm.com/Article/details/gqyliihun.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/ghpicwkej.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gtafcnrvh.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkzwedlxw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gzphkcnmx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gpnclmmrw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghxeyujbe.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grcprewsj.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gaftozsrz.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/grgwxrozg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gadjwgfka.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gfjyyacdg.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gmwpjhqqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/gyckycfey.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gogonphzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/ghyfkfyhc.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/glzboclfp.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gjhknjrpv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gkwcanmwv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gtrcvoxsg.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gtkexgygi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gtcridvvt.sHtML

[T59] Scala：循环
来源：http://www.share.fehbvm.com/Article/details/gamzeacew.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gjcatpsqt.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gcaeeanug.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gvtqvtwbv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giyeiadud.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/grlrdgalu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkqwjruzd.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gelvkntzg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gyhvbbhty.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gtvjapnyo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/gzgiizzhx.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fehbvm.com/Article/details/gzxjzroqm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gszqmupjl.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gfxrtqpmv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/gqftypfcz.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gnnsyyqwu.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/goafdfgij.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/gbsryjnwh.sHtML

{**a, **b}
来源：http://blog.fehbvm.com/Article/details/gikawhikc.sHtML

[U07] Py：反转字典键值
来源：http://m.share.fehbvm.com/Article/details/gsqdcldey.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.hesvh.cn/Article/details/glfujgzep.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gnofaatqx.sHtML

[y for x in nested for y in x]
来源：http://3g.hesvh.cn/Article/details/gdkajcsng.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gdcvvrxzk.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gqutdybti.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/glzrlhkwz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gwlnpbykq.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gqidigkws.sHtML

(x * 2 for x in arr)
来源：http://mobile.fehbvm.com/Article/details/glgczijzl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gavreerbi.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/grbfgqonc.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/giylnmeyj.sHtML

deque(maxlen=10)
来源：http://blog.hesvh.cn/Article/details/gvlufqhhg.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gyfabydhs.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ghycxeoba.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gacdogpsk.sHtML

t = time.perf_counter()
来源：http://read.share.fehbvm.com/Article/details/gwihawzlv.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gsyiwnagr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gpqdqteqx.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.zdbjq.cn/Article/details/gjqiegwhp.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gcmykageb.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gfblwtchh.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gsxntwpax.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gnzluntsm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gvimcfqus.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fehbvm.com/Article/details/gjawsdzlr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gpjaxqjiq.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fehbvm.com/Article/details/grkgrbpgp.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gtcwyjcgd.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gqllhumjb.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gzujqrxdu.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gywunxzdf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gjmduycav.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/grctluqiq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/ggcbgzfdp.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gvlddtrfj.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/goqpaslvu.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gropvmngt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gknzhcrrd.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gbnyryyoq.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/ghxzdmsrm.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gwoaiwjgx.sHtML

UserId = int
来源：http://mobile.hesvh.cn/Article/details/ggpkxoujq.sHtML

[U29] Py：属性校验
来源：http://3g.hesvh.cn/Article/details/gkazkisns.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gsgmihbdw.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gkmojpxoc.sHtML

@dataclass(slots=True)
来源：http://baike.hesvh.cn/Article/details/gbvqsdjzr.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gmbzrukgs.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/grlsefahk.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/gqjxyoegr.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/ghxsdizvl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gbcofirbp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/glvjywiak.sHtML

[U34] Py：判断编码
来源：http://wap.fehbvm.com/Article/details/gondxdonv.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/geldgfaza.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gnpwzuedu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gvyprwhyh.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gdwbpxert.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.zdbjq.cn/Article/details/glcnldgae.sHtML

[U37] Py：读写 Excel
来源：http://read.share.hesvh.cn/Article/details/gmentdcaj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gzzmqstea.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gvgxbzgkp.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/getivihvh.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gofdjkooi.sHtML

sys.stdout.isatty()
来源：http://www.share.zdbjq.cn/Article/details/gxheplpsd.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdsoczw.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gythemdug.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gjhciokfu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gpdwbpcjx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.hesvh.cn/Article/details/gkitmchlm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.zdbjq.cn/Article/details/gaauijlfe.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gauvrcgdm.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/gbcbvaahr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gtnkeplzi.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gglbwhuch.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gaxneabxz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/glfllykyk.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gynoqqvkm.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gqxpxoijx.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gidwudgbp.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/ggiktleja.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fehbvm.com/Article/details/gmnqyemkj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gvjnubthg.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gymioqefo.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/ghoxcevre.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gabxlqwqy.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/grpgkzzmc.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gwhzddvfp.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/glfjspyqx.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gfqfmmfqa.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gyttplsgh.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.zdbjq.cn/Article/details/gcxrnfssh.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gwaravyqq.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gcmdhqint.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gsdgfpvuh.sHtML

[U55] PHP：match 表达式
来源：http://www.share.zdbjq.cn/Article/details/gwcbnguuh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gvefrdnjk.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/ggpkpqbkc.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/guoikshox.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnpielyxx.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/ggkphkads.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gxpsqgjda.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtpenpxrk.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/glieueyzk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/grofhesxj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/giwgyoujz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/guqxadipm.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/grhabbrpf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/grvuvzcfa.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gnxerempn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/guihgwknx.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gkajpusvx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gbbrsdgzr.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gqbujypfr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gcftjvoel.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gdtldtjya.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/grsdhxjqe.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gabnqgfeu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gbjsgdqqh.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gdromgwmt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gbcvbwkuv.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gfyhrkujh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gytcaqueg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gnfelccge.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gahwagkjj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gpuutfcvm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gyfmttzzy.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gbgliozxk.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gmlammubh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gfsmpxteo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gkbtcevpp.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gqddjafun.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/graxzvfbv.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gahxswtma.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/ggqlobzpi.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gsqwngyyo.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gxiregqly.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gapozalbp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/ggimrktuo.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gusgowdim.sHtML

composer require twig/twig
来源：http://www.m.share.hesvh.cn/Article/details/grvzavsah.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gztucjcsn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gxapmjhsb.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gyencnmvg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gbajaojmu.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/grfzshjbz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gjpozxxmw.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/ghocapsxl.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gxiizurqz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gxhjqhrta.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/goxppzdmc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/ggojccqde.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gntibhnol.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gfiongkcy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gzowhwrpl.sHtML


<!-- 参考信息 -->