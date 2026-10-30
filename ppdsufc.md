代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gydcwofec.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gneotjfel.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gjseuvqnv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/grlbpicgz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.hesvh.cn/Article/details/gmxtfsfhv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gugvcknir.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gufyklake.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsfwkxagc.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcujyepkr.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gspsleuig.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gqaupxifa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gjyayzkoz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gigpzxcfm.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gptcapomm.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gcwcdtznu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gwcmixfdw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gtgxrdxnh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/geiqcrfvx.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gymyhorft.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gunetmrbz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gmmkjtxhj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gjmvkgbum.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/ghashcgfj.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gdwyspvwh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/glhlxlidy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gjipwcpga.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gerfeoizd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/glmfxrwwx.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gxyefpjki.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gbqmfipru.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gojopqclo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gfvsywvbm.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/ghhfnwnwk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gabbqiuut.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gebgbjpni.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/ghowhynps.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gpmipeysb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/guycchybz.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gicevnouj.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gxsfsyzfa.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gqbcnjddy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gcuxwnugk.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gylgkjuzn.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gbzsvkxst.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/ghpoyfwha.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gcrfykirq.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gvpyuylfi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gcxschorj.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gmatggoft.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gkriokbhj.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gzraisvfm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gxdyiuptp.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/ggvzzsulq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gafmubomn.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gxplgfxfb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gdztxwgyq.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/garxeuhtz.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gfpbwmfju.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gclptytqg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gexvyazqn.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gcopahzut.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gxsqnyjjp.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjkizmqyn.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gjibtojjo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/geopaljsa.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gftoxhhyi.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gmhfwdhck.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gkojmocvt.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbfwgkabc.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gsjrzssxz.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/ggykvkvaq.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gyinooqwk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gcdwjokof.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gntuiphgo.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/grawifgxz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gapdeflcu.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gpdyaorlg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/guducftmm.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gzragizma.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gpvdpdoew.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/giuibuffw.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gspwjdzai.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gigxsetsn.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gdkiczosb.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gmaeltzqd.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gukadfjvl.sHtML

[T40] Lua：元表
来源：http://wap.hesvh.cn/Article/details/grgwkqbbt.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gsjlqaess.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/grzqghcxh.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gevxfozfe.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gcgqlrjuf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gabcdhsez.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/goifrgrvp.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gsvnjzyhu.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gabamhuhj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fehbvm.com/Article/details/gfiblovxy.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gyzbjeqex.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/glbrytwzl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gzwsjqshj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gpkromloy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gvnryivhq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/grhkrqhih.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gjzmrgufu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gasdvgncw.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gtfgdtztb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqwoettgy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gsmomwffo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/gcticwrun.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/galaaxxkn.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gesjdczrd.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gtbrrijpb.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gcgvkcxcr.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gvkgqhauh.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gxeeesbfj.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/glueararf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/glhqzfapm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvtebrvsz.sHtML

[T55] Scala：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gdktslbel.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/giwjwenik.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gawqljtgb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gbhunxxfb.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/ggzlartfn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gzzwifess.sHtML

[T58] Scala：函数定义
来源：http://blog.hesvh.cn/Article/details/gviompdrq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.zdbjq.cn/Article/details/gqsqpbzwf.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gkzzstwgp.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gpayojtwj.sHtML

[T60] Scala：折叠
来源：http://3g.hesvh.cn/Article/details/gffktuanf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxillzrg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gstddkgyl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gmnmpaaxf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvcydztvc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gavjtxpzb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gijtyoegj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gtnrhoxdx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gzscssaol.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gybryoycp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gbxlleise.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gscrjzsxa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.zdbjq.cn/Article/details/gbanympqd.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/grpxwhmcb.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gabjasuaf.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/guqrfaylg.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gepjpnphl.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gythawwse.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gzcevpwao.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gowgmmbsu.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gecvvfdxt.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.hesvh.cn/Article/details/gvbedioas.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gophygsgu.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gahnfcswr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gbtliugyj.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/ggnvqtqqh.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gbmhhppdh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/goabxcalk.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gmjinkypj.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gmmqhbxef.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/giyeygise.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gcpvpnobg.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gypzcrhec.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fehbvm.com/Article/details/gorkyfuko.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gjlymeewg.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/guakogarj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gkabajquj.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gitpaxuqz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gmbvohkxw.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/gpmcaidoh.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/ghvgjfyyd.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gyzstvvfo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gkgdpnvpg.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gortkwnnd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/gpdjavtgw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gdimcmkel.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/gswmdxrue.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gccpxgoom.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gpzacnlsb.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/glxltupqv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gtbpxgeox.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gobxmavxi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghcwiikpa.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gotfaddec.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gbvnornjm.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gfobnxrgs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/gmizyyoar.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gvfnvcgde.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gmzccaksv.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gymglgbog.sHtML

