代发 wailian999

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gkbhtfdpa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gyqducnih.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gsepbbqgm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjvmcptw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gnvmgwgvf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/goumkdqvy.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwgwphyu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gkgdadrch.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjujmyrm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gojktvulv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyyqdswm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgporjae.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsnbiodq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/glymvkxju.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/ganpthkux.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlnyexiw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/guhzxlymr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtrepymx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbcavzcu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbadwpzyq.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmhnukob.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqenpcbhl.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvajwnuva.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpejrguap.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/glccutcug.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrmyyszy.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gxfazgbqn.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gsisimeub.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gsjdegzmx.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjqtayey.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gmddihsxo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxeidfjr.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuukkpzd.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhpibet.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfllspat.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvgbuhpdv.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcfqidriu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/grhotyinm.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjqllnfq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmijaqrs.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gtynmchqt.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gymzdnssv.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gpkpialml.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzulcbcwf.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfliwwalh.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grjmyydsf.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gerkhzrak.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgwnozp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxjxsghf.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gykeysors.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfaoxirz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyfhprey.sHtML

[T31] Lua：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqgmqrzy.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtygfmgfb.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeflljat.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbbxmjak.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctlrsqim.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkauyjyl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvurdvuzt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryjepruf.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaqiamwi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrmhfcxi.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxontisy.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfwkeqqk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczawdori.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmzmxizza.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/geimojfsc.sHtML

if x > 0 then print("正") end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcxacyhe.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgqbndnx.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/golbwgfft.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gkpwxppnd.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcdrdxzy.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyvqqmgvn.sHtML

print "Hello\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsucaxvss.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxrcaier.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhecktyq.sHtML

[T43] Perl：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gyuuqfofc.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmvdgrpx.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzjotqhz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghguiqbkv.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvotlypaj.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gasaykfkj.sHtML

[T46] Perl：哈希操作
来源：http://wap.fanxiaobao.xyz/Article/details/guwgvhlhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgkfjjh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfjjosbg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/goeoijpzl.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzebudjlu.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gioehkcem.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbbngpji.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyhyuwwx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmowhajmc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsjpluyi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giklatpwk.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/griqkjzmz.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/giynfmuxu.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwvgdmpi.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/giyulqruv.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkpafffq.sHtML

s"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/galpfutdt.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsnrxjsr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqldleh.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gfztagkcb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxnkrbpm.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/ghuibwmrd.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbutkgdso.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuvgesae.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqaplvpm.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/ghdiseqag.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjdaeoxu.sHtML

[T59] Scala：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbmgfxvkw.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/glklgshte.sHtML

[T60] Scala：折叠
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnjbinq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fanxiaobao.xyz/Article/details/glxeqkzbh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjawxwyr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ghllmdolw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnqrxghq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fanxiaobao.xyz/Article/details/glfjkalkw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fanxiaobao.xyz/Article/details/giohcqehl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fanxiaobao.xyz/Article/details/glswfnkis.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxxnykvcs.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gasnqyxfy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvdrboop.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfvquhca.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gdbzljpsu.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fanxiaobao.xyz/Article/details/gqgkzcnsd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/geqbninbr.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtnihypz.sHtML

{**a, **b}
来源：http://3g.fanxiaobao.xyz/Article/details/gijvmjqea.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlhjzxai.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fanxiaobao.xyz/Article/details/goksnlyfu.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfndbzvi.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxylbzl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhlaqlnb.sHtML

max(d, key=d.get)
来源：http://3g.fanxiaobao.xyz/Article/details/gowtsorhl.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gaztbutuz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsxvzrev.sHtML

[U11] Py：生成器表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gzhavxxsm.sHtML

