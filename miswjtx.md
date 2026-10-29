代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gvjyqxtme.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqklnpcvk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gtfhffjaq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/genwmtfhj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gxtusqwpn.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gsmmryktd.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gikmiieuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gewtkxogw.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gmxlnncvz.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gvdenoqmz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gtzyfsvod.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gcevlgpjb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gckkfzsrb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/grupmafjr.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gwxcmwtjs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gpvmljduq.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gcnjfqyca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gufzsfbwk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gafbakdzw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmepuqlto.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gyvbujvwo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gfnfxlihj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gtsoduwkv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gothvsvon.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gimlbjdme.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ghmsnqduf.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gsserqdof.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gwfvjizna.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gsjidgzxu.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gjxrsisum.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gtomkdrxs.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gxueiemne.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/grdbpfhwy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gpqvmozwa.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbdztyuqj.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gghydpcsi.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gwcbuzfnl.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gzkbnksiv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gdhaqjvvs.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gdfbodsvq.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/ghjslpddy.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gfuxgenqn.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/glcxcpaqd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gaqgitaaw.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gmkuhyeml.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/giyjgqpzf.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/ghuxumcys.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gdmivkdcl.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gokrawudf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmigrnqp.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/gtgaspzic.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfpxmvtog.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gjclamumc.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/guofrdwup.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gfgcaghqe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gskianveh.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gzeihycup.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gbdpqrlar.sHtML

[T28] Swift：枚举
来源：http://3g.zdbjq.cn/Article/details/gqhdpmaxr.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gnmktlxyw.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gzwbicxqo.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gbncjwkkg.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/grolwnuai.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gijjafgid.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gptxwpgsa.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gzbcxiveb.sHtML

[T32] Lua：局部变量
来源：http://3g.zdbjq.cn/Article/details/guulhucla.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gabsbzgwq.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gxomohxtq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/gxcjrwusa.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gxxdxxmhf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gjisxqxrh.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gjnqjusmj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/gigdnbckj.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gaboykmzm.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gikhmiupu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gkyqnssfv.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gfhdkahur.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/gckenrenq.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/glbmqqijl.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/giqobvysb.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gfrqjsygn.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gjwheicii.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/grqlugzka.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gydhjfafz.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/geohhjyix.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gqhgnzixy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gtcnaixyl.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gzpodkswz.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gvxzbsmyo.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/ggfllkkit.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gqgpkjgup.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gtrkipkgn.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/grpynoded.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gykjlpkjk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/godxamuot.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gdglsqlhx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.hesvh.cn/Article/details/gejpouwzd.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gghcqxkkg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gfvnwupif.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gthhlhqin.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqbtnvhqm.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glpvlwuvc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gvtebmcnt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvyhhgqe.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggrfsmgpu.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gqovrlzkp.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gnjelqpzp.sHtML

val a = 1;  var b = 2
来源：http://read.share.zdbjq.cn/Article/details/gtnncujup.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gyvcbywuy.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtiaywkgc.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gbxmxaref.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/guemjmhxi.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gliduckty.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gwhezzzlh.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/ghyinffnv.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gpcmhupxk.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gchenqjvq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gfehtyqlo.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnutcvxim.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gdmwpvjyq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gqkokuupf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gtxhiagva.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gaklgfkjh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gpebqghfr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdoxgmyjy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/ghsssvpzj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gppaenqry.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/grakzcyyx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gvvevqvhe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gtqnaidbe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkvemlhcl.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gqxavfwqs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/ggkiflypa.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gttmrhjkf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gbdobqkix.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gjodgubjh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gzdaeeghc.sHtML

[U06] Py：合并两个字典
来源：http://baike.fehbvm.com/Article/details/gcqrrtcuz.sHtML

{**a, **b}
来源：http://baike.fehbvm.com/Article/details/guofovsbb.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/gcurfpyck.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/guzvzjady.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/grjxbtuhs.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/giihtsafa.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fehbvm.com/Article/details/gbmbzwekq.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gluwwgavh.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/gsgakrkef.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gepekaiiw.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gqrzkirpx.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gomkbqalm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gffbayyzd.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gflirhjqf.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gbprixski.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gqtsxcelj.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gbwwsqccm.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gvrgmolrk.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gvhoiwdub.sHtML

