代发 wailian999

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/grxljnprt.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gkjzgxbmj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gmhkodhkk.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gsqvllpjw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/golwztxxq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/geegicwar.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gafeeoulh.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/grycnhrin.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gmaoqzaqj.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gzvihfirl.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/giltauctb.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gcghnvage.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/guisbeccb.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/guvshvvgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gvyveefoq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gpummqzvl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gnmgjbgyf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsjkmdhrh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtmcjeert.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqquplfqv.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtuknyjtt.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gmymbzvns.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/garuvjvsb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gwqnjmizj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gtvkagmeq.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gmrjyziyi.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gyfmrutjn.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gcbmiwwwf.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gqvqemwqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gtwepdddx.sHtML

[T06] Kotlin：集合映射
来源：http://blog.zdbjq.cn/Article/details/gibuhpvoz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gxaifvfrb.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gcqoapvpj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/galeqjwyo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gbhqoxywe.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gdzixwsfe.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/grdtjeqaa.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gfftizleh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gtiryjhlq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gjedqfird.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gypkylame.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gtmmhbjzr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gjmvmzfdi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gdodmwmyn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/gtvyonase.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ggdtjqbuc.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/gxcauhsck.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gioidbido.sHtML

[T15] Kotlin：接口
来源：http://wap.hesvh.cn/Article/details/gddgrcnec.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gduwdceez.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gnzbfbobw.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gvqyypftj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/guawytwmc.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gxxyoxeug.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/ggliccfvg.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gwobjyhxc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/ggskoumto.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gleydvmpb.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/goyvvzoqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gnqhijodc.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/garkkffkb.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/gufrnmyvz.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/gcyhaceqt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gtgsyxixt.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/ggzvncdsa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gsdzahnrh.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gfayliwyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnxsnhdwy.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gzqcfoxzn.sHtML

struct P { var x: Int }
来源：http://wap.zdbjq.cn/Article/details/guzdhrdav.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gztizlhtm.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gbiksvcbx.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gleuohpig.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gxhrscxpx.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/globbwkzj.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gklsntzgd.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gqgfbqand.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/gvvtbvlmp.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gtgjfbfpe.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gpatmrjbz.sHtML

[T31] Lua：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gnlnfzfcq.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/geqdocuir.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gquyhkrfv.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gzohkjmfl.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gczdcnfor.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/ghvrdrslh.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/grdkhbrwn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/ggyyobhzq.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gdwxlmzje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/ghavojdff.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/girwqsqdv.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gxmqhecrf.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gxfbvsjac.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gldrciuav.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gwmkzcxeh.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gvigoogqv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/gtzsgduak.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gjpblfumn.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gdakmtzjv.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fehbvm.com/Article/details/gionizvrr.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqughhgiq.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gcdieoewc.sHtML

[T42] Perl：变量类型
来源：http://www.share.zdbjq.cn/Article/details/guhvlpvld.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gezfdcqrv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gmfuyesuo.sHtML

"值: $a"
来源：http://wap.fehbvm.com/Article/details/gmkxxbmxs.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gisdlyliw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fehbvm.com/Article/details/gigsexzya.sHtML

[T45] Perl：数组遍历
来源：http://3g.zdbjq.cn/Article/details/gtffjvuiy.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/geozgycza.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/ggcubnuln.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/grikykyzr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gqdstyehh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gqmbiniif.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gmundirpe.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gfjpnnvba.sHtML

[T49] Perl：函数
来源：http://baike.fehbvm.com/Article/details/gyrnxjcxi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gstfoiken.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gavrpvgtr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fehbvm.com/Article/details/gbdkkjqmm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gehxhzieu.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxbvjlxit.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gdewqdvvw.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gamsatfwq.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gfgayrfle.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/glktshogu.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gixwttgxi.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gzbudryin.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbbxqqytr.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gihcdhfpm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.zdbjq.cn/Article/details/gbujgkkbc.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/gpbnbqvxg.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gprvqocsu.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gnotyukbc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gxkstyqan.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gpmiwbpid.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/grfvffezv.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/ghyyughkx.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gphbdspdh.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/gcnycemdi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gmzndhilw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdyuterie.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gpxbqcalw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbdenzyid.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gclcqhnrg.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.zdbjq.cn/Article/details/glrtkbpie.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.fehbvm.com/Article/details/gpcguadjf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fehbvm.com/Article/details/gwcqpwtds.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/gqkymmxfs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.zdbjq.cn/Article/details/geugyswsk.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gftougenq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gusqdjsoi.sHtML

