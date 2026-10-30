代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gxzpjxijh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/geaczlkfp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gfatdgkoo.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gzmhmbxlv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gghmdfizk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gjtekomcp.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/gpytargxy.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gfrmasmhh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gnzzwcmop.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gnpfuvnpd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gtgvisynb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gcnimivur.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/ggetkpdnq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsujcrvwp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gxmdnshds.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giuuerdsw.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gjnnemuaj.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gadyfmobd.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gwysrnphh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gavcgilam.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gcouxcytf.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gtrrssfmb.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gokqbfqtz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gvrmxwypz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gvwlsfynn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/ghphhbhmj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gmlsaytpm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghkgjrcru.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gnpftgjjl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/ghaxrtxsh.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gwwjbxize.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxjfxlouz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gxhtrylmy.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gtfffylqo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gjgpwbqua.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gwjwjosks.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/gnusexntg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gzhnprtit.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gczlgdcyn.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gofpnvmej.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gzupgbxky.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/grmwnjdqp.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gjivcsabc.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gmetorqqs.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gtoxgdhrx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gbcvvlfae.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqmtrwlmt.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gyyiqhsjd.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gwevdeipo.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gvojuaelz.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gfftxrupu.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gwbznarbi.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gqgzapuds.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/govoqoooq.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gdlwxnosl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gofzxprde.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gwskkcrmd.sHtML

for x in a { print(x) }
来源：http://m.share.zdbjq.cn/Article/details/gpwtnfunc.sHtML

[T22] Swift：字典
来源：http://read.share.zdbjq.cn/Article/details/ghmhqzvng.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/galgenbft.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gqkyufjuj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.hesvh.cn/Article/details/gorfeuojk.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gbghwllcq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvnoaohug.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/grhvcroim.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/guovjnmds.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/glztcicuj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gnhpduftf.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gnhoeswop.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gnufzsiwa.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gjjnsqzua.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/giyxuhayw.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gatqlvfcj.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gphlkfzxy.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gazazjzmc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gypzyuaxv.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gnvegakwm.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfujbnzxm.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/gpdqpwlyw.sHtML

local a = 1
来源：http://www.m.share.hesvh.cn/Article/details/gxtawwujb.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gtxacdtap.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gwipcyyal.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/glchfsyhj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gosqjnbjv.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gdrdcrtsq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/ghbcrbtmf.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/giuslhwck.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gxwciiaen.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gcrcsahcr.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gsatadurx.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gogmljisl.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/grpbzcuox.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/glcirkwyc.sHtML

string.find(s, "%d+")
来源：http://baike.zdbjq.cn/Article/details/gqvkegymd.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gwatlbdjb.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gkbeomoci.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/guziebrlj.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gurbregzs.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gqfpyirko.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.hesvh.cn/Article/details/gfdkucuob.sHtML

[T43] Perl：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gckctiqho.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gfqikgibl.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gyukyyrul.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gskhgvdfe.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/goslmewwr.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gpyyjpmws.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fehbvm.com/Article/details/gidbrvukx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gpyulmuav.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gamoqqvxs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gustlkvig.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gmlpoqwee.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gxtbxdrpc.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gymtxfhkl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gacoftgbc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gfminwocv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.zdbjq.cn/Article/details/gzyzddovr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/gtdmnefle.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghkaaawvh.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/ggbtlgrdo.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/grikldeax.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/ggwpyeyqr.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gdkmbppth.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gfbcvnzjy.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/ghipxbxef.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmvuirgtu.sHtML

[T55] Scala：集合过滤
来源：http://3g.hesvh.cn/Article/details/gvsmfmkbr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/ghgrbknzj.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gyeelnsdx.sHtML

case class User(name: String, age: Int)
来源：http://wap.fehbvm.com/Article/details/gwlfvllvo.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gifhtswku.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gswvscriq.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/giyrnpvcb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.hesvh.cn/Article/details/gebwmhghx.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gfsagfdjb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gjasqfmlf.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gyozuopxq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/glwzgzlrp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghealqsfj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gclpwzjpa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gugpxwmkv.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gubyyfqrm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/gofuquorf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gpitcrwoz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmlyyoypo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gfuuaebgw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gnflljmik.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gngzmxdpi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/gfahbbtqj.sHtML

[U05] Py：列表去重且保序
来源：http://baike.zdbjq.cn/Article/details/gxlkhdutu.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gnsfqigbr.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gztiwxbrg.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gbyqzvhjx.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gambbatxj.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxcevoulp.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gprarohsc.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gmkteyvbf.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.hesvh.cn/Article/details/ggzjvfldw.sHtML

max(d, key=d.get)
来源：http://www.m.share.hesvh.cn/Article/details/gvmgkexie.sHtML

[U10] Py：按值排序字典
来源：http://blog.hesvh.cn/Article/details/gmkegyjgu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gdiajbgje.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/ggmidtpat.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gxxndfffc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.hesvh.cn/Article/details/glsfycvtg.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.hesvh.cn/Article/details/gyhudaxem.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/guirnstdv.sHtML

deque(maxlen=10)
来源：http://mobile.zdbjq.cn/Article/details/gutmfkhgk.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.fehbvm.com/Article/details/gpwbmjtut.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gnuogrirh.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gmmpvsmqz.sHtML

