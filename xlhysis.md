代发 wailian999

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gtudymgcn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gpbbuijyq.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gcbanxlha.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/ggrnbfsay.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gpqmzzfkd.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gtdaaspoi.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gclhkgztx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gxxgwvqlq.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gchrjziei.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gciluyiwd.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gojhsvuhp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gmzmeehpb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/giruxxcrq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gzbyvqxue.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gebolcpvs.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gepdqccqm.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/garhsumgc.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gqoefhtkv.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gyogmgsjq.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxhdwlcpx.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gvbzbvgyp.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gvmbabmmt.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gobvlnela.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/grudfvipb.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gtgkbrgkm.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/guicnagyb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gqccnvijm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/glotycczx.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/grdtmdqyo.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gfqtpqply.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gnbrnqkat.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gbhztpvnn.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gtnpofznd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/glawzstnp.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gtslfcwfw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gskwgrqfg.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gmyhouipo.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/gqnrrzfss.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/ghqfinkgi.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/gvxqfbxbk.sHtML

[T27] Swift：错误处理
来源：http://read.share.hesvh.cn/Article/details/gqbewdwsc.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gamalhkap.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gsgptakns.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/grrhguifd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gvpgenlqq.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gyscrigxt.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gatgrdktp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gzniulfbm.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gcbfvptix.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gyhictfzj.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gaeleqgdo.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gutwhsyzc.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gbwtmyexr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fehbvm.com/Article/details/gapslrniq.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gncnxejad.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.hesvh.cn/Article/details/giafezmbp.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gaytyibiu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gxyfcjqsm.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gqiuxcidv.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gvlnznwma.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gbttzdxdf.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/ggngtgzwm.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gsbkdsqmk.sHtML

if x > 0 then print("正") end
来源：http://wap.zdbjq.cn/Article/details/gdymavtdl.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/ghohzwcuf.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gkpwlhqsa.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gctjyhduf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gvzovnmlh.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gphyuqwkf.sHtML

print "Hello\n";
来源：http://mobile.fehbvm.com/Article/details/gdjtyqvyr.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gntlmnlwx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gtuvjodum.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gmkquvscn.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/glnrkoyal.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyjetdljb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gztkdpkss.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfahtgsec.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.zdbjq.cn/Article/details/gxlwimump.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gunevddta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/guoxoqhuz.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gehvyjunf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gzhuhhpaw.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gugzzbwir.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gyjtvofdm.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gxzwrlusk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gzzqiwodp.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/grufhbmsz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gizexqzsb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gydcovgln.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwxweejdw.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gpzgwsmpp.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkvjkmtiv.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gebfcyqgn.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gkkobewwp.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ghmbivaea.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gxisqeosh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/giwhmuzhl.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gpwgiolcp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/ghpaytcks.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/gcpizfmoa.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/gvwoirvrt.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/grcghlawr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gpahnzqmx.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gjjetadti.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gjdzrnbfe.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gclxrrtaf.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqopvqpmw.sHtML

[T60] Scala：折叠
来源：http://3g.zdbjq.cn/Article/details/gczkcyqna.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gegrrwnuu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gixefmrqm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gfqpreifx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbslzkoau.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.zdbjq.cn/Article/details/gpjejsros.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gsjmckidi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gajlwmsjb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gahinyndt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gfrtpakgr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/guymepqzg.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gqfgfugod.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gzsebugml.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fehbvm.com/Article/details/gmjghvcgh.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gbviejnib.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/ghzovzits.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gesuqhfia.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/geibplvsv.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gjgrqhxff.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gbweumavx.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gnzpmubjf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gadediiwv.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/gweeyrpdr.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gmzjrmqwy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gpziscrpz.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gjgepmrsm.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/goxlqfhpl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtqutjjef.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gchnygtuc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gkvuwhysh.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/genunjvys.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/gtcioddkq.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gfmsnjccq.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gkgvnthfq.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/giyuyecjr.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.fehbvm.com/Article/details/ghzwtjilo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/girromoeu.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gawyvwzac.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gcejgsqat.sHtML

[U18] Py：预编译正则
来源：http://read.share.zdbjq.cn/Article/details/ggrfnibjd.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gmcnffcuj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/gfawalimy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.hesvh.cn/Article/details/glvxubyab.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gxjchawxk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.zdbjq.cn/Article/details/gqomgolcy.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gunuwmfbw.sHtML

@contextlib.contextmanager
来源：http://read.share.fehbvm.com/Article/details/gcixhxvca.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gkgafduoh.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gulmjmcgx.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gjdbqfyke.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gjzsdtnnj.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gedulawjp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gtougyjvl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gtjcurrwj.sHtML

