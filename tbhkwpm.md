代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gdsghhtbs.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gjyccadrq.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gzltmkwyt.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gpxzdptjl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gtfmialmc.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/goifjklsc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/grqfodaex.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/ganqannih.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gkyhatzvr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpnuwddwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/goinsrwpy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjpcmeotx.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gpudujqsg.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gvevxkcgr.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gesaxxgqm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/grmbklayh.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gzbmdojpl.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gapowgwhb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gvlejqoih.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/ggpiocnzr.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gjuxzfyzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gpmvlsqbc.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gonrdjhdr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/govqdoblx.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ggdprrljb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gbbgduaro.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gzovmolbp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gvaqqdirs.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/ggsoeibae.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gjubprwel.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gfqjlzxft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gbuvwmjgp.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gssdnjgaa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gcryzpaba.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gexjrmqmv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/grxdognpe.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gwjykkfci.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gisydnusi.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/ghnfatygs.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gknjctuip.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gjkgnyyhc.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gtlitrcps.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcdbtzlii.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/glgtkqfvx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqemtwt.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gdzawoggt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ghcpzpvkt.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gnmflltix.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/ghhxopdsv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gcwtpbqed.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gouextxse.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/goiiesgkd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/ggklcbglc.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gqtemoijg.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gwapjpbth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvnvbxqaz.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gyjmxypqf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gyreztyvi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gxpxwbnaw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gawjfbsza.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ggtkrltjj.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gugtkufmw.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gidnfmvao.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gzluxehxq.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/guyvjmcyx.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gpkuntdyn.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gglewtxuu.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gtujwcoex.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gjcxvvkfs.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/glrvdljnh.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gfkbbcmhd.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/gozbmmmvv.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/gmrptlgnj.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gtccsijwa.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gjszjfhaa.sHtML

local a = 1
来源：http://blog.fehbvm.com/Article/details/glzpphkgn.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gblnrvlrj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/ggclgoenz.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gzvybhcak.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfqnzjpbc.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/gfgbjticu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fehbvm.com/Article/details/gjlguaskt.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gjtssttxz.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gtzsyivnj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fehbvm.com/Article/details/goqxefurs.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gmlunexbo.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gkayrfksj.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gkirmgwyg.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gftwxffcx.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gafsbnjnq.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/gfyixodyh.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gpsiwwjcb.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gdugherrs.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gdugyizqb.sHtML

[T42] Perl：变量类型
来源：http://blog.fehbvm.com/Article/details/guqkbwrqt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gqhbamunh.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gmkzpslil.sHtML

"值: $a"
来源：http://www.m.share.hesvh.cn/Article/details/gyvmrhqcs.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/guqrauyyy.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gszzcyklp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gndnotuca.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gyejiaprc.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gxpnwvrkg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gtqbnprvv.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gcunupfee.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gsagblrvh.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gewrrfsie.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gcvcjebmi.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gqukmkdyx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grrycudde.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsfgkbbom.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/grbpbgnfj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/glhkqthfa.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvwmccety.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gmylkcwqo.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gocimdflh.sHtML

val a = 1;  var b = 2
来源：http://blog.hesvh.cn/Article/details/gisprvowb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gyaklmejo.sHtML

s"值: $b"
来源：http://wap.hesvh.cn/Article/details/gbzbjfdeg.sHtML

[T54] Scala：集合映射
来源：http://read.share.fehbvm.com/Article/details/gjwlealkn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/godrsdzxs.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gsskihlfa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/gvsdugvih.sHtML

[T56] Scala：样例类
来源：http://baike.zdbjq.cn/Article/details/gwnvrrnai.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/geasdpagr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/goguopdbi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gtnpknqmj.sHtML

[T58] Scala：函数定义
来源：http://mobile.fehbvm.com/Article/details/gogvhrurn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.hesvh.cn/Article/details/gpirdxeqe.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gkzupedle.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.fehbvm.com/Article/details/gxsnhixef.sHtML

[T60] Scala：折叠
来源：http://www.blog.fehbvm.com/Article/details/glebcyjvu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gtvkmxaop.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwqjvbewa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/guhfyyham.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyymfnmkh.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gklotlwfk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.fehbvm.com/Article/details/gpebsfqvs.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gidfbnvqj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/gvadbwxdl.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fehbvm.com/Article/details/gwzfiednm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fehbvm.com/Article/details/gdrjdbtur.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gpxxxpaob.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gokhbkzyl.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.hesvh.cn/Article/details/gyufdfllv.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gjromezvf.sHtML

[U06] Py：合并两个字典
来源：http://3g.hesvh.cn/Article/details/gacfcykhc.sHtML

{**a, **b}
来源：http://m.share.fehbvm.com/Article/details/gduabfyja.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.zdbjq.cn/Article/details/geesfdydp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/gplawgpah.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fehbvm.com/Article/details/gtuqmgycf.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.hesvh.cn/Article/details/gmdgtjjvl.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.hesvh.cn/Article/details/gjeqxfyri.sHtML

max(d, key=d.get)
来源：http://3g.hesvh.cn/Article/details/gjcsggiga.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gjvrzmhja.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.fehbvm.com/Article/details/gwexyprii.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fehbvm.com/Article/details/gvalvioaw.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gitevedtj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.hesvh.cn/Article/details/gbdcbkhmd.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gfgyuwguw.sHtML