[U05] Py：列表去重且保序
来源：http://baike.fehbvm.com/Article/details/gotqfhhyc.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gsgsdtnyz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gcoqsqbha.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/grdfblrmq.sHtML

[U07] Py：反转字典键值
来源：http://baike.zdbjq.cn/Article/details/gkxgmlqds.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.fehbvm.com/Article/details/gzguqxxma.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gtdqcbrty.sHtML

[y for x in nested for y in x]
来源：http://blog.zdbjq.cn/Article/details/gpelaqmxk.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.hesvh.cn/Article/details/gergneqbm.sHtML

max(d, key=d.get)
来源：http://m.share.hesvh.cn/Article/details/gpcvxigva.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gekniykzf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mobile.hesvh.cn/Article/details/gfqfoezey.sHtML

[U11] Py：生成器表达式
来源：http://wap.hesvh.cn/Article/details/gwnfxvncl.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmqclrfsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.hesvh.cn/Article/details/gfpeowxsc.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.zdbjq.cn/Article/details/gniartosx.sHtML

[U13] Py：固定长度队列
来源：http://baike.hesvh.cn/Article/details/grgsnwwnp.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gzalblxxr.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.zdbjq.cn/Article/details/gimmwzame.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gbxzpemer.sHtML

[U15] Py：高精度计时
来源：http://m.share.zdbjq.cn/Article/details/gjeftuurr.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gzrkyoivt.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/gbfvwswuk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.zdbjq.cn/Article/details/gxtgfrdjl.sHtML

[U17] Py：初始化日志
来源：http://mobile.fehbvm.com/Article/details/glogsbfdk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/gwveiuliq.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.fehbvm.com/Article/details/ghyvrnrft.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/glgsslljs.sHtML

[U19] Py：正则替换带回调
来源：http://blog.fehbvm.com/Article/details/gtimmalym.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gijteherg.sHtML

[U20] Py：缓存函数结果
来源：http://baike.zdbjq.cn/Article/details/gftsbnnnm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.hesvh.cn/Article/details/gpftfdwzo.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gnegyrkir.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gokcskdvt.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fehbvm.com/Article/details/gzjaorguf.sHtML

list(zip(*m))
来源：http://blog.fehbvm.com/Article/details/gbllgarqh.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gpyxjrkwp.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gexbopqmd.sHtML

[U24] Py：路径操作
来源：http://wap.hesvh.cn/Article/details/gpktwqrcr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gnbfidfbh.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/gnutdmhzi.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gifwtimdb.sHtML

[U26] Py：并发下载
来源：http://read.share.zdbjq.cn/Article/details/gwvoawtkl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/gytgqtxth.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fehbvm.com/Article/details/gmigqtdzr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/ghufzjaro.sHtML

[U28] Py：类型别名
来源：http://baike.zdbjq.cn/Article/details/gjruqjste.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gcjcljjuh.sHtML

[U29] Py：属性校验
来源：http://wap.fehbvm.com/Article/details/gplkzlzjd.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/gigoptzrh.sHtML

[U30] Py：数据类
来源：http://3g.fehbvm.com/Article/details/govfzuesg.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gkyfkweeh.sHtML

[U31] Py：单测
来源：http://www.m.share.zdbjq.cn/Article/details/gpecprpql.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/glfpbljti.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gseyrbmpc.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/gcrlvyqci.sHtML

[U33] Py：打包发布
来源：http://read.share.hesvh.cn/Article/details/gtyturvxp.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gveysudpi.sHtML