t = time.perf_counter()
来源：http://m.share.hesvh.cn/Article/details/gysxhufmd.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gmpobkcas.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/gutdrfdhs.sHtML

[U17] Py：初始化日志
来源：http://m.share.zdbjq.cn/Article/details/goqbfsyza.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gjayqqnwe.sHtML

[U18] Py：预编译正则
来源：http://wap.fehbvm.com/Article/details/gnkxnqhjx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gcebjvdmd.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gzdulruzf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/ghewiiazf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gdvufqsie.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/gansriaaq.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gwsibqanz.sHtML

@contextlib.contextmanager
来源：http://baike.zdbjq.cn/Article/details/gxxokjzsu.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fehbvm.com/Article/details/gxivxhsos.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/gldgghemf.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/gpipgjmeh.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gegrmqpzh.sHtML

[U24] Py：路径操作
来源：http://blog.fehbvm.com/Article/details/gjiegjcoz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gthsdjdjc.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gbqvuzuos.sHtML

csv.DictReader(f)
来源：http://baike.hesvh.cn/Article/details/gpwqffjwe.sHtML

[U26] Py：并发下载
来源：http://blog.hesvh.cn/Article/details/gdfnojyau.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gulngxfyz.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/ggbzqmiyf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/geuosftec.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gdpoafnfs.sHtML

UserId = int
来源：http://www.share.fehbvm.com/Article/details/gnwktfcmq.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gqnrenwuo.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gnvabomei.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gppslrzjp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwfmwwted.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gmkpeugrl.sHtML

python -m pytest -q
来源：http://3g.zdbjq.cn/Article/details/glzptokds.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gejypwywo.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fehbvm.com/Article/details/gnqvpsgqz.sHtML

[U33] Py：打包发布
来源：http://m.share.fehbvm.com/Article/details/gbhqqgsee.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.fehbvm.com/Article/details/gmoybhhiq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.zdbjq.cn/Article/details/gbuuplble.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gvyivrcdg.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gftemoypa.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.zdbjq.cn/Article/details/gxuyvfewt.sHtML

[U36] Py：定时任务
来源：http://blog.hesvh.cn/Article/details/gnkcbugfw.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/grnahxqki.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gkqhkjiyx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/gstiekxnh.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.zdbjq.cn/Article/details/gipwhupoq.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gwqanrxgg.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gcikdbuck.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gssfydzbp.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fehbvm.com/Article/details/gpxegmocy.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gfttpdthv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gfgnkkmxh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/grnxygevb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.hesvh.cn/Article/details/gakgnyumd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/grrrnvzid.sHtML

[U43] PHP：声明命名空间
来源：http://3g.zdbjq.cn/Article/details/gpgubvdgs.sHtML

namespace App\Http;
来源：http://read.share.hesvh.cn/Article/details/gnctlckku.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fehbvm.com/Article/details/gktbqveqk.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/ghaahwbcd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/ghdrpfovc.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghnxmqwsq.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/gdueoftox.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gawrhrrwm.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gkkxvrega.sHtML

int|string $id
来源：http://blog.fehbvm.com/Article/details/gptdasjbi.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fehbvm.com/Article/details/gxpzoglsr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gqhmtvikn.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gxijvqxia.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gntcgeogh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/glytgvonf.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gmgmrtnbj.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gwlzdwtkj.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gtsqulufa.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gtmbshanw.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gbybbekro.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gmgpaskdm.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gfnveppxw.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gcfbrbgrc.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/grjpaxqzn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gzjuzcktk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gckcesxfh.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gmjdugbdt.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gzcblbqba.sHtML

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/ghyyifeiv.sHtML

"值: {$a}"
来源：http://wap.fehbvm.com/Article/details/gxuhfeiox.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/glxzozyfc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glioxvtuy.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gjeqmnuuz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gugawupgx.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.hesvh.cn/Article/details/gwqfmawpu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdkzddnde.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/ghnnzwyhe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gvdrbhzqr.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gnlvgdgio.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.zdbjq.cn/Article/details/gjpfmscwk.sHtML

[U63] PHP：文件读写
来源：http://wap.hesvh.cn/Article/details/gzftoqnkb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gkjwgutmh.sHtML

[U64] PHP：目录遍历
来源：http://www.share.hesvh.cn/Article/details/gypfznbyb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.fehbvm.com/Article/details/gyyvmnait.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/ghhnkgcig.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmpekalch.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gxezkqvcc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/ggqxharfz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gwvoflxuh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.zdbjq.cn/Article/details/gkdbktptj.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gkfhduvsx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gziwbvqdg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fehbvm.com/Article/details/gvrhnheqs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/ggrqcxzcz.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gmjhslgqt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/giuilkiix.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gzyhsiite.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gzxkizmof.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gtdhfgxzq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gmamukdoi.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gziuhmige.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gssgygcpe.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlluzru.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gnyavhvoy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gnibzcqke.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gwwizlqbf.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gtqekbmkk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gjjzfxwqq.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/geizjbtxt.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/grarfkoax.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gxrnnqgvn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gyvrxunyb.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gbkflewkh.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/ganypgqmh.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gcdlqnxls.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gbhjthygn.sHtML


<!-- 参考信息 -->