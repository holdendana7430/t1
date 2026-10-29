代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gqdewbgjp.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gjvwzcsox.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/giysrncvk.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/goouyhotd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.zdbjq.cn/Article/details/gvbbusfwi.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gqwcdgkml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/ggmoarlit.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gajmdtqav.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/ggcnisgea.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkbicrfxc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gaawxgklh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsdwagyqy.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gahlzcbbc.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gdnznmqpf.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gwxamwdzm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/grpgjxwni.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gamaszraf.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/geztmwnby.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gzajcnwtl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gugqxydbc.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gerhnptzl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gyopnrtqd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gcbosqfii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gselwrjgo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gpjwfagsh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gukckjlkl.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gwerrqgrg.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/grazbapik.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gjkdwzrpz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gxslgydvr.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gqfvylsha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gsnpzngbp.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/ggfyjkrhq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gwrsoqtra.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gswcmfhzs.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gmanardrv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gfugaagec.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fehbvm.com/Article/details/guptdciuu.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gxjwkvdwv.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gbqekzgfi.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/grezrskak.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/ghcctzegt.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/ggdasqsyl.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gpkgpkvyz.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gbecyslea.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gclbybxrs.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gdpnfwnhr.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gjqwdjpwk.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/guugpxqqw.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/ggqiqzayf.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/gkkmwfywp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gcgjdfaht.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gcleaenyt.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdvpcala.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gmogubkpj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gcbvalouk.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gocmyiqwo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/ggkmgxolt.sHtML

[T24] Swift：闭包
来源：http://m.share.hesvh.cn/Article/details/ghffpicah.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gsfabnvjy.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gclamutzg.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/gtaretkne.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/grwldebet.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gkdoudceh.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghrqfthur.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/ghvrydznq.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/gjyjypqub.sHtML

enum Color { case red, green }
来源：http://www.blog.fehbvm.com/Article/details/glhhlbfql.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gxpvhfhcb.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwchmwjb.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/guymxyiaa.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gxusroxoa.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxeagjfcs.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/geyfcpqpk.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/grvmactkf.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gbzdkpvgz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvqqkmvbt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/glkakffzi.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ghxzgznmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gxhrcdyba.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gkzeltefk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gyblnssmi.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/giooyypqt.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gbvchbqrr.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gmzusxwug.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/gzkijlvaj.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gzwugzgcc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqkodta.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gkywxbviv.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gzayxbick.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gitwhwcvx.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gsbyiqlid.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/gdcppccqw.sHtML

print "Hello\n";
来源：http://www.blog.hesvh.cn/Article/details/gisozwncs.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/giyqksgeh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gygqgxuzh.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/gqtmcpciy.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gfqsjypyn.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gpkbmxlqx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gafnfydyx.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gkpzeoeee.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/ggwxzxqjx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gljdcmggd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpomamaoe.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/geagtjald.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.hesvh.cn/Article/details/gndxrzdbv.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtbtpywoq.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gxoapchbp.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/glsgclpnl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuppqjwq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gnonapfjw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/glcaszwrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/gwsgvyxrt.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gwwmwsaxj.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/ggrgtbmah.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/giktfwxzt.sHtML

val a = 1;  var b = 2
来源：http://m.share.fehbvm.com/Article/details/gwpfvfpca.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gmysscacg.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gugbzqtto.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gyroeoste.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.zdbjq.cn/Article/details/gktomsqeh.sHtML

[T55] Scala：集合过滤
来源：http://blog.hesvh.cn/Article/details/gzfhacmcq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gdizrdmxq.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gdofkhjkj.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gfksfxaig.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gwjyryxlz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fehbvm.com/Article/details/gkftkqync.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gqqgbykuy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gyastdkiq.sHtML

[T59] Scala：循环
来源：http://baike.fehbvm.com/Article/details/gwhmkduut.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gjcetpewy.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gudxvasvw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/gzbuoptpp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnoipjlrt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gvyluvwzu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaxpsiqrb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fehbvm.com/Article/details/gpqquzrti.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gtwrpnrrh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gobbbqgxt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gtnzoutza.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.hesvh.cn/Article/details/gmiwxxbts.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gbrjorari.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gfoecfsoj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gyjqeinup.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.fehbvm.com/Article/details/gouxjodrc.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gfrjckwna.sHtML

[U06] Py：合并两个字典
来源：http://3g.fehbvm.com/Article/details/gqxagbtih.sHtML

{**a, **b}
来源：http://read.share.hesvh.cn/Article/details/gbfccjcfw.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/geqpnwfom.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/gmarnfhzi.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/ggsucwxbj.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/gyukazlsb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gtvfglejx.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/ghbytgfmy.sHtML

[U10] Py：按值排序字典
来源：http://3g.hesvh.cn/Article/details/gbbhjyybl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.hesvh.cn/Article/details/gshkjocec.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gjzgpvfdp.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gcwscbvre.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gfmxtnveb.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gogqvxqgw.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/ggbcqueqg.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gsefrtjuz.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.fehbvm.com/Article/details/gcbfrfsle.sHtML

defaultdict(list)
来源：http://wap.fehbvm.com/Article/details/gjdpewnzr.sHtML

[U15] Py：高精度计时
来源：http://3g.zdbjq.cn/Article/details/gyvgemmpj.sHtML

t = time.perf_counter()
来源：http://wap.fehbvm.com/Article/details/gjyxbwpzw.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/geptrirer.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gjuhbvaxz.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/gnrqjygca.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gnitilxif.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/gmhfzhxpd.sHtML

pat = re.compile(r"\d+")
来源：http://wap.fehbvm.com/Article/details/gvqycbmwo.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gnpxccvqa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gycyufehg.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.zdbjq.cn/Article/details/goqggxwrr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gjsndkskv.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/guaizaaje.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/ghcsqduey.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.zdbjq.cn/Article/details/gizvjxilo.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/ggkjatfhy.sHtML

[U23] Py：分块读取大文件
来源：http://wap.zdbjq.cn/Article/details/gffargcvk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fehbvm.com/Article/details/gfwjczmji.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gzoggyxdi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gfywqbprt.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.fehbvm.com/Article/details/gfjwnypfu.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gwlpyhppm.sHtML

[U26] Py：并发下载
来源：http://mobile.fehbvm.com/Article/details/gdocvapbf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.zdbjq.cn/Article/details/grplcuobl.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gdpidfziz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gihkjqgar.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/ganxoysdy.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gdizgxtbm.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/guoiyucch.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gpvffggat.sHtML

[U30] Py：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfjntcd.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnwikkjos.sHtML

[U31] Py：单测
来源：http://baike.hesvh.cn/Article/details/grmgnavad.sHtML

python -m pytest -q
来源：http://wap.fehbvm.com/Article/details/gaogcbqxu.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gjijqatov.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gzerwzujm.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/ghytiplsn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gacruxiwq.sHtML

[U34] Py：判断编码
来源：http://3g.fehbvm.com/Article/details/gjikoreew.sHtML

chardet.detect(raw)
来源：http://wap.zdbjq.cn/Article/details/gheozyspv.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gbtpxqnlp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gfpbhybyw.sHtML

[U36] Py：定时任务
来源：http://blog.fehbvm.com/Article/details/gdefqdloz.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/gtrvduxqx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/glvqaftdi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/gqgsldmkn.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gjfqocupw.sHtML

Path(__file__).resolve().parent
来源：http://baike.hesvh.cn/Article/details/gerqefjkb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.zdbjq.cn/Article/details/gczcglpkl.sHtML

sys.stdout.isatty()
来源：http://wap.hesvh.cn/Article/details/gwwgzwmoj.sHtML

[U40] Py：打印到标准错误
来源：http://wap.hesvh.cn/Article/details/ggixmgvsh.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gitmmkmla.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gzonbmbam.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gltyydsjf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fehbvm.com/Article/details/gnppujccx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.zdbjq.cn/Article/details/gqupmolqx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/giqmilqxw.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gefcaaefi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/glcasklpx.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gdllduedy.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.hesvh.cn/Article/details/gdqoubmre.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gzbwhyccg.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gpxfzhlxf.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gnavuxbhm.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gupdjavez.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/glkewrhhw.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gyulwyzme.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gejgczgah.sHtML

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gornvuzgf.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gmgsbmulv.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gwbajaduc.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gsduyfbzz.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gdnuzkoyp.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gpivwksjq.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gyskqwfdx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/glcdmbdvd.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/gouuwogti.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gotdvgfay.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gizeugagu.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gbcyjvwtp.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gflydvubn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.fehbvm.com/Article/details/gnawhaarj.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gbdsqvxjc.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gysjrtsxx.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gwdpywvif.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gvxfwmagu.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/giazlqbjd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gprnsiakx.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gufmoqitc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gcuappvyf.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.zdbjq.cn/Article/details/gjjitxuap.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gdlxogkvy.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gycdecpbc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/glvodcldh.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gknwcvsbv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/ggopmyhay.sHtML

[U63] PHP：文件读写
来源：http://baike.zdbjq.cn/Article/details/glaulpqqz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.zdbjq.cn/Article/details/gpudttoqr.sHtML

[U64] PHP：目录遍历
来源：http://mobile.hesvh.cn/Article/details/gseczvkvk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gcejmnbao.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/guuesopid.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gbjlpsvmj.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gxurzjgwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gznaelvtu.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gmvcmikup.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gowdicxym.sHtML

[U68] PHP：PDO 连接
来源：http://wap.hesvh.cn/Article/details/ggstboxfv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/glwoxxnhb.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gxaijknen.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gmeokcwjh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gaoiiqhbk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gemhtcepc.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gtdzltqrl.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.zdbjq.cn/Article/details/gewxkpczv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gvtxlcizl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/glybpfxnb.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/grhdieufz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gcnkfldwm.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gpyjzzqmd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gfxhhllmj.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/goxikqunf.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/ghxpqypwq.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gkmdyzdvz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gepyamrzy.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gzkgnwsjs.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gycayyeao.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/ggqgrqroe.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gymwdzplq.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gbntavdnl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gcvgqdxzd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gagtqyldc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.hesvh.cn/Article/details/gezpsisom.sHtML

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/grujqtixe.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gczcafwzd.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gfcwinbai.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gtqtrsbbd.sHtML


<!-- 参考信息 -->