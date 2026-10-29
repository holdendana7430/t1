代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/ggtcuzsih.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ggiosfdmb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gwjufuiho.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpsiuyvih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gyednagai.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggcggptvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gwpsqvsoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzykdiokv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gmddptlah.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grqzpunsa.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gircmesva.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gqsauqvdf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/glxzgitqv.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gkkwaurzd.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gmpxwykwq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/grffyoxnx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gihuxkmhf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gmxqakgea.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/grsptkcbt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fehbvm.com/Article/details/gkstowvrx.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/grmnhpnlv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/gnfxmsprc.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ghihucgjt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gclxiqfzv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gavxrgntr.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/guvfvtgrb.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gflkkieqe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gceubvcns.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gesbijxfb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gfuzotwvp.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gnjvxgsnu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjgqrbomq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gmejdjvlk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbzyoscp.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gkrkvjdad.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/grleqmlxj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gadmfxibb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gehhyrggn.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gldtwgoyl.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggpgpvutj.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gxdamzped.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gdulphbiz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggmisrtwr.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gxbadvlca.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gwhtaanox.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gqxqzjvjx.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gkwlsgptm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.hesvh.cn/Article/details/ggwvicobo.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gdxfvoahx.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/glcotqnvx.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gdqzlhiuy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gwlevlnkg.sHtML

[T23] Swift：函数
来源：http://mobile.fehbvm.com/Article/details/gwbgccyml.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gyslvynpj.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/ghsxpzvgj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwyywvwmk.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gkqzuazxk.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gdkufiylm.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gnswuaafm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gmjymilkn.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gbzvzhyvv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gksamompz.sHtML

[T28] Swift：枚举
来源：http://m.share.hesvh.cn/Article/details/gtfrsvcts.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/goibznogz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gfinhzmod.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/goywqivve.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gjsamklbz.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gvjjcaqmt.sHtML

[T31] Lua：Hello World
来源：http://wap.zdbjq.cn/Article/details/ggkgybhpq.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gheeqquwm.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/glrayehxn.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/giulkpjjq.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gbvqjjocr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gqulagugz.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/glxmovnmv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gamxtwaso.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gwhbuvtoy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/ghecfcqxi.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gmxwbegcl.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gphuqeogv.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gwerarkiq.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gbgjcfkvf.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gujpcedlx.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gbcismqwt.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gadmtyztj.sHtML

string.find(s, "%d+")
来源：http://m.share.zdbjq.cn/Article/details/gbrrrefqw.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gwvfkwrqs.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/guggpjtvv.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gqfcdnahe.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gvcpduqgj.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gsugomkdj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gytyiaasz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gqmtgykqx.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/grdcrgwuy.sHtML

[T44] Perl：条件
来源：http://baike.zdbjq.cn/Article/details/gwgkhvdmy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/grhsvgqrd.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gbuhkkvly.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzyatbsx.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gaktedkcl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gesyzghpu.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/groqxvngc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.zdbjq.cn/Article/details/gpagtwuqh.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gztnqkrop.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/guhhyfxkx.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gfwfasrtl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grghblrru.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gznbkdsmf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gycwabvvt.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gluuangfy.sHtML

[T51] Scala：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gceapdfyq.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gkoxhepii.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/ggwpffdfp.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gdtqvtnje.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gjthlshbk.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gbsuoumhq.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gmnuznlse.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/grckwpvks.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gckrsmmtd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.hesvh.cn/Article/details/gofgdrdkc.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gwfniqmka.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gvebmlhdn.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gwznalxaz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gymttayww.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/gygdnmztx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gfkfbqokn.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gveyrmnzt.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gvqgvcqlt.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gqmejxeba.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gfclgjych.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbgwncqmf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gwnddvvxc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbnnjluce.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/ggysuudxj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gtjbaxfbk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gpfdsbtwn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/guhxptykq.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/grxylrygi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.zdbjq.cn/Article/details/gmjhncilz.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/ggvbyygtl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/ghrrdyprz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gkobmpqys.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/ggrgvelvg.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gatmytqrm.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gyanahgud.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/glplzfldc.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fehbvm.com/Article/details/gvunafvhh.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/grttuejdl.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gqgbovabk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gegeqmlfd.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gktxjszpw.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/greqwvxjs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gpwxmrvob.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gpujxtlfe.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gpjdcwilx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/giwzfmmro.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gihjmzfwf.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gxzzplger.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/glviijjfv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gfwbhlwvd.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gfnapqnij.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/glbgolsll.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gwhcelhzx.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/gbzvfrtgn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gtyocxvwq.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/gbgivdjhl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/goixovhgc.sHtML

