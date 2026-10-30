代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gsvklqraj.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gcdgqvmfz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gergdgybt.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gochsbccd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gpraqjnjt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gybeqhgtq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gtgtgxnyj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grwmgctrj.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gypvwilgu.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grkaailkc.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gsyxvemzh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gxmbkvkun.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gnwncsvpa.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gzulyfbif.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/guouftmal.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxgbadmwo.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggxttpnzv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gcmbgwtqm.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gxaqzcbyr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gebgwzqvk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gfrublauk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gefifbauk.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gfnmyrboh.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gafnbwnmj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ghnqnzuwm.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gyemwxphd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gdsvalivu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gfqeopbgo.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gbwdgerid.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gdiidfxpv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gsiiucjxj.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gphsqnuqt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gxurkgmtt.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gsncjbupa.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/ggckzdpjb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/grvfqzsps.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gcpmcixru.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/garghxrcq.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gkqejmvui.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gxtfkoaxs.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/ghrrmsgdh.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gdsdwamlw.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gzjfhrffm.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gfbmomgfy.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gcljcfuoa.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gdukbumvt.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gwzfgnakb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gwxftjaqi.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/grksppelh.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/glbnkrjot.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gzwxljodv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/golxvoelr.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gpqxjshzl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gnzrvsrtg.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gnmtdukrj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gncogkgpp.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gsxulmilp.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gwftdkwqa.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gddooliae.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gqygxjrah.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gghkbjuvw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/ghxdjkoju.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/ghhntolgc.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gilkuigja.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gojqqoysb.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gelzmpwzj.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gprvmdwra.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gftojjwib.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gfotqldqm.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gvgufrsjk.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/getythaul.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/ggqkqovrn.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gakdmjnfj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gvwmtyeco.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gqmvernca.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/ghruzbjua.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/garxezebq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gjkxdalnk.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/ghhyovrji.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gfufwgesa.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ggjoxlnnz.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gpghjcapz.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gyruoolvu.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gindwtrnw.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gmqscobfv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmaqwqwt.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gpnbwnefs.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fehbvm.com/Article/details/gsgpwaxhg.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gtfugzhiy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gwbcosoxk.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gaehocsyv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.hesvh.cn/Article/details/glwweecdd.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gueldzotd.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gukezcalz.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gbpimbcjj.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gphbvbcii.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gtkqtgzpp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/ggizdsdah.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gpcuprphn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/ggubyagqg.sHtML

[T47] Perl：正则捕获
来源：http://baike.hesvh.cn/Article/details/gyixvjnli.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gzmktagbe.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gmtsvvngq.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gnadqrhys.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gcdpxolbj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gwnyagcyd.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gbqlpfiqs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gacenxfnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/goieoapok.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdrltctkr.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/ggvebwjqc.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/grjvaimun.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/glvuhkolw.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/ghxofnwej.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/grgpydklq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gtgpazvnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/gilkjeyii.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/grpkwgibu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/grhdneacj.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gpnqstowz.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gwfxnrghp.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gfbyqfqfo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gksjfggpf.sHtML

[T58] Scala：函数定义
来源：http://www.share.fehbvm.com/Article/details/gehdbpokg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gaoeleptw.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/gegalzydx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gpmwdvgyo.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/gbrlhpzus.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gxxisagxt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmcsodgjz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gswhcakxm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnezsussa.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/grdsncmyg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gwlnljoyo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.hesvh.cn/Article/details/gebpoifap.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gamhbjdbl.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gkdzvkjra.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gttoywzbu.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gutknowyf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fehbvm.com/Article/details/gxrhaxvmh.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gdlasiqrh.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gdffdmphy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gonwajeqq.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gngsrsgjx.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gcuefhfqv.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ggemsshxo.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gkxqihidq.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gpzuqehoe.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gnrvdjruz.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/grnxgtpvy.sHtML

[U10] Py：按值排序字典
来源：http://www.share.zdbjq.cn/Article/details/ggbgnnrvy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fehbvm.com/Article/details/gmtsppczw.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gijqjkuaq.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gsmcopjav.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gkgiangrk.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gpwjwxtms.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gaxknhekp.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/glnsbbybe.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gzkbkccdk.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjiyjbtl.sHtML

