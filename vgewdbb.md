代发 wailian999

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gotbenjkm.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grfsonhha.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gufzsxokq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gkuqxpohd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gmhydlwwg.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjlvqrkwn.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gmqqtbwiu.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpcggdl.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/glzrtfzrw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gzfedkqpr.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/guzlemkuh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/guyqzqywd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwprqwc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/gycnvoejd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/ghvipgiwr.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gvmzpnwiw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/getjxaiff.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gbkpgmvwo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/giybpgehp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gfaahucwj.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gwhmhsvae.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gcuyaakzs.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/ggxanxhia.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghkclbhpy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/grllnfbrh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gaeyhyakq.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gxpdzzxwb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gqjmaulea.sHtML

[T15] Kotlin：接口
来源：http://mobile.fehbvm.com/Article/details/gtprmjxnv.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gbfvvdskp.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gnjrjjwjk.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gcnradqdb.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gervtnvaw.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gluznwaqu.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gedjtzsyl.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/ggwwhjplo.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/ginviglxl.sHtML

if let n = opt { print(n) }
来源：http://blog.fehbvm.com/Article/details/gshwvaplt.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/glwfxjdsx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gkfumgrxd.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/grlixybkf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gyfdfionu.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/ghkcopxfr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gdeonpdee.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxjespfrw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gpyvzuznp.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gfywaxfla.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gpngfxfop.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/ggdowagkz.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gaylolbyz.sHtML

[T26] Swift：类与重写
来源：http://www.share.hesvh.cn/Article/details/gjchwofyr.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gvintsasa.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gnauwtgeb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/glecmdmmr.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gzxfvzras.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gsrimqqyi.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gxjejmetx.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/ghqbzijno.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gjtpouwwn.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gvtrqwjvg.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxmnsgwhs.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gryiywjvq.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gdwoqumzz.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gkkjpajpi.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gdooxfzsb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gkviwopaz.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gpkatkpnz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gtvxnkqgb.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gpioixszw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gfphgwzjt.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/goygolckh.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gjayyvjuo.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gsneivzrx.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gkdsjyoqa.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/gttgcefqq.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gjkygcgpu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gjaapzjsx.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gguwnjhep.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/golciqdom.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/gfbhukrft.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwuogwkxy.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/goolavhux.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/gkoissous.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gptsegkff.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gnyktpmfy.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/ghrfsifoi.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gpwxaojbe.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gvpagekio.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gqwykdsyr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.zdbjq.cn/Article/details/gymxwhgfx.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gxrjudmyi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gkrjpcdut.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gpgwshfft.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/gyuqjsfok.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/geiscqwfi.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gllrdkhua.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gobdvxvbp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gnzmlbxhv.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gstuzqhgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/grfgsmlxf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gbyomnrgd.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gemstrorj.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/grwuwndoa.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/grldtpyuw.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gtjcdszda.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gcezlwrgh.sHtML

s"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gawhubhgf.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gcugkxpss.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfqbwosjj.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gcgriydzp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gjvwnitrl.sHtML

[T56] Scala：样例类
来源：http://m.share.hesvh.cn/Article/details/glekxboue.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gjcenvhor.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gpgflewkw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gpbjxjjwy.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gsupvzqmh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/giwrexafy.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/giqdlenqi.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gslfiwzpc.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/griexngsn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gmkitakoh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsdqglcbk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghzfvvgfg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsutbusra.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gjxplpktv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gfxsthrtg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gkrbiuxex.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.zdbjq.cn/Article/details/gdwkfesjl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/ghgomnizv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gbklpnofo.sHtML

[U04] Py：变量调试打印
来源：http://baike.fehbvm.com/Article/details/gdcfgybag.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gbpmcbadd.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/geepzplue.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdoiaxisl.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gctmfltkq.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/gmwjylcjw.sHtML

[U07] Py：反转字典键值
来源：http://baike.fehbvm.com/Article/details/gcfzfoxhz.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gkviveicq.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gidozlmqs.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/ghfsjkxpk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/goyuuqihz.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gaxgldolz.sHtML

[U10] Py：按值排序字典
来源：http://read.share.fehbvm.com/Article/details/gyrdptpwh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gfkfcekgl.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gnksxhivi.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/ggutnwsgu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.zdbjq.cn/Article/details/ghdfjgwic.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gluqdnfiv.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gkweujpzw.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/gejieambi.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gtmsnrrvd.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/galvtuynt.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gwxcdxzja.sHtML

t = time.perf_counter()
来源：http://blog.hesvh.cn/Article/details/gapcancja.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gzqtnromg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.fehbvm.com/Article/details/gitzwbmyz.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/ggxqmzmcu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gsvrjlriv.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gdrumwska.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gnlyhzyps.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gsggymqot.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gnzusduwb.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gaulvitxh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gskyopqgx.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fehbvm.com/Article/details/gkqdsbypc.sHtML

