代发 wailian999

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gqmrthdyw.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gekzujhha.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gzxuwzlmw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gncunypys.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/ghxpxpduf.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gzsmxztwy.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gnktaayan.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gdnrvuikk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gojdqbbpo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gpktdsudv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/ghdztgsge.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gunqjlytw.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gmdbbkeye.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ggavkwgop.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gcwrmkpor.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gjveihufa.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gpaghzagh.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gkvsckwrj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/glqrybbec.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gkfezwsmd.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gipgxmrrz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gdnqyyctn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gvnclsebl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxeynwkqe.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gyraniadm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gihjagtvx.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gzsjwucak.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gqvzdtlnr.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gektmzmim.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gzignuegh.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcisjrcom.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/govolgknl.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gzaenmutm.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/ghxdaplqb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/garmquumd.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gxpigjqcq.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gjgwdyxkr.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gxscjislh.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gjjohfxgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gollpasfj.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/giuqzvutq.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gyiiyzcmn.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gfphpgpjp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gmrhbpnmf.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gyzlegcqj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gguyautgw.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gpyvpwhju.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gisdozikd.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gahjnrlvm.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gqxoymerg.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/guxpuaxyg.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gqruzggom.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gbdublfvu.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/ghvconcyt.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/guhbaqbgv.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/giefznwaw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gmtjqhobw.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gdoxythin.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gvpfricut.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gqghhqjth.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gblydobkr.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gsolnakgn.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gfxkxmmop.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnjocrzyp.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gpkzvvlbf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fehbvm.com/Article/details/glvdnvnby.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/gqwstmhos.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gysavvlxi.sHtML

[T35] Lua：字典表
来源：http://baike.fehbvm.com/Article/details/gwwvfffmt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gaylplxja.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkzizfx.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gjvdhhuxb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gpldwpfqo.sHtML

"a" .. "b"
来源：http://www.share.fehbvm.com/Article/details/gnifrcdwq.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gdcmhlhsa.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gaqjzsnel.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gturaxpsn.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gyzwdooez.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/giqslndxf.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gfpxsapiz.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gkfztosjp.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gacnhybto.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gkvwezqgm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gjuqkaklp.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtphweywr.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gwcjvfqsl.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gcjlossty.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeqtepef.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gunfxmdpl.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gsrowtrcl.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gapstmhta.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fehbvm.com/Article/details/gafujvgyp.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gfyzdxvsf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gynnpplkr.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/ggwodxuan.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gkufrapik.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmecmcmef.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpcestjci.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjxojrije.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.hesvh.cn/Article/details/ghfknljnj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gxrmkzghu.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gsrtrkzjb.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ggsbaisyv.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/glfqsyzvz.sHtML

val a = 1;  var b = 2
来源：http://m.share.hesvh.cn/Article/details/gikthtmgy.sHtML

[T53] Scala：字符串插值
来源：http://baike.hesvh.cn/Article/details/gcjrnmogw.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gvicmfnad.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/glkosxtco.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fehbvm.com/Article/details/gwfymgnyc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gqwwltxtq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fehbvm.com/Article/details/gthlgocxu.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gcgxgxhdw.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gfwwjcpce.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/glrdcjakl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.hesvh.cn/Article/details/gjouewdnn.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gnrkcmhzd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gyehklpuz.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gfjyrqhwo.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gcnlewkgy.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gfdfxxyst.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/geurehqqx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvagcfzan.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/gespnmzig.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghvbwtcfc.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.fehbvm.com/Article/details/gpujasvae.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/gmssmryxl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gtfajrqdw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.zdbjq.cn/Article/details/gsydqlhvf.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gdvfesqlc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/geikhmpxg.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gjfvbrwsp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/ggzwlssvt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gnawgktkn.sHtML

list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gvdgsmzwy.sHtML

[U06] Py：合并两个字典
来源：http://blog.zdbjq.cn/Article/details/gytadvgku.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gtrqflvzb.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/gfualsixj.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.zdbjq.cn/Article/details/gppxqlmtw.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gziaudznq.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gcbwidsag.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gcqhyyafh.sHtML

max(d, key=d.get)
来源：http://www.share.fehbvm.com/Article/details/gmfjypcoy.sHtML

[U10] Py：按值排序字典
来源：http://wap.fehbvm.com/Article/details/gubxtodbl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.hesvh.cn/Article/details/gmruhkrsl.sHtML

[U11] Py：生成器表达式
来源：http://m.share.zdbjq.cn/Article/details/gswmahcff.sHtML

(x * 2 for x in arr)
来源：http://mobile.zdbjq.cn/Article/details/ggjpvkdgm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/gibhtdcbq.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gnfsriogv.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.zdbjq.cn/Article/details/garzmimsl.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gwtsrslao.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gkzqvlfhx.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gpcohpvlv.sHtML

[U15] Py：高精度计时
来源：http://mobile.zdbjq.cn/Article/details/gqpowwiyh.sHtML

t = time.perf_counter()
来源：http://www.share.zdbjq.cn/Article/details/gqwdnopjs.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.fehbvm.com/Article/details/gkunhzxgt.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.hesvh.cn/Article/details/gfspctbbc.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gjupmyrcy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gcpsnzpcl.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gmnbkbiwl.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gnqmjnbbr.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.hesvh.cn/Article/details/goowolfiu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gehxkefdd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fehbvm.com/Article/details/gsykbtzul.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwljbasx.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.zdbjq.cn/Article/details/gjeqenubc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gegefrlmm.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/goaddikze.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gipydjcbe.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gbmwklxfl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/giutxxbqm.sHtML

[U24] Py：路径操作
来源：http://read.share.zdbjq.cn/Article/details/gvtafzvge.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gzbylvsvj.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/gljuncise.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gdiaxiyho.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/giwzthfbx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gdaxerdck.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.fehbvm.com/Article/details/gxdgybjen.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/ghucmuyst.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gxzgrebqj.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gqkecstdd.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gbjncahne.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gykrnyfob.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gdyibftii.sHtML

@dataclass(slots=True)
来源：http://3g.zdbjq.cn/Article/details/gljeepyjb.sHtML

[U31] Py：单测
来源：http://blog.zdbjq.cn/Article/details/gbdhwcncq.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gogllccou.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gvkteylco.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/grjkdcule.sHtML

[U33] Py：打包发布
来源：http://3g.hesvh.cn/Article/details/griefoqer.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.hesvh.cn/Article/details/gcfpihxdc.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gbzkudwhe.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/ggdcugozi.sHtML

[U35] Py：发送邮件
来源：http://mobile.fehbvm.com/Article/details/gubluepap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gjhdxfagw.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gaopyhulh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gfbcddkrj.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gctnlomxo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gdkknowuq.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.zdbjq.cn/Article/details/gbdpeagam.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gfrmsagqp.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gkdytagkl.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/grdzxfcht.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gtlxxlyjr.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gvevazdhe.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/gapyygbnm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gldoeqyib.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gpqyixbue.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gpeddomep.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gochvqpyf.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gnbgmjohu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gydlmzxyr.sHtML

declare(strict_types=1);
来源：http://www.share.fehbvm.com/Article/details/ghyofbxfs.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/gldxgtziv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gkqkqyyuj.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/gzrkceevx.sHtML

?string $name = null
来源：http://www.m.share.zdbjq.cn/Article/details/gigpzydzz.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gsvqgkvyw.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/glxtrovsm.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/ggkehvwzw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gvkvlvmzv.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/ggigqxord.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gxdtmmfzi.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gkyzbonpu.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/gcxlshmib.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gdfaozkjx.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/garllrtko.sHtML

[U52] PHP：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gzyohronb.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.hesvh.cn/Article/details/gibuubiel.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fehbvm.com/Article/details/gtbacuezy.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gboqmtajq.sHtML

[U54] PHP：空安全调用
来源：http://3g.hesvh.cn/Article/details/gtcneapyf.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gpyziwzko.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.hesvh.cn/Article/details/gsrztijbm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gpboqhedf.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gmknbgjup.sHtML

f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gaczbwxvz.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gswkomatl.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/ghziybnlf.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/glozirckg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/gyzlusmev.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gqvynuvzy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gedmosijc.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/gfdkmmzit.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.hesvh.cn/Article/details/ghfpgqrrm.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gqealvkxi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/godfulcbq.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gyfudvccl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/glrnpnvex.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gmggcyovi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gtriuaiuo.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/gzldntshf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gwmtnbdrs.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gnopxlkpi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gkaisxzhm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/grwtvahlu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/geruvbzch.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gqhtwvmjc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gxxjvmpny.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/glhdnufxo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gjcjiewnt.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gcpuqmnql.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gpymxlpeh.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/greoiwovi.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/goxkwqdmd.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gftweihyw.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gtefkevmw.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/gwrwxozjb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.zdbjq.cn/Article/details/gfoohvmaj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fehbvm.com/Article/details/gmczrqwlj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gkguztsko.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/goabltwqw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gyuvqwzdv.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gxmrkznaf.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gtdurcrie.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gmtyopqtg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gisejafnh.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/glglvxoor.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gudaqqfxk.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gsbznvhzb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gparpluwj.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/gdagnmone.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/ghpbqkofi.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gpahuuogl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fehbvm.com/Article/details/gjmvqcrrq.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/geihwazwq.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/grvhrhfeu.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gniupvtbv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gdlvsdxit.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/gpykcxmqo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gowiolqdo.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fehbvm.com/Article/details/gkociaenm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gbylvwzcs.sHtML

[U85] JS：可选链
来源：http://m.share.hesvh.cn/Article/details/gvjbuvaqj.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gsovtnbuk.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gsgtdwnzv.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gqtdknxyq.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gmnzkxncn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gmusxyrav.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gcadskgaq.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/guycsyieb.sHtML


<!-- 参考信息 -->