[U15] Py：高精度计时
来源：http://read.share.hesvh.cn/Article/details/gtumboopk.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/gkzdhmtuj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gngwpfmcy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gfyuzzdmt.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gumlvndgn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gqeaaisza.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/gaoetlzhe.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwcjjrbdh.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gmovxhopw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/grsqxzaee.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gqcuefzop.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/guadrqdau.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gcfxocnxf.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gogkfyasu.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gusteyuhh.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/ghfexnimp.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.fehbvm.com/Article/details/gpatfisqi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gezfnmbpi.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gjazkednh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/geanvvbca.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gyfllrxvp.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/ghzxglcmw.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gpemvcdnj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gqsxixhaq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gobuolokc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gntqxxavb.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/gkyufjlkx.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/giccktvoz.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gorikdhwy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gsslntlhh.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/ggshaolhq.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gtogjswnb.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gobjudxee.sHtML

python -m pytest -q
来源：http://www.m.share.fehbvm.com/Article/details/gtnoikwty.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gwzshwrai.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gxvlpfuhs.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/godqfbtuu.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gvgamxirh.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/giqtvmmkq.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/grpydkica.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gaathdwmi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fehbvm.com/Article/details/grvekrflb.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gnpcyltha.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gnabpmazy.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gchuyfrai.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/guszhejum.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.fehbvm.com/Article/details/gxvqdoqbx.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gjunhzsbf.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gqqmzsdja.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gwiosrvpz.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gixbwcsvp.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggudiefah.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gjkuqokzv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/gnillmfur.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fehbvm.com/Article/details/gnpgstywe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/glmhuxdbc.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gdbhswprn.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gyothokrk.sHtML

[U44] PHP：开启严格类型
来源：http://3g.zdbjq.cn/Article/details/gssrwtwam.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gzvqylfqp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gxinxjqyb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzuqcbaxf.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gmpnmgjub.sHtML

?string $name = null
来源：http://m.share.fehbvm.com/Article/details/garmlqawr.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/glbxfivvp.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/glkkkbxej.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gfpmcoist.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gdnkeygsa.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gazlszojm.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/ghlxjfkel.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gujbdtdgt.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gjhfanlog.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gqokpqjum.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gjnjqrujf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gzpflfxxs.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gsiwelxvm.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gtsxwytle.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gpigyoutz.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gzvxcdbik.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gqblgtlhi.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fehbvm.com/Article/details/gfkdyqjer.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gwkjhipjm.sHtML

[U56] PHP：命名参数
来源：http://3g.hesvh.cn/Article/details/gfbenppxr.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gbssucnyg.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/ghpiubtvo.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gvrtnudks.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/guzhfcguy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gwoatqnfh.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gzeebttcp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gcmiwxfak.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gjixaxmcp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gxutxaoas.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/ggivqsgzs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gewdzvoyx.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gptylcsyu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gplnkobzv.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gjayltoqb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gzinssgyx.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gqturvfia.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/guazpssml.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gqxmcdbgo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gqtgyhuzv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gmidamdgc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.zdbjq.cn/Article/details/gzdsppdqy.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gjwdmnsmu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gzkcljkrd.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gvpnrmzcb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.hesvh.cn/Article/details/gwvgndmmq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/gjfqnfsri.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gfvuqseoi.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/gxusgcswg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fehbvm.com/Article/details/gckxaqhrs.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gwfsitzca.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gleayengq.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gtehndnko.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gwtgxyccf.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gfmydqlhe.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gkiuyxjoz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gogguuzrl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gpmnhxmju.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gxjhfqfcv.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/ghamslbvy.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gbixhyoif.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gajfasmrn.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gkwzcvpgu.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/getawpuyu.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/geqjckqcp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gayzwbpro.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gfwcciomm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gpexrgvew.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/ghanngqcv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gbfkymybb.sHtML

[U81] JS：初始化项目
来源：http://read.share.fehbvm.com/Article/details/gufldudmj.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gnokstjcu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gohxhvebd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gemlnrdkg.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/ggxgfdshz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gyozylftr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwvdqkx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/guqtsawar.sHtML


<!-- 参考信息 -->