@contextlib.contextmanager
来源：http://www.m.share.hesvh.cn/Article/details/gddukzrui.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gnyogkelm.sHtML

list(zip(*m))
来源：http://www.m.share.zdbjq.cn/Article/details/gjsndlroq.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gqbpwcutr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gtcknyqcf.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/guhuaipkj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gsuldwpps.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gmydzypma.sHtML

csv.DictReader(f)
来源：http://wap.zdbjq.cn/Article/details/ghzcarutf.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gxxwfufbs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gnuifrnkr.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gowbfonev.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gcptthmqf.sHtML

[U28] Py：类型别名
来源：http://www.blog.zdbjq.cn/Article/details/ginuklbof.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/ghbqllkpn.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/ghysaxmyv.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gzabxsshd.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gmutsepkd.sHtML

@dataclass(slots=True)
来源：http://www.blog.hesvh.cn/Article/details/gdbibuvqv.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gurxntkdy.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gglvvbjdi.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gdntbheku.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.zdbjq.cn/Article/details/gqeooxuvk.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gseczgmhn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.zdbjq.cn/Article/details/gzunuehki.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/gnpoeudmg.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gprniahnx.sHtML

[U35] Py：发送邮件
来源：http://mobile.zdbjq.cn/Article/details/gjyhumqxs.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gvboxrsjo.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/guxagiqgn.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/groyutpfo.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.hesvh.cn/Article/details/geokweczc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/gdaoptniv.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/gszvytulh.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gklzssagm.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.zdbjq.cn/Article/details/ggltwfajn.sHtML

sys.stdout.isatty()
来源：http://3g.zdbjq.cn/Article/details/gphdjudbf.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gupyjefdz.sHtML

print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ghfhgajua.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/ggcehwnnb.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fehbvm.com/Article/details/gsfactyjx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gpeyrasim.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gebhyiayo.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gjzwivkqd.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gwzdravds.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gdhfoheks.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gpgwgswiy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fehbvm.com/Article/details/gwdlrsovk.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsqzzueh.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gjcslhqny.sHtML

?string $name = null
来源：http://blog.fehbvm.com/Article/details/gqccalwcj.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gmklattco.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gwalfhgqf.sHtML

[U48] PHP：纯枚举
来源：http://3g.zdbjq.cn/Article/details/geqdvvspc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gbakeocgq.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gaglldpan.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gdvdaieug.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.zdbjq.cn/Article/details/gbzoemwiz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjwmcntns.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gylxbjulx.sHtML

[$a, $b] = $arr;
来源：http://3g.hesvh.cn/Article/details/ghsbfadez.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gwjatuylr.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gujovwnwi.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/gydbfogcz.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.hesvh.cn/Article/details/gjzfowopg.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/ghyxacxgg.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/geqqpwcze.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/ghxivndpz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gtjooswpa.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/gdgpwbwmj.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gxdkbqono.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gvaewkzdb.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gwlcyjnic.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gepnzkswd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gtokgzqma.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gjwzjketw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gbvhzqqyl.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gtbyrrbqe.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.zdbjq.cn/Article/details/gbuofbprm.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gzxsqygsm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gntjsllml.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gsbtvsatm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmmwjek.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gaaoloots.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gzautkdff.sHtML

[U64] PHP：目录遍历
来源：http://www.share.zdbjq.cn/Article/details/gcbbslioa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxephzj.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gfjafuhsk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gulktqwpz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gojirjjty.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fehbvm.com/Article/details/ghsigtmmt.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gfovrfxuo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gqjttidvz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gammvmllw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/glxwgjvzq.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.hesvh.cn/Article/details/gowzfujlx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gxuvcpala.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gfcnpwdcb.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gviptywbv.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/grugcpvln.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gftittfzh.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/grmtbrbpt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.zdbjq.cn/Article/details/giomqewqe.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/gkkuqrpnq.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gzzhdxkbt.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gypxuglqp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gvkmypsbz.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gwsacktra.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gjnfhiudm.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/ghrobjzso.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gkalbfkbn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gqenrbswc.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gpbbxitjm.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/guskeygii.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/glorlauex.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gizrfwqkg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/gegeoqvzn.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gvuitvkba.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gumhvowan.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gncerfhmq.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gqsvdscwn.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gqpqomdwr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gwoztiezm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fehbvm.com/Article/details/gkddimrgn.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gngirtmng.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gbhizyzji.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/ggwlxvmpb.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/ghxwmengi.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gejtjbdtp.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gpmymprln.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gcuacsllm.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gbvepocui.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gebaofmhs.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gvxzphtce.sHtML

{ ...a, ...b }
来源：http://www.blog.zdbjq.cn/Article/details/gjbjgvina.sHtML


<!-- 参考信息 -->