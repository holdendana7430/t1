代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gnjixjlsf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbxjbowod.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gdlcfblno.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtryuzrcu.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gexjlgdpf.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gknxipudu.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gkkuqfcgn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gsufevtzm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gtcwcrseh.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/goylkanob.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gclwmwyuw.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ghmtzuzwe.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/gjpojgdbv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/grkftmdhv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gpcjfinky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gpgeccgvm.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gtavvtlgp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gyxceumrg.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gksizvaxs.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/glsvztrzp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/glzfkxqhb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gmoqsswur.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gtjhhddzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gdmklacie.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gdgpnvebz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gqydzebsn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/glceiotlr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/grwfknnfh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/giwtnyyyj.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpcksqplj.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/gzloabsir.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gxouiiqtu.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gwfybflsh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhweilhs.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggbffbrce.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glaoxqkdv.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gacttfaao.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gmpizldlk.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gfqrwngmu.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gddkfwjqn.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gztaufbsx.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gdnpgvtzp.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gtswrxboj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/getswcxyh.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gymiuuixy.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gwcfbmzbt.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gnovsarps.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gukzdtexx.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gmfmivebs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gixnljigv.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gxihwpmut.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.hesvh.cn/Article/details/gvxlloxuv.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gmjsmtcob.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gpdfjqbaw.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gpgxqxzmk.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gycirfrws.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gvpnccpfl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gjjvqhmif.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gyorfkxhp.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gpdpkexqg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gchrdlods.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/geisitdfx.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gjgiwtbch.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gajybkbnh.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gsxdtgray.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gtgjmjwmq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/ghtqjwvyh.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/geupljuil.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/ghcumxgwh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gtgtygfou.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/guzcyaemy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gatvjnpnm.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gjnqweeox.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/grveykdhc.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ghexvlmsf.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gucqkkahv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/geveifcos.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gezxsyvjz.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gatkucogy.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gtjckzijk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqgphptqv.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gawbdjcqr.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gfbtekijw.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gcnfwldcj.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gecqceyiz.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gjljqstvv.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gtebzruna.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.hesvh.cn/Article/details/grurvekim.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcmrjrrdr.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/guxgyhzic.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gfqdacegw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gnjizuzlc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gyvltagtq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gzpoifsqn.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbzpotgzl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gizzdvyay.sHtML

[T47] Perl：正则捕获
来源：http://blog.zdbjq.cn/Article/details/gnxvpxeck.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gppehkhhw.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/gxbdgxedi.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/glcrddxhi.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gwapsuxsu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gcixkwzda.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gbgonbgoo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gkyhvlbkk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gkkwzludx.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gjayxlmzr.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gamwgehpv.sHtML

[T52] Scala：变量
来源：http://baike.zdbjq.cn/Article/details/guniobqef.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gpqkhxmcn.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gjquruuix.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gadvrdpts.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gjboozlbf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gznapbhqf.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsxjrvqrz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gmraktwjn.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/gzuotcsgh.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/glhfsmbdp.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gjtvubbci.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gwuvyyqzd.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/ggkamwwdn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/ggfzcmbbe.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gfkerxlki.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/glsyvslww.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gltvteqhn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/grteklatf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggofhprkr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gfesruhlw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfpmlpalr.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gqcmcqnxz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.zdbjq.cn/Article/details/glbicqeap.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/goqpbcnnr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gplcnlxux.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.hesvh.cn/Article/details/gtdmkikfu.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gyjckbwlt.sHtML

[U04] Py：变量调试打印
来源：http://m.share.zdbjq.cn/Article/details/gptyklggv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gbgrjidyb.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/ghrwpnxlx.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gsskznxzz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.zdbjq.cn/Article/details/ganzemfjx.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gqtnyadji.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/gesksxycg.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gfwbtnxxk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/ghvjzhmnx.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gfospeefd.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gdhsukbaz.sHtML

max(d, key=d.get)
来源：http://www.m.share.fehbvm.com/Article/details/gnvdbbeya.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gwquzyser.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gmvntrojo.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gvvvetded.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.zdbjq.cn/Article/details/geyvzaweu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/gexjrzdqc.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gazlnzsmx.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/govuvavib.sHtML

deque(maxlen=10)
来源：http://wap.fehbvm.com/Article/details/gpoyofhaa.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gselceuxz.sHtML

