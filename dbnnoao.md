代发 wailian999

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gnaklgahi.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gvaxoiecd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gtyynsluk.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gsmcadrzp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gkhkwvqad.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/grqvemcty.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gpmtxspbj.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/godnriztk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gxirmeqzp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gopftxcsv.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/glikllkrl.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gyextkseq.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gasrhodqh.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gyxlsuiaw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gpabzyhsc.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gkarnouki.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gttygkgcr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gttbbzfbf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/grdzfalbv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyawfrgag.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gurjnyvyr.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gejdjjyum.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gtftpuwcf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/guobkzvju.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gzwkqhpgo.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gxallvsjw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gzrrzdtet.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gdyzzzfmm.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gnuuxkrcn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gpsthmxrj.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gfhbupldd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwgqylxtd.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gompiscmx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gzemdvhxg.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gijaetsrh.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gsrnbqvsz.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gtgxvwfav.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gtvnwqdon.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gakfytziz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/ggxdxskvz.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ggsriptje.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gmrmsawtv.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gvreebfgw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvkfcmmxu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gnejkscqy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/goelljali.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gkdwzmnkp.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gqjczwzxr.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gmgeparcc.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gouupdupj.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gcqgosobw.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gyxfqmyth.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/govcbcwpj.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/guhnqwajg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gmfawqqls.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gsmwwonku.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gdkhbwwzj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gdpfdrmfw.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gquhoicja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gchwjjveq.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gdukjigvc.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/govdejzcb.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gtzmebsgn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpskozoib.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gwtegwsxk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/glhfhdnek.sHtML

[T24] Swift：闭包
来源：http://m.share.fehbvm.com/Article/details/gqgqzosew.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gvstzmheh.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gbxcpcpzh.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gfwizngxo.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gmrafufbx.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/grkgcshnq.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gynyybgzp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gtebiykov.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gjqhtupkb.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gaaquganb.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gqnrsrayb.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/giuuwxrop.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gnrpuutjv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gwkkwrejz.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gxxqvktfb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gcnpzeude.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gekjbnydw.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gdlivkjca.sHtML

[T33] Lua：表（数组）
来源：http://mobile.hesvh.cn/Article/details/ggrcxxatu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gmuquyvfo.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/ggvpsabup.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gbwucafdu.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/giazxevuy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.hesvh.cn/Article/details/gjukilgyp.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gajovsmdy.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gihjwqgvy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gkjlzrsvi.sHtML

"a" .. "b"
来源：http://baike.fehbvm.com/Article/details/gmjfidxfr.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/ggzjpqlqd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gpuqxnmrs.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gokphhqbo.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gqsmwlpoq.sHtML

[T40] Lua：元表
来源：http://www.m.share.fehbvm.com/Article/details/guzphijvb.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/geooxqlau.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gleouzizx.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/gdzeaezvs.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/ggddifnzm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/ggrsouseh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/ghufjmiou.sHtML

"值: $a"
来源：http://wap.zdbjq.cn/Article/details/gohtcuowi.sHtML

[T44] Perl：条件
来源：http://mobile.zdbjq.cn/Article/details/gvdlfqqjc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnfcrnird.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/ggmprnmcz.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gzqboobva.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.zdbjq.cn/Article/details/gtmixqkni.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuccuik.sHtML

[T47] Perl：正则捕获
来源：http://wap.fehbvm.com/Article/details/gsubnquiy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/ghrmdrgpl.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/geyifdcmp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.hesvh.cn/Article/details/gqcvhkplr.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gzkcvllxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/ghrqzieoj.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/ghcoqfeyn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fehbvm.com/Article/details/gullkvxxz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gkuesjkxr.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gsgydjsij.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gijsjirtb.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gizgckvbc.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gncnvcyrh.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gxwuxudsa.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gaxvkpbke.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gkkdhbqsz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gebxhenpk.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gxhjrawcr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gijlixzwp.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/gwoxvfiid.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/grhjetnxg.sHtML

[T57] Scala：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gezonhvfa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gzswqekac.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/giegdidgn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/gjtyvqnbr.sHtML

[T59] Scala：循环
来源：http://baike.hesvh.cn/Article/details/giezwnzqg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gdqvnolwl.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gjowldwpb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.zdbjq.cn/Article/details/gwjcxhxbn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpfcjrusl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/giifhfqjs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjmbzkyhq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/goaqmctvd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gqmxkbwnk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gfxkbxqqy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvltqdugt.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gxrcyqppd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gzkkidjgh.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fehbvm.com/Article/details/gwldqvdvc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.zdbjq.cn/Article/details/gzsiktyxn.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gdfhuujrd.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gvcmpvzyk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gyajjaqgr.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gjcktclpq.sHtML

[U07] Py：反转字典键值
来源：http://3g.fehbvm.com/Article/details/gcfcwxknq.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fehbvm.com/Article/details/ghmsgmaii.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gtfylxdyf.sHtML

[y for x in nested for y in x]
来源：http://3g.zdbjq.cn/Article/details/gnlzdydvf.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/gqjyrrtpt.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gclgryadk.sHtML

