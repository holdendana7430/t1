代发 wailian999

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/ggxwejvho.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gnylfckjh.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gfwngeswb.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/guyxxymjp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gdxlsepji.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gmgjzhynz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gixbwsiaj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gdlthjtat.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzoohkdku.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gtsplciwd.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/gydkyudly.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gskalgbje.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gqeozfseg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/galcsbapo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gkkdaegyv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gupixcado.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gilpwmacu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gzxcnzprq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gwvwhzwxb.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcjouauki.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gnnrkxqna.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gwbcxmwzy.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gwxpigxhh.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gjcddjeph.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/grqjylqhx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gkebpsxxo.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnlauiyfu.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gezeabsbc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gskojwdhy.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gepxebvps.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gzqbmugtu.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/ggkeutmpb.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gvimzawqg.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gxqsjhgwc.sHtML

[T20] Swift：数组操作
来源：http://baike.zdbjq.cn/Article/details/gptunjqli.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ghgxhjszk.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gpruygzoi.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gcbooqpec.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gsfecztxk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/ggshboapa.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gojfuiqhv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gsnxtedkh.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gksnfefgj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/godylfmjz.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gegqhcqjh.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gdmlrmuyd.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjxqkjpkc.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gxubxeyve.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/ghmysxrud.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/geqvywyta.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gdfkigmdb.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gfmmtjwdf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gzwcykqqb.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gmegxdhui.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gyqmrcgch.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.hesvh.cn/Article/details/gppiovgmi.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/giqfuewpe.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gnivcxwiq.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gdgaauaph.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gjokprekt.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gqkuhvsdf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/ggedrfncz.sHtML

[T34] Lua：遍历表
来源：http://read.share.hesvh.cn/Article/details/guoqctbga.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.hesvh.cn/Article/details/gmsqidyby.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gkjqyoqev.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gcdkzgnft.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/glvofjvsg.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gcepeockg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gwszyowut.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gajlhyvjm.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gczkdqpui.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gmkedgcrx.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gprenwith.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gpcwevaxi.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gifwwltkg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gzheacodt.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gamfnpumb.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gjwxzwpcc.sHtML

[T42] Perl：变量类型
来源：http://baike.zdbjq.cn/Article/details/gukxvbbwd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gwblzzmgg.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/gftgcboww.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/grckweqkm.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/garaoeicc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/grdrcxnad.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/glczpdlts.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gatjsochu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gthtyzjhy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.zdbjq.cn/Article/details/ghuswcfry.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.hesvh.cn/Article/details/gtfvnmodi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gjyyebcuw.sHtML

[T48] Perl：正则替换
来源：http://3g.hesvh.cn/Article/details/gpuzeeuwq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gffbmudie.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/guobmvdqj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjknknjgp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gqfivaubg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/gxwxzfodh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/glchraalx.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gshytvjbp.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gzfodegyp.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gssijoznb.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gzrsdxfgx.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ggpcmnaau.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gmewjsjih.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/ggffwzjgv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gtmzcpxmm.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gzppnorux.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gacdotuen.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gzsotgxjp.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gqooqtned.sHtML

[T57] Scala：模式匹配
来源：http://3g.fehbvm.com/Article/details/gaezaoefb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.hesvh.cn/Article/details/gcphabkyl.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gcspbmdhx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gsbeywqff.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gcpptavug.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gmcevhrwy.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gqjazkjtp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gvzqwizzy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goeklqdwn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gimqlkckv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjijhhcwn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/ghkegqmji.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gfgthfxsm.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gtqgrqree.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.hesvh.cn/Article/details/gnopjzjnr.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gophwmkxa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gyxhxlnqk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gdvlsyqgx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gjkjrorjg.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gpgtutfhv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/garhfgzwr.sHtML

[U06] Py：合并两个字典
来源：http://baike.hesvh.cn/Article/details/gbotngccw.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gykkoxtau.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gcdzfragj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gccqggxwz.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gnljrgnxn.sHtML

[y for x in nested for y in x]
来源：http://blog.fehbvm.com/Article/details/gzkniysvt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.fehbvm.com/Article/details/gzhshdzij.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gxtdmnwll.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gtfteprhn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.hesvh.cn/Article/details/gqgwqziwy.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gewucfoev.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gxpioyedl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/geoqkjzrv.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gzkqtbaxk.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gmjzmciaa.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gzrfkhbtg.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/giipbogut.sHtML

defaultdict(list)
来源：http://www.blog.zdbjq.cn/Article/details/gutyhhstw.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gfqyvwzjl.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gjstqdyyf.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gturddhcr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gnazksfvk.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/gcdocaajb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.zdbjq.cn/Article/details/gembstxlx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gszzslqez.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gyfbqocpu.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gjfdyfdwn.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gfunrtcae.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/gwuqnmvhw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/ghedkooaq.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gqjghgzjr.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gafwgwntv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gpqtiglhv.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gkzpnmbnh.sHtML

[U23] Py：分块读取大文件
来源：http://baike.zdbjq.cn/Article/details/gptacoloh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gdifzyijb.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gvkypvzgd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gpzhsyxlo.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gkxtlgnfz.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gcxuykmzp.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gffiqgxaf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.zdbjq.cn/Article/details/gpipzuxvx.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/glqdvyeot.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gwuvzutzs.sHtML

[U28] Py：类型别名
来源：http://baike.fehbvm.com/Article/details/govubfsmz.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gfrlbsgch.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gsdgxmsmm.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gimjctywa.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gnkihybpg.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/ggmorsizi.sHtML

[U31] Py：单测
来源：http://read.share.hesvh.cn/Article/details/gvcrxswij.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gpxwkjjgk.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/gzuscfluy.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gqtanykse.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gkgpyxole.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/ghemvgxnx.sHtML

[U34] Py：判断编码
来源：http://www.share.fehbvm.com/Article/details/guswpsqmx.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gngpgaxgv.sHtML

[U35] Py：发送邮件
来源：http://blog.fehbvm.com/Article/details/gesliqnit.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/gvvqqzwvn.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gvcdhtnlv.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fehbvm.com/Article/details/gqdshfwtx.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gtgsuggsc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.zdbjq.cn/Article/details/guorburuz.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gvkkzcurz.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gydxedlyd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gdbdkxjkl.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/gigmygxpi.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/grkbkczqb.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gkzyanyul.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gczcxlybz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gxdhgdxmd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gbumdbmoy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.hesvh.cn/Article/details/gcezeuggf.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.hesvh.cn/Article/details/ggazhqtoq.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gfubjadmc.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gwmnrotij.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gtkviijxl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/goifbscyd.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gutxlqmlt.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gorxlumsz.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gtchevytc.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/gaxylmcqs.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/gcxgtprxy.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/giakbkgnj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/gmwtiwbpg.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gpebiykkl.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/glrmqriiz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gjkeimmns.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gqwetxkww.sHtML

[U51] PHP：数组解构
来源：http://3g.fehbvm.com/Article/details/gsmqahmwv.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gqoodkioa.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gwfszsdof.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gfvskpjdj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gywogcbcv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gbwirzsrq.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gpfdfphmr.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/ghjkitecc.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gowwowifv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gmmptwlrg.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gjlxzngyz.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gznaiwmyn.sHtML

[U57] PHP：字符串插值
来源：http://3g.hesvh.cn/Article/details/gtgckyqfx.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gauosqxkf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gkfblgtkx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.hesvh.cn/Article/details/gdlgoaubw.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gopycwlug.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gnsjbjonr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gjysaweao.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gsvxiloni.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gzdrtpvjs.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gboabrikh.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/glifodwel.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gxhqeujua.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gxlhbxtan.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gesxuitgi.sHtML

[U64] PHP：目录遍历
来源：http://baike.fehbvm.com/Article/details/goqmwzxpt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/ggoemlnhu.sHtML

[U65] PHP：会话
来源：http://read.share.hesvh.cn/Article/details/gmujfrfkg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdoemqgpj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/grjpedziq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/guytwpjog.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gewdztxuq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/ggcviumig.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gcbzmipxm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gvthlmfxz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/ggfslpciz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gjzxqqmao.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gzeecgwft.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/ghcixxlzr.sHtML

[U71] PHP：抛出异常
来源：http://www.share.hesvh.cn/Article/details/goligtwoa.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gzukzlmpa.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gijwixbhg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/gludgtwnk.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/ggzioluug.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gyyznkhha.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gjzrfrinj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gqimfeshh.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gwvlzcscu.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gnytfqhfx.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gnfxlaojy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gqtzubvgz.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gggehzska.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gvalharrd.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gdvkblagz.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gvikvjkmg.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/ggnqtpnpn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gwkbpburk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gkgmyxmtg.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gkjcdptaq.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/goyrvuqop.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gpxaafsmb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/gquczaaem.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gyqtklsbp.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gdbiizsmw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gixxntbrr.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gjvhkintu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gezpraqfe.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gocthqlgn.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gwcahkkbe.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gokembtyx.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gzmhgonwo.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fehbvm.com/Article/details/gsfuktsoe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gufhonyqp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gqfqjndrv.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/ggdjosdab.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gpellnnti.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gijsjnzab.sHtML

[U90] JS：数字数组排序
来源：http://read.share.hesvh.cn/Article/details/gjwecsqrb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/ggwscepvz.sHtML


<!-- 参考信息 -->