defaultdict(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gztmpttml.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/ghizgxpoi.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gosdtcibj.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gztrntuhc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gdwbhhaok.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fehbvm.com/Article/details/guxgntgfj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/gyxodzcff.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/grrimblpb.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gfovilnkn.sHtML

[U19] Py：正则替换带回调
来源：http://3g.zdbjq.cn/Article/details/govzeztkq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gdnsflmfg.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gyueijxrd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.hesvh.cn/Article/details/gunxnhwlj.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gtsrywpzp.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fehbvm.com/Article/details/gxsqojbxk.sHtML

[U22] Py：矩阵转置
来源：http://3g.fehbvm.com/Article/details/goopmrakw.sHtML

list(zip(*m))
来源：http://baike.hesvh.cn/Article/details/ghqbwqxcc.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.hesvh.cn/Article/details/gaqdxibkj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gotpqtqen.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gnxdxfkgo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/garhubcwr.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gwtldeirg.sHtML

csv.DictReader(f)
来源：http://read.share.zdbjq.cn/Article/details/gmehrbtfg.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/goxzrlckm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gxhviksjd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/ggndzvtru.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gxkpxbmke.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gemnsahpv.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gifvwzcgc.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gosvxolai.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gptgvqoiv.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/ghgtverga.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/ghghdngnr.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gdfkgxjvz.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gdpcngnlc.sHtML

[U32] Py：代码格式化
来源：http://www.blog.zdbjq.cn/Article/details/gqguayene.sHtML

ruff format . && ruff check --fix .
来源：http://3g.fehbvm.com/Article/details/gsrvipdrt.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gtogllqei.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gqzmlxoom.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gduadaiuq.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gikhtewke.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gyczponxw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gddchvevt.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gbdsxwauq.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.zdbjq.cn/Article/details/grvjosxin.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/gerhebzsu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.hesvh.cn/Article/details/gzjyvpifq.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gxhzmzqfg.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gbmbxziah.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gmilruivg.sHtML

sys.stdout.isatty()
来源：http://mobile.hesvh.cn/Article/details/grzsolusn.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/gufegolga.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gxsxrrwow.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gzgmpdcun.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gmsaovzbo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gcxipwkmj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gajtacmwg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gmacdgend.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/grvvudmkf.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/grzfkgcxo.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gqjtwzfzg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gtamqfogp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gynxnprhh.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gwvvsgesi.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gxwygexry.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gsizlbrrh.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gbndoilff.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/ghqbiukvh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/ggewehtdm.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gzmhmihti.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gmunokppc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gbyiwvpro.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/ginovfzmp.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gnpgijexu.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gyteyjwdn.sHtML

[U52] PHP：箭头函数
来源：http://3g.fehbvm.com/Article/details/gbjehesun.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gbbhxngik.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/ggpewtaas.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/grlqdxxxa.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gnnpmomue.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gvnbxvmjc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gondayzfz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gojqcmfto.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gplvkaupi.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gcuqjqusn.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpjwhcmor.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gnuvlicfr.sHtML

[U58] PHP：数组三件套
来源：http://wap.fehbvm.com/Article/details/gjufgtwgq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyxkzaguq.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gbfivipwo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/guuoogivn.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gopcmttyi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.zdbjq.cn/Article/details/guubhllpu.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gncigekrn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gdkjmshwz.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gdjifxgof.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fehbvm.com/Article/details/ggwglsoie.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gxjmpyegr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzfmgbo.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/golpkmsfg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gwpswrbhs.sHtML

[U65] PHP：会话
来源：http://3g.hesvh.cn/Article/details/gjmbytcth.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gnxxqvdtk.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gbptdrlso.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gytfmbrpe.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gvvktjueh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gqspfrmbi.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/ggmuzsxep.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/glnbuvvxi.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gjlxgnszp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gosavldgl.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/ggwtaljkw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/guzqgcjbx.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gditxbjiq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gpymayylf.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gfamxmusi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gsatdnxgn.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gyyoyavhr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gjdxqznkb.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fehbvm.com/Article/details/gwjtvctlq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gqmniqubb.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gsbftxadh.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gkpdqknde.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/gkkycgacd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gyshxkyhq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gexvlywse.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gxiytbqjd.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gstksmdlw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gueupspqg.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gcsjyugev.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gjjzfntyg.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/grjbnjkdq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gbrzevujb.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gbtagwtsj.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/geebrumxv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.hesvh.cn/Article/details/glzboqkzm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gilapfrsc.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gdtnzpcjv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gixsncigl.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gyygogahf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gzvqvdkif.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/gxqfqabno.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gqgdkmchm.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gqgujtoxz.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gejuejzzs.sHtML


<!-- 参考信息 -->