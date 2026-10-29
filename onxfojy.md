代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.hesvh.cn/Article/details/garpzooiu.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gzkfeyfit.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gvarrzawt.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/glnoobfua.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmlzrcffn.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gphzfvyeh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gdasmlyph.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gjkikfshq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gktaaekes.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfxccydsr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gtfxuzfvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqygfcfki.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gbbdwcpwx.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfubliril.sHtML

[T02] Kotlin：变量
来源：http://wap.fehbvm.com/Article/details/ghmhujcxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/grzclikmp.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gtxfmrxmv.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gphznkpui.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gtrhiuplk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gjodzdikk.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/godzqsrxx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gycjmgqry.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gjvhrynjh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gpypsxjie.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gxeotsrsz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gjcphijzk.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/girzitcpx.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gxedxhblb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gitbosaqx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gojepyanz.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gamowhfqw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/gusuyckzg.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gsvuaccxm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.zdbjq.cn/Article/details/gfphpatwp.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/ggvhnaedn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/godlcskex.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/ggictlpmd.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gragjzonb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gzxjuumgx.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gljnsrjha.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gqdaovaat.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gbnklykqa.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvrrblucx.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcmzakekh.sHtML

[T17] Swift：变量与常量
来源：http://blog.fehbvm.com/Article/details/glzlkxqic.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gsuymghng.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gibujxdni.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gezexbeiv.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gocdwhcyz.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/ggncmfvdn.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gyindppmb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/glmkylwfe.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gstrdbuvu.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gouynhndv.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/gjvkjgqjz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gkeciqxgj.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/gonruzwpe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gjgsdpvte.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gxxqilkvh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghzjsxstq.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gnpuxiofu.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gidkmjdva.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gzmklvplq.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gqvocxjst.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggvcnryib.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gkcezsrqm.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gkpvvzslv.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gbkrjefby.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gvtwlsojb.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gweysjajq.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gvwtdyldl.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/geynwdfps.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmourylfb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggtqspmhv.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gcauvkmaq.sHtML

local a = 1
来源：http://read.share.zdbjq.cn/Article/details/gpnsprelr.sHtML

[T33] Lua：表（数组）
来源：http://read.share.zdbjq.cn/Article/details/gbjpzgklq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gvalguzwr.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/gqjcfmazg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gzrprxsqr.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gnodlvofo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gqjzyjvrm.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gtyldhygp.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gsevlxtyq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gdkvxfqjo.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gctrsqsqa.sHtML

[T38] Lua：条件
来源：http://www.share.fehbvm.com/Article/details/gcuggpshz.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gmdbavwyt.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzqbqraox.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gruhlkbju.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gxdgiadun.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fehbvm.com/Article/details/giyoxomuh.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gixurfbrj.sHtML

print "Hello\n";
来源：http://www.m.share.hesvh.cn/Article/details/gllxkkilo.sHtML

[T42] Perl：变量类型
来源：http://read.share.hesvh.cn/Article/details/golegzakj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fehbvm.com/Article/details/gqpybknlj.sHtML

[T43] Perl：字符串插值
来源：http://baike.hesvh.cn/Article/details/goskhwmdw.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gwcujuvhe.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/ggmdsugla.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gemtczcgr.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/gwerlpunk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gfujwiurz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/ghwmpnrdk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtawokut.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/gohmdgthd.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.hesvh.cn/Article/details/gahsjqxll.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gkbeyxxti.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gmkdysrso.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gidhxllqa.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/geebibmvb.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gsxrzjrlu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gpookotpf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gzxjhxtdo.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gnrzuabmb.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/gbqqxhxoj.sHtML

[T52] Scala：变量
来源：http://www.share.hesvh.cn/Article/details/gtkkpytzk.sHtML

val a = 1;  var b = 2
来源：http://wap.zdbjq.cn/Article/details/gqnashfzs.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gjvnmjrfv.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gofddgbpo.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gheekhmlp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gfehfycgs.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvfgkjfyz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gcmwojavf.sHtML

[T56] Scala：样例类
来源：http://www.share.hesvh.cn/Article/details/gczqhbxcz.sHtML