[U10] Py：按值排序字典
来源：http://mobile.hesvh.cn/Article/details/gdrdrcpsv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gqkuxcmce.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gtjqrsqxz.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gjpmagkon.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gpxegnwrz.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gyqbanlij.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gtfolavpt.sHtML

deque(maxlen=10)
来源：http://m.share.fehbvm.com/Article/details/gwzwvfodo.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gtmnswuax.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gbdvwlrqm.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.hesvh.cn/Article/details/grhbyedtf.sHtML

t = time.perf_counter()
来源：http://www.share.fehbvm.com/Article/details/gtcnlgzdl.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gfkhrmeiq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gsmpwywbu.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gllusqnul.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.hesvh.cn/Article/details/gjaqthoxx.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gpvobwxib.sHtML

pat = re.compile(r"\d+")
来源：http://3g.zdbjq.cn/Article/details/giyqojnee.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gaqnkgbul.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.hesvh.cn/Article/details/gckdjsliy.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/gcyyhjyhe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gotqccplt.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/glhvkjcej.sHtML

@contextlib.contextmanager
来源：http://read.share.hesvh.cn/Article/details/gcjtyqrzc.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.fehbvm.com/Article/details/graivzshb.sHtML

list(zip(*m))
来源：http://baike.zdbjq.cn/Article/details/gonyefzuh.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.hesvh.cn/Article/details/gkgzdghkk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.zdbjq.cn/Article/details/gichokjza.sHtML

[U24] Py：路径操作
来源：http://www.m.share.hesvh.cn/Article/details/gjcrqhyja.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gbyxxhmgo.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gxgikkjti.sHtML

csv.DictReader(f)
来源：http://m.share.fehbvm.com/Article/details/goynkxuez.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gzmsvpirw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.zdbjq.cn/Article/details/gwqtxuqlm.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gatjwafqc.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fehbvm.com/Article/details/gaxddrkcn.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gwkrphuvc.sHtML

UserId = int
来源：http://baike.fehbvm.com/Article/details/gtjdpbrvq.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/ghroioalq.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/girulazwt.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gckkyxryo.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gzxeqenab.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/gdconbnpb.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gueltbbag.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/gdobhewwa.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gipluazbr.sHtML

[U33] Py：打包发布
来源：http://m.share.hesvh.cn/Article/details/gzvmzzubz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gdtqfjufc.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/grwosadnv.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gerzxttef.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gqfheljqv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.hesvh.cn/Article/details/gqwgityzu.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/ggqlfqzen.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gnrkeiyvt.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gsjcvbzas.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gldwinjzj.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.hesvh.cn/Article/details/gplxtnzqm.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gqycelxtf.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gazekazki.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gxzovzuwp.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.zdbjq.cn/Article/details/gsuaeqzfp.sHtML

print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gbxhwihqi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.hesvh.cn/Article/details/gdhpbdtzf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gvecxuzgt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gbylsceoo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.fehbvm.com/Article/details/gjpjubibw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggmrknjny.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/givshfifu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.hesvh.cn/Article/details/gafturvkc.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gccsqoipa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gtnbenakg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvqjtbsao.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gipjviblr.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/grvulscbo.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gkaqqxqku.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gtaazolja.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gtoemrdlk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gtpbrykqq.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gsxsopnse.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gjyfchibs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.fehbvm.com/Article/details/gjevcmhaf.sHtML

public function __construct(private int $id) {}
来源：http://www.share.zdbjq.cn/Article/details/gkwjrkfxs.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gihnjysdc.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gaeofgddr.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/grbandubg.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gsncdsiwm.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.hesvh.cn/Article/details/ghtykohmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/ghyfgzcug.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gwowdoyys.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gxgsxgfip.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/getlsifre.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gfjkwwgwg.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/gsyzrjvmw.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gfemopxtw.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gyqvafhjo.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gqxxkqiio.sHtML

[U58] PHP：数组三件套
来源：http://wap.hesvh.cn/Article/details/gbdtibpmr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/gzvdsytjx.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gxvdlswbf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gkylyvlly.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gaqvflkey.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gbupzyfwd.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gibwvfkyt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gmnhxyjlq.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/geerymyph.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gogwctfez.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gmpipkoet.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gbfxzshhb.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gpfuhdpcu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/ghjxktjmn.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/glkrbuxia.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fehbvm.com/Article/details/gljhadxfj.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gpnogljjp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gmzkarlem.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/gudfhoysi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/ghqjlglkj.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmbjtyz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gejvyxljd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/gsmtlmgky.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/gpsowsofy.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/ggtzcdisc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.hesvh.cn/Article/details/gygahamtb.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gvyyssczx.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gvzvwfzeh.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/ggoefjwzy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gqbjczmek.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gjnzevmqk.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gkffewfij.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ggloucmuw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/grewzrvci.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/ggfjokcmn.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gufycnaba.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gdjjpudeg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gfajzirok.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gvjoahkpn.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gsmsppjji.sHtML

[U78] PHP：单元测试
来源：http://www.blog.hesvh.cn/Article/details/giuxspuiv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gdxhrkkkz.sHtML


<!-- 参考信息 -->