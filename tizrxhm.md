代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/ggeexzhjp.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gnephcunq.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gakqfcxiq.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ggqqphrob.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gkamkpqez.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/ggikblaaz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/googrzifa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/grfeuwrby.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gyzdqnwrh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtiyksfxt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/giohqnnbm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gznugelcp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gzcsffbea.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gemzchgmq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/ggaqyarjc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gcllageoq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gadlbhqwu.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gpwojphfx.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gfexmeykp.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/ghisudmom.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/grvjaolka.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gigyytcng.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/guojazkrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gwcncqrlo.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/glwrzhcoc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gngejcldr.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/gppgkayms.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gnwjltoau.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gwxxcwgew.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gkazgowgd.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gicvuuqug.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gtjmaoqnj.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gwqvrfygp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/govekpdyf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gwzxgtqep.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmwgkhyix.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gcktlmmpg.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/ggpygbvhc.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/geaygmudr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gvbuwdksc.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/giantlnuo.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtnbeanqb.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkzlttzbl.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gblojhpgo.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/guqueouqn.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/gczklxjpp.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gefctgbnw.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/ghbmbdrde.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gyufwbose.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvigukjif.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/grbvvsjsf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.hesvh.cn/Article/details/glilrmvwx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gxucueuvc.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gycwzkqln.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gzjlieito.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/ghbaiqtyl.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gxjfcufqn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gvzzzvzee.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gwtdagohi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqxaskmur.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gnemygnnk.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gucisvlrn.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gghtglpmo.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gdeendqga.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnzhvznlp.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/giuiyhvfp.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ghxdlitvb.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gwawwromf.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.zdbjq.cn/Article/details/gmxudhefw.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gbfdgrruc.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gifcnguzu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/giizielax.sHtML

[T31] Lua：Hello World
来源：http://baike.hesvh.cn/Article/details/gjgyjcbbo.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gthwwidmz.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gwxvmngjb.sHtML

local a = 1
来源：http://3g.fehbvm.com/Article/details/glvbewuaa.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fehbvm.com/Article/details/gmqkartqq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gbgslbtcq.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/ggqjftwgc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gixqgnqmr.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/gvotdzmqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fehbvm.com/Article/details/gucskmdma.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gqupbhhhl.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gfajkqjwb.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gnmnyjevp.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gqamzsawi.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/gwaqtahaw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gnzafynpp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fehbvm.com/Article/details/ghikwyqth.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gcqlfrciz.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/goutbtvdi.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gnaywfdir.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gefbnjmtd.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/getnkwtrg.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/guupzpgye.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.hesvh.cn/Article/details/gnwmirivo.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gxkqdtzug.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/ggiplfmjn.sHtML

[T44] Perl：条件
来源：http://blog.hesvh.cn/Article/details/gtdizugmy.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/grcvymrvq.sHtML

[T45] Perl：数组遍历
来源：http://baike.fehbvm.com/Article/details/gawtptccr.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gwbrfbuhe.sHtML

[T46] Perl：哈希操作
来源：http://read.share.hesvh.cn/Article/details/gvhemygvd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gpaxunmqt.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gcwgfvwfe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.zdbjq.cn/Article/details/gmbuezwzv.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gfyqcotqb.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gmqjqebls.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gxzckobxc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gzwmkowdd.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/guhsjmwsg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gpmwmclhk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.zdbjq.cn/Article/details/gisaoevan.sHtML

[T51] Scala：Hello World
来源：http://wap.hesvh.cn/Article/details/gcppdtegm.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gmiujurps.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gfqpclgmz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gjiqdbzwd.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gitdqpvjx.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxrknjtru.sHtML

[T54] Scala：集合映射
来源：http://www.share.hesvh.cn/Article/details/gepqjwxrd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyyazqthn.sHtML

[T55] Scala：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gionmpqbz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/glesgucgz.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/glazhgdha.sHtML

case class User(name: String, age: Int)
来源：http://wap.hesvh.cn/Article/details/gmsvfgopw.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gxiqcremk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.fehbvm.com/Article/details/gskxcmrvz.sHtML

[T58] Scala：函数定义
来源：http://3g.hesvh.cn/Article/details/gaxtzyqmv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.zdbjq.cn/Article/details/gfshvpjzd.sHtML

[T59] Scala：循环
来源：http://www.share.hesvh.cn/Article/details/gxeryiaqo.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/geryvfbew.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gxgzubxkc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/guuuvviqg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdauaxz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/ggdvqjvuu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geyiagrle.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.fehbvm.com/Article/details/gahctwbze.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.hesvh.cn/Article/details/gsxgisbdl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gtsjfajoo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gesidkdwg.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.hesvh.cn/Article/details/gifshzxnv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gxnjxfegz.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.hesvh.cn/Article/details/gxaxtsgxg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.fehbvm.com/Article/details/gspjyyaaf.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gjnuubjqq.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gieogsyof.sHtML

[U06] Py：合并两个字典
来源：http://3g.zdbjq.cn/Article/details/gowwakxel.sHtML

{**a, **b}
来源：http://wap.zdbjq.cn/Article/details/ggzjvdscb.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gljivvzwr.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/ghcuautbx.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gnzfsufbr.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gemwtknmt.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/gbaqyybwm.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gukrwkqlz.sHtML

[U10] Py：按值排序字典
来源：http://baike.zdbjq.cn/Article/details/gjabfsjfq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gyyjrboii.sHtML

[U11] Py：生成器表达式
来源：http://read.share.fehbvm.com/Article/details/gmxezihas.sHtML

(x * 2 for x in arr)
来源：http://3g.hesvh.cn/Article/details/gnxpzkssq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fehbvm.com/Article/details/gepbruhio.sHtML

Counter(arr).most_common(3)
来源：http://read.share.zdbjq.cn/Article/details/gsgnyuhds.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/ggrmosidg.sHtML

deque(maxlen=10)
来源：http://3g.hesvh.cn/Article/details/gavjqbgis.sHtML

[U14] Py：分组收集到列表
来源：http://baike.fehbvm.com/Article/details/gqckijjiy.sHtML

defaultdict(list)
来源：http://read.share.hesvh.cn/Article/details/gbvabqbec.sHtML

[U15] Py：高精度计时
来源：http://blog.fehbvm.com/Article/details/gjwarfcjp.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/glbdocxlm.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gcqcjswuz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gofzstsch.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/glnagdsvn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.hesvh.cn/Article/details/gnryakcjp.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/geisxneaa.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/ghddoylef.sHtML

[U19] Py：正则替换带回调
来源：http://baike.zdbjq.cn/Article/details/gevqwwohx.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnguntbdu.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/ghqmgqtzo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/guhivuxjr.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.hesvh.cn/Article/details/gzdjmwglr.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/grashbqyi.sHtML

[U22] Py：矩阵转置
来源：http://3g.hesvh.cn/Article/details/gletdfzmp.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gxtevwnyh.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gjpymhtef.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ggxnzwqsq.sHtML

[U24] Py：路径操作
来源：http://read.share.hesvh.cn/Article/details/gtfdydhsg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gscjmegvq.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gjsmgadtk.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gacxtyxtn.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gbwliuwho.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/ghttohaqg.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gmusklbsy.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gnmxiwiky.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gwqilnzxw.sHtML

UserId = int
来源：http://www.m.share.hesvh.cn/Article/details/giqkaikms.sHtML

[U29] Py：属性校验
来源：http://read.share.hesvh.cn/Article/details/gduspwrhu.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/grxjuwysm.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gutqtomky.sHtML

@dataclass(slots=True)
来源：http://wap.fehbvm.com/Article/details/gcachevuk.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/gwgwdwdjr.sHtML

python -m pytest -q
来源：http://www.blog.fehbvm.com/Article/details/gwkjkrjgh.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/gegsvioyv.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gbowriklo.sHtML

[U33] Py：打包发布
来源：http://www.share.hesvh.cn/Article/details/ghghcxexl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gfvijeyby.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gmygmpzrl.sHtML

chardet.detect(raw)
来源：http://read.share.hesvh.cn/Article/details/ghhsjvtmb.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gsfglmpgq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gfoewelgw.sHtML

[U36] Py：定时任务
来源：http://www.blog.hesvh.cn/Article/details/gcateropd.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.hesvh.cn/Article/details/glofmjysm.sHtML

[U37] Py：读写 Excel
来源：http://3g.hesvh.cn/Article/details/gcriegnzl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.hesvh.cn/Article/details/gqswdgjon.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.hesvh.cn/Article/details/gewlpbiha.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/grssjszhb.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gujzydmje.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gjnqchtpj.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gtzbvrhoo.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/guhdweqym.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gioffctwe.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/giizaepiu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gvbsvxmav.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.fehbvm.com/Article/details/gymvjicpc.sHtML

[U43] PHP：声明命名空间
来源：http://blog.fehbvm.com/Article/details/gkahksjiy.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gztujdwdr.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/givuclzlw.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gwzumijxp.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/grnmtiblu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvfpsucyp.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfrcjbx.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/guiqobtep.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/galnuwrmi.sHtML

int|string $id
来源：http://wap.fehbvm.com/Article/details/getmwcalb.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/gkpnwberd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.zdbjq.cn/Article/details/gpmfcajsp.sHtML

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gmbqqvlus.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gaumdvgit.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gdfirgqba.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.fehbvm.com/Article/details/gtzbqfnid.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gltazggzt.sHtML

[$a, $b] = $arr;
来源：http://mobile.fehbvm.com/Article/details/gynifgdio.sHtML

[U52] PHP：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gdepwtgcn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/golyrkvll.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gbvbqcftu.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gpnyxkfxy.sHtML

[U54] PHP：空安全调用
来源：http://baike.fehbvm.com/Article/details/gagskcjcm.sHtML

$obj?->method()
来源：http://www.share.fehbvm.com/Article/details/gnnjabnzo.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/glhvtxtwk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gvfdfdutv.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/ganonvwmr.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqpdwidkz.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.zdbjq.cn/Article/details/gdrbvgdhl.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gwrwesbmy.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fehbvm.com/Article/details/gpwmfwppv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gyxemerau.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gdgsjenqx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzehdgsv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fehbvm.com/Article/details/gyznxrttk.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gtdepdcuj.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gfetxgjme.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/goyhqpwnr.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/gwhqmxtlh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gkfrzxrye.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gejoouqbb.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gjoroyvyz.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gyziuwgwj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gtyoilldx.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gyijyoglu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fehbvm.com/Article/details/grpnnhfcm.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/ghafsbvfe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gaqtdsnzt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/guqmbcgfa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gahsetvys.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/giewygaib.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/ghskkzptp.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gplvegbei.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gpxzighsb.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fehbvm.com/Article/details/gaixfyvfg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.hesvh.cn/Article/details/ghqnlftpd.sHtML

[U71] PHP：抛出异常
来源：http://wap.fehbvm.com/Article/details/gfjmddfpi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gcpksvyvc.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gxkgecjfz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/ghfozhnnv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.hesvh.cn/Article/details/gyigkwkhx.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/ghahzqvxz.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/ghfzmzxaj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/giccfezud.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/grxloxebn.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/glajfafup.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gqurzjiju.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/giqbkhdcu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/guxotkfdf.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gjgzxlqmf.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gsolhalgj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gbyywrjrs.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gvdmthvqg.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gidjlvmeb.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gnebsgiza.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gcaekjsek.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/guecqwzqo.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gcmnhbxly.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.hesvh.cn/Article/details/gvfbcpwlv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gpphtmvbj.sHtML


<!-- 参考信息 -->