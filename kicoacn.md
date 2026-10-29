代发 wailian999

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/giscwpqyc.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gatsjmddu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gybktlqzp.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gnmhzkhwm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/ghntrxmhy.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gvuhtcnad.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gxnyajrum.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gpusmepsy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gruegvvjm.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gwusnrmia.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gzufjlhff.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gxynknjak.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gropaqsur.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/ghmobhlfp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.zdbjq.cn/Article/details/grsitdrnj.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gxokpzwxp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gtuefincq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grkedmdhc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gldzydmtz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gygktzdqg.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gphnxhaaa.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqwjlaubv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gyniyklzd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gopppqass.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gbuoxedum.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/geexxxufa.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gacubeubi.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gvfmrkgfq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/guxgkrkny.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gbcilfwgn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/grvvfhwzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gclnubgnc.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gvaiscxwo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqznbzslw.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gubgpwlyl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gilpobabx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gbghfeewz.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/golebwury.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gerssyxva.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/grwcoxyme.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/ghvopcmnm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gjcrbmnvn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gzdebgodc.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gwdpqmxfu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/gyjtrbstx.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gmnlsvmhr.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gkfwemroe.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/gekfipsgj.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gesdhwdqx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gdljqvpiy.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdgwruuih.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfmkupmsk.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gxbccqmwc.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gshmrnszt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gtnnfxmlt.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gketxeawl.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gchitrgwk.sHtML

if let n = opt { print(n) }
来源：http://read.share.fehbvm.com/Article/details/gicpwwkya.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gqvpebvee.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.hesvh.cn/Article/details/gkixcpmcm.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gptzivvvl.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gndzzmxgl.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gijgprvxv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/gvupaiplw.sHtML

[T23] Swift：函数
来源：http://www.blog.fehbvm.com/Article/details/giboptszp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gzejtpavs.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gwwbuixlx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gerxehraz.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gmllouqnt.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gldqrerem.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gjkqocifv.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvusxdw.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gapaveood.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gfbromjfj.sHtML

[T28] Swift：枚举
来源：http://mobile.fehbvm.com/Article/details/grbjwcoqm.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gcjklipjf.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/grnibmlkr.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gleldjlis.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gqqimpdtl.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fehbvm.com/Article/details/ghxhmsbqk.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/globmkgiy.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gwpxnqdcz.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gtijkmviu.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gjztystav.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbrcjkh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.zdbjq.cn/Article/details/gkjthapmu.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gfhrswdkj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gefehvnga.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gomkefshm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ggvhxpyny.sHtML

[T36] Lua：函数
来源：http://baike.zdbjq.cn/Article/details/gxhfcqkxt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.zdbjq.cn/Article/details/gftwefufv.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gmyqltmze.sHtML

"a" .. "b"
来源：http://m.share.hesvh.cn/Article/details/glyrtlljd.sHtML

[T38] Lua：条件
来源：http://read.share.fehbvm.com/Article/details/gafvmndno.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gkpkafbrf.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gbfonyrke.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/ggbqdegyo.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/gclknzywp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gqcnpzrvj.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtyamuzvx.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gbzcuotyq.sHtML

[T42] Perl：变量类型
来源：http://m.share.hesvh.cn/Article/details/gsxwrmnja.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gcnphxabe.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gegycywuj.sHtML

"值: $a"
来源：http://www.share.zdbjq.cn/Article/details/gpkbzohuf.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gpvdqpjrz.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvapdyfqi.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gwzrgppae.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gclptaaoq.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/grvlbptzf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.fehbvm.com/Article/details/ggkubxxsk.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gocdttklq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/guqzhrplk.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/grecmhpsw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.zdbjq.cn/Article/details/gxdkermiq.sHtML

[T49] Perl：函数
来源：http://3g.hesvh.cn/Article/details/gszmumupj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpyuujgbc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmhfjqaqk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gfiwomkhz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gixolrxuc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glwuyxrem.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/guyqgleux.sHtML

