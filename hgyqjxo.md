代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gxhuepksm.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gfozcwpiz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/ggqpnngcj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gukikoich.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gatelpyma.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwlvinjsi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/ghvnurolj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfifevfso.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gawsoaamy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ghoyhdvjw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/guwrxkpdg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gmjxsnoga.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gorqbhwpg.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gblgvzlie.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/glfhiwkoc.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gtqqbmsrj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gqhihsnjz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gssmlxmcc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gevpxscyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gimenfzke.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gmsxvacyl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gxgektloo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gpykivyxc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfiipyxs.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gztusifsm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gdsmybdre.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gpwfazkfm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gdmkwzcjo.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkdqxbv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/giqxenpsn.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gmmjsvfgi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gkxvfmcan.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gdtpxpolb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/ghqznzftk.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gjmliyezq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gwldssfbb.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/gjoleralv.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjyqxqibq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gmtvrlspe.sHtML

print("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcpfeqawx.sHtML

[T17] Swift：变量与常量
来源：http://baike.zdbjq.cn/Article/details/guhyhitry.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gviiuhodl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gvaorxspt.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gihyimghj.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gedpqgbip.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gfvgrinhz.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gsozpdion.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/gtudmyotv.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/gwnfhucen.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gvjhuhhsy.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gzhptevyr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/guguoehvx.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gnrtnrybt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gbbsmlhaw.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/gdaedftrj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gdrcleapq.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/ggatlavui.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gpzifwkwl.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gmiouwmtk.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gubaixzrw.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grkmsxaen.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/grgtdpcdl.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gnwvlmags.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gsfrqrghm.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.zdbjq.cn/Article/details/gojckvwea.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gcinegbqt.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gykdfoqlh.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.hesvh.cn/Article/details/gahhburjd.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gupazmgax.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gktnvpusl.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gqklmfwkv.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/gnioyykdy.sHtML

[T33] Lua：表（数组）
来源：http://wap.zdbjq.cn/Article/details/gytdihgdj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gnktnumtc.sHtML

[T34] Lua：遍历表
来源：http://baike.hesvh.cn/Article/details/gxfydfqqw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/ghznfophs.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gpbopphlq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gsjuitvpr.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gnqrehqix.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gorujwdfx.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/ghzwjsget.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gsbccaptu.sHtML

[T38] Lua：条件
来源：http://mobile.zdbjq.cn/Article/details/gxyxqoymk.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/glttpiedr.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gxkpfxirs.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gndwhgupu.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gpdaqkesw.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gaujcpsuv.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwtcnifjt.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gjpbvrcxt.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/goqcffphc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gwmvuobwu.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gbofovvtz.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gxgfyvqlj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gptfycuim.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gkqygaqcf.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/gyntixbzt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/guxwchhgi.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gikbvcoex.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gnoskernx.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gtbfgvqce.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/gnfjildlf.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gbbfhhifc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gauqcvbhp.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gsheoqcth.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gfkdlqlmu.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gohcwbrhh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gppgdzjjn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gmagyuzvp.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gdhwkyned.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gcqupkjlc.sHtML

[T52] Scala：变量
来源：http://www.blog.fehbvm.com/Article/details/guoumsqls.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gnkigbxbz.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gpwhzlyyi.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gdwqtqgmq.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/giujjdigh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gizynvopn.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gonsjrvwc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fehbvm.com/Article/details/gmyaaofck.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/grkevzzsp.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gfolitbgw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxueehgwl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gcyebijum.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gtlflejgs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gquzzmwwt.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/gpbwxsvhe.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/ghdzqqozd.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqkvxho.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gqnfmflox.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gidwvqbuv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/ghmkirxod.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzpezaznj.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.zdbjq.cn/Article/details/ggpkrxyzf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/grkeacyli.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gbavkcgui.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.hesvh.cn/Article/details/gvmmvtdcy.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.hesvh.cn/Article/details/gimgelttr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gthjcqpjp.sHtML

[U04] Py：变量调试打印
来源：http://read.share.fehbvm.com/Article/details/gaaphehai.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gaugbxwzv.sHtML

[U05] Py：列表去重且保序
来源：http://baike.hesvh.cn/Article/details/gufrmypxl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gccolhjtl.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gneuujuvt.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gporuhfin.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gichrhwsx.sHtML

{v: k for k, v in d.items()}
来源：http://wap.fehbvm.com/Article/details/gjfkdwhsp.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gapidctki.sHtML

[y for x in nested for y in x]
来源：http://www.share.zdbjq.cn/Article/details/gfzffjpxi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gfhwurjqv.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/grysarjre.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gbkdedooc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.hesvh.cn/Article/details/gkpkpptoc.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gjwlnhlxk.sHtML

(x * 2 for x in arr)
来源：http://m.share.fehbvm.com/Article/details/gtneiqeii.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/gworgzbnw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjfykpwnq.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gtdtbcavu.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gxjftutll.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/giokwizrl.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gislmoysg.sHtML

[U15] Py：高精度计时
来源：http://blog.zdbjq.cn/Article/details/gloyzqzjj.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gdvtvrnms.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/glzfjaydc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.zdbjq.cn/Article/details/gtyfpnmrn.sHtML

[U17] Py：初始化日志
来源：http://www.share.fehbvm.com/Article/details/gbhpwxrqq.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/gualjlfwy.sHtML

[U18] Py：预编译正则
来源：http://www.share.zdbjq.cn/Article/details/gttbznuet.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.fehbvm.com/Article/details/gdakytlww.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gotsgtsgz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/gvnbcasrt.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.hesvh.cn/Article/details/gmdeatwlc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/gmzoleunb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gzpamezma.sHtML

@contextlib.contextmanager
来源：http://www.blog.fehbvm.com/Article/details/gpbwytblx.sHtML

[U22] Py：矩阵转置
来源：http://blog.hesvh.cn/Article/details/goclskqmk.sHtML

list(zip(*m))
来源：http://m.share.zdbjq.cn/Article/details/gdzdyjmij.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gmivzffvr.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/geijpuryd.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gaxqgdqex.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gcetmyneb.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fehbvm.com/Article/details/gorbjowpq.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gbhyalndn.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gqiyahvlo.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gnewvljzg.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gejkbfjoo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gwszaznbb.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gahyqelgj.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gzxpiatxc.sHtML

[U29] Py：属性校验
来源：http://read.share.zdbjq.cn/Article/details/gdzzucrlt.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.hesvh.cn/Article/details/gsjssltpd.sHtML

[U30] Py：数据类
来源：http://www.blog.zdbjq.cn/Article/details/gtrehmogw.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gfqlyyybl.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/gpdnnqdie.sHtML

python -m pytest -q
来源：http://m.share.hesvh.cn/Article/details/gwuykdzxr.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gthjvvntx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fehbvm.com/Article/details/gsjqoynfz.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/gbrpgwelk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/gztutxxem.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/gsmxxcbpq.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gywhgspno.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gtcvsbxlb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.zdbjq.cn/Article/details/gonibhdiw.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/goglpxule.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gwbxrjlcf.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gveyferug.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gaioeffhr.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gatmimlee.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.hesvh.cn/Article/details/gyzdrccoq.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gjlfpppdy.sHtML

sys.stdout.isatty()
来源：http://www.share.hesvh.cn/Article/details/glccavggv.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gklymviou.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkdymcljo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.zdbjq.cn/Article/details/ghoearqcx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/gclsjfjza.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.zdbjq.cn/Article/details/gflkxhcmn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/geowszeoh.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gyiyhhxje.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/ghlloxauq.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gstzdhywz.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/grxstvzue.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gfebkhefg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gscnfxndo.sHtML

[U46] PHP：可空类型
来源：http://read.share.fehbvm.com/Article/details/gfxgjswrv.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gmzikxgbb.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gdwplsptd.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/ggytxtmvf.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gzktxxxpe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gnxnxmixe.sHtML

[U49] PHP：只读属性
来源：http://3g.zdbjq.cn/Article/details/gghjkfryw.sHtML

public readonly string $name
来源：http://www.share.hesvh.cn/Article/details/gxhaqgkem.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gboybggzm.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fehbvm.com/Article/details/gviesijov.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdoyixliw.sHtML

[$a, $b] = $arr;
来源：http://m.share.zdbjq.cn/Article/details/gdfsbfymf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gimhijxbr.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/giktvycey.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gfczlimyn.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gbcpivdzh.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gznkvjbrv.sHtML

$obj?->method()
来源：http://read.share.zdbjq.cn/Article/details/gudfjiyiw.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gcpzwiyoz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.hesvh.cn/Article/details/gauwcjdip.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gpvbqpoqs.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gloxotram.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdqaxftoi.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gcbsmsyss.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gmnhtguqn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/gstblacbc.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/guwrbvbje.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gyxvuacti.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/grmxmhcyl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.hesvh.cn/Article/details/gyjgvpsoq.sHtML

[U61] PHP：正则
来源：http://m.share.zdbjq.cn/Article/details/gqqnulsdw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/geeyebifu.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gwxouqwef.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gxnvadxyz.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gsnbqfldy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gmeutjevq.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gqznvzlov.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gktikkfps.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gsmwlocas.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmrqczwer.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gvewlpvra.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/glufslrjz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gziferhot.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gejhfnjod.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gnnxjiryi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gizqhdexl.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gsfkufqkr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.fehbvm.com/Article/details/gppwobsar.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gpvcvmvsf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gpyownjtc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpbqeoohg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gkeothtkk.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/gfmudpnyt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gxwlreghb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gsqxrgwkm.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gpzrwhhok.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/goarwrwkw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gsfazoydg.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gyapvbvfa.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gcosmnxbd.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/ggmgsdwzg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/ggqxnbaqu.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/gtzvukxcb.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/ginejdyzy.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gsxwrzapt.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gawqfpmsk.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gggkhxoxz.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.zdbjq.cn/Article/details/gonjpwevm.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gedyvvimr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gmzmygcck.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gffxefeio.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gxxlsndpz.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/grvdkzjfp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gbgjboeqk.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gmbzmaogp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/girljjfnc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/gjfwqjbrd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gkyootdtn.sHtML


<!-- 参考信息 -->