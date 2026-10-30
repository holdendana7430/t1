代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwokuqrrl.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gpycqievj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaymqpir.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrrkobcb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/glphnhowp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gswxipaqz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/glqsbuyne.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofgfjjwo.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gcykmybte.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gapobakww.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkrzuzhy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gaptabvym.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gmalwkcrs.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdivxnrdy.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbpswtiv.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpmnkwal.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gblbbatey.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gognndarc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/grbhqjwfl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrggjwgx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gsecsnpvg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuqcbyuy.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gjjwirssy.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/goxrqvyud.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gmerdngqr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzmcmjpe.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmcegrhg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gmegkvumh.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gxzxdzfiv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyrwsjne.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcrqukgb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzzkmmqo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykhmhiju.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfmsqspks.sHtML

[T14] Kotlin：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gsngupcqz.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzicqcggo.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gtggsztnc.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gnfycftet.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbuvxpof.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjuyeoixt.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwhhjdec.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gmbryuikn.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/giotvdupv.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghopniyof.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/govveluwk.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyassgpsx.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpyjduhwl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrbuilc.sHtML

[T21] Swift：遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmqgnybum.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebvkpglf.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gwelkvkpz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaiiwybh.sHtML

[T23] Swift：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnakbckvb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gdljfcird.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaljayqx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/guwgfqlgi.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gyzfbdmoz.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gvfoeovbs.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/gydfjepkb.sHtML

class A: Base { override func f() {} }
来源：http://blog.fanxiaobao.xyz/Article/details/gadxsxqxz.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzcbjmtb.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkoxqrya.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqxudfpi.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gsspdmyvw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmiptxbv.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gorqfseqi.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gljwfwzir.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhfrgzc.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gnjcoseif.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsazvpku.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/geohppfav.sHtML

local a = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gxhgloxlb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmplsjduq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gtnnhzysq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/grosficnr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gycwxaucs.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/grzvaukyb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/geobfhyim.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilmzdvox.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtjozvgx.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/geazmrcem.sHtML

"a" .. "b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbiurkdbh.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvyaxjopg.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebgqbpzk.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/geqalqxey.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsdyvftq.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhqxsxjd.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfayrsh.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glmpjssfa.sHtML

print "Hello\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvihqmdbc.sHtML

[T42] Perl：变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gxcreeaqk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwvvjdna.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtblmptyz.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwquanpxy.sHtML

[T44] Perl：条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gskbdsmfw.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdiajlik.sHtML

[T45] Perl：数组遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ggbgvzrqk.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gssqhjtbf.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtammoit.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbrrltors.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/guxcopqcf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnivmjleu.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxcrfafep.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdxgrtzw.sHtML

[T49] Perl：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcoxttdz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpsegdgu.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdgbputux.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcxgoszl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmsbytdk.sHtML

[T51] Scala：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmiajuehl.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmmzisuv.sHtML

[T52] Scala：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrigalbk.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpydjgcz.sHtML

[T53] Scala：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxtcqfshm.sHtML

s"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuykkvwv.sHtML

[T54] Scala：集合映射
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgsvnalg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbmshekm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrsmeazq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuksciee.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqnadtkp.sHtML

