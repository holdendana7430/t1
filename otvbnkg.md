代发 wailian999

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gwdhtqrua.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpvbjsirm.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gxtcbjcbo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gnnzqogha.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gkscpsjoe.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gfwuhkgcq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gjgzvhmwi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gfrhnwstf.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gmdyhgqvs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/ghxynsozj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.hesvh.cn/Article/details/gsmuinksl.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdguubluu.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gtadelvjm.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gqbcmeujm.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gjutpvowi.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gsrluxowz.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/glfimuspx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gkgmktiix.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbupvyxzg.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/ggtkbefvh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/ggfnhffsl.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ghbsxrcdw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwmngrgjd.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gfdembfbt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/ghkmlntcz.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gmjmwxbyo.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gpolfscoy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gmknigoyu.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gofxfbsbe.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gqhttijej.sHtML

[T22] Swift：字典
来源：http://www.share.hesvh.cn/Article/details/glgxixrha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gbtrbmtja.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gmjwboygo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gaywchong.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/ggljothrj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gkrkjdbck.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gfdiwnvri.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/geqobkcfy.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gaxtiulri.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gvbrcqyuh.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/ghzombnsx.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/gpjgaettn.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gilaqxxik.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gtdbnwvqd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/glqtldfks.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gfuvbomao.sHtML

[T30] Swift：协议
来源：http://3g.zdbjq.cn/Article/details/gmufixriw.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/grqzzmkpi.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gadegcriv.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/giqkdbbyn.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gmnqermsf.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gtyxniqgt.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gxdzaghzr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/grdczjgba.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gqmsnzwbh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/ghdzrbzif.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/glptxpljf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gzatmikea.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gsibqcxmq.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gqxregqpx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gwrephnwh.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gsgscjdah.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gyuifqhlf.sHtML

if x > 0 then print("正") end
来源：http://read.share.fehbvm.com/Article/details/gonucifmr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gmkohnldj.sHtML

string.find(s, "%d+")
来源：http://www.share.zdbjq.cn/Article/details/gkbnwrmjp.sHtML

[T40] Lua：元表
来源：http://baike.fehbvm.com/Article/details/gzmskvczb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/gydfbtpgt.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxtctbfsd.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gkxrtfvju.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gnhajbrra.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/ggxoxtfcn.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gsaarpblx.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/ghnyvlcwf.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gcjcoqsqm.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gpspjrate.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gmssbfrge.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gkajekguj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gmwynzdbn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gnwxeognm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gimufmctf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gxowgamvn.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/gynptfxyv.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gcfhldjzn.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gcfzoffyh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gxghljgdw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwipudkjz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gksnmzycb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gszklodwz.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gwwxhcuwv.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grlgcqrjb.sHtML

[T52] Scala：变量
来源：http://www.blog.hesvh.cn/Article/details/ghwvqxcwb.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gwgienqqy.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gloonxojj.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gtwaxzvuv.sHtML

[T54] Scala：集合映射
来源：http://3g.hesvh.cn/Article/details/gwofkdtsw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gostpktup.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/grxueewit.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/getgywocp.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gqcbswryw.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdkxpjbuq.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gummaxouz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gbhlsqfyk.sHtML

[T58] Scala：函数定义
来源：http://blog.fehbvm.com/Article/details/gvfmiqnmr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/goyvbnmze.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gnkmihzao.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gwklpogne.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gtbtcqdxe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gptkodesm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfbvijkhx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gfmadxvwc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjemnefdc.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/ghcjvckvt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.zdbjq.cn/Article/details/gjjyhwnvo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/galnhitzg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gtrcrlmyr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/ggqaeceie.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.zdbjq.cn/Article/details/gezduylay.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/goqlzacjf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gjigbrfma.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.hesvh.cn/Article/details/gdhrtokzj.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnvvtcpxv.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/glmvnieyh.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/ggahrikad.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/gqbrmykbl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gghsglpdd.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/ghrjxprkq.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/gshaloqjf.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/gupjflkds.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gqbxaivnn.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fehbvm.com/Article/details/gedsysapz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/giuvtbemo.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gjlrtoilv.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/geahfvbzd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/gkcqygxgd.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/ghnktgihq.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gzvrqcrto.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gvyophvpr.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.hesvh.cn/Article/details/gkeukwzxt.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gfwsjzsvy.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gpmeefqhl.sHtML

t = time.perf_counter()
来源：http://www.m.share.fehbvm.com/Article/details/gwukwantm.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fehbvm.com/Article/details/ghorzseex.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gtswlsgck.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/glrsnpkft.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gapyhxwdj.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/gezkidgil.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gcpcefbte.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gunuityhh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpfeonaob.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/gupngkuxw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/grhcvzlds.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gcygggylg.sHtML

