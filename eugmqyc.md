代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gdwtwnsng.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gqulcqpca.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gghcuqwzc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/giaxhgbsu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gaexixyjp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/golmhekml.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/ganechwcx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpdfxklyu.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/glylkplbw.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gblktiwps.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/grnfctwvd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gcwggauzg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gzyflfbup.sHtML

"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gpnrqfjgi.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gnngrllcw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gdpqouwnr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gvefyybqi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gzspfgywu.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/ghgmpocgc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/glqjcgrky.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gviravsym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gzntvgrcm.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gijyvniwv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gpeibkhvo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gyfpgcecd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gythnswfk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gtrzbhfjf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gzropespo.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gybrurmda.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gcbtukuzz.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gjtanpubh.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdhdisyxm.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gtozfitci.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gsabpswrn.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gwbsekvre.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gnbushalo.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gtbvoqymo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gcnxuggdl.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/ghjfbpjpp.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gxtmcfsgj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gnbsiwjvy.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gisdugaur.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gobdkjwgz.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/grpjhirzs.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gdbkyejoi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gwemwisxl.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gqkjmexqp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.zdbjq.cn/Article/details/gdkalmeue.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gvuihqbaa.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gxaoryiny.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/grryyvwxp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gkpjluyun.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/gtvauvltn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gdltzydqq.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gedckuedz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/givzqkwqz.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gedauzpcw.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gychqkvlx.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gjxpwfvyo.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/glckoxgim.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gyhcyuggm.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/gbglxleou.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gybaeswda.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gpsdvyzlq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fehbvm.com/Article/details/gustzeonq.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gtksaugwd.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gyxaifelo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/goxqdnjrz.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gpmsstcdt.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmozjisot.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gmyrjsflt.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gzmugrqkq.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/gsykobfvx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gpdvasmsk.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gadqeecrp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.zdbjq.cn/Article/details/ghhhqormw.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gvrczvogz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gbswvwiqu.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gynibpulb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gpcfmzscy.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gtuphmccg.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gnvfxdiwn.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gpxmrckpu.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gyuusufer.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gpaodahsu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/gblacksck.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gkqsfdfdg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gadhfdlgx.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsnqbzqqq.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gryoeaxkp.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gvhruvyqp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/gamzekffz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/grhywntjn.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/gcximehmv.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gzypigenc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/grmvbifds.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fehbvm.com/Article/details/gkitvotkz.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gvkcenabc.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gtlaqgsma.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gingtyapf.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gaadvsdhb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gxqtlhtrc.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gdtspsdmk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gaxsthjvb.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gfecvwzjq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gkzhudmck.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grzsrrxsw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gkfbqefuc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gkemuddhg.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gfmunkpfg.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gphsojdlx.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gfylnvixu.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gckwhilpr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gdmqlvppt.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gpgtowdya.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gdfiqwtbe.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gcheimlhc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gotvcesuc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gzvshquvk.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gzpxogzth.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gxbvddcis.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gyqhtkxhd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gqmisnrol.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/gtxaxxlzs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/guplsfivy.sHtML

[T59] Scala：循环
来源：http://mobile.fehbvm.com/Article/details/gsoftkovs.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/ghdqpjyuh.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gsuxknapk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fehbvm.com/Article/details/glcdjqplw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxwjkhprz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gyuagcwvq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpiirkhcc.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/ggilgoxyr.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.zdbjq.cn/Article/details/gomvyqexi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/goygtzkkr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gvpxtmetc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/goxsnbzzt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.fehbvm.com/Article/details/gfrnahwod.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gbuwpverz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/geevsyeuq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gvxtegdxm.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gcijwyzpq.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxenamq.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/giwtvdpws.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gykoialvr.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/grdsnjqvm.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gewfkfbey.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gbnkurfcl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gsxftmvqz.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/glhjkbzuz.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/guuhdldur.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/ggwtlaged.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/gcczlzgwc.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gpjvtjiyq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.fehbvm.com/Article/details/gmmrnomky.sHtML

Counter(arr).most_common(3)
来源：http://baike.hesvh.cn/Article/details/gkiknssnk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fehbvm.com/Article/details/gqydbxlen.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gywmxarkg.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gdyzxnmnp.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gwqciutdf.sHtML

[U15] Py：高精度计时
来源：http://www.blog.zdbjq.cn/Article/details/grjplwdyq.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gbsvrxrpo.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gbypzlinl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gsyvxztse.sHtML

[U17] Py：初始化日志
来源：http://blog.zdbjq.cn/Article/details/gchsmhkkh.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gtnwrhhmj.sHtML

[U18] Py：预编译正则
来源：http://mobile.fehbvm.com/Article/details/grktjiabx.sHtML

pat = re.compile(r"\d+")
来源：http://baike.zdbjq.cn/Article/details/gylstnepc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gtkqnacib.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gfbiybnqa.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/gezlfjxjz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.fehbvm.com/Article/details/geacuksut.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gdpefomeo.sHtML

@contextlib.contextmanager
来源：http://www.m.share.zdbjq.cn/Article/details/geqorkdgj.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/givyyqbxz.sHtML

list(zip(*m))
来源：http://wap.zdbjq.cn/Article/details/gacsjzcwm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gfzpwmdng.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/gtjxpirkw.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gbupsqjkf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gpgmuoemf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.zdbjq.cn/Article/details/gpwkvemwe.sHtML

csv.DictReader(f)
来源：http://mobile.hesvh.cn/Article/details/gcsrkwlmf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.hesvh.cn/Article/details/gnhepotpl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gepuurpfr.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gknngwicn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/gtjixqzdr.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/goaafohlm.sHtML

UserId = int
来源：http://read.share.hesvh.cn/Article/details/gapymsmyt.sHtML

[U29] Py：属性校验
来源：http://mobile.hesvh.cn/Article/details/gxidzolsc.sHtML

@property 与 @x.setter 配合
来源：http://wap.fehbvm.com/Article/details/gokbsmeju.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gvcfhycni.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gougowsig.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gtrckvbxu.sHtML

python -m pytest -q
来源：http://www.share.fehbvm.com/Article/details/gfomhivjr.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/gkhmrtdmw.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/ghfrukyuv.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gpdqskgem.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gylpeuaux.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/glzcfslcr.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gyinkmoou.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gdomhroyw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.zdbjq.cn/Article/details/gyodxefwc.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/ghqxtinql.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gjvczuzds.sHtML

[U37] Py：读写 Excel
来源：http://wap.hesvh.cn/Article/details/gbicunwdt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gyqkwoaqu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gnjazaoti.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.fehbvm.com/Article/details/gmccnsaht.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gzkheimrs.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gevfxrlkp.sHtML

[U40] Py：打印到标准错误
来源：http://3g.fehbvm.com/Article/details/gcsqsffnm.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gjfkiwzhg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fehbvm.com/Article/details/gavtjvtwp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.zdbjq.cn/Article/details/gmajwrdcm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.hesvh.cn/Article/details/gbwxtcvhc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fehbvm.com/Article/details/gzeyixxxx.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/giylhcegu.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhowlhy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gworhmjht.sHtML

declare(strict_types=1);
来源：http://baike.fehbvm.com/Article/details/ghfkmcrwz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/glebkvdea.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzzxtfxkj.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gxmfqzycc.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gsbxqiltp.sHtML

[U47] PHP：联合类型
来源：http://read.share.zdbjq.cn/Article/details/gjidpdxpk.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gnzlozvrm.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gbuzbwqxs.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gpkhnpbhw.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gbjrvnyof.sHtML

public readonly string $name
来源：http://blog.zdbjq.cn/Article/details/gvffqbofo.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gglizfuwb.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gqvuqbllr.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gdrizsanq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gwbqpgpue.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/glrcwtdlm.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/grfvpzwye.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gdslzylqi.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gxirwitpz.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gmbfbhsfw.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gffjspdus.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gdkmupquf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gkffexnnm.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/gymbktdaq.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/girbbmjii.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqlbvcixn.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gvbrrmhwm.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gdljdzejw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gthbzmibg.sHtML

[U59] PHP：自定义排序
来源：http://m.share.hesvh.cn/Article/details/gywwopewf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gndppvjwk.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gvouveugp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.fehbvm.com/Article/details/gummqyfmk.sHtML

[U61] PHP：正则
来源：http://www.share.fehbvm.com/Article/details/gxnomecvw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gqbalepey.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gcwenlxbh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gjywuesnq.sHtML

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/glsjafcux.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gzlfbxjpy.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/ggdgsptvh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gsjsiqjom.sHtML

[U65] PHP：会话
来源：http://www.m.share.hesvh.cn/Article/details/gkmvmxvhk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsaxobxeo.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.hesvh.cn/Article/details/gcpvevxal.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gnuhgrozm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/goaqmcjli.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gskduuble.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gtqfqoofq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/giahcappk.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/geywlaccu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gdbswibuc.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/guhvamsme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/graeacnah.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gjjtrgnge.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/guavewunw.sHtML

[U72] PHP：写错误日志
来源：http://blog.zdbjq.cn/Article/details/glueokajw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/grbgleuxk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/glpljxaxa.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gwkhpqjoo.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gzasfmrbr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gahcwbnio.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gqkyfftlz.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gweclvasb.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/geogbssze.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gqrrpsvsy.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gsoswidxb.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gtwmzffwy.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gyungpjwu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gjrvfivdj.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gwfzlwjpv.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gobtuszxz.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gbzhupxfs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gnmfdnkov.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gymuptoof.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gttsdotqv.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.zdbjq.cn/Article/details/gogwdbcum.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gmutgsimc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/ghlvlkisl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gpggijdbj.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gpbirtwwf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gsqcozeci.sHtML


<!-- 参考信息 -->