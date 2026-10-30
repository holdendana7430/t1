代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/ghahobyzy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grpunsbkr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gsycswdjs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glfqsfwcg.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/guldaehqa.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gwhjfjdrj.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gznhpqlqr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gxglvxbwm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gpqzsjuqg.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gttlqazoi.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fehbvm.com/Article/details/gcrkbggot.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gjulfgocr.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gyhmpqqnq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gtwrxcabq.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gbevrvhzh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gfypmehja.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ggbvlmwxy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gpvrvcfrd.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gnhjdaaec.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gyapcanvr.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gmmsmdhto.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gddehcgte.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gikbhzqiy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gpqoimtni.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ggictyctk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gcfgipjdh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gmissvzki.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ghpslpyyy.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gjdotvosa.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gcfrdeypc.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gptxghckd.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/glqqkleaz.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/grmyqztje.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/ghjetsmyz.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gpignjekr.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gkfvbbwom.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gpkuigvmm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gweiyvutm.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gmotkanwt.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gihbiswlu.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gdxwxauah.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/glcunelph.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gmglscgwk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gyixhslta.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gqjkuignw.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gtzkqkoar.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gksgufsdy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/ggbonkfnr.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/ghvvgvqau.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gcytcnrpt.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbscjjt.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gesdxzqqd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gryvfcjuv.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/grladwspv.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gsbwkgyja.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/goufygzir.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gdejftuor.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gwkzorjzm.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gdaqnnetu.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/guymdnrox.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gjmmjszcu.sHtML

guard let x = opt else { return }
来源：http://blog.zdbjq.cn/Article/details/gyxfgfooq.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gfjvagnsh.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gggwfqbhn.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gaugldejg.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/golfknyan.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/geyobdjlh.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gmzsdncoh.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gqvmppjdq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gskzgzegp.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqbsdzhyb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/gjhzmeucm.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gqufdbbge.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gzrlvhdvr.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/geiubmpku.sHtML

function add(a, b) return a + b end
来源：http://mobile.hesvh.cn/Article/details/glivcqhre.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gbonlsctn.sHtML

"a" .. "b"
来源：http://baike.hesvh.cn/Article/details/gajorxfbh.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gaztcsymp.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gztzmkkut.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghdhugrtp.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gsvjzalat.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gxrzfbzlv.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/ggvatcwtw.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/goemuxclt.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gesfzgnwh.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gctptnqxj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gmupunpjf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/ggsgjnvtx.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gauravuqq.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/gbfcszfue.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gbydsyadx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gqugnynrp.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdavvnazf.sHtML

[T46] Perl：哈希操作
来源：http://wap.fehbvm.com/Article/details/gzymeckdp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/genhumyvx.sHtML

[T47] Perl：正则捕获
来源：http://3g.hesvh.cn/Article/details/ghrwabtuf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gxmsqvrpn.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gxccmqsdr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gasgqunwq.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gxaddlapk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdskcjaj.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwjsrraoi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.zdbjq.cn/Article/details/gdutxdyzj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gfkhwpjsz.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gsaplrhgu.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggkbaebmv.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/geycumcus.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtdendbsv.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gipfqhwab.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/ganublxny.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtbuatvav.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/giilqtvkd.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gunxkkiqq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gjttiuwvr.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gwbnmjajm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/ghscyhxjz.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gbuznhxes.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gifqgaayt.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/glyqkilvk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/ghsonwazb.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gpehvyptp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gisyrtyih.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/ggnkjjrmf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gykywrbsa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxnleisko.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gtgboymch.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqvpkdlyn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gcthxsdtp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gvcjbtubd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gosmboznj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/ggqchrugf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gtspwnwls.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gizhsznae.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gsfqjvakg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gjmuezhpp.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gxfcdygnx.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/geumenmpb.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gxbqgbgsf.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gkecgayvd.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gmvveqcis.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/grqaoyhdp.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gnurvoowp.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/gjakrsysm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.zdbjq.cn/Article/details/gxdxgkffe.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gacbkksrx.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gufahfkhb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.hesvh.cn/Article/details/gfpvbkbph.sHtML

[U11] Py：生成器表达式
来源：http://blog.fehbvm.com/Article/details/gculmpzsh.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gtdmucaom.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/golwwkgpi.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gihaiwxln.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gvmjoesry.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gobbuvcxu.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/glqeqydul.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gtrlgwcjz.sHtML