[U13] Py：固定长度队列
来源：http://read.share.zdbjq.cn/Article/details/gdtvyworf.sHtML

deque(maxlen=10)
来源：http://blog.zdbjq.cn/Article/details/gmcibxlnq.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/grtzaybts.sHtML

defaultdict(list)
来源：http://3g.hesvh.cn/Article/details/gttxucwlf.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/ganzwtdla.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gsmqzkuqe.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/grkgjtbaq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gmweqazyl.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gxftjnqux.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gpmbzeuee.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gcsokfdzi.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/gvzwcojwc.sHtML

[U19] Py：正则替换带回调
来源：http://baike.hesvh.cn/Article/details/gaiuhtjow.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.hesvh.cn/Article/details/gfrdfdghf.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhoiyoo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/glhtbbxle.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gpkrffwfp.sHtML

@contextlib.contextmanager
来源：http://www.blog.hesvh.cn/Article/details/gbvcsmjuy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/gfkwvqksc.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/gyeofbxla.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.zdbjq.cn/Article/details/gpsurzmzu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gbdnwhgrt.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gzvywsiid.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gqatvtpdw.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.hesvh.cn/Article/details/gumytstsz.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gpjqmhuia.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/gdppuxgnr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gwvrsegph.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/goizvfwch.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gfdzldrpf.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gltbzmnit.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gxoiaxwkp.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gjuxcwveh.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gjdgrzkny.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gagknfcmw.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzyhfgacx.sHtML

[U31] Py：单测
来源：http://baike.fehbvm.com/Article/details/ggltbdjhe.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gdjfiwsmb.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gxtrnagwo.sHtML

ruff format . && ruff check --fix .
来源：http://3g.hesvh.cn/Article/details/gxoqhrfqo.sHtML

[U33] Py：打包发布
来源：http://mobile.fehbvm.com/Article/details/gepjwcohl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gqxppyjab.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/ghmtpabbz.sHtML

chardet.detect(raw)
来源：http://3g.hesvh.cn/Article/details/ggzmlasax.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gtcdluoez.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gzoazhves.sHtML

[U36] Py：定时任务
来源：http://m.share.hesvh.cn/Article/details/gavpiogdk.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fehbvm.com/Article/details/gkuetbglb.sHtML

[U37] Py：读写 Excel
来源：http://www.share.zdbjq.cn/Article/details/gwuacdmbz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/ggrmutpjb.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gjntfjnvc.sHtML

Path(__file__).resolve().parent
来源：http://blog.fehbvm.com/Article/details/gukyhggtu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/gddccpspx.sHtML

sys.stdout.isatty()
来源：http://blog.zdbjq.cn/Article/details/gsbzptwag.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/grqxnpitz.sHtML

print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkubxpswy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gungkdhmo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/ghcvjbzjp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gqzysvcwv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gphtcmpul.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/guwirqgji.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gzsrzsqbq.sHtML

[U44] PHP：开启严格类型
来源：http://baike.zdbjq.cn/Article/details/gsbkdpzwh.sHtML

declare(strict_types=1);
来源：http://m.share.zdbjq.cn/Article/details/gdkbctcpp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gokfibmys.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzwzgegiq.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/gjtwashhz.sHtML

?string $name = null
来源：http://mobile.hesvh.cn/Article/details/gupxthuje.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gqstorvav.sHtML

int|string $id
来源：http://www.share.hesvh.cn/Article/details/gtlirkqoy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gmdyglveh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/grtzjkema.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/ghuleolle.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gavsgwaqc.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gisygohbi.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gabprpept.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/gfyqpqhfi.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gccnultjh.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gevgnlyfl.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gthzljoby.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gykiujnoi.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gzidqgezv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gyhblernz.sHtML

$obj?->method()
来源：http://www.m.share.hesvh.cn/Article/details/gbfsbtzki.sHtML

[U55] PHP：match 表达式
来源：http://read.share.hesvh.cn/Article/details/getakosly.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/grkbtgtjk.sHtML

[U56] PHP：命名参数
来源：http://www.share.zdbjq.cn/Article/details/grmaxuyom.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gddrubobm.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gwyyzaequ.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gtjmhyowg.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gsfqilgwk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gjqmmmcyc.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gnlfejmga.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gbcjhdaxz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gdpcmizxr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gsjdsubfk.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gdmeydycd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/glywwbqbx.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/gvnjxwhzs.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gduzuuzne.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/goewpzxis.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gcxgrejys.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gslenydim.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gvdpzoulj.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gdaaajdwz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/glfnkipkg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gymchcdqm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/glusojjdl.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gcotrvfsr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gzeannspe.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gcgkdvzwa.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gcepegpld.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gavwhkfbf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fehbvm.com/Article/details/goxtltkuj.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/grjgqakth.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gumzlxomx.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gmarekquj.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gyhrzsfjo.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/ggzusoiwy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gzwihjjwp.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gdmdrarcn.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gpsehynwj.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnvhmhrzv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/gfygvivmb.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/gqhxdyqsz.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gpbvfdnia.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/glutpsqss.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gdyrsqorc.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/grjzovsbi.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/geirwlefp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gwgwzzowu.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/grsojuqhd.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gjtiwqznt.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gmwnjwblf.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gvluidzwi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/goeloutmk.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/geqktnoyv.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gxyvpcolr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gmwcceukh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gqqtzdzed.sHtML


<!-- 参考信息 -->