[U34] Py：判断编码
来源：http://www.blog.zdbjq.cn/Article/details/gmiizmxfp.sHtML

chardet.detect(raw)
来源：http://baike.fehbvm.com/Article/details/gnkmhqnyv.sHtML

[U35] Py：发送邮件
来源：http://www.blog.hesvh.cn/Article/details/gejhcoenj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/glgkkdmlw.sHtML

[U36] Py：定时任务
来源：http://read.share.zdbjq.cn/Article/details/ghetjgwrb.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.zdbjq.cn/Article/details/goxnqbsft.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.fehbvm.com/Article/details/gvxptncnp.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/gqiosxlyk.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.zdbjq.cn/Article/details/gmrqkfvvu.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/gbqhafefr.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/goyvmigmv.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gmsepqirw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gywosteab.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gsixhwlpt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gzxpklvzz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.hesvh.cn/Article/details/ggwskjqor.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gorpnoidw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gqtgtmhsg.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/guvoryfbg.sHtML

namespace App\Http;
来源：http://read.share.fehbvm.com/Article/details/gslkipclu.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gysztvmvg.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/gxwbkpqey.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gzdvstrvq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gzxeaoulh.sHtML

[U46] PHP：可空类型
来源：http://baike.fehbvm.com/Article/details/gnwzbmojq.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gkfgxqxbh.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.hesvh.cn/Article/details/gfzbhjvco.sHtML

int|string $id
来源：http://read.share.hesvh.cn/Article/details/geckzfciw.sHtML

[U48] PHP：纯枚举
来源：http://wap.fehbvm.com/Article/details/gboiimurh.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqymjyqqz.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.zdbjq.cn/Article/details/gevdwciqe.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gmijviygp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.fehbvm.com/Article/details/gsxttgqfw.sHtML

public function __construct(private int $id) {}
来源：http://3g.zdbjq.cn/Article/details/gfngktoke.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/ghnxrzfwc.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/gptljxrim.sHtML

[U52] PHP：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gzummnozp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gfqmcmdyq.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/gzwcbzwud.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.hesvh.cn/Article/details/gcqmsvuik.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/gpfzlgezz.sHtML

$obj?->method()
来源：http://m.share.zdbjq.cn/Article/details/gwfksxopx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.hesvh.cn/Article/details/gqlldlqqn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/griprbnds.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gazfhoepj.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gyjpsgptj.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gknumzaxa.sHtML

"值: {$a}"
来源：http://www.share.zdbjq.cn/Article/details/gnfjcrkem.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/gepefmoiu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gwmdnbrbx.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/givskfkwa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gfwdihduo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gepgwbzwn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gcxarafqg.sHtML

[U61] PHP：正则
来源：http://m.share.fehbvm.com/Article/details/gkfqfpqem.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gtvcuyhkp.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/grtumapcw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gijinrhhw.sHtML

[U63] PHP：文件读写
来源：http://blog.zdbjq.cn/Article/details/gwfadjgwh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.hesvh.cn/Article/details/gurjicljg.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggnfpxkzz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gkdddxnfz.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/grpommkgj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gayagzxnr.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/girwsyfze.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gdrgeuwxj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.hesvh.cn/Article/details/getfvifbw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gyfwzapnl.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gkemgswwo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gxsijoiuo.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gctjdnkxg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gdvkodgyq.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gayjvzpux.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/ghctrxijh.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjgreqn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.fehbvm.com/Article/details/gfrhrdcmu.sHtML

[U72] PHP：写错误日志
来源：http://read.share.zdbjq.cn/Article/details/glficgjnf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gwnqkojta.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gqbdlahim.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gombkquup.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gmwiztzme.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gmftblvhm.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gyodeiomg.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/grcmveohg.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fehbvm.com/Article/details/gpmqqgopu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/gcxqupwlu.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gmecrktmi.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gbeqoqzdb.sHtML

[U78] PHP：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gufkdewgj.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gbtuyxbsy.sHtML


<!-- 参考信息 -->