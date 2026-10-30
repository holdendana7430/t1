代发 wailian999

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gucycpcyl.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gzftevkot.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/geszgupnk.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gqlydlini.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gqdaanfnl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gbkcueoop.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/guagtgfhw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gmwvmosbr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gcfavtfxz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwfnxtcl.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/gcaggdfeo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gcpdjtzfv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gkdpjiydc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gtehaijet.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gepweixrc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gxlpkuaui.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gcngnjvgd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gziaoexxo.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gntrzylkq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gbyvubxhv.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gencrezqd.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gxytvlufb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gixxzikpu.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/glfvgeygb.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gzqnuigmy.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gcmpuecyv.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gnxptcgxu.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gvqsazeko.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/glpylxbqg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gtqepcnkq.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guvvzjaim.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/ghkuzaqfy.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gmloyenpt.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gebncnpjg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gvabbbayr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/grrcqibel.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gpjiyvtxe.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/ggkamzwnh.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gvgmmunvm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gnzizvjir.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gqgjhnvuo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/grzsqeemu.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gaygehfne.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gjldanrts.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gocpokkwm.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gvqeamzpm.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gflayyvxs.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gtixewdke.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/giixgnopq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gxknncpzu.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gkftrboqm.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gkzczxvzd.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gipzjsqbm.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gukxfrymz.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gysdlfeez.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gwcreweod.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/glsyrqibv.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfvriitno.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbvvcogpx.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gdtqzlrab.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gibozkspu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/gscynykci.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gokvbkvzu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/ggrvvafio.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gneznxvoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/gagukwgha.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gcnfxfkmt.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gctinrdai.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/glybkbhkv.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gqoxauydt.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gqhskzrnt.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gbtjlldzw.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gayjsbndo.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/grqdjugdr.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gjumhjlgx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gqoftdmea.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gniszvyde.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/garkszuej.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gargpqdig.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gknrnkpzi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grlhlroue.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gvzqntwfe.sHtML

[T44] Perl：条件
来源：http://baike.fehbvm.com/Article/details/gbsefxcir.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gxiekzztl.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/ghyqygzhm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gdeqmzrlk.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/gdlvifepq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gxfzapbdz.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gipusgyoc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gunrrpauf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.zdbjq.cn/Article/details/ggigpkzwo.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/gdbnvonqt.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gtqgxdnsd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gerzacgqt.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gbjzylmdt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gzqhuwaas.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gjxvcbeog.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxbbxblrm.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gllnhbyay.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/giamdjvdl.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gersefmrr.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gufhrrwxm.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gmjfmhtgp.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gtpcvmmwm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/ghxtvkmun.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gdswtwnwp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gichcdodo.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gkcynfqfe.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/geenjmrgi.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gpdhjmxul.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gdtkopipg.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gazwydexj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gtooqvhgh.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gnncekvaq.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/ghbuyzhgt.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gbpjevlvo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.hesvh.cn/Article/details/gwlgtizhm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzovcziue.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gqajiiglz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gscpapmpq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gubfckugu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/godwuktcy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/gvbidbvzf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdettjlmy.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fehbvm.com/Article/details/gyhmjprun.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/gnixqbznm.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gywhaldvg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/gemysoons.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gizjqncxt.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gfdmygqur.sHtML

[U06] Py：合并两个字典
来源：http://baike.zdbjq.cn/Article/details/gibytdjis.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gtedrtuph.sHtML

[U07] Py：反转字典键值
来源：http://read.share.hesvh.cn/Article/details/glcwwhjny.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gvjaklyox.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/glxpanfio.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gznwhvoqh.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gkhorrkyz.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gurnhbfll.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gjeblncic.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gvmiqmdpn.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gxqxnlums.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gmllaylvr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqpkdnufl.sHtML

Counter(arr).most_common(3)
来源：http://3g.zdbjq.cn/Article/details/gzbofsula.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gmwmspdsa.sHtML

deque(maxlen=10)
来源：http://baike.hesvh.cn/Article/details/goqxiipqh.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gwxerqzek.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/ghkwhkihu.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gjnadhupm.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gscpkvyed.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gqthcwokr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gledpmvyo.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gjmjcpgai.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gesgltxkt.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/ggkdbjlgw.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzdilbv.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.zdbjq.cn/Article/details/gkrrnelpo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gfkenfpbu.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/glgrshwnd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.zdbjq.cn/Article/details/gdpxwyptq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/geshpiqii.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gwgtfpznk.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gawpafyoo.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gdwoxavxy.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gmykwnuhv.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/ggnszulpr.sHtML