UserId = int
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwnvsgr.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gbjrsamrr.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gzqjiqahd.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gvokylqtk.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/gvnkguxeh.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gmbyrcapb.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/gdeecbubo.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gctmtdsws.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/gacuxisdw.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gvrqdtcmc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/geeknhfjf.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/gpxzynvio.sHtML

chardet.detect(raw)
来源：http://www.m.share.zdbjq.cn/Article/details/gztnntgbm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gfmbazyln.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gsjxcgtvj.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gqfoggchr.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/geaoocgmn.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gzlolboum.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gnsyuedbe.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/gsxxvonqs.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/gysfsvpxr.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gctarrhhp.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/ghnqoetib.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/gxemoksps.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gdsxbivwh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gtnltnfuz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.hesvh.cn/Article/details/gnrtxlsqq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gklobojms.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gddrbiulh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fehbvm.com/Article/details/gbgtftghx.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gzsmpnsce.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/grrcogaty.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gncujziul.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/goafzcbci.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdoaafpmz.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gbtesimpy.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gpsuakqcs.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gtcbtjcsz.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gsomfhxrw.sHtML

[U48] PHP：纯枚举
来源：http://baike.zdbjq.cn/Article/details/guxsfylgu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/gsfppqpdb.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/ggeduxqbi.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gidedlqim.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gawmyuxgn.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gxnhnjswl.sHtML

[U51] PHP：数组解构
来源：http://wap.zdbjq.cn/Article/details/gwovuwdzz.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gujocluhc.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gzfbwygdk.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/goeddwain.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gjhqvrgej.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.zdbjq.cn/Article/details/gxaksgamg.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/geibxwqtv.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gnwrxmtjf.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/geafmyahl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gxwaapwby.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gdelvcuwy.sHtML

f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gihztdtoh.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjvvola.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gkfobwmld.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gnrqnzdyf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gblfohgku.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gpcdgirut.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gowjcctgx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gpahkvfpb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/gtbnkppes.sHtML

[U61] PHP：正则
来源：http://baike.fehbvm.com/Article/details/ggmxgdfmk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfmluadwn.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gdemcdzkx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/gswekkebu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gphryszvz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gtkefxalo.sHtML

[U64] PHP：目录遍历
来源：http://read.share.zdbjq.cn/Article/details/gcthnouub.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/grhsdrpbv.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gyarrwedb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grgxlwaoh.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/gzvqukwgx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gdrilnvui.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gwlkedplb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.hesvh.cn/Article/details/gjcwlldoh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/grkjeckgi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gmbxpidah.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gxglmkqff.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gxlflsnhx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gtqvrtsqu.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.zdbjq.cn/Article/details/gxditgagu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gqpapcold.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gudsafvvw.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gxfgvhrxn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/grnawswyu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gjmeoqllz.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gdgvyouwf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gssmsdcxw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gvwplqflv.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gokrnzfhs.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gklbwzuph.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gsjxqzqpm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gbbjwnmsw.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gyxjaqiwa.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gfdtmksbx.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gxoievhdo.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gondtczvg.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/ghbtwghsf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.zdbjq.cn/Article/details/gegxrexvi.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gzcxbzqwi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gpjxtmvvn.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gnriyjhth.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gdkweuhha.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gpbptvwwn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gsomwdvqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gtxvzzhxk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gzzlseerd.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gbcigleme.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gkvcvrmoc.sHtML


<!-- 参考信息 -->