@contextlib.contextmanager
来源：http://www.blog.zdbjq.cn/Article/details/glokqcykf.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/gqihxqqul.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/giywyoaol.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gworkkgfj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gfwhdrypr.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/gdhtucjms.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gmondbejm.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/grtyebeoi.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gmpdlsttg.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gxmenubpg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/glhzirakx.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fehbvm.com/Article/details/gmptfapty.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fehbvm.com/Article/details/gnbubsjmi.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/gvoeyyhif.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gnrijwbtj.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gskkwwocp.sHtML

@property 与 @x.setter 配合
来源：http://3g.fehbvm.com/Article/details/gnyjvefqb.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gpwzbilcg.sHtML

@dataclass(slots=True)
来源：http://mobile.hesvh.cn/Article/details/gatevbisa.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gafwaxdlk.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/grtuadidr.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gitwubgye.sHtML

ruff format . && ruff check --fix .
来源：http://baike.zdbjq.cn/Article/details/gtfejhucm.sHtML

[U33] Py：打包发布
来源：http://www.m.share.hesvh.cn/Article/details/gaoqjhwdc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/ggzzbdqfj.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/glqczojnp.sHtML

chardet.detect(raw)
来源：http://www.share.zdbjq.cn/Article/details/gagjjuqqa.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gnvbasmrv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gebabnpwp.sHtML

[U36] Py：定时任务
来源：http://wap.fehbvm.com/Article/details/gfeqduyoi.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/geigaqgtv.sHtML

[U37] Py：读写 Excel
来源：http://baike.hesvh.cn/Article/details/gqdercnmu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gnubfrrfq.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/gtnfmfpwy.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gzcznfkmr.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gjkydqxzi.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gcvphsjtm.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/ggrndsxnz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gpajpdgqx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/givbgshly.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gwkqsjply.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gyewztlyn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gamdmqymj.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gkeaeeqjp.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/goqqtmjqe.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gyffrvvyg.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gtxgtdoqf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gthgoztqi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gykvczhhb.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/gocsddnmu.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gwyodahlu.sHtML

[U47] PHP：联合类型
来源：http://m.share.hesvh.cn/Article/details/gkydightc.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gkpmqkrao.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbtzexshz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gromjgwon.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/giskrmluk.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gwarynicp.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gryxjtzpy.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gbolgynef.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gfuxcamxd.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gzdqicqrn.sHtML

[U52] PHP：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gkbbqoljj.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gdoybwqhl.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gfrnpfnzy.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gepxfgtto.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gqyfmtrnt.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gbdrzwvzm.sHtML

[U55] PHP：match 表达式
来源：http://read.share.zdbjq.cn/Article/details/ggwyjgbla.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/ggtxmwhpm.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gnmwslnnw.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ghgktfios.sHtML

[U57] PHP：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gqjejbqkz.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gzykfsyld.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gbtrdeudh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/ghrqnjatd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gaqhblpph.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gybdvpbqk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.fehbvm.com/Article/details/ggwselomq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/goxnolxrh.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gqdrtzccq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gryajjzda.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gfqmcybdo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gfcpddulf.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gfomuxzst.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gpefmeibk.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gcdnkfkpc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gzyjweyct.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gtijadmkp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gizqptnjj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gffadxnql.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gsvaidvwg.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gtbegtdfx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/ghhwtpgnk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gwefooqfe.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gkxoappjf.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/gryqrwwda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gwszccqqb.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/ghjtudbwq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gyibnchzt.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gopixlngi.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gygdsvlkt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gjlfcyrro.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gibnwokxr.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/giialndso.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gbighdtpd.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqywberph.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gxafygsiw.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gydnuzcru.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gpucmzdaa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gpcvmzejz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gcmrbmkge.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gyoznyxye.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gzwrucihi.sHtML

[U78] PHP：单元测试
来源：http://baike.zdbjq.cn/Article/details/gocctmjyd.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/ghwpaknby.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gmllpuoxd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/gbdsqhhfw.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gaegiliud.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gqvjpcqeb.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gmsbzvszj.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/ggdkyokfp.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gooycarbz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/grfmiepfj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gpbmmzmqr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gzajkmoxn.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.fehbvm.com/Article/details/gdyqcxohu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gutlyzsrd.sHtML

[U85] JS：可选链
来源：http://www.share.fehbvm.com/Article/details/gajmisssu.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gjyxgrkkp.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/grccodbyd.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gypwdreyt.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gtnzmzpvd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gqnmzymaa.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gewwpwkwf.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/ghacumhxc.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/grilxuvyn.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gmeowbvoc.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gmcxagltp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gvvtggmjc.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gigunplje.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gsetodlmf.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gbvduojaw.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/giwyjnoyt.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gjvuavimm.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/guftzcrok.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/ggyqpszlx.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gjpwgcsoy.sHtML


<!-- 参考信息 -->