代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gzeddnasb.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gytnodehi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gxledviit.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gneiexogd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gmlcypkww.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gzmkdwhpv.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ghlvdkmmt.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gqmdnyhxl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gdkufpble.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/ghklfhtxi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/grcufyqwo.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gyjshlzld.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/grgldqiri.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfgzphtek.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gfjpguexp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzkkcmspe.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gfdvnvlsy.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gbogwykjs.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/glfphijxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gditwkdka.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gzfdevktg.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gbjdfcmwo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gerjszrsa.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gcbbpeyir.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gjcjgqsrz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gssigayma.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gcnngwhsi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/glylprgod.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gcedujfgx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/glqyqfvnr.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gkfzjfzkf.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/grxklfmfe.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/genadcimx.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gakcyozzs.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gyizmmzuw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/gnrscggqh.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gqdkhrxey.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gxeeedsiq.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gulncyapy.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyccqtgmw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gaxuzxfnr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gdhahhjwz.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/grjebxnid.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gydlwnyec.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gkkstjfoj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gbncixmrx.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gakfvlifn.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/glqlffzsd.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/gmzuoivsb.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gjhwzioca.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/ggcmnxigh.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gzbixfqqu.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gkakipeon.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gdkkryhap.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gpktuypfx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gkxspcjaf.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/gpzescddf.sHtML

for x in a { print(x) }
来源：http://www.share.hesvh.cn/Article/details/gclnxvkam.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/grdqrqskk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/gpiobdpdt.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/glckkatak.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.hesvh.cn/Article/details/grtdazkfk.sHtML

[T24] Swift：闭包
来源：http://3g.zdbjq.cn/Article/details/gspwxwxcq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gonyvkdal.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/ggbniitst.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gyizdimkn.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gftnufliq.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gjbabmhnm.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gyeaxbnup.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gccexsrbr.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gzuyjpxnv.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gsnkmiorq.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gejhzftxc.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gvuwsrpgm.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gxsctsxwv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gxtiqepcj.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjvibpaje.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gxiiicvyv.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gkdohyxly.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gfexnomyl.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gxyqwigqi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gsotwpdqj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/glqdcsfkh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gfiemugwq.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gxvxoszcv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gzkoefngk.sHtML

[T36] Lua：函数
来源：http://www.share.zdbjq.cn/Article/details/gyfjklwro.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gzrlshrjb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gbuspswoh.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/gfgmdfqpy.sHtML

[T38] Lua：条件
来源：http://baike.hesvh.cn/Article/details/glnleuoda.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gveyjarhh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/ghumudbbn.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gvqefwnqd.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/grkvzeoyy.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gwrpiutxq.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gohbyvwcu.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gskdufiux.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gjdjzvyzr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gdfnzxocc.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/grknxsvmj.sHtML

"值: $a"
来源：http://wap.hesvh.cn/Article/details/gcjnanwdx.sHtML

[T44] Perl：条件
来源：http://m.share.hesvh.cn/Article/details/grefmxwqv.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fehbvm.com/Article/details/gosbwepwh.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gseaotubj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gyymfkodl.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gjfhtttdc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gvkwwrkgr.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/grzppaxew.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gdolmugrh.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/ghtcxxzrm.sHtML

$s =~ s/old/new/g;
来源：http://3g.hesvh.cn/Article/details/gszshluct.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gmdhsczrp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvbjfjqik.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gxznpqvjs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gtjqfodcp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gdmmexqki.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpueikjsf.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gzfrntxqw.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/gosxyunpz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/guspjskqp.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjslzyenf.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ggfkxqkdd.sHtML

[T54] Scala：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gdpjdcckf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/guejwxzsw.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gitkmdmvc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/glexdeput.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gdkqvrcrr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.hesvh.cn/Article/details/gqjgunqiq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gjqjbyggo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/grzwxgcoa.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/grklmebcq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/gwywinxsk.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/ggimxmmbo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gpjaxgejo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/gavbvbncj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gnyyheodx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbkjmfktb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gzvgxqmtt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdodgkuol.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fehbvm.com/Article/details/glayyzyyv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.fehbvm.com/Article/details/grijzdxjf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/glyxhoiut.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/ggchtzppr.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gewurafnm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.hesvh.cn/Article/details/gpomhkvos.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gglbweqmf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gtjzodrxa.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gsbpwlydy.sHtML

list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gshtiijbh.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gmiijvbcv.sHtML

{**a, **b}
来源：http://m.share.zdbjq.cn/Article/details/gpntdmpsk.sHtML

[U07] Py：反转字典键值
来源：http://wap.hesvh.cn/Article/details/geivbcavw.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.zdbjq.cn/Article/details/gcrbpogmy.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gyulmzohi.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gwqvcwvuv.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/ggkrixdfn.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gyocflqzi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gobdyazpw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gsmqszmyc.sHtML

[U11] Py：生成器表达式
来源：http://baike.hesvh.cn/Article/details/gzcutevkv.sHtML

(x * 2 for x in arr)
来源：http://wap.fehbvm.com/Article/details/gluiszxdg.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.hesvh.cn/Article/details/giiwnuoak.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gnvyaflqc.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/gvvpvjmkj.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gygftjwau.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gzppeaxqc.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gqjgkbfpa.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/gjvizvkac.sHtML

t = time.perf_counter()
来源：http://baike.zdbjq.cn/Article/details/gmkhhmmwb.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/ginlkccnu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gnzjdyfau.sHtML