case class User(name: String, age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhbmyxpn.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gihpqpfbp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuruvhgq.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmfkvwchx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvophfcaw.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdjzxeav.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glwggejio.sHtML

[T60] Scala：折叠
来源：http://3g.fanxiaobao.xyz/Article/details/gnvyikkpu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlitrzzh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjxjsnxn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxkinwtu.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guonujcfp.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrhnabnx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzlvoxib.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbcrxjmq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdmlhyye.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiiyojwv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fanxiaobao.xyz/Article/details/geqoqkoch.sHtML

[U04] Py：变量调试打印
来源：http://baike.fanxiaobao.xyz/Article/details/gjzbswaov.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fanxiaobao.xyz/Article/details/gteichdpg.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fanxiaobao.xyz/Article/details/gwukcimxw.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwljunwfl.sHtML

[U06] Py：合并两个字典
来源：http://3g.fanxiaobao.xyz/Article/details/gefifjjlb.sHtML

{**a, **b}
来源：http://baike.fanxiaobao.xyz/Article/details/ghpmfqhpe.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsofuoupf.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gcvnztytj.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gldzfevhb.sHtML

[y for x in nested for y in x]
来源：http://baike.fanxiaobao.xyz/Article/details/glhvccneg.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gmeiznhji.sHtML

max(d, key=d.get)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhblgnbg.sHtML

[U10] Py：按值排序字典
来源：http://m.share.fanxiaobao.xyz/Article/details/golfyukhq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyxcubtf.sHtML

[U11] Py：生成器表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfabrqwqc.sHtML

(x * 2 for x in arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxshzdiju.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbplmtzmz.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavccuzhv.sHtML

[U13] Py：固定长度队列
来源：http://wap.fanxiaobao.xyz/Article/details/gyzqnaiqn.sHtML

deque(maxlen=10)
来源：http://3g.fanxiaobao.xyz/Article/details/gdxkibafk.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gevdjmdsf.sHtML

defaultdict(list)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgakdkkl.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/gioexwapm.sHtML

t = time.perf_counter()
来源：http://www.share.fanxiaobao.xyz/Article/details/grlyzxedv.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fanxiaobao.xyz/Article/details/gaqemazbz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzoylmdh.sHtML

[U17] Py：初始化日志
来源：http://wap.fanxiaobao.xyz/Article/details/gonugeyuf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbvccjf.sHtML

[U18] Py：预编译正则
来源：http://3g.fanxiaobao.xyz/Article/details/gdhkxhylm.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/ghehcsgap.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.fanxiaobao.xyz/Article/details/guppuiqdt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.fanxiaobao.xyz/Article/details/grpvwdury.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fanxiaobao.xyz/Article/details/gnfpcxfoq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fanxiaobao.xyz/Article/details/glsgiadbo.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fanxiaobao.xyz/Article/details/gulosfahz.sHtML

@contextlib.contextmanager
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmnistb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzgqhroi.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicvsyvgf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwipqtyvj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytawhjbs.sHtML

[U24] Py：路径操作
来源：http://3g.fanxiaobao.xyz/Article/details/gdupymlxd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhqnveiv.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fanxiaobao.xyz/Article/details/guppjtsxy.sHtML

csv.DictReader(f)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwkkarqy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxactaej.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntdwtdhn.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitqcmytg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fanxiaobao.xyz/Article/details/gngqnycgb.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gdyfpweka.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gqwlncezv.sHtML

[U29] Py：属性校验
来源：http://blog.fanxiaobao.xyz/Article/details/gczibbnpc.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttmelbpy.sHtML

[U30] Py：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gslkmjnow.sHtML

@dataclass(slots=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gsqdujnwa.sHtML

[U31] Py：单测
来源：http://blog.fanxiaobao.xyz/Article/details/ggcbyppmz.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gpklrlevl.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjflxgzer.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmfjguck.sHtML

[U33] Py：打包发布
来源：http://blog.fanxiaobao.xyz/Article/details/guvhvmdkn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gfxniiuuj.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbkmpib.sHtML

chardet.detect(raw)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdehcbdr.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gtxhcqoqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrcsphec.sHtML

[U36] Py：定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtvjfmsjc.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fanxiaobao.xyz/Article/details/glvuvnlyg.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtodghrr.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fanxiaobao.xyz/Article/details/gaggynhzw.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvijghdnr.sHtML

Path(__file__).resolve().parent
来源：http://wap.fanxiaobao.xyz/Article/details/gcwhtyqmi.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/ggalrbzes.sHtML

sys.stdout.isatty()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhtffow.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fanxiaobao.xyz/Article/details/ggzskyjoe.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gpdmmwzgi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdytbqo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwbvcbdz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxduwckc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.fanxiaobao.xyz/Article/details/gbznrswmz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgquboi.sHtML

namespace App\Http;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvketjdu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gybbajpnp.sHtML

declare(strict_types=1);
来源：http://wap.fanxiaobao.xyz/Article/details/gtatipnkm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxpvuon.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gchdwehhp.sHtML

[U46] PHP：可空类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gytzoiwqy.sHtML

?string $name = null
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrbknchh.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gahzyeaqv.sHtML

int|string $id
来源：http://wap.fanxiaobao.xyz/Article/details/goryxqtiq.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgoedoah.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsfnqileu.sHtML

[U49] PHP：只读属性
来源：http://www.share.fanxiaobao.xyz/Article/details/grigsuvgf.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gemezbjlc.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdsfdfsa.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvbjhzvp.sHtML

[U51] PHP：数组解构
来源：http://blog.fanxiaobao.xyz/Article/details/gysvsqrvq.sHtML

[$a, $b] = $arr;
来源：http://wap.fanxiaobao.xyz/Article/details/gafaltjdh.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvnswfaoi.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdydsgzq.sHtML

[U53] PHP：空合并运算符
来源：http://baike.fanxiaobao.xyz/Article/details/gxjoogvab.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoowrheo.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gixrxwdml.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsphzcxj.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsenpapqk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/guzujrixs.sHtML

[U56] PHP：命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuhviigg.sHtML

f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxafqbpba.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwmzqlru.sHtML

"值: {$a}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggwqxvojf.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjzkete.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfieokaqp.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdfhmyxg.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxpcdcvo.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gkrzekdii.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbykszmw.sHtML

[U61] PHP：正则
来源：http://www.share.fanxiaobao.xyz/Article/details/gyauycvzl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgwumppw.sHtML

[U62] PHP：日期对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgjeogwk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fanxiaobao.xyz/Article/details/gachbxsvr.sHtML

[U63] PHP：文件读写
来源：http://wap.fanxiaobao.xyz/Article/details/gmprtbeef.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcshehzmn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/giwkwjrcj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fanxiaobao.xyz/Article/details/gvyysjxed.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwrumixx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glhujgqhj.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fanxiaobao.xyz/Article/details/gigooazop.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrozsrrq.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhbpxwgj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpwegbog.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fanxiaobao.xyz/Article/details/gwszjaqqv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fanxiaobao.xyz/Article/details/gxvvedrbb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsesxtwhn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gblkrjusy.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwtvebek.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/giwuzkdot.sHtML

[U71] PHP：抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxfeeonbc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmkryieo.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdczwmbr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gvzonowit.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gquhyqppk.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fanxiaobao.xyz/Article/details/gczskcxvu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grknchuvl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdmienhr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyotgvnm.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/gjykdnufh.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gumuaptes.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdyotkgb.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdknkvxl.sHtML

composer require twig/twig
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhuooivv.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/guggbwcyn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fanxiaobao.xyz/Article/details/gglarzwog.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/ghilbayrp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gypygguks.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmepmrfsu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fanxiaobao.xyz/Article/details/gagcfjshl.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslsavtmr.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gykuxubvq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gtwrxmrfz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghhzoujff.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwhjupfa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzyhcntv.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsytxsyo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymajijkz.sHtML


<!-- 参考信息 -->