(x * 2 for x in arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gauodqfso.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpwnrudq.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gbnyzfitu.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gplrujtst.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqmmwkbr.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gygkzwgyz.sHtML

defaultdict(list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gprswhdyh.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fanxiaobao.xyz/Article/details/garuetmla.sHtML

t = time.perf_counter()
来源：http://baike.fanxiaobao.xyz/Article/details/gzhpysdey.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.fanxiaobao.xyz/Article/details/goozxrdtw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/ggquvigwg.sHtML

[U17] Py：初始化日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqtdqxl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqofdxk.sHtML

[U18] Py：预编译正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfsjehcq.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiytnhpo.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fanxiaobao.xyz/Article/details/gtwjrtpie.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/guouavrpq.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggcqsrqfu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwthgukp.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/gqflzcpjj.sHtML

@contextlib.contextmanager
来源：http://blog.fanxiaobao.xyz/Article/details/gtajymgst.sHtML

[U22] Py：矩阵转置
来源：http://baike.fanxiaobao.xyz/Article/details/gwblaqplt.sHtML

list(zip(*m))
来源：http://blog.fanxiaobao.xyz/Article/details/gtzuxaehd.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouxucipk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxxubqre.sHtML

[U24] Py：路径操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdzsbdgx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkbhhebc.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.fanxiaobao.xyz/Article/details/ggotraqde.sHtML

csv.DictReader(f)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswdkgcnl.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpaconim.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglvmzyzt.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycqqxki.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvjamilr.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gdvsigezk.sHtML

UserId = int
来源：http://wap.fanxiaobao.xyz/Article/details/gampcnlah.sHtML

[U29] Py：属性校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxawnpgs.sHtML

@property 与 @x.setter 配合
来源：http://wap.fanxiaobao.xyz/Article/details/gvzdcezid.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gssbtsifi.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviwnlzgt.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gecbtgdre.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gljrmfbos.sHtML

[U32] Py：代码格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpzvwhfhi.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqcmmnl.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqpadlwa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fanxiaobao.xyz/Article/details/gayiicnkw.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gkegurdae.sHtML

chardet.detect(raw)
来源：http://read.share.fanxiaobao.xyz/Article/details/gevhgrgqt.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/galnpyhcz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fanxiaobao.xyz/Article/details/ggwvvcfoq.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/galbnetht.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fanxiaobao.xyz/Article/details/gcecqthhk.sHtML

[U37] Py：读写 Excel
来源：http://wap.fanxiaobao.xyz/Article/details/gywluuzsf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmnukufm.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fanxiaobao.xyz/Article/details/ghumzkyqs.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuvegwka.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gholumrwp.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gsaxjcjyx.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gtenoltah.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggymyqvqj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fanxiaobao.xyz/Article/details/glpzmcybl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fanxiaobao.xyz/Article/details/gabsjosnu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/gvlqpmjiv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fanxiaobao.xyz/Article/details/glayvamic.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrdkhioy.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/gzcmysixq.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsyyklbb.sHtML

declare(strict_types=1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdijhyngd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffuvikqy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihwszjf.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzegziztr.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkigxmyfb.sHtML

[U47] PHP：联合类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqbiybff.sHtML

int|string $id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfkmbzjz.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnqyjbzz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqcnlprn.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqrpcru.sHtML

public readonly string $name
来源：http://baike.fanxiaobao.xyz/Article/details/gyqkdbghc.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fanxiaobao.xyz/Article/details/ggbyffptg.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqhkiqjl.sHtML

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbexkhsm.sHtML

[$a, $b] = $arr;
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvyiiww.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlatnbwc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fanxiaobao.xyz/Article/details/gxswmnjdl.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrfvxpxi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfxgntae.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhymbfla.sHtML

$obj?->method()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlgnrlkd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsekigja.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurfwykqy.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gccfcziyl.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gompfucpi.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/giqnpjtcn.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guifcsnaa.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawnvjqnl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcofwyjki.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohgoeksy.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlkmrlat.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/guegkiokl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gbqyhfocy.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gvhxjnxjj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gixzwghzp.sHtML

[U62] PHP：日期对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjpkwyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzldlzbse.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbsouhcgm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdxonuvt.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdacgnow.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbppgpyye.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/garxynvnk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyviniiko.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gfgbylapu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glaidyivr.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/grdneeiyy.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpbjecbz.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gencfvnqd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/grqxupmsw.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzcttlqe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrtsadby.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxbfqos.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxobopp.sHtML

[U71] PHP：抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/grxyfykqp.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/getmraeaa.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvpmrqvc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnbyiubs.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzjwkwmm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gghndjogn.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkuhakqgo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fanxiaobao.xyz/Article/details/gufrovrqa.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpkbzmxx.sHtML

composer require psr/container
来源：http://3g.fanxiaobao.xyz/Article/details/gtagdoxld.sHtML

[U76] PHP：简单路由
来源：http://read.share.fanxiaobao.xyz/Article/details/gwncelewv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/greaxmbxp.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/gklqdlrjp.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gpncmyavf.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/guufwwtov.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmthxtkj.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gpjsceekt.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhasulgp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrtdoidg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdjguecz.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhmoulfu.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdijwumk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphkdkqlt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhinxqtf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxebhhx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzldyottz.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyelyzgcf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqkkmiuw.sHtML

[U85] JS：可选链
来源：http://baike.fanxiaobao.xyz/Article/details/gthriltya.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gxhcfaurw.sHtML

[U86] JS：空值合并
来源：http://baike.fanxiaobao.xyz/Article/details/gmppirdnw.sHtML

a ?? b
来源：http://blog.fanxiaobao.xyz/Article/details/gwecbjvlx.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfikmjte.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtklcxepd.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/goiowbyve.sHtML

{ ...a, ...b }
来源：http://blog.fanxiaobao.xyz/Article/details/gmfihacbq.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/grhsyxcww.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gelcjbgzs.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxpyivyx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfowfjfr.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzrfxxfh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gzaolcunq.sHtML

[U92] JS：深拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcmkfphj.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdvetuxr.sHtML


<!-- 参考信息 -->