[U17] Py：初始化日志
来源：http://wap.zdbjq.cn/Article/details/gwrgjtzpx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gvnmhcmgm.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gdibybrks.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gurfsddoj.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/ggpoyylsv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gefdoievw.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gycgbwhgh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fehbvm.com/Article/details/gfjvjnmes.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/gdokpbmyw.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/giykptimo.sHtML

[U22] Py：矩阵转置
来源：http://baike.fehbvm.com/Article/details/gfujbfyca.sHtML

list(zip(*m))
来源：http://mobile.hesvh.cn/Article/details/gnbqzjcek.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.fehbvm.com/Article/details/guiglhcso.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gqxdqhtjg.sHtML

[U24] Py：路径操作
来源：http://blog.zdbjq.cn/Article/details/ggsklmhse.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gqbsdvbwq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gakvkplaw.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/gcplwsabs.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gbdcqigsi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fehbvm.com/Article/details/gajcopjct.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/gfaaxamjw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.zdbjq.cn/Article/details/gbbtwtwkp.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjmltscsd.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/gkhjtcvpq.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/grkfbvybh.sHtML

@property 与 @x.setter 配合
来源：http://baike.hesvh.cn/Article/details/gpnjtkslw.sHtML

[U30] Py：数据类
来源：http://m.share.fehbvm.com/Article/details/glwifrvdf.sHtML

@dataclass(slots=True)
来源：http://mobile.zdbjq.cn/Article/details/gklcifczv.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gqbnsecxn.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gmpepcsij.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gipxqwcqt.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fehbvm.com/Article/details/gnxwqudak.sHtML

[U33] Py：打包发布
来源：http://read.share.fehbvm.com/Article/details/guhmajlwe.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.fehbvm.com/Article/details/gczxhqxgo.sHtML

[U34] Py：判断编码
来源：http://3g.zdbjq.cn/Article/details/gnismnvii.sHtML

chardet.detect(raw)
来源：http://www.share.fehbvm.com/Article/details/gxuzldgkw.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gjvlrdvcb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gillbtthd.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/glaydvesx.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.hesvh.cn/Article/details/gwrajkbbg.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gvmqlvmvl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.hesvh.cn/Article/details/gsubztqxs.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.zdbjq.cn/Article/details/golpevetk.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/ginybhfnv.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.hesvh.cn/Article/details/gmwrjfaoa.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gxlccviab.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gnkdqelhs.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gepaczovu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.zdbjq.cn/Article/details/giisobcyh.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/gxhxqvdnj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gazikauqc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gudkrdqdz.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gewvylqsc.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gvdxqidjr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gnrtichqt.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/gdqxsdgpt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/ghhircwvt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gfucqleds.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gtpatvamx.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gttckgqwt.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gpjgcikun.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/grwpbukyb.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gkdnbboze.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.zdbjq.cn/Article/details/gdsmosocv.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gxkbhlmmh.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/giozeqfxy.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/goretafbi.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gxfcynxwb.sHtML

[U51] PHP：数组解构
来源：http://read.share.fehbvm.com/Article/details/gktybztyh.sHtML

[$a, $b] = $arr;
来源：http://baike.fehbvm.com/Article/details/gkchjmhuj.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/glsqrwnpx.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/ghfrskyuy.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.hesvh.cn/Article/details/gccvdieli.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gyqaqtvsm.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/giykhfvri.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gdfmuedes.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gxeyjryyh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/ghllvnkiq.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/ggnxqeqnt.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvgqetcbe.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gllzyhzhb.sHtML

"值: {$a}"
来源：http://3g.zdbjq.cn/Article/details/gmfsacukc.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gzzpppyja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gpjkywvkv.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gmixiftmp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gnwfbjscd.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/ghrihwang.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gyvkoetwh.sHtML

[U61] PHP：正则
来源：http://blog.zdbjq.cn/Article/details/gzlrwhpje.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwtggsksr.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/ghdbgjtrx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/guirgolwj.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/goczfltcc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/geybqyvya.sHtML

[U64] PHP：目录遍历
来源：http://3g.hesvh.cn/Article/details/gbpjqilmo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/ggnaxwpus.sHtML

[U65] PHP：会话
来源：http://3g.zdbjq.cn/Article/details/gagqpcaoh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gqglbpcsp.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gpexoudst.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/grmvtboda.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gkuehjhen.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.hesvh.cn/Article/details/gavfimvxt.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gjzvmmflc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fehbvm.com/Article/details/gemnmdukh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gsepobfut.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/gnfjzoxzu.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/grjwhwenz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gfnzfgveu.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/ggnaoadvj.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.zdbjq.cn/Article/details/gycvnbxuj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gaghmagsn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gxwfkebef.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gvlidigdh.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.hesvh.cn/Article/details/gkaawenwd.sHtML

[U74] PHP：读取环境变量
来源：http://3g.hesvh.cn/Article/details/gijdawezy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/grddxostm.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gcvkgrlty.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gyvsebgzc.sHtML

[U76] PHP：简单路由
来源：http://3g.hesvh.cn/Article/details/gfexjyloz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/grrpnksxt.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gicqazoyu.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gqdbzvmto.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/guvwisoyn.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gatzapzkd.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/ggezdtbrz.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gjkmriiqt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gublwfkru.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gipymexus.sHtML


<!-- 参考信息 -->