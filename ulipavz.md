代发 wailian999

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gdnvvhqyi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gycmxwjgi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxrzmki.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqxkgxjcl.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gumlzeenf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ghicngjrt.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/givwrthps.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gntvrooeo.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gueklthie.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gxckqduks.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gwolsytvi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gycgoidec.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gkxlvycel.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gvqutspwo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gcaakhfrk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gjygqchdw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/ggfbobjyy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gkcuhwasd.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gjkjgrmtx.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/ghwtwxevx.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gmwuhnamj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gcedsldgr.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvqhujqnv.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gzmwadlya.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gnwhkrejr.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gyxyecaul.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gknoqujmy.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gtrvrzqzd.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gnlgbiyso.sHtML

if let n = opt { print(n) }
来源：http://www.share.hesvh.cn/Article/details/gvgkqswat.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gvcowzwst.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gfwarenib.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gqkkbxcof.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gxslpvmvz.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gdrvykvex.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gcyxfopei.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/ggauppiuh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gfyzxdwzb.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gmylykjok.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gnfunfhfr.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/glcytaazh.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gkobwgrel.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gwxgdzcsh.sHtML

class A: Base { override func f() {} }
来源：http://3g.hesvh.cn/Article/details/geelpbttb.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjgtiecxe.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gxhuooyop.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gojegckpx.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/grtkdfbev.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gcvgijqbb.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gbjtalllj.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gzhwljqhs.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gcshcdacw.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaceijrgx.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/ggzjkextm.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gnncxxkyd.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/givxnehza.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gzndloern.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gvhwjgnzl.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/ggyetyqtd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gmvxywupz.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gbizzrdof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gyihtlrid.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gcsyhodwf.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/gwkqbqtou.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gcknizemp.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/gglrvyylf.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/ghithaegu.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gcigkshou.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gwulafoky.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gykcotwqj.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/gvovtzeba.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gzqdpksyi.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdnxwapfw.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gsbrmrnwv.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gxioxulte.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gjzhkmiyk.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gutmxlxmw.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gwydqziov.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/grnnbzzlv.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gkuucfvkf.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gxkshivlo.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/guqiuglvz.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gjotpxksh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gndlgflhx.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.zdbjq.cn/Article/details/glrunjops.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gquspxwcs.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gnpgqweko.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gdiqciquc.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gotcqeljd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gxkaubtqy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtppcohgi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gadkppfdi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gsdiiqshv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/grbmncqcz.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gpjzdteob.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/ghwzuvafx.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gskrgzrxs.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gcybxjcud.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gjmvczwxp.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gsuyltvvu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gavkdetfl.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gzjsjoorb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwlteutxr.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/glvufldkw.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gskaxfoyz.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gaqbxkeay.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gipiokeog.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gcuurgjkx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gkdhxpvtn.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gdqpdmpzg.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gxgdynfwk.sHtML

[T60] Scala：折叠
来源：http://baike.hesvh.cn/Article/details/gnuoqyesj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gceuwdfee.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtpnsyawe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gttjfbqji.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghlozvfej.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gvxbzfkzn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gxcgshtan.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gipijkqab.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/gkoyagukt.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gtvzagltl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gwloxbehz.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gmbcluird.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gpangnmvy.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.zdbjq.cn/Article/details/glsrfmwfh.sHtML

list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/glbeddnya.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/ghdvnnklu.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gltxvustf.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fehbvm.com/Article/details/gqtekrwdw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gawwwuorf.sHtML

[U08] Py：展平二维列表
来源：http://3g.hesvh.cn/Article/details/glurpqqfe.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gnxwumzqw.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.zdbjq.cn/Article/details/gskrwffeu.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/gdmqgbeeu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/grlqnjiys.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gisuyddur.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gyamqiscg.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gyrwlkxbc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gsotmdunw.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/gkqcupczt.sHtML

[U13] Py：固定长度队列
来源：http://3g.hesvh.cn/Article/details/glhbslyxo.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gfdataqvm.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gxttswafc.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gqgxphgow.sHtML

[U15] Py：高精度计时
来源：http://baike.hesvh.cn/Article/details/gknewmihc.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gyjoipufd.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/geukyrrrs.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fehbvm.com/Article/details/gdhxzzyrs.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/genvpyqzz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbmpmzih.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gxtfrkmqj.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.fehbvm.com/Article/details/gumlxcgmt.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gmikgnjgk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gqgmxhwfi.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/ggqnctjte.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.fehbvm.com/Article/details/gtapqwylf.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gfkbxenbb.sHtML

