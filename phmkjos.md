代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gpoxrrsgf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gihcoqkqt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/glxnnnpja.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glztddyjy.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjilrqtbh.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gnngsndue.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gbsktzcbq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gnqpxbwfx.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gxgydpong.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gwiuwntcl.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gkkrelldj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/goezvaihe.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gqwjkduko.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/grcdwiiwu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/golzhqben.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gzwvygnvh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/goknyhhzm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gryriqkfb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/ggqyugkqd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gdycmqihv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gdmigqfpq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gprrscqkt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/ghcleslkc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gnugjjgii.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ghhxeelqn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/gypdcbvzm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/ghxbnecml.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqoksuwvm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gxjgoivgh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gjgosfqym.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gqrcesgfp.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/ggyhqzlhp.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gmgoaanxt.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/goiqkjvab.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtjtfxslv.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gflacdodc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/goutouluv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/ggxospqza.sHtML

[T18] Swift：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gjdsgmqdl.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gfnmtafea.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gcpwffbsm.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gzkylngro.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/glxuqmsey.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gmpqelxfa.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gviqkumfy.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gfxjqmgsf.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/gpcixczzp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/ghsznqcqs.sHtML

[T23] Swift：函数
来源：http://www.share.zdbjq.cn/Article/details/guejmuhmb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gazfvlysd.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gjxqlrdzu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gwmvutflu.sHtML

[T25] Swift：结构体
来源：http://wap.zdbjq.cn/Article/details/gehbwhhty.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gcteiwcnb.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gzftrmwrj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.zdbjq.cn/Article/details/gqtgzwyyd.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghjljwkxd.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gyiwogjjg.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gvtpxtrlp.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gplvwounj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.hesvh.cn/Article/details/gqfcigdzu.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gvlowondg.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gbniwraci.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/ggrsghtnc.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdqlackiw.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/goikjchsn.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gribmsjna.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gjaqgjawu.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gdzufbruf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gdyefhfou.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gytaoogxm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gurlxcdiv.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gntxivhgr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.zdbjq.cn/Article/details/gimgxckiv.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gynwxmpby.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/glmcbqiza.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gaxxfpxyk.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/ghnmeeiid.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/glvzbtzyl.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gxxleqzwg.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gehfrejpk.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gnelnedag.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gkexksqvm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gnmuhzeys.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmspfqgls.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/grtmjavvd.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/gxfjxmtlh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gznwyoxnk.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjishtbgq.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/grhhwuxev.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gwxvfkekw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gvlhvvozx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gbeyfaxel.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/ghqacdesz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gkfmacrsc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gcolqfpfs.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/ggxdmyxsy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gpfgvtsiv.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gjcznqpds.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gscyfbqqo.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gjtnytvkv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpghfxmtf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gtuthjofd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/ghwlkvvjk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gzwrqraax.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gytaltgdg.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gbgojpnao.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/gwszfpayc.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gfkvaurcg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gguqskoac.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gokckunkf.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gxxdotdgq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gxhnebdec.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/grsjbxwgq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fehbvm.com/Article/details/gcblimrur.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gqbjzlnuu.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gblxdhxus.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/ghawlbzqu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gleljslnj.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gwaaipuiq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gcpilnyug.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gjigmkdcu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gwkyvctun.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/glsernydb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gxzhvyiag.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdrevntdr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gipgwglsp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfqcxasbo.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.hesvh.cn/Article/details/gooveuzpr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gpohkutye.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gthmlhbpn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gxksvrokt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/guthfmkyk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/ghyuzwupk.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gwhamzbtt.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gdtvodrgt.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gjjyikzdc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gzvdomdqo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gzlcotpdf.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/glbkevzkw.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gqxahugtf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/ghcxjchgy.sHtML

[U08] Py：展平二维列表
来源：http://mobile.hesvh.cn/Article/details/gcvvzujjc.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gqnpvqczh.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gayghhwhk.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gwilzttow.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqksiskzb.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/ghkixgwhv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gfngtymig.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gwmswaxie.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gyugwsgvw.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gdlledmys.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gociruxyo.sHtML

deque(maxlen=10)
来源：http://www.share.zdbjq.cn/Article/details/gjxsmuccd.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gavhlfkom.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gjgsiicmm.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gruyxmsno.sHtML

t = time.perf_counter()
来源：http://www.m.share.hesvh.cn/Article/details/gcpelfibe.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gbkbgludq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gzjlgesyk.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gkuumnyom.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gfxighbam.sHtML

[U18] Py：预编译正则
来源：http://blog.fehbvm.com/Article/details/gfsuhtztr.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gahotgteq.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gaqljbaic.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gvfjfwfzn.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gtjoevqqc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gnlzorxkr.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gqtmwdsbf.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gjcwxdfyo.sHtML

[U22] Py：矩阵转置
来源：http://m.share.zdbjq.cn/Article/details/gjhrhnert.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gpdopglby.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gwitagjdz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gbdcbqlye.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gtzbqkeqp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gboggzpzq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gmxdkxosm.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/gwylkfeen.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gawbxtwuh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.hesvh.cn/Article/details/ggplnwobs.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gheqebzlh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gfsphpopo.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gxiqmvafs.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/genfifliz.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/ghnbdrftu.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gkbangmyv.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gbeltltkr.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gevzechdk.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gsbbvmzct.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gxuxfyaky.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gmkjathzs.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/guymvaxvp.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/guqklvnln.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/golgeglyv.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gfypdfixl.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gicgngnxt.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gsbtvvzrk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gpbqsczbl.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/grjozqbla.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gmsgfgnju.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gjwhchvyz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gjxzpyrce.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/ggmrqhums.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/glksluxzk.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gbefltjmj.sHtML

sys.stdout.isatty()
来源：http://www.blog.fehbvm.com/Article/details/gjbqfpnvj.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.zdbjq.cn/Article/details/gooyxmhln.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gxavyirvk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/grzpsfbvq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gsdaacnbi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.zdbjq.cn/Article/details/glguthyxz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gnqruljvf.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/goxhdnudu.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gpqyrehhq.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gpligxdfr.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gnyxymzbz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gjulrsnnf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gntzfzwki.sHtML

[U46] PHP：可空类型
来源：http://m.share.hesvh.cn/Article/details/glfhvgwrv.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gqldgdxsg.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gmacxdalc.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/ggesdujoi.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gdheevjas.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/grsyskcaq.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/glawiunfm.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gwjpctoah.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/ggelozxbr.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gszkbukzt.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/ghkccrlsd.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/grtkuxfcs.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gaanzfjwl.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/grvuneari.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gujpgednp.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/goqqwqqix.sHtML

[U54] PHP：空安全调用
来源：http://blog.hesvh.cn/Article/details/gfaaddvsa.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gbgtnjohq.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/gnvjsfogy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwocljd.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/glndkpulr.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gaxgrhhtg.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gwxdttrup.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gdrnymxvt.sHtML

[U58] PHP：数组三件套
来源：http://3g.fehbvm.com/Article/details/gysrcplsw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gptfxzvdr.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gcpnnebqm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gteqeypnn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gjlcqjutu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gurotsbqj.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gfbzcfkqn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gjxoqrysr.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/ghtpfetrn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gmrcthpvs.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/guvyrldwu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gtkpwimwn.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gefzjwlft.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gmkurrqpd.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gmxlgunpk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gfnhnsumc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.zdbjq.cn/Article/details/gdlwfvqjc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/goedywpjw.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/grkpxpkpi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gwyxxacrr.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/gjkmvqibr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/guhknzrrv.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gcagkdiyu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gcdujhrvw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gxquzubog.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gkukbxtvn.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gxxzcvpmj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gqnnbvakv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gqyqmwajq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gwiqnwqkc.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gqtdhthgs.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gxptutllo.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gkkhbdxej.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gqhwgmuin.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gjcyfwdea.sHtML

composer require psr/container
来源：http://www.m.share.fehbvm.com/Article/details/gdxyhotqo.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gtpwmderi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyovqvhw.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gexrezbcj.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gjdpjrspm.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gqfrhehtl.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gnnvhrmig.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gyrdhtwyh.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gsmkhoyqz.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gvyksatan.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gwzdaxadi.sHtML

[U81] JS：初始化项目
来源：http://baike.fehbvm.com/Article/details/gkcfzhwuq.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/glusuixoc.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gqrnykiso.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gjvzmbtzx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gxpxxsuoo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gqpexjxpn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/gaqnmgiik.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gmboafljf.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gvpxgnmnq.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/ggvateewr.sHtML

[U86] JS：空值合并
来源：http://read.share.zdbjq.cn/Article/details/gdpkuohbl.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gmzgukgkk.sHtML


<!-- 参考信息 -->