case class User(name: String, age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gldygntbg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gwtzgfonm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gdxrbqdle.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gzsaarptp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.zdbjq.cn/Article/details/gpcmlcnrg.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gzkppwukl.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/griqpxemw.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gcksipfzr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.zdbjq.cn/Article/details/gxqwavdvo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbsafjfqc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gbkayhclr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghxqjvxrg.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/groayesvu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gulcuovid.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fehbvm.com/Article/details/gaqojsqoa.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gzvcgqoap.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fehbvm.com/Article/details/gtxaefeku.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/gvfvvijpq.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gsvfamoop.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.zdbjq.cn/Article/details/gwlcsuwhh.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.zdbjq.cn/Article/details/gkmkilfnc.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gpgwgsvdd.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/gygaiepkf.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gnroxufiz.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gfqzxcegf.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gmvzqmbdo.sHtML

[U08] Py：展平二维列表
来源：http://3g.fehbvm.com/Article/details/gasnbddbx.sHtML

[y for x in nested for y in x]
来源：http://www.blog.hesvh.cn/Article/details/gnbtpjemn.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gacklnuzd.sHtML

max(d, key=d.get)
来源：http://wap.hesvh.cn/Article/details/ghkstcdsa.sHtML

[U10] Py：按值排序字典
来源：http://3g.zdbjq.cn/Article/details/gvzpzqsfv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.zdbjq.cn/Article/details/gzpxbjqxe.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/guygwqnvg.sHtML

(x * 2 for x in arr)
来源：http://read.share.fehbvm.com/Article/details/gvnhivwlh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.hesvh.cn/Article/details/gmlheymyx.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gskaeacql.sHtML

[U13] Py：固定长度队列
来源：http://m.share.zdbjq.cn/Article/details/ggyhbbofq.sHtML

deque(maxlen=10)
来源：http://m.share.zdbjq.cn/Article/details/gmqiaftft.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gturerdud.sHtML

defaultdict(list)
来源：http://blog.fehbvm.com/Article/details/gpanqlemd.sHtML

[U15] Py：高精度计时
来源：http://www.share.fehbvm.com/Article/details/gwtctihut.sHtML

t = time.perf_counter()
来源：http://www.share.hesvh.cn/Article/details/gtasdhudj.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gsurzqlda.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.hesvh.cn/Article/details/glegdvsgz.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gueikuftk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.hesvh.cn/Article/details/giiczhblz.sHtML

[U18] Py：预编译正则
来源：http://baike.fehbvm.com/Article/details/gmcmwihpe.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gpzkenrrk.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.hesvh.cn/Article/details/gddavsaxh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.zdbjq.cn/Article/details/gpctmkofe.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/ghwuaxvzw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/gnhlbqjqc.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.hesvh.cn/Article/details/gyfkhzjkd.sHtML

@contextlib.contextmanager
来源：http://baike.hesvh.cn/Article/details/gzlpultwy.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.hesvh.cn/Article/details/goxgsnkij.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gdrgvneyx.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfmqjws.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/ggkhxnemz.sHtML

[U24] Py：路径操作
来源：http://baike.hesvh.cn/Article/details/gazqwncjh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gjgmkksmd.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gfedkkqer.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gqtzuagwu.sHtML

[U26] Py：并发下载
来源：http://m.share.zdbjq.cn/Article/details/gipeudqbz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gmhwkakjr.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/gacojzibi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.zdbjq.cn/Article/details/gvhacpapa.sHtML

[U28] Py：类型别名
来源：http://m.share.fehbvm.com/Article/details/gctmojixp.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gyqkqclyl.sHtML

[U29] Py：属性校验
来源：http://www.m.share.zdbjq.cn/Article/details/gqzclgzdy.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fehbvm.com/Article/details/gxseykcdg.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/ggmmerkol.sHtML

@dataclass(slots=True)
来源：http://blog.zdbjq.cn/Article/details/gmozdthdw.sHtML

[U31] Py：单测
来源：http://m.share.hesvh.cn/Article/details/gvwywulkc.sHtML

python -m pytest -q
来源：http://read.share.hesvh.cn/Article/details/gkamlygxl.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gpusvoyud.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.zdbjq.cn/Article/details/gwfkdwkqz.sHtML

[U33] Py：打包发布
来源：http://read.share.zdbjq.cn/Article/details/gfwlnujay.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.fehbvm.com/Article/details/gzchpyrza.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gebdftmit.sHtML

chardet.detect(raw)
来源：http://blog.hesvh.cn/Article/details/gsknhbcjg.sHtML

[U35] Py：发送邮件
来源：http://baike.zdbjq.cn/Article/details/gaohtnzbg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gqlvktjft.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gkvkkbzcs.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/gzapkeumx.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gwbahchuw.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/gxeckdyiu.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gvdigmcnw.sHtML

Path(__file__).resolve().parent
来源：http://baike.fehbvm.com/Article/details/ginhpscfq.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/gramakitg.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gzpvztjxr.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gocuemqdg.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gpxmhhkbu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gzauewswk.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.hesvh.cn/Article/details/gsmesqlib.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/geecrjtwx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/giewjoqfc.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gjzcnbkho.sHtML

namespace App\Http;
来源：http://wap.zdbjq.cn/Article/details/gbvelohag.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fehbvm.com/Article/details/gpypwccnf.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gvwfxgwdx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fehbvm.com/Article/details/gyufldroa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gkoklmdqo.sHtML

[U46] PHP：可空类型
来源：http://www.blog.hesvh.cn/Article/details/grnsmrbld.sHtML

?string $name = null
来源：http://blog.zdbjq.cn/Article/details/ggwxbjojv.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gfsuxbgeq.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/ggdjbvzwg.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gvhzbxcie.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/goujdrssr.sHtML

[U49] PHP：只读属性
来源：http://baike.zdbjq.cn/Article/details/gleyzixaz.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/ggwqlhhfo.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.zdbjq.cn/Article/details/gsekbcrxn.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gfymkdymo.sHtML

[U51] PHP：数组解构
来源：http://blog.fehbvm.com/Article/details/gchszytwc.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/gengehxwu.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gfjtxsyns.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fehbvm.com/Article/details/gfoszkewl.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/grzvfbwcv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.fehbvm.com/Article/details/gycafrsdd.sHtML

[U54] PHP：空安全调用
来源：http://m.share.hesvh.cn/Article/details/gbhozhhwa.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/gvsnxqhsb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gvkqqflxq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gpwtvuuyz.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/gryfghked.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/glcmkigok.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gyiyhqdxq.sHtML

"值: {$a}"
来源：http://www.blog.zdbjq.cn/Article/details/gfgookfzh.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gjmpftsjf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gdwhteaam.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/ghyystkee.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gcuptsbtr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gqdyeodnm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gpruyfpzt.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gqluuobhy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/glnvixzvt.sHtML

[U62] PHP：日期对象
来源：http://3g.fehbvm.com/Article/details/goylwflsx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.hesvh.cn/Article/details/glvpsfmrl.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gfoenupvs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.fehbvm.com/Article/details/gbmkkxeqs.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gwcuvxcsx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.hesvh.cn/Article/details/gwraixgsc.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gtowrwiwy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gapuumxsl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gcudmwimw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gpukztkcw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gttodcyso.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gdxehcbya.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fehbvm.com/Article/details/gsinpcmud.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gloicorex.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/guzknvkvq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/gwxestalm.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gyisyidfd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gapajitck.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnkbtfgqk.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gnhnkicvn.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/ggyrffkjy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gpladeyyy.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fehbvm.com/Article/details/gpkbivotd.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gytkvzkod.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/guyllqwix.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gmntilyox.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gxourkdxk.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gydbdltdv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/guepzrdfs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/glrjooept.sHtML

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gyfadkhsd.sHtML

composer require twig/twig
来源：http://blog.hesvh.cn/Article/details/gcrezqeua.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gejubtekl.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/ggzidlaaj.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gawecokyo.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gcabesrnn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gbaqrimdh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.zdbjq.cn/Article/details/gwtgchaxj.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gfcnjscji.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gbxvfazyt.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gkimdgaaa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gkdbfwkls.sHtML


<!-- 参考信息 -->