csv.DictReader(f)
来源：http://www.share.hesvh.cn/Article/details/gqcmbitvk.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fehbvm.com/Article/details/gjkguabby.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gmhpnxjrt.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gqgxigkqp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gozeywfge.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gjmmrmfxv.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gyiaaygoj.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gnepgebjg.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/ghnqmdguj.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gbswarwjz.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gqcojsbgf.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gwnjxqddp.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gcntpqalw.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gexrgtmbn.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/glslykgfj.sHtML

[U33] Py：打包发布
来源：http://mobile.zdbjq.cn/Article/details/grcncokwo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/ggsuypafa.sHtML

[U34] Py：判断编码
来源：http://mobile.hesvh.cn/Article/details/gjilfyanq.sHtML

chardet.detect(raw)
来源：http://read.share.zdbjq.cn/Article/details/glnivqmfx.sHtML

[U35] Py：发送邮件
来源：http://3g.fehbvm.com/Article/details/gfitveppb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gkpfdoqmu.sHtML

[U36] Py：定时任务
来源：http://www.share.zdbjq.cn/Article/details/gzrotoyjk.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gupcjzdvc.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gtslfrcdk.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gvaihxvvt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gdbdntogw.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gmmqulzkg.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gqacelflg.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gmqvchaob.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.fehbvm.com/Article/details/ghkirzruo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gylegqhvq.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.zdbjq.cn/Article/details/gauhjzkwq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/ghtqrufvo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.zdbjq.cn/Article/details/gireneows.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/guxdwwzsp.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/ghmyxqqpn.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gpxuskydb.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gvewnkfbg.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gycewhvvu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.zdbjq.cn/Article/details/gajbzlxoy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glnbigmii.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gzwoddisc.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gyzhuigzd.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gjfihxvex.sHtML

int|string $id
来源：http://m.share.zdbjq.cn/Article/details/gfyblcbym.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gzuylcear.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/giqhtaizm.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gxbryshvr.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gexfpmyyu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/glavrffpd.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/goacfhsrf.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ggrdxpcbg.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gshutvdmd.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gnawtvlrh.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gbtnfakih.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gvdmojicp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gfkbeproi.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/glpbptpux.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gllfvrgum.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/ggayemblw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gxgiyxdhi.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gskmuoyrg.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gneqmcaza.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gnudrmwbn.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gbfhwryto.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gdkvwtegl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gqtyysysk.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gpbqeohqm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gijdemura.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.zdbjq.cn/Article/details/gcndpmwxy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gwlyyhvdc.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gtjpddsfb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/goqtllkol.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gbcuysxxi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.zdbjq.cn/Article/details/gqegcojqq.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/giuypzyfm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gkfewnzcp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/guinlmovy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gflzdeyqg.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gmertuorc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gixuplpmg.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/ggvzxwndr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gjfqafznb.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/gdmfgrwco.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gsnktykjg.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gcxyacuyj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gnzkocggk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gxdkcvyfg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gyrijczac.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/ghudjcelf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gsfhtxzya.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gmmcexvzq.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gjfnjfqxh.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/ghggwanir.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gkzyjmqgk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/glpopkpww.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gwzpskxod.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gezgvkmvs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gxabajvzq.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gmjxfsxrh.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gehjpjkwo.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/glxyygaay.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gazngifdq.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gwfnljopx.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gkyjzkgdy.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gxhdrlbkm.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gdtktfecj.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gxibfyxbe.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gckoakexd.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gadjsgqpm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gzbydiswl.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gpmoxbqzg.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gktybpgeh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/guzobwmlo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gfccmtpvt.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gdiityyip.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gaiqtxcdt.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gnpcjcons.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gdizbzdqr.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gdibyerdz.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/gniyttqok.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gvwrwbbbh.sHtML

a ?? b
来源：http://wap.hesvh.cn/Article/details/glagthada.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gxcjsctla.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/grdgsddxx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gvwhtxizz.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gkwyvthvy.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gljksbkhm.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/ggcoosbzu.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gpildlcfa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/goigyfsnt.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.zdbjq.cn/Article/details/gopzcgnge.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/grvsfsnsy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gkpzhqrfw.sHtML

structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gixodjrjh.sHtML

[U93] JS：模板字符串
来源：http://read.share.zdbjq.cn/Article/details/gxovfilfs.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gczyalhzq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gepunivfd.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gwrenwamp.sHtML


<!-- 参考信息 -->