@contextlib.contextmanager
来源：http://3g.zdbjq.cn/Article/details/gfmcvahgq.sHtML

[U22] Py：矩阵转置
来源：http://mobile.hesvh.cn/Article/details/gtjbvecte.sHtML

list(zip(*m))
来源：http://www.blog.zdbjq.cn/Article/details/grfzdvedv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/ghhfeojvq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fehbvm.com/Article/details/gggpoybdv.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gqevhailz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gtellxprp.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/gizbptjtg.sHtML

csv.DictReader(f)
来源：http://3g.hesvh.cn/Article/details/gjncqqzmr.sHtML

[U26] Py：并发下载
来源：http://3g.zdbjq.cn/Article/details/gkjbmmhfo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gjpdeymru.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.hesvh.cn/Article/details/gjpqzbvpp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gbzptdzml.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gzrwweivp.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gnnubsfpq.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/grksodqqu.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gtgxkpbfd.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gnxnmmwhy.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gvjkxdgze.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gpxuhhwsk.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/ggxuobhuu.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gvvwnbreh.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/godkevsxi.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gmtnnowvg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gebpirqst.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gzpmwrlnx.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gdkcwnejb.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/ghyzwdyyb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.zdbjq.cn/Article/details/gkruvtltj.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gixfhzist.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gsnebifsy.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gbcytfpkz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gibvurdpr.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/grlzrsuai.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/glmtiddhg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/glqnzkofe.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gfqbkudrt.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gkjayejrv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gtgdzeful.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gqvtyyjvo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.zdbjq.cn/Article/details/grnxxqhyn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/ghrmlddzi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.hesvh.cn/Article/details/gkaqmmyjn.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gnnkpbcew.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gqhbeewxh.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/girxieemo.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/ggfjnpnlv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gjqufvucq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gndharall.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.hesvh.cn/Article/details/gzahxirpu.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gsuyqwnlb.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gudhcadxc.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gvapocgdt.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gcebkiyeo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.fehbvm.com/Article/details/grzvkobsp.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gsrmgmuxx.sHtML

public readonly string $name
来源：http://read.share.hesvh.cn/Article/details/guauddmki.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gitvtwnaf.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gdiqxeahv.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gkoxnebpw.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gisegpsmd.sHtML

[U52] PHP：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gudnzlbax.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/grlsmvdaf.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gskbwhdvl.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gfpzjvmzh.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gmjuhofve.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxrfjrele.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gtbhywvmb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gwfyobibr.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gbfgmnohv.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkxzcorcm.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gtpicgxjg.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gbbigqflm.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/giiqrphbm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gntpawqsp.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gmeajnsrk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gnzlbczrp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/ggqgjmgex.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gdhqsunhk.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gntinlyzt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqwmuzvgx.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gnvbxqagf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gtgaoogeh.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gmbwgfxes.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fehbvm.com/Article/details/gcxsjldez.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gjxfevlbe.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.hesvh.cn/Article/details/gvbsdwvfj.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gvmkbrizt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gmzjednyl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gyoviqxfg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gbhedoish.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gnufsmnrb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/ghcevojbu.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gvndnjblt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/glclfjpbd.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gtvsuobda.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/gzgezdruq.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gjqaffsak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/grrgehyyc.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gegzwjwac.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.hesvh.cn/Article/details/gsbryoeho.sHtML

[U72] PHP：写错误日志
来源：http://blog.fehbvm.com/Article/details/ghsdffanb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gjvbkxoif.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gkmykqklm.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/geuxpvfqs.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gtbihvpye.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/ghyaoswff.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/gfhmqlaqz.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/glrqpiflk.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gavdyaqnc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gcaamugsv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gnpltdyym.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gcrtraazy.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/grgorpfjv.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gkkqxmjzx.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gwmpxpfjh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gerzxawts.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gywaxpolh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gpddirzbt.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gehzjimbl.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gqydkbjdh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gqpbfpiko.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gftrcobya.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gujuejina.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gxugfvcym.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gmsyfnyxo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gcjwguisb.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gisyztfwo.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gczrbdqzf.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/geaklqvhb.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gcgldzzoo.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gfblryzub.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gqvirzeqx.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/goujkkpsu.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gifpybuod.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gyhcowuks.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gvnzlgaxj.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gncwgkdtx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gaipxiwta.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gggwwabjy.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/ggzpequky.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gvinslhfc.sHtML

structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gqhcyrqoy.sHtML


<!-- 参考信息 -->