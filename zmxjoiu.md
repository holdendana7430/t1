代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gbkcyzfwj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/ghickjugi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gxaktgyrh.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gvggxyecf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gvmsvkwxv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/ghgkbgaoe.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/ggknwgzke.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gacsysjtp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gvucpqnzy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/geictwbet.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gwnfqnzou.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/ggujeoswj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gsotzlrhd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gitszcjoy.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gwmrdfedk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gxkkdtghs.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gfzvwmnyw.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gkhymaxey.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gzynaayue.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gyyfnpbxa.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/grjiarysl.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gifxbbaab.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grhgmzpwe.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/ghxonzxjr.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/giwjehnec.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gceyrydhh.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gloehuvqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gyrchjylu.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/ghgglxmtm.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gxflyohlq.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/genwxypra.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gpxdurzps.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gatdcgqke.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gkeaxgmzl.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/goxtodpxj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gvvqznzcv.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gliltkccs.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gljrwuqhk.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gmccbyjog.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gljgcuspk.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjapsib.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gyayigeis.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grfzfianj.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gqfnippvg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gfeylfruz.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gjgmaonzg.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gfyzeiwcd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.zdbjq.cn/Article/details/gstmchfla.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/grsprryzq.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtfobhmhz.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gagroddrs.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gxnybjqge.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gwpwseqjq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/ghhiioryx.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gkgdoiyhh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gsfspwylj.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/geeaomalv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gdymyvyyw.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gfboprhon.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gdslpouaf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gxrssgjxb.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/geczyylsu.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/gxcsicywq.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/ggmbbwcdn.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gehapaadf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgkqbxn.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gpwszojkt.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gjtpywcxm.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gaxxvsefh.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/glhnmxndz.sHtML

[T42] Perl：变量类型
来源：http://wap.zdbjq.cn/Article/details/glqqsynxt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/geouvovgi.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gusanczxy.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gjwxraqok.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gijemkpqt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gczfniefy.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gfgtyvyhl.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gwzvsptwg.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/glqjvwgro.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gvyqiljms.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/ghqlaygxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gxdgajabx.sHtML

[T48] Perl：正则替换
来源：http://blog.fehbvm.com/Article/details/gmexqrjyl.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gcjhyldrp.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gsujizffn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbvnzhnml.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqlogliiw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gjkrynjpc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gsaztjjqf.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gugudlcun.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gxypyqnps.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gfsihhika.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/gmrinikpo.sHtML

[T53] Scala：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzdjdprbz.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gcifsycul.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gioppyovb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.hesvh.cn/Article/details/geacawfxn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gpxzgqmlv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.zdbjq.cn/Article/details/gonvctapn.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/ggsuiyxnl.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gtcpjhnwl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gdttukdgw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/giveiseft.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gpmspmeke.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fehbvm.com/Article/details/gmnknidtz.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gaqgbdqxx.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gndgmdrwg.sHtML

[T60] Scala：折叠
来源：http://blog.fehbvm.com/Article/details/gjjpoivue.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gpoaietyh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmjggpukv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gqyahgezf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcdvdyyed.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gkauoxotf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/genukdjjx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gnwwtxgmf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdmftwbxx.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gsqkwodon.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gaowqeirk.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gaoulsaqs.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.hesvh.cn/Article/details/gffmanztq.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gmsdajlxw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gvdxaymmf.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gcglxjfzk.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gffjugrle.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/glawnbbnf.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gjndwxpmp.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gnvbmvqpq.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gvjxvjyrr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gxlredyqt.sHtML

max(d, key=d.get)
来源：http://blog.hesvh.cn/Article/details/gqeiduprj.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gkszhtoqj.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gqbodywcu.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/gebejwvlo.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gsoiqfivr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/ggonqwbpb.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gghwrilqm.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gugwnirgw.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gcboawxlk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/ghurcmabq.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/glkisyfuo.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gdxyketuy.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gjzncfvth.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gidqbvlhb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gxoijmzaq.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/glnnxyjsq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gzauclwaz.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gnavbafyo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.hesvh.cn/Article/details/gbjsvqpwi.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gwrcqcvxd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.zdbjq.cn/Article/details/gsujapkss.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/grgmqxiji.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gmwectdew.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gyvvmybmq.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gvtsjyrve.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/gbarsdbde.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gpoujpzdp.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gkcbrhhxy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.hesvh.cn/Article/details/gvmddyicw.sHtML

