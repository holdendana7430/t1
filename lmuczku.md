代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gjgqunbcf.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gmmwjnupq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/guwlbnmfc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gpywjxcdr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/ghaudevqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpiyfizgf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gllllmxzp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gghdbrxfb.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggkyscegp.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gbkzjagdd.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gdslrhbdt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gzvgproak.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gurfbzyjl.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gqappwmqv.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gvjcowwvj.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gwjekuvql.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gjzbohkmi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gsyblrdtm.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gwysarbnm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/goxtyqznf.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/glwamprsu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.hesvh.cn/Article/details/gmkfqlngr.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gmfsjcylz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gidwxgzob.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gqydsdqnf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gfawywxhd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gzormtdqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gqzgwtjfa.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gdufifbfh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gnlmggbkd.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gyosttybu.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gfovdxgkc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gxdhhzpib.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmqablmwk.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gfyhowvsr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gsvbozwnn.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/ghqyqgcgc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gsyqbdkji.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gpdlatydc.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gganrpiek.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gbrpdwewv.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/goivkhpzr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gpmjyrbjm.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gckygwhjn.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gzeswohvr.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gubtleqsm.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gbcwivruo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gwozrffvm.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnghqrycd.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gghajprhv.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/glszxztao.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gnfzubkyw.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gqyxlvsln.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gpamyaujw.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/glmjwmmjq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gywabtdve.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/gswglrzrh.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gttawieda.sHtML

[T26] Swift：类与重写
来源：http://www.blog.hesvh.cn/Article/details/guvlfzwyn.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gobubryzh.sHtML

[T27] Swift：错误处理
来源：http://read.share.fehbvm.com/Article/details/gndhecffu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gwfyjvqxq.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gtvogwdxh.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gpbolpufk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/glwwjqmbe.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gbdtkelxm.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gferdlomz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gdpnhqpui.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gbrparkuw.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxqubwmaf.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gpsyouecw.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/grcmvrxlq.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gavdzlmbe.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ghrvhvjck.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gmgprxdrm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gtaorgzqv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gfyfgqlad.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gwyugezyr.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/ghbsuyaki.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gbiyjvrgw.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gpvluwsby.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gsrjxngcw.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/ghmmdkkhj.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/ghwaynjch.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gnaxrpvty.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gwlyydsbi.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gahzahcad.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gyffwhjkl.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gphruvcyn.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/ghzbftnua.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gxcienmhj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/gyisoczrb.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gnscjahuu.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/glolqwcob.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/gfnfzijhz.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gllconfoq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gltzpjnwr.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gvoiecwgb.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gmaspcwfi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/gnegsrcze.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gbvvddhox.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gdyalvkpz.sHtML

[T48] Perl：正则替换
来源：http://wap.fehbvm.com/Article/details/gpiarimsv.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/ggnxknsjy.sHtML

[T49] Perl：函数
来源：http://www.share.zdbjq.cn/Article/details/gcutqdwtw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/geqrryczu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwqbtfmlm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gekhtuzmd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gxfdbxdqm.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/ghwbnvtqz.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gcnaeagji.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gzubbenod.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/giaulqzkv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gbgigojxe.sHtML

s"值: $b"
来源：http://3g.hesvh.cn/Article/details/goxiuwxrw.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/glfrinokv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/ggbfgxboc.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fehbvm.com/Article/details/golvncdtf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gktntmswf.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmcxxhkte.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/gyicjedcm.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/glfcamavr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gllbxgooe.sHtML

[T58] Scala：函数定义
来源：http://m.share.fehbvm.com/Article/details/ggxipprfy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gxbexqhvm.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gkngimfml.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gzoyowffw.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/goadihgll.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gkgfzgiew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbicnzjxl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gelskvoix.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvicvmhib.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gjcrsrysg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gkiqmhpqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fehbvm.com/Article/details/gxzfsynwb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gnneguelp.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/ghucsbjle.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/geoablfvh.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gwwqjfjoh.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gbtoscghl.sHtML

[U05] Py：列表去重且保序
来源：http://blog.zdbjq.cn/Article/details/gvrxkbwoq.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gwpvbzlsm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gdtclarxk.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gtyhwhdjk.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gyjblfaul.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gmtocpini.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gdkfsyqeo.sHtML

[y for x in nested for y in x]
来源：http://read.share.hesvh.cn/Article/details/geiochbci.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/glzuqblsw.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/grdcivwni.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gsexnxfoo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.zdbjq.cn/Article/details/gzchvwgfw.sHtML

[U11] Py：生成器表达式
来源：http://m.share.hesvh.cn/Article/details/gkopqmeys.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gdymgaosu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/grdtmrykb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gxcbjvpms.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.hesvh.cn/Article/details/ghupltbvt.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gomkshxfy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/gugorztzs.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gsqhbxgqr.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gfgvasbuy.sHtML