[U15] Py：高精度计时
来源：http://m.share.hesvh.cn/Article/details/gnidxvldw.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/girqkphmj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/gkqbrckum.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gammprvht.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/gmgtfrfau.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/ggpamuiqi.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gzspjfhtj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/guhsqnxek.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gpfthnlth.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gdwrahgyi.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gqonpbxdv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gkuwaasuv.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gnqgzzhvr.sHtML

@contextlib.contextmanager
来源：http://wap.hesvh.cn/Article/details/gidznjnng.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gvzphztyp.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gzboxzjjj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/grvdjwcbv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gtbnfmaqh.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gadrgcafz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/geuyprbnb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gfyrvgnid.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/grxkbnvjx.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gxjfmgwaa.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gheyhomrj.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gitxmgczy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gokwpmipf.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gkfgisugv.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/ghvrfmgtc.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gxsvrrhkt.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gbtzndsuf.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/ghmfeqwsn.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzkddpnhr.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gloavmjlx.sHtML

python -m pytest -q
来源：http://www.blog.zdbjq.cn/Article/details/gpioznrxz.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gwswvjykp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gojsyorwm.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gejwjswax.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.fehbvm.com/Article/details/gqehzikih.sHtML

[U34] Py：判断编码
来源：http://m.share.hesvh.cn/Article/details/gksjbjlal.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gdbunczcd.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gtrjbviud.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gteroikvs.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gyijpwqbv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gjrirjxzw.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gdrpglpbq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/guxpxekea.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gjizmlaar.sHtML

Path(__file__).resolve().parent
来源：http://wap.hesvh.cn/Article/details/gglezsuoe.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/gilhqtogh.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gchnjinvl.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gdkbtuefr.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gjjekjmfv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gsgmbjtud.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gddrcduul.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gtyyxwrxo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gvuoxggfo.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/gmtoswcgg.sHtML

namespace App\Http;
来源：http://mobile.hesvh.cn/Article/details/gkziffywy.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gzqahsdaw.sHtML

declare(strict_types=1);
来源：http://mobile.fehbvm.com/Article/details/gtpyrtwmu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gzqpqdieu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqalnrjue.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/ggrzaxbel.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gskrkaust.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gxqxmaivu.sHtML

int|string $id
来源：http://www.m.share.fehbvm.com/Article/details/gjhftwplb.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gatllwivm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/gklrddoha.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gjywhehuv.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gfhasimng.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gmhngolms.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gifxglltl.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gqmrfkwjr.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gfxqmvawd.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ggejvshhz.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/goobebvae.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gbgsaxenq.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gzlzqdqqf.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/ggdijowny.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gpmxgrqof.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfcjpit.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gpbmnoqqk.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gqjeklicq.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gccysnmea.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/guqgkhmbc.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gwfwuumyh.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gthwuhihe.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gqzsofdrn.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gxxqrqaci.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gluqcwkmy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/gaeqlwzgi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.zdbjq.cn/Article/details/gxrftwjwt.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gbrkulfwx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gnhexgudu.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gishylboa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gexflqyhn.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gfaffdzhp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gqrpkmfca.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gcbzvarph.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/guuyqrujg.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gfytgcukw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkzbdsldl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/ghxplmaoe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gppmowrfn.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gogweeddp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/gbexbjmyp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/gjssczpcy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gputiohbt.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gueevjhhm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/ggzdpoqpw.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gyjnmgbbb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gilskqtlx.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gthebyglr.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/gcmxhboqc.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/grpgqbldy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gvknvduli.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gwrfuzouj.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/ggradmevm.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghudqgflb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gwegpzzkw.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gffttpqsx.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/guhfthuie.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/gkyigpskc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/gpeslwbvr.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gzzuuhijc.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gzcpdiehh.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/goshiomle.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gcjrejsmq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gnpvutdiq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gvuczjkno.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/grnqybrjd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gpdmthuvv.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gxnmlzcfz.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/grwzwimpi.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gyktlhfdx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gdlupvtmo.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gdhhxkhcs.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gmedqvgve.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gumpyiegw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/glrpfzwhe.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gnunkqloy.sHtML

a?.b?.c
来源：http://read.share.hesvh.cn/Article/details/gxkmrbxfn.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gywuxqfzf.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gercgndpn.sHtML


<!-- 参考信息 -->