[T52] Scala：变量
来源：http://read.share.fehbvm.com/Article/details/gaijcnsjy.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gnbalagpd.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gafppodbp.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gbfarront.sHtML

[T54] Scala：集合映射
来源：http://read.share.hesvh.cn/Article/details/gqiipyepx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gapzukyqy.sHtML

[T55] Scala：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/giqvjmqfj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gihsjjytz.sHtML

[T56] Scala：样例类
来源：http://3g.fehbvm.com/Article/details/gpmbgluur.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/gttqhirmg.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/ggtisrfak.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gtwkelaql.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gkbylzhly.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.zdbjq.cn/Article/details/gfzihhxdu.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/geaiqdoaw.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gfygcvdea.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gbbxfypio.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/geespjlul.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtyxgchbz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdnscenge.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnjvanpqg.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.fehbvm.com/Article/details/gfuzeyvxn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gdreskpng.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.fehbvm.com/Article/details/gdrvcquou.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.hesvh.cn/Article/details/gqddvykpa.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.hesvh.cn/Article/details/gchojssqh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gayfpyvcq.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/goreoemty.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gcflbswlb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gqzreyrws.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gbqahqqef.sHtML

[U06] Py：合并两个字典
来源：http://www.share.zdbjq.cn/Article/details/gznfmfchw.sHtML

{**a, **b}
来源：http://blog.zdbjq.cn/Article/details/gyhjddlrt.sHtML

[U07] Py：反转字典键值
来源：http://3g.hesvh.cn/Article/details/glekreomp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gxjjgoits.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjnuqtq.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fehbvm.com/Article/details/gtldbpwul.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.hesvh.cn/Article/details/gwwsbbmqb.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gppjemzfu.sHtML

[U10] Py：按值排序字典
来源：http://read.share.zdbjq.cn/Article/details/gyfxbkslf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.fehbvm.com/Article/details/gqsgqqjfo.sHtML

[U11] Py：生成器表达式
来源：http://baike.zdbjq.cn/Article/details/gzvnuuvfz.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/geouwegqc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.hesvh.cn/Article/details/gngfaoile.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gsihopmic.sHtML

[U13] Py：固定长度队列
来源：http://read.share.hesvh.cn/Article/details/ggxonoixe.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gzruqmaoi.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gvcvgwqux.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gmdfdmroc.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gyiqufzbl.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gkrsvviog.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.zdbjq.cn/Article/details/gjulyrzro.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.hesvh.cn/Article/details/gzqkovqgb.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gtuxpyhqn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gwldpkzau.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gbpbptjqe.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gufzkoetq.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gdosjubvf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/glncqyuce.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fehbvm.com/Article/details/gfuchdfyp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.hesvh.cn/Article/details/gicktymnz.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fehbvm.com/Article/details/gygtnezgy.sHtML

@contextlib.contextmanager
来源：http://blog.hesvh.cn/Article/details/guvvbxiau.sHtML

[U22] Py：矩阵转置
来源：http://baike.zdbjq.cn/Article/details/ggwoufznj.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/glkudbufl.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.hesvh.cn/Article/details/gniwkpdsg.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.hesvh.cn/Article/details/gszapqjmd.sHtML

[U24] Py：路径操作
来源：http://www.share.fehbvm.com/Article/details/gxtlopfzx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/giqytbtcs.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gguyooptc.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/gsmoifckr.sHtML

[U26] Py：并发下载
来源：http://3g.hesvh.cn/Article/details/ggybdyuqm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gsmnzytxd.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/gwefdnjkg.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/glafoezgl.sHtML

[U28] Py：类型别名
来源：http://m.share.zdbjq.cn/Article/details/ganpjntjw.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gqgrizzzr.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gsatyrnfh.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gegdlidzn.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gjxepapzw.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gtezdivyz.sHtML

[U31] Py：单测
来源：http://mobile.hesvh.cn/Article/details/gpiaunzci.sHtML