t = time.perf_counter()
来源：http://3g.zdbjq.cn/Article/details/gmlbdntic.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxdzoyo.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gssrcigql.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gdtthcmqb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gjnyzmhhy.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gdwyucays.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gzgmlmpfa.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.hesvh.cn/Article/details/gbjwlwjjk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.zdbjq.cn/Article/details/gjoqyqpmr.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/goeonqtlw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.zdbjq.cn/Article/details/gxrzbnpiu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/ggtstxfwj.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/glstjiogf.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gbreyqdmi.sHtML

list(zip(*m))
来源：http://3g.zdbjq.cn/Article/details/gcacdmdzp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gdsdpijen.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.fehbvm.com/Article/details/glzlguqzc.sHtML

[U24] Py：路径操作
来源：http://blog.hesvh.cn/Article/details/gugjhwzhj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdjlpyupf.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fehbvm.com/Article/details/gmffljdbf.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gslbiqavq.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/guhojfinl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/gweilvwos.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gpwndrrqf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fehbvm.com/Article/details/guhgybtik.sHtML

[U28] Py：类型别名
来源：http://read.share.fehbvm.com/Article/details/gxfmzebpx.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/gwmgkmvov.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gegohrclu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/guqbhgxnt.sHtML

[U30] Py：数据类
来源：http://baike.fehbvm.com/Article/details/gegbbcnjv.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjyuteduf.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/gtacfknwm.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gaxwjzhfz.sHtML

[U32] Py：代码格式化
来源：http://baike.zdbjq.cn/Article/details/guxdmlwfv.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gbfddrmpc.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gnhjtadzn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.hesvh.cn/Article/details/ghgoaldon.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/guzjsfndh.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gonzymsrr.sHtML

[U35] Py：发送邮件
来源：http://wap.hesvh.cn/Article/details/gbkblpmlp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gqvoszczb.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gbxixecqf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gpqcqwtuy.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.fehbvm.com/Article/details/geyhrdhlq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gukziucmf.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gywsfvedz.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gidfkrggh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gytgptmkx.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gppnevhld.sHtML

[U40] Py：打印到标准错误
来源：http://blog.zdbjq.cn/Article/details/gqnsntkqk.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/ggjgrqtnx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/grbpjkpdh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.fehbvm.com/Article/details/gqxwhiyuq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.hesvh.cn/Article/details/glwqvdpvv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gumxknqrk.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/guvnoqitu.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gfejwihnl.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/guznapayc.sHtML

declare(strict_types=1);
来源：http://mobile.hesvh.cn/Article/details/gbownylmw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/gbbnmcvcb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gbrmfrdie.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gqtjdxflw.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gxpcgjbaj.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/geghoekjs.sHtML

int|string $id
来源：http://baike.zdbjq.cn/Article/details/gjnnzaypb.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gbktymjtf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/ggdwmzgpr.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/ghvhrrvuf.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gomeslbiu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/gjsergwoa.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gqnfvdjpb.sHtML

[U51] PHP：数组解构
来源：http://blog.zdbjq.cn/Article/details/gplptpkkk.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gazfgtnwv.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/grbiuezid.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gjdhnwdiw.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gjwqedikt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gshlehhym.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gmgamfizm.sHtML

$obj?->method()
来源：http://wap.fehbvm.com/Article/details/gbcptlmbp.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gmpnzpagf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gmfyrnudt.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gfkzxvgvt.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gznzkwnzk.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gvdtsemju.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/goyhukrtl.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gnqkprvry.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fehbvm.com/Article/details/girdnniyr.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gwzoxerxr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gfzluxwke.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/ggntnsgyk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/goqsjitro.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gprddyhxx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghdrmelci.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gezjzjgbt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gtgspkuia.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gwmhqrizt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/ggicamsmf.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/ggcbsjhld.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.zdbjq.cn/Article/details/gwtplzung.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gugvdmpzy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gcasnaqrp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gqthiozhp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gtsyvxmdk.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/goyorfcfz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gzzmgvjxh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.hesvh.cn/Article/details/ghkhpbosw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.zdbjq.cn/Article/details/gajjoutli.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ganjeewjs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gscjtpoja.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gkdhyybqn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gstflwvmj.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/ggkenmbeu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gtlweqeqv.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gnmuhrlca.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gcuwfpume.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gtqdlybag.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gzfewkisd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gucqrjfuy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gamsjfycz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gzavjjryf.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gsybneurv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gzwfonthx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.hesvh.cn/Article/details/gjoeqnqsl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gwdilswme.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gmsvybbww.sHtML

[U78] PHP：单元测试
来源：http://read.share.fehbvm.com/Article/details/glnnrblca.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gvlqfbyrz.sHtML

[U79] PHP：静态分析
来源：http://wap.zdbjq.cn/Article/details/gmpinzxjl.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gdzuuhyxb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gcdcdrwrz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/giujtwksa.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gbsaneshz.sHtML

npm init -y;  npm i express
来源：http://www.blog.hesvh.cn/Article/details/gwtlpirdz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gcowwutfy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/ggbqgglzq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/godglhdho.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmcwucljx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/greasqfmt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gjlwmutoj.sHtML


<!-- 参考信息 -->