[U24] Py：路径操作
来源：http://m.share.hesvh.cn/Article/details/gdykyzxkh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghrteryky.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gezaaipnp.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gippsrvbh.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gnfprpgay.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gfyvqjlog.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.hesvh.cn/Article/details/gpphhnwcs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gfwtfnyzy.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/gflmoshxe.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/gpbhpzbxh.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gullepize.sHtML

@property 与 @x.setter 配合
来源：http://www.share.zdbjq.cn/Article/details/gevezcxqk.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/gqbajkpik.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/gpnxazfki.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gxzhqbnko.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gxiwgtahd.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gtscabhfv.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gyxjracqh.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gaycikhme.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/gqzcfdjwm.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gioleerlb.sHtML

chardet.detect(raw)
来源：http://www.blog.zdbjq.cn/Article/details/gyturwkpi.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gpozjggwo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gxcogiztx.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gtpjzwkzg.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gcjsuhqsu.sHtML

[U37] Py：读写 Excel
来源：http://mobile.hesvh.cn/Article/details/gckzwdxkg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gmblgrshj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gampttakn.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.zdbjq.cn/Article/details/ghsqevgjw.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gamvhalwr.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/glmvttjqf.sHtML

[U40] Py：打印到标准错误
来源：http://3g.zdbjq.cn/Article/details/gvqpfcbnf.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gepfjkkuo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gpssdzgbu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/gunfgjjpu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gwcbarnxe.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gaasbwhfi.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/goqwitsdh.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gweboepfb.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gfcwcsnml.sHtML

declare(strict_types=1);
来源：http://wap.hesvh.cn/Article/details/giqjorktg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gyhcevnby.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gasusdnos.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gdhlzancr.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gshhzkwba.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gdodpumfz.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/glhnwiqtk.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gzkmbwaxl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gdrayikpi.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gobdhvigg.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gjzpzvulu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/grzrqoeng.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gpippzazj.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gkcvlvphd.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gznjxidcd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gfnvqcogv.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gwheflqtn.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/grvjbgrir.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/gaiiywrrq.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gbysvtmbg.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/grknzbdxa.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/glpehshaz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gwujpwbmz.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gpposrwij.sHtML

f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkqmopkgl.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/glqgipoqo.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/girtfcpat.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gujcgkxvr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gkacwlbca.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/ggdcbachs.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gevedooxf.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gvccjrhpz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gzfglxzrh.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gmakpufdy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gvqchdsal.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/guwtkvlut.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gadlsuspu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gdnbgdkit.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gukneeklh.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gkwhmipzp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/gkxavdukq.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gyrifjzrm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gpololhmk.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gshxgsqqj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gijgkiizy.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gkyihvwwc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gotgmszeb.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/guwcsriwk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgdzntbi.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/guelolyhl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gobfjydpv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.hesvh.cn/Article/details/gtkadypaa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/gfzqstcrf.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gxjvqqgdr.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gerqbergl.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/guedpfnna.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gavohoapd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gkgfqxkig.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gegcmagyq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/guospjrua.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gmsbvmfai.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gpdmfjsse.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gllxxgjbr.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gnxraatuf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gcohshkph.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gdloeowps.sHtML

composer require twig/twig
来源：http://www.share.zdbjq.cn/Article/details/gbdcalauq.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gzbpennoe.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/ggljezsqy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gthoqvdcz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gkngcibmr.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gehworxlb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gkumcdrlb.sHtML

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gqelxlrhy.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gdhzsnbfl.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gzdainyey.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gtnzflirn.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/ggciwwefq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gunwpmqlq.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gnafgbleh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gocpjbita.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gosdpgkpw.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/ghafzpbog.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/ghmjyuavz.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/geltsspyv.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/geyynhcyy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gymncftzd.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/gmozpytjm.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gcpelqqij.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/glnlpfwia.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gacxvxgfs.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/grqppwbqe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gwrwchrev.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gegaxzern.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gyrnxknsn.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gwnafjkvy.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gpwdpelvr.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gaqjonorh.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gqyjdjsnq.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/gbvuuvnli.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/gvqfqojou.sHtML


<!-- 参考信息 -->