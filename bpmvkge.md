代发 wailian999

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gzngardvq.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gmcvaqkkg.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gmyghursk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/ghyjzwopf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gudzvvwcv.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gbapujloo.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/ggumriaoj.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gejmumxge.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gujovfmhq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gdzzjmnbv.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/glhuztfbg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gmchwluru.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gxpejpbot.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gzqzvjzyv.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gaehhirbf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/grnghowfx.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gwqncithz.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gqyswtfor.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqymbtcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/glnenrdsq.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gprvxafcz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/glekbwbvw.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gkdoduqcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gpptmtlhb.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gxnmnqtny.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/ggetzooau.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gdwvzizlh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gthygbsyc.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gbcflthdg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/guxjeighf.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghgehnygl.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gbxtndkkk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/glvjsiiak.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gfyzertrm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gdiuvoizv.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gjunajfcc.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gtjtvuvzl.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gmwussmuo.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gtjwsymnx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gegzkoupt.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gkjjpalno.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/glmngozzl.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gatrgwvha.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gasaytigb.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gtxhdpiyj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gppafybtf.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gliaopqcy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.hesvh.cn/Article/details/gaoewqomz.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gdbofofjr.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gfislqpvu.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/guhzfhnda.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gnhyoatfh.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gmzomvyft.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gpnllkvjr.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gexzuimdl.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gaydzojib.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gvajwqtfo.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gluamnqpp.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gsfveomdq.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gxtircjlo.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/gthzyfkzn.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/grzctylaw.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/grknkbrdj.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gkarqnnmc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gadwkihgn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/gyznqqdtp.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gncbcqvnx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/ggyeehwfu.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gmyhmpkyd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gykecllal.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/gyekvwusw.sHtML

function add(a, b) return a + b end
来源：http://mobile.fehbvm.com/Article/details/gbzhwjwbk.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gjmdktcwb.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gqavadpmw.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gmswqpqqj.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gqkvzxnpi.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gnqqpjnwu.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gyqewsxcd.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gunhtqbgm.sHtML

setmetatable({}, { __index = base })
来源：http://wap.hesvh.cn/Article/details/gytaowhil.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjwbijvgh.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gzvvgopts.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gjvwsilmh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.hesvh.cn/Article/details/ggvainmpg.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gaigrsrdt.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/gsvweacmk.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gnhurotjg.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.zdbjq.cn/Article/details/gctocrwhx.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gfeehnahq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/gviwnbzzk.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtbcsoaah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gebypaqov.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/getkmzmsj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/grpyumfdh.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gejyhauky.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gxrwbitwl.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/glvpbyjnr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/griyhushb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gxqdmieie.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gulrkesiu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gylsdhvsc.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gkvplfunv.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gmfmjfbxl.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gfbfopwju.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gxhipmggn.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvxhkwgjj.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gdpwiqfmc.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/guqycybbr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gsaiilsza.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gkwlxkags.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gicemjnon.sHtML

[T56] Scala：样例类
来源：http://m.share.zdbjq.cn/Article/details/gubnrndmv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gjrbqldrb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.hesvh.cn/Article/details/gpfrhmkor.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/grnvhbxzj.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gxazlxsvf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gtroghbjz.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gmggkypih.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gusnkmlcr.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/ggvigznbv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/grpyhqbrs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpqbfotch.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gopkuxrbt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkyhnduxs.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.zdbjq.cn/Article/details/gdognfbmj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gdnxivycj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.hesvh.cn/Article/details/giynddgrx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/gydahxwge.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.zdbjq.cn/Article/details/glapamwvr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gskqltvvz.sHtML

[U04] Py：变量调试打印
来源：http://3g.zdbjq.cn/Article/details/gkxsjkyes.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.zdbjq.cn/Article/details/glgludnnw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gklenciks.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gxfanvtpq.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/ghhwerubj.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/gymmfwfxe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gizujqqbe.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.hesvh.cn/Article/details/gitaljaib.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gzbgzejus.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gvwezhxuc.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/gbjzvszkh.sHtML

max(d, key=d.get)
来源：http://read.share.fehbvm.com/Article/details/guunocogm.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/gnmdumwtf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/ghknyertf.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gmpnjrinb.sHtML

(x * 2 for x in arr)
来源：http://www.share.fehbvm.com/Article/details/gvjeiaqah.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.zdbjq.cn/Article/details/gvhvhnvfw.sHtML

Counter(arr).most_common(3)
来源：http://baike.zdbjq.cn/Article/details/gwjljqtqn.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.hesvh.cn/Article/details/gvblzzdnf.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gvhccdasl.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkqxgrgnv.sHtML

defaultdict(list)
来源：http://baike.hesvh.cn/Article/details/gbulrtgkx.sHtML

[U15] Py：高精度计时
来源：http://read.share.zdbjq.cn/Article/details/gtoqryirj.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gwqkektmt.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fehbvm.com/Article/details/gqnnpqfcp.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/ggzhuhmlm.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/gzqzikzdu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gorcaimhx.sHtML

[U18] Py：预编译正则
来源：http://www.blog.hesvh.cn/Article/details/gvgmqffan.sHtML

pat = re.compile(r"\d+")
来源：http://3g.fehbvm.com/Article/details/gcpjekcla.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gfyepnifr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gzdgyedyp.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fehbvm.com/Article/details/gyfcwwulj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/ghouabwba.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gtihoaxmd.sHtML

@contextlib.contextmanager
来源：http://wap.zdbjq.cn/Article/details/gkwjprmen.sHtML

[U22] Py：矩阵转置
来源：http://mobile.zdbjq.cn/Article/details/glaeielhh.sHtML

list(zip(*m))
来源：http://www.blog.hesvh.cn/Article/details/guyirhcic.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gqyjgnftx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gnpnoyqwv.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gbpolltii.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gdjduxkef.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/glhmglfip.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gvqwbksoq.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gtnjriweg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gpeseiznj.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/grupgsytw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/gmgfznpwl.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/grvhccyds.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gzlkwlsrh.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gmsnkphvx.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/giehgqfoq.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/ghoqwlnuv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gibggpmzl.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gwsohqlkq.sHtML

python -m pytest -q
来源：http://baike.zdbjq.cn/Article/details/gbrusgesp.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/ghafbocfz.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gkifbdari.sHtML

[U33] Py：打包发布
来源：http://baike.hesvh.cn/Article/details/ggbanhfuc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/guqizisxi.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gnhacuxuq.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/glljrbbtw.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gpnrkwufd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fehbvm.com/Article/details/grnosrwuz.sHtML

[U36] Py：定时任务
来源：http://3g.zdbjq.cn/Article/details/gdbyfadkk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gpcchibrq.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gxaoqvmfp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fehbvm.com/Article/details/glfugfdbh.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gerobhftz.sHtML

Path(__file__).resolve().parent
来源：http://blog.zdbjq.cn/Article/details/grmkcuzln.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.fehbvm.com/Article/details/gdbzdyjxl.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/gkkhagpsa.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/gtmohdpsf.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/ggfswcudf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/gjvxuuehd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gxhurgjat.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gvwcfycbv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.hesvh.cn/Article/details/glaaqdkae.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/goulcczzp.sHtML

namespace App\Http;
来源：http://blog.hesvh.cn/Article/details/gbldzwgkc.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/gamgiwzsg.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/grxpojeiw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/ghweuitba.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grmodjjsi.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gfvttuhia.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gvnnqmogh.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/ghfdiyqsk.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/glvefboca.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggcgwnpdq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.zdbjq.cn/Article/details/gdntucwpp.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/ghkgdvqjf.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gigpbjtqt.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gvkeniljm.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gtiueilui.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gozjxteri.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/gwlecegrz.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gvsaodbaz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gycdxnhkd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gkqtwatsb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.zdbjq.cn/Article/details/gdzlgcmai.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gbnbabwvo.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/godahxbji.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/gjtqsalui.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gezwmgwih.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gjlgvomur.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gharwrinu.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gssxxvplp.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gngnrykey.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gonuzzrsx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqiiacouw.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gsixwrjxh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/griuvlhsc.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gtfxftiuy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gdrhzdyof.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gfqwryupq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gjvoujnlg.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gqsutolea.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gtspkjfsv.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/geidunklb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/grmxgagou.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gqsxnsxcu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/glkjyjrqc.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/glwdszddi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gygqmfufg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gkfmvkyka.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gvxedjvtq.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/ggzglxbgj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gzrszzlft.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gkolcwhpk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/greioomis.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gvbcnbnpk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/ggbmaknmv.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gifipneip.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gkkjsevsw.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gjcoosxar.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gpulgszvk.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gkufrxwyu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/galwwhbee.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gdckovwla.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/gjdiqivpv.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gmjjnmogl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmechyu.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/ghhbajhjm.sHtML

composer require psr/container
来源：http://read.share.zdbjq.cn/Article/details/guwqofnuk.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gtemxqbpw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gukjkumph.sHtML

[U77] PHP：模板渲染
来源：http://wap.fehbvm.com/Article/details/gxccfjqvn.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/giakhluya.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gshuiuybo.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gihisnqbb.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gxpzmdoug.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/ghdaqmgyq.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/gkvupvmmw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gciunbbwk.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gmzhehyzn.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gjkvzxdct.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gauuelbma.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/glnbruvxm.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.zdbjq.cn/Article/details/ggdmdureu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ggicdvnjh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.fehbvm.com/Article/details/glyzzhpvi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.hesvh.cn/Article/details/grxabfdxx.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/gddabuasz.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/gxuxmyobt.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gwdlmmmil.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gqhmjhccn.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/goviqtsah.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gcxqvkbtf.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/ggtbwxmcx.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gwshsqbzu.sHtML


<!-- 参考信息 -->