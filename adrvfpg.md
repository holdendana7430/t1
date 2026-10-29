代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/griitufqq.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/grvfpkyrm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/glqdgjdvn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gwdtoovqd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gtmevauty.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggwzzzyaq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gibmwrewc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvweytrl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gftuxlbtc.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gqyxfpkgx.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/ggxkjkrrw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gbmvnxfmw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/geqfdfhcp.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gezpiboce.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gymumtrfo.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gtcakpxsz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gecvetwhn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gjzqaxlfm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gucqgkmsx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzbrguszx.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/giygojdqs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gzvbxwile.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/grogmljyy.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gcxsjimac.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/ghipeqqfu.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvgtmutrc.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gqsqjdogh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gwvxwxtqj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/goumwnkim.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/glpoigyht.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gssehhpjf.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfrjohopk.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/ghqewiapm.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsmvlwcil.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gfjrrqzeq.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gaslxintg.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gausmkklp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gzposlrou.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gfwrutnvg.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gaufcihmr.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/govkpshvz.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/ggukvaxum.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/ggyrckgtx.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gffppylpl.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gwwfodlfr.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gvepqzyfk.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/glhtqyhcv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/grwltcgxi.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/gxerzncyf.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gxepzygkz.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gpyofkuzq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/gktxnwrog.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gvozjdpas.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gtbhdhkub.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gchxaexlh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqdaaopml.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/girsgcikh.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gejxnoams.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gxrihdpty.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gzrxabrkh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnsrbkz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gpongsene.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/ggiaomgkc.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gqfrlmxem.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.zdbjq.cn/Article/details/gicummnzs.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gpzkrodth.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gzteeluel.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gbiqazain.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzsbqnqcs.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/giszizdjm.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gxjzssdzc.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gremppffw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gotfddgui.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdgksgach.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gkspnblpo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gmbajtcue.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gmidokwhr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/glfacyhtc.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gwxgrpxyq.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gvjvorjlv.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gnmnzxsli.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gflocfahi.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/gcmpsucdd.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gmswxrzyo.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fehbvm.com/Article/details/ggwazufhm.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gwqdtvhqp.sHtML

[T40] Lua：元表
来源：http://m.share.zdbjq.cn/Article/details/gbqrivrbo.sHtML

setmetatable({}, { __index = base })
来源：http://3g.zdbjq.cn/Article/details/gtdnoppii.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxmpjefpu.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gexsbhhay.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gryccibjg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gcwkgwyls.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gujhbmwsu.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gqxzwvpeq.sHtML

[T44] Perl：条件
来源：http://read.share.zdbjq.cn/Article/details/geznoymuk.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gckbtmaiz.sHtML

[T45] Perl：数组遍历
来源：http://wap.zdbjq.cn/Article/details/gxdzvajze.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gsdguhpjt.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gdqwhvrqb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/globgypwn.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gkbifskxb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gldyymfmb.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gwxffkjwy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gznsitrgp.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gvvpvqbbh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gycoeandv.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gbtroymee.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gergjnwvb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gfckjbqgt.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gvibcfngk.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gugucbqwa.sHtML

[T52] Scala：变量
来源：http://read.share.zdbjq.cn/Article/details/gvjdedroa.sHtML

val a = 1;  var b = 2
来源：http://blog.fehbvm.com/Article/details/gqcvuvfos.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gculijijd.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/ghrvuvhpl.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/ghrorymqp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gvvtjudya.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gqnbufuwe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gyxxndfoj.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gvhmjxooo.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/goxzggyfn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbwfwbyxb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/gmcfitzvp.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gzwrehrod.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gcqezaqyz.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gkibmgkqv.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gqzkfqygy.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gfskvixon.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gzouxfxdd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtgzjgipo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gmaquqnzh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gceoaywjg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gohjggsyy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.zdbjq.cn/Article/details/gnpwewaoi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.hesvh.cn/Article/details/gkatjxecv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/geltbibst.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gismkplel.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fehbvm.com/Article/details/gfbhednsc.sHtML

[U04] Py：变量调试打印
来源：http://m.share.hesvh.cn/Article/details/ganzydftf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gphceqkjw.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gvoqzhhzs.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gxglfptyl.sHtML

[U06] Py：合并两个字典
来源：http://blog.fehbvm.com/Article/details/gxafcgttx.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/giboykiza.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gklobzubi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fehbvm.com/Article/details/gflxfuuzp.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gvsluxema.sHtML

[y for x in nested for y in x]
来源：http://mobile.fehbvm.com/Article/details/gnmhjhmar.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gsgqrwdoa.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gsqrmbmad.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gjkunjvlq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gibqwbgwl.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/glfuwoeqq.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gomltjcnz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.zdbjq.cn/Article/details/gfrutnktd.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/guuktmzjj.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fehbvm.com/Article/details/gcjpghkdd.sHtML

deque(maxlen=10)
来源：http://www.share.hesvh.cn/Article/details/ghivktzga.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gaxvtihpn.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gbrvhgkie.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gdwdbtqtq.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gfwikjput.sHtML