[U18] Py：预编译正则
来源：http://blog.hesvh.cn/Article/details/gvyftwzvk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gbbvwzmqw.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.hesvh.cn/Article/details/gvbpwehnd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gxagibkkw.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gtmyicuqk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gllyydpqw.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.zdbjq.cn/Article/details/gwxmltvmn.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gytsmupgy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gpaxbshxc.sHtML

list(zip(*m))
来源：http://blog.hesvh.cn/Article/details/gzboxkioa.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/ggmjxtsgu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gtobwljhz.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/ghefotnfu.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmxvzhykq.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gzszggugl.sHtML

csv.DictReader(f)
来源：http://m.share.zdbjq.cn/Article/details/gcskkfycs.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gddzvxmln.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fehbvm.com/Article/details/gklvoblgm.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gsuxsyoug.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.zdbjq.cn/Article/details/gndydingh.sHtML

[U28] Py：类型别名
来源：http://blog.fehbvm.com/Article/details/gszjdbtva.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gcocgzrkg.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gxnbpojlh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gclnfuuaf.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gmjmjjabe.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gycssawag.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gmeqwfcss.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gsskzsxmh.sHtML

[U32] Py：代码格式化
来源：http://read.share.zdbjq.cn/Article/details/gtxmbvejn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gvzmrzisa.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/giypvygmc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gsxdakeze.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gyslwpxkw.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gkuujcpbo.sHtML

[U35] Py：发送邮件
来源：http://wap.zdbjq.cn/Article/details/gcapzjrch.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/gkiegbczc.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gmpeqvfrs.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/ggbqwbdfl.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gyqrqviza.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gfeishujl.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.hesvh.cn/Article/details/grdpscueo.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gnfrlkhus.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gulhltwdn.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gzvchotre.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gqoyrmaki.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gqdycqvcy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fehbvm.com/Article/details/gsmldnkiu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.zdbjq.cn/Article/details/gnfupwcls.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.zdbjq.cn/Article/details/gtzjwxtum.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqjsxoggp.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/gnbjftong.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gfhqlqyss.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gwkwwpyts.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gthzisebw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gxouqksod.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gkwhmesxs.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gyxqvvzqu.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gazbhzbsz.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqcecxsfo.sHtML

int|string $id
来源：http://3g.hesvh.cn/Article/details/gjalubtkq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/ginltuqgq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.hesvh.cn/Article/details/grrmfujwo.sHtML

[U49] PHP：只读属性
来源：http://3g.hesvh.cn/Article/details/gtfbhebgg.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gmenrzqvw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/glirkudyu.sHtML

public function __construct(private int $id) {}
来源：http://baike.zdbjq.cn/Article/details/gdnolisjv.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gzsnhknjt.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gjudggkgw.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gbgwiejud.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.fehbvm.com/Article/details/gbyjzmvru.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gryjvxtcv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gnwrnjtxk.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gxmhpymuv.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/gosbgkebq.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gpnuxvqkk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gozfbukob.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/giopaaeuz.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/grqaimqyz.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gjrdapuop.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gpzafpora.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/gvhcwknsl.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gyiiesztj.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gbpbhdbvr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gcyhdfxbk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gvdsguzot.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.hesvh.cn/Article/details/ghtjovlpi.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gfjlmzsfx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gznvosrvd.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gxfbqtrpm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gdxnyvkin.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/gazkkccoa.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.hesvh.cn/Article/details/gqyvskakr.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/guufwxtsp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fehbvm.com/Article/details/gjjkzqwrv.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gsgohghxa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/ggymlikib.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gjgqhtvbu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdwgeon.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/gyvtdemol.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gzkkyxtdh.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gavcgtsiq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gcozsodpm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/gvisybytc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gdferbrxh.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gjfsehfkp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gkwuqjklh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/grawmfkiy.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gyukvduxh.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/gqwzfzzif.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gozzercye.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/grrdkxtbw.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gddbvzymi.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gfiygcqtk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/ggxnpvrhq.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gipoaykuv.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/ggnkwdsbq.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gknsorbmb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gqcyoapsn.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gipblovjc.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/grqvwqkyd.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/glcfwrlsr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gxhcuomou.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/ggghizpdx.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gegzbokbq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/ghrwjmzxv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gphukpkdm.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gweablecp.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gswyxrzut.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gunkgzpgb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gmnqecyyk.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gqjblsvyj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gwupkefsk.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gmnpkoosl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/grkpbrdyp.sHtML


<!-- 参考信息 -->