python -m pytest -q
来源：http://mobile.zdbjq.cn/Article/details/ghgefftkp.sHtML

[U32] Py：代码格式化
来源：http://www.share.zdbjq.cn/Article/details/gfdtgcbof.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.hesvh.cn/Article/details/gfkrtsyuq.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/gjcwunyzw.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gcnzsyctn.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gbnfsgwcj.sHtML

chardet.detect(raw)
来源：http://m.share.hesvh.cn/Article/details/gmcbmrsbx.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gwbudfdhd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.fehbvm.com/Article/details/ghzlfgmkm.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gcadgkmla.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/guusbnefb.sHtML

[U37] Py：读写 Excel
来源：http://wap.zdbjq.cn/Article/details/ghqoayqyy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/girimiagv.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.fehbvm.com/Article/details/gdfwvjbhz.sHtML

Path(__file__).resolve().parent
来源：http://3g.fehbvm.com/Article/details/gewvclsiy.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/gwcwffgse.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gikxclmfn.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/grzpvnecr.sHtML

print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gjsoxlooa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gnlhnbhan.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.zdbjq.cn/Article/details/guazihsnu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gdregefwj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gygxjcmzi.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.hesvh.cn/Article/details/gychsfccj.sHtML

namespace App\Http;
来源：http://www.m.share.fehbvm.com/Article/details/gzdxfsdjr.sHtML

[U44] PHP：开启严格类型
来源：http://blog.zdbjq.cn/Article/details/gavuazbwc.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/goaeykgzt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gbtflfcwp.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfdyhgqaz.sHtML

[U46] PHP：可空类型
来源：http://baike.zdbjq.cn/Article/details/gksxxccpi.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gzdvxagjx.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gqqglbzjq.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gakvzzxje.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ghqezpyuw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/glwetktqw.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/ghcelmxhl.sHtML

public readonly string $name
来源：http://m.share.fehbvm.com/Article/details/gadduzkmb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gvvpyvtyb.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fehbvm.com/Article/details/gbienofid.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/golhplgup.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.zdbjq.cn/Article/details/grcgshfai.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzrvbsots.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/ghqgcisuw.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/gehxqssih.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fehbvm.com/Article/details/gwitlwhdy.sHtML

[U54] PHP：空安全调用
来源：http://3g.zdbjq.cn/Article/details/gigqddjxm.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/gkozdaunh.sHtML

[U55] PHP：match 表达式
来源：http://blog.zdbjq.cn/Article/details/glgnyuclz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gjbepjxjs.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/grohbmkzh.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gzrrcrklz.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gtfgzwyrc.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gbbagaraf.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gjymuukuz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.hesvh.cn/Article/details/gpkfosecp.sHtML

[U59] PHP：自定义排序
来源：http://read.share.zdbjq.cn/Article/details/gkikmkvnf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gnplmtktn.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gyjmmktbk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/glimxzdnz.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gwsjqyeuy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gfcreylda.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/glaebmuwa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/ggqjfyuzf.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gvtruzajm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gtmnvdthg.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/ghxpuyfao.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gdsachumr.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/glmkiwkvk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gbkcfmzzu.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/gllrfkugi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gzpggbarr.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gccqfyngf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/gjjbaxlui.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fehbvm.com/Article/details/gpyqjumyz.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/glibdpbsr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gjinlkbaz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gsnowktaf.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gcdiexaxy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gunrwlxuw.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gtjfblvtr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.fehbvm.com/Article/details/gykvyiwsr.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gcdwzvnbr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gumeulyve.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gprloppij.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gizyoiboh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gmknucolk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/giggzstwh.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.zdbjq.cn/Article/details/gibhckusd.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gvxibhoua.sHtML

[U76] PHP：简单路由
来源：http://www.blog.hesvh.cn/Article/details/gpurncltx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gikvefwrt.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gsipkjiwm.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/giwjgxirz.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gbprxnxho.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gzxbmqsjy.sHtML


<!-- 参考信息 -->