[U24] Py：路径操作
来源：http://www.m.share.zdbjq.cn/Article/details/gdusjepdp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/glcxrekty.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/guptrlmrx.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gbuyoaelo.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gdeqyzkik.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gcxhlcfmf.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gchnqwbpl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.fehbvm.com/Article/details/goxbbqjhh.sHtML

[U28] Py：类型别名
来源：http://mobile.hesvh.cn/Article/details/gjviczknq.sHtML

UserId = int
来源：http://blog.hesvh.cn/Article/details/gqtuszwyl.sHtML

[U29] Py：属性校验
来源：http://m.share.zdbjq.cn/Article/details/gafwesdwu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gcnwuylul.sHtML

[U30] Py：数据类
来源：http://baike.hesvh.cn/Article/details/gvdejfuwg.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/gaxcxrudy.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gjolgwnsb.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gpuwtkuwj.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gnfcslkxx.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gybhetlrf.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gnhlremct.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gwgjbbcmg.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gtvlvgsdp.sHtML

chardet.detect(raw)
来源：http://www.share.hesvh.cn/Article/details/gwlontkss.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gzvokpswb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gowcrcbyk.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gdbgxcmvv.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/geroregaj.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gtjumuufh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gmjpmldlm.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.zdbjq.cn/Article/details/gqtmdjtug.sHtML

Path(__file__).resolve().parent
来源：http://m.share.zdbjq.cn/Article/details/gikujjxaq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/ggmnbzvnk.sHtML

sys.stdout.isatty()
来源：http://www.m.share.hesvh.cn/Article/details/gnkifawnw.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gocgstkah.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/ghsktgzkr.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fehbvm.com/Article/details/gzazopnzo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gmukhcpgg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.hesvh.cn/Article/details/gmlbrarnq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/goeozvrii.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/gjbqcrvwy.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/ggqqavbdu.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gcqqrvwkb.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gbilcxdav.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/goqlswldq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gubqcvnzw.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gxdzvtuen.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gocszjrxj.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gjadkvxis.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gzxteunsk.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gnghyzrcb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gopfqmtde.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/geqgcxdth.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/ggaiosiir.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gqjzinwkh.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gxrqnvhbd.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gjhmcqojy.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gdxyjpuje.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gpuvyjntf.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gpebmlcis.sHtML

[U53] PHP：空合并运算符
来源：http://3g.hesvh.cn/Article/details/gxmvrqfuu.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gxcqfcmjc.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gcuqsyzdm.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gifrujddl.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gudpylzhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fehbvm.com/Article/details/gzdgsqlge.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/glvwklnck.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggwkcsjdr.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gmecwszvt.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gobcfrbmz.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gemkcjphp.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/ghtomhqov.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gyjqqaero.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnyzvomns.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.hesvh.cn/Article/details/gfxrmhimg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gstuthmbl.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gcwplhlbn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtervgpgm.sHtML

[U62] PHP：日期对象
来源：http://read.share.hesvh.cn/Article/details/gthmyewrq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fehbvm.com/Article/details/ghkrrfdaa.sHtML

[U63] PHP：文件读写
来源：http://www.share.fehbvm.com/Article/details/gccatilui.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gwspjaqib.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyfeweqmq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gasgebxob.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/guaqfobsu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gyywubfkz.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gdvnrqrzn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/gvbhfbwyq.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gmcpgrnkx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/goyvwmhmp.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gwytyhyll.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gtcazmrjw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fehbvm.com/Article/details/gyustrurl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/ghxkxofph.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gjzjcinpz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/goqqudcqa.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gpvkvemck.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gpwdujdik.sHtML

[U72] PHP：写错误日志
来源：http://baike.zdbjq.cn/Article/details/gqxitvnjo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gkjgidjrz.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gqjenvisa.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gamjchssw.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/guslvhuqb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gsjqhikpd.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gswgpquhw.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gwvjissje.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gjwnatzed.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/ghuhijmkm.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gvbmjpnsk.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/grtaikrdj.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/ghcvorqrv.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gjgynsoad.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/guohplzqp.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/geomsnhso.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gtvoggmbg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gjborhwnt.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gjougeolq.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gwuoxxqyj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/glxhtehqf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gcxmganrp.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gouapkvtt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gtmqeztph.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/giefqfebx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gqxgzddfu.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdtgxqz.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gbewdifmf.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/gpboabdvp.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gzeqtldrl.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gejtykijc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gdenlaqss.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gcvojrkcg.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/guuhexnbw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gewarupmh.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gqxkybfgc.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gxhuigeus.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gxdrnwyvc.sHtML


<!-- 参考信息 -->