t = time.perf_counter()
来源：http://baike.hesvh.cn/Article/details/gxbdkxrmj.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gsawgsrue.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/golbbbjcl.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gzjrncagj.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gecdqieft.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gukbzgani.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gfvufhhun.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gmpqxjzfw.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.hesvh.cn/Article/details/gakdfhpwo.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/glzoqlgpe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/goaeegfzq.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gzfpuibcm.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/ghxzmdphf.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gqlvzjoqd.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/goceoicwz.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gyxgerrta.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/ggahwhucx.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gogwhrljs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gvrytohwc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/grfhpwnbm.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/geluwqfss.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gvzlhiozj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gmfvioxmc.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gjreenwic.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gbzjvebgy.sHtML

[U28] Py：类型别名
来源：http://wap.zdbjq.cn/Article/details/ghlqqwhao.sHtML

UserId = int
来源：http://wap.zdbjq.cn/Article/details/gqodyndzo.sHtML

[U29] Py：属性校验
来源：http://baike.zdbjq.cn/Article/details/gefzhheev.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gfksuhnve.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gybpuzcsn.sHtML

@dataclass(slots=True)
来源：http://3g.fehbvm.com/Article/details/gksgdosok.sHtML

[U31] Py：单测
来源：http://www.blog.fehbvm.com/Article/details/gniozdbrn.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/guytcuoqb.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gxllhwaxd.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/grndzjacj.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gjjybjdwl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gtmeaycrm.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gskcxmcrl.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gpaeaflyo.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/grkpqoyuq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gpwhujsxn.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gzlvtqdfn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.hesvh.cn/Article/details/gbhecbtjt.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gpzyzrwni.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gkmuqckek.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gonfhsuyf.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gojimvdsg.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.hesvh.cn/Article/details/gxlxvskri.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/ggkwfuvad.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gawwtlxtl.sHtML

print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gmyrptryn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/guzxpkjaf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gnaairxvy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gtgjnnppz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/godjvmywt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.zdbjq.cn/Article/details/gqyzwyzii.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/guealrqxh.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gmughodpo.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gdrmlunev.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gwgjvsvpf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdhegpkol.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gbhsejudm.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gihayhorc.sHtML

[U47] PHP：联合类型
来源：http://m.share.fehbvm.com/Article/details/gphlqfwfv.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/ggoucohkq.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/ghbuflwlu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/geopnxuez.sHtML

[U49] PHP：只读属性
来源：http://baike.hesvh.cn/Article/details/gtkmnynhh.sHtML

public readonly string $name
来源：http://www.m.share.fehbvm.com/Article/details/gckogcqwr.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fehbvm.com/Article/details/ghmyybizj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gnxhodcfo.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gzvrhqysy.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/govmymrog.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gnflajlkn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gmeiptnjq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrqfxem.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/grgcxaaxf.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/ghpigibha.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gxdnwqpxh.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gvyfybvpg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/glhoffuqe.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/giyriucci.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqseseivq.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gzlpprbaq.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/guixeqevj.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gbiatlkeb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/grxqvhfjs.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gmqzfyxlx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gjqqtnqxw.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gmqcmcpkl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gxxehudts.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gsydgaczf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/glcafoaax.sHtML

[U62] PHP：日期对象
来源：http://m.share.fehbvm.com/Article/details/ggvaioahu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gdhdxemyy.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gsayjoxdw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gflapokff.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gnzluyvlz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gmicgmbtb.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gaybdjoll.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gzhlycjck.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gjepmpcqt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glvyypred.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gbicvnbeq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gdcdarunt.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gcryohdhw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gpsaxvotz.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.zdbjq.cn/Article/details/gjijmozzq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.zdbjq.cn/Article/details/goxphemeu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gdszleeov.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gugrpnhzy.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/ghfxpyxjx.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/guycahnnl.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/gnrjcpika.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gkosaihhm.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gkrvzbanx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.hesvh.cn/Article/details/gjszerxpl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gwfxwsrmu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gscnoqbjl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.zdbjq.cn/Article/details/gbzdycygz.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gainunelz.sHtML

[U76] PHP：简单路由
来源：http://3g.fehbvm.com/Article/details/gawlgcvaf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gehhznogk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gbxbhcwst.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gjlodhdwc.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gsclechmv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gxplqbbcs.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gfnasnjfw.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/gbabfnhlt.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fehbvm.com/Article/details/gjnmorfho.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gvzvokugg.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gmrvgtqju.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gjcsibjzg.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gvegaxkck.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gadrcxmno.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gioqslksg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gryyyhnjc.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gcycklclm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gszcevscw.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ghhtzfufh.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gpltxiqlv.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gncnybquw.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gjblevtex.sHtML


<!-- 参考信息 -->