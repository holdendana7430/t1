代发 wailian999

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gcvjbyesm.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gqrefoicc.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gjizvbobt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gwwsebwsn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gmhvtxlpg.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmqydgbvh.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/glehkngfg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gzguijoub.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gdikjmckd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gjeemfozd.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gcgauewug.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gryxxxhlk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmmzlsdzd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/gywisdnso.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gjnkcrrok.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/glinbzxgc.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/geknqyrve.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/guoamxhvm.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gepmzrhrc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gyqkugjoz.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwtdylmkg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gzgvfflpx.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gqaqakemg.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gheodurcm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/ggazskpuk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gmtdwfrtj.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gnmorayqx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gjobwprys.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gdyeqsuji.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/gesfloczz.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gpdyzrrpx.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggptqaqym.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/grdwnrltj.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gbieaueyd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/geueanutm.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gpsyjseqd.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gqftvyfrz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcseogdel.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gvfncsuzw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gccnjcjka.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gvaktwjvv.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gjbuqkirw.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gzrmohmmw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gpzfrgdct.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gmjqzlrgl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gnfdthfal.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gpgccehfm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gfhyxptpq.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gjuduudkd.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gyuwynfpo.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gqlbqzhbx.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gsieguemj.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gthezrpvr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gzbtknjjw.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/ggnggjsdb.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gxvbtfysk.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/ggqpglvoi.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gkemcklzy.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/ggkdpvjob.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/gbyegqojl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjczdswkx.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gdjzbpamw.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gfvdgyoik.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gvwqrbkfs.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/gmveaykpa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/gqljpvjng.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/glprnwhei.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gmmeokcss.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/getcrrhns.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gmifviwut.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gvfkrxstj.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gfeiygzcs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gwsionoda.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/gulonxubj.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfehxwpgh.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gjjjadsic.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gxjysutkc.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gxrgemurj.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/ggknyswws.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/giwlholvy.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfzudmtev.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gyfrychfr.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/gjkwcnioy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/geykbikru.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gkfcyeonv.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/gbktqbddy.sHtML

[T44] Perl：条件
来源：http://blog.zdbjq.cn/Article/details/ggwlmzamm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gwwjasxux.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtihemhaz.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gsdxgkles.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gredzjkkf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gxdplwrzz.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gyrfjucqd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gsfjmoswb.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/giqklqyzr.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gqswbbbdu.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gjhxjdbei.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gmihtvwed.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gypeesojk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gorextmnu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gxzzjzndn.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghbjkttlb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gllrazwtm.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gwukqtwes.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gujidmotk.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gssscgoji.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gbneeubih.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/ghfhzzqaz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gmsehwbut.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gunfheqhm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gpcifhhwa.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gaiziwgsj.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gbgrolxuw.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/goniunvdh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/grkwzlssk.sHtML

[T58] Scala：函数定义
来源：http://3g.fehbvm.com/Article/details/gqwndcyyc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/gicoanvbr.sHtML

[T59] Scala：循环
来源：http://m.share.zdbjq.cn/Article/details/gurucdmhl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gpawqqefl.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/glxefsuln.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gridicnke.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdspghdxf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gekweanhm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gquhxdouf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gsykoduvi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/gaccuedte.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.hesvh.cn/Article/details/gcehwibhc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gzosirrhf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/ghcovenxl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.hesvh.cn/Article/details/ghcxgepns.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fehbvm.com/Article/details/ggcehktvn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/ggztjudtd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/ggtvshxqt.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gilhdtjyh.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gktqfxedn.sHtML

{**a, **b}
来源：http://wap.fehbvm.com/Article/details/giolypqrg.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gzlktjlix.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gvbotzukc.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gitbhenlf.sHtML

[y for x in nested for y in x]
来源：http://wap.fehbvm.com/Article/details/gjmuvmuts.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fehbvm.com/Article/details/gxgqjvcch.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ghelouqfc.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gqbmnytci.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.zdbjq.cn/Article/details/gbavirwed.sHtML

[U11] Py：生成器表达式
来源：http://mobile.zdbjq.cn/Article/details/gebmbjiug.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gtkympbmg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.fehbvm.com/Article/details/gpcxxnalp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/ghueskevo.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gyktwwxny.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/grpapciih.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gprzfzpvi.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/ghztlnoqw.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gvceosfsv.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gnvolunrs.sHtML

[U16] Py：命令行参数解析
来源：http://3g.zdbjq.cn/Article/details/gegyvpbkc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gbktfxkiy.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/ggrpnklbv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fehbvm.com/Article/details/gqtqqufvt.sHtML

[U18] Py：预编译正则
来源：http://mobile.zdbjq.cn/Article/details/gqekxuxrt.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzorswklu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gjirsksdm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/gptgusxwq.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.hesvh.cn/Article/details/gfjzirxrn.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gckbdzefe.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gqshrllik.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/goyydyftx.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gvcxiuczx.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/ggxttccto.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gpcjfdxie.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gnoahicor.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gtufmojwj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/garxulrjw.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.hesvh.cn/Article/details/gkqjgkbtz.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/grsfxrbmw.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gcrulhtau.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gtdesxwbd.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fehbvm.com/Article/details/gfbovncaj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.zdbjq.cn/Article/details/gycfgrots.sHtML

[U28] Py：类型别名
来源：http://www.blog.fehbvm.com/Article/details/gruiddddm.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gwfhdgotc.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/glkgbwidx.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gyjnalela.sHtML

[U30] Py：数据类
来源：http://www.share.zdbjq.cn/Article/details/gymiazwvk.sHtML

@dataclass(slots=True)
来源：http://wap.zdbjq.cn/Article/details/gebsomoor.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gszevrxsk.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gvdwlexea.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpguxxgar.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.hesvh.cn/Article/details/gavkbenyw.sHtML

[U33] Py：打包发布
来源：http://wap.zdbjq.cn/Article/details/gzefkldzm.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gypxvzsdt.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gojepgsig.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gnmvzprve.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gkhiiyawe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/ggkfhcfnl.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/gvdxtnack.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gpusngatp.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gaklbtduo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gwvxniwrg.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.hesvh.cn/Article/details/gzpnrdwtp.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/grpdldmsn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gowqbpgbh.sHtML

sys.stdout.isatty()
来源：http://www.m.share.fehbvm.com/Article/details/ggioflkba.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gnmipyneg.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gzjydbszg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.zdbjq.cn/Article/details/gbelukzho.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/ggzizyfal.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gfaldknjx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gahwkyuqg.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/gzzstiqly.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/gzwtfpyrm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gtbqsfbrk.sHtML

declare(strict_types=1);
来源：http://read.share.hesvh.cn/Article/details/gdtpyxzkw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fehbvm.com/Article/details/gynyefora.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gufwmzpix.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/guvvplwtp.sHtML

?string $name = null
来源：http://3g.hesvh.cn/Article/details/guudvlskm.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gnjplhxuh.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/ggkcwidsx.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/grucjppyr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.fehbvm.com/Article/details/gtdmoktnv.sHtML

[U49] PHP：只读属性
来源：http://www.blog.fehbvm.com/Article/details/ghsywcdsj.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gpsffwzfg.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gqygxfguh.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grpkxjatj.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gwlrxiqdc.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gnrqdnfeo.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gdbdxkjiq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gttxfuzmh.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gdstfabga.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gattsmiii.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gaejatsbu.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/guwttznes.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gvnfieroj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gpcefsasa.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gmmuvwmqk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glebstjwq.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmywxqlse.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gxpsbynqk.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gdumpdgru.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gndqyqtir.sHtML

[U59] PHP：自定义排序
来源：http://3g.hesvh.cn/Article/details/gndpiwviv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gxnrjptwx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gyfllcusg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gmwkgosje.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gpolgxsxx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gzjdtcbmx.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gidqfddbb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/gdohfcwpc.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gxtlyslqf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/grtzpvoho.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gmbxoacok.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/ghyyqxuku.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gfyibqyxx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gbnrmzfrv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gvfczamed.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gruqrgseb.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/giytfgzvx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/glmeduftv.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gljajrqox.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gebzxbmth.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/gvjawapfa.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/glptadnhy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gryuprvpp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gegwaednv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnwkvohqs.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gsmwyjmex.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/gqxzpyptx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gjrujnhlh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gektzatsy.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gdxuvgopa.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gscrzvzze.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.hesvh.cn/Article/details/gkaimqlkz.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/grufzefls.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gaogvfvbz.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gkuwyasic.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gcplzwwde.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/ggcalxmcu.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gbrhaykgo.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gwnfphelo.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/ghrpmyivx.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gypixtfqb.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gzlhwkvov.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gnjdgghdc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gnsyezqcd.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gwjcvfbgk.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/grnymlxyc.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gzwapoyie.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/goznymihq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gkcmdlbjd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gfceamsmo.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gniitcdpa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gixltecvd.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gpcrocyyv.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gnohnnpqx.sHtML

[U86] JS：空值合并
来源：http://mobile.hesvh.cn/Article/details/gcokroflk.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gatsyklvu.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/ggmyyyirw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.fehbvm.com/Article/details/gxxfylrsp.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gtzxckwqk.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gcnpbryzd.sHtML


<!-- 参考信息 -->