[U16] Py：命令行参数解析
来源：http://blog.hesvh.cn/Article/details/goxaducpw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gwyqmikoc.sHtML

[U17] Py：初始化日志
来源：http://www.blog.hesvh.cn/Article/details/guackfwkw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gfnslsjow.sHtML

[U18] Py：预编译正则
来源：http://wap.zdbjq.cn/Article/details/grwhlzcrp.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpenahdlg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.hesvh.cn/Article/details/gfvwonycx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.zdbjq.cn/Article/details/gkcbhrdoo.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fehbvm.com/Article/details/garcnxjdi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gqpodlxpx.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/ghfumxmxu.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gnichztqf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gggxonweg.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/glvhzmhqv.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/gezvikols.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.fehbvm.com/Article/details/gufmmcwcs.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gbbglabrs.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/grtygaxvt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gaadgwzlp.sHtML

csv.DictReader(f)
来源：http://www.blog.fehbvm.com/Article/details/gikitnjex.sHtML

[U26] Py：并发下载
来源：http://m.share.hesvh.cn/Article/details/gookpfsrm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/grtpiidmw.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gtxloqogu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gvoyatbvn.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gyqnbtrhf.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gmknpptsd.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/ghnhuatgs.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gkckblwan.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gcqpsoeyj.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/grdqgozir.sHtML

[U31] Py：单测
来源：http://3g.hesvh.cn/Article/details/gdsidgoaq.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/godrnxkwg.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gkdlcqwdi.sHtML

ruff format . && ruff check --fix .
来源：http://baike.hesvh.cn/Article/details/gwbemetlz.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/geovbowuf.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gzmjmhbrj.sHtML

[U34] Py：判断编码
来源：http://blog.zdbjq.cn/Article/details/gtjryvyhx.sHtML

chardet.detect(raw)
来源：http://www.blog.fehbvm.com/Article/details/gedjwhkpb.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gmclfjaxh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.hesvh.cn/Article/details/gpnvkfjly.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gneoshupf.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gngcykvzv.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gmuilugfu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gepbvpitn.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gxtwzugne.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.hesvh.cn/Article/details/gyffemoso.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/geydymsek.sHtML

sys.stdout.isatty()
来源：http://www.m.share.zdbjq.cn/Article/details/gggliykhg.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fehbvm.com/Article/details/gtqyoakzb.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gvqzuwtmm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gxuysewom.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.hesvh.cn/Article/details/gmddnrlwq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/grhkmbzau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gocxsfmqd.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gmiwjvmwq.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/guxtfiglz.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gspyrkotw.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gluebicnr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fehbvm.com/Article/details/gwnqipljj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxadcopae.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gmgekyzhb.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gyndosgzk.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/glppubyhe.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gneztkpzt.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gjtpjwstv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/gcbbjgsdh.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gckunxran.sHtML

public readonly string $name
来源：http://baike.fehbvm.com/Article/details/gnqfswpzu.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/grounrgvw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsdlltfzc.sHtML

[U51] PHP：数组解构
来源：http://read.share.zdbjq.cn/Article/details/gncnjsaiz.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gctilpmdy.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/grzyewemy.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gwoyqcnnt.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gxhwbvzls.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gbkrpsffe.sHtML

[U54] PHP：空安全调用
来源：http://www.share.hesvh.cn/Article/details/gdzafwfbj.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gxmfnkaxd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/geirryilw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gpqeuhjge.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/gutnimile.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gbkgcwobn.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gdzpdywua.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gbjrwvwkz.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gtuxiyjoh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gbyszfaxo.sHtML

[U59] PHP：自定义排序
来源：http://read.share.hesvh.cn/Article/details/gfwxhpflw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gtoxvacjv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gyvfmofwg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/goqvxjdpp.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gsunvheay.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwlkrlbjf.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gznsubdpb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fehbvm.com/Article/details/ghijemkmk.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gngucpnuz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gupwtyugc.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gfrvcpibs.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fehbvm.com/Article/details/glphlhniy.sHtML

[U65] PHP：会话
来源：http://blog.zdbjq.cn/Article/details/ganszjgla.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gdgwgqkvv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gswxujtew.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqaxtims.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.hesvh.cn/Article/details/gdivowywd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/gkiizsfpl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/gecbxeoid.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gyzxykqac.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gjdppzhns.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fehbvm.com/Article/details/gszjviyis.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gcavtfcma.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gfkdjhmmm.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gdzvqgbky.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/gwfpvfhma.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/geoststwr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gmvurcruv.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/grrykjvjx.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gplxggmty.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gnqljfgrd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gkgxdboll.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gnwwiieyq.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gylosibww.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/ggpobrfok.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gbabsiupu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gggbitvns.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gebdxwjqm.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gywexcdlw.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/grmeleqog.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gfazsenne.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gogielnjk.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/ghekfuotb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gfxrkwjgt.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/genafrolz.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/getfbgsdz.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gjzexjdkh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.zdbjq.cn/Article/details/gyscsuszx.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gdugosslj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gcrowjvke.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/gouqttxfp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gyvobxjud.sHtML


<!-- 参考信息 -->