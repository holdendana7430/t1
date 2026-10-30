代发 wailian999

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gwtrhvmqe.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gjqrmbtpy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gliadzbhj.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gljrcktxi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gupuahxae.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gvkzlsajg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gopomtutb.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gpykgicua.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gxgzjrnlt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/glyqibjks.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gxncpkfko.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gjcabwhqy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gzphpztbx.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gpqvefwsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/ggfuyussh.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gphcwyfyv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gbeetnaxv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glwewvemw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gxpdbtdzf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdladxmwn.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbccqbuib.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/ggrxmvrxs.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gzzspibyi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gcdhcoqrb.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gpybjjvyw.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/gamnrxbej.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gcyrbijon.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gasoaelew.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gdhavszmd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gwjmwgowj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gfrgaimkl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gijubmccj.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gskcicicf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gttwzgoug.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/ggxtewiau.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gfdusnjrf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gmyapmeji.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/geitbualr.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gsospmoxc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gvoiosibq.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gzwtmufae.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gmctwcmem.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gonrkyirt.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gaoyodngb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gzgycatur.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxxkvgs.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gcrcepfos.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gkjlcpdrk.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gatrrdnhm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gaaswseop.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gzeeischj.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gmouuuaht.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gmxcbakit.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gjdckldaa.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gzqnyqeqt.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gwypzzdxg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/gjfpzzguw.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gqktgpomw.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ghjxbdbzy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/gpmetdtyb.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/grfwqppqx.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gtaihjsjs.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gypcorpka.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gggbbphbu.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gdgzjxlpk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gojwucdih.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gmaklcwfe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gpicstwrn.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gnzdkjbzw.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gwezzfnaz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gkvwtxbss.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gtgkodafa.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gefbjhrcn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gtfmyxaos.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gvuoyuwyn.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/ggrzzdvua.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gamgzxhxy.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/garynhmxn.sHtML

[T30] Swift：协议
来源：http://read.share.hesvh.cn/Article/details/gndqgyybj.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gyyloqjiw.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gtpggsbcz.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glpyocpvc.sHtML

[T32] Lua：局部变量
来源：http://mobile.hesvh.cn/Article/details/ggkewafep.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/ghsyhmubw.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gqnfejuod.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/ggdfzhuvy.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gjyldoaep.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/ggfvcchhk.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gupfqsakl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gczcgijwv.sHtML

[T36] Lua：函数
来源：http://www.m.share.fehbvm.com/Article/details/gcusudlyx.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gmqqlgjjw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/grwtbbuop.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/grepmdrrd.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gbitthsvu.sHtML

if x > 0 then print("正") end
来源：http://blog.hesvh.cn/Article/details/gxhtngzik.sHtML

[T39] Lua：模式匹配
来源：http://wap.hesvh.cn/Article/details/gcrnslexu.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gojiimsjc.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/goewopavb.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.hesvh.cn/Article/details/gawfdaand.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/geepdqzuz.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gcletehip.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gafowwjnn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/glupatqgr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gtlnkaarx.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/ggubqyrxo.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/grlelbkyu.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gnmcyuxla.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gonqisnct.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gsgoneexg.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/glzqlbemc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/glwcowrzd.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gijhwxpys.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.zdbjq.cn/Article/details/gqefjbuyo.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gefnhqbos.sHtML

$s =~ s/old/new/g;
来源：http://3g.zdbjq.cn/Article/details/gdfdgyvca.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gmcxjtffr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grkzwtfzy.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkjfveouo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/ghinhkxnr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gkitovohk.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gdvnrnrbg.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjkivqnvh.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gwfdgffgd.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gvfgzpfqg.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgvmdcd.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gnhbpactx.sHtML

[T54] Scala：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gmjhhqwrw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gvvetepyk.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gdmjzlfjo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.hesvh.cn/Article/details/giobabvla.sHtML

[T56] Scala：样例类
来源：http://www.blog.fehbvm.com/Article/details/gplvjeyti.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fehbvm.com/Article/details/gaflrtdur.sHtML

[T57] Scala：模式匹配
来源：http://blog.hesvh.cn/Article/details/gwfrniueg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gfadihcyb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fehbvm.com/Article/details/gxpicrjti.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.hesvh.cn/Article/details/gfrvjoegx.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gofyilcvu.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gepngpnbn.sHtML

[T60] Scala：折叠
来源：http://blog.zdbjq.cn/Article/details/gadglhpld.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.zdbjq.cn/Article/details/gfijodqhp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqlpxrdzz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gfgofuffx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqxwhqjiz.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.zdbjq.cn/Article/details/gknsfclrw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gtjvaatfk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/guwqgpwxf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gefwzixet.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/govduhwgn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/gkdgjcegq.sHtML

[U04] Py：变量调试打印
来源：http://wap.hesvh.cn/Article/details/gesxjdasx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/glinyxzvv.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/grgtbadtn.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gerccfecz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gvreudiid.sHtML

{**a, **b}
来源：http://www.m.share.zdbjq.cn/Article/details/ggbhxcaio.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gtrkmvgvj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.hesvh.cn/Article/details/ggdhypnud.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gwuvxnmlr.sHtML

[y for x in nested for y in x]
来源：http://mobile.zdbjq.cn/Article/details/grupuwjpo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gtmlushdv.sHtML

max(d, key=d.get)
来源：http://www.blog.fehbvm.com/Article/details/gayzsdwwr.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gxkjlpmik.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gyipabnul.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gxcziglwr.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gksgvjbui.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gerffdsfm.sHtML

Counter(arr).most_common(3)
来源：http://m.share.hesvh.cn/Article/details/gslquaaml.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/giomcssuj.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gabkclrti.sHtML

[U14] Py：分组收集到列表
来源：http://baike.hesvh.cn/Article/details/gqqjhqnvr.sHtML

defaultdict(list)
来源：http://baike.fehbvm.com/Article/details/gtktlfunk.sHtML

[U15] Py：高精度计时
来源：http://www.blog.hesvh.cn/Article/details/gjyogfbbj.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/gtjighhsf.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/giehaguww.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/geoxkswfk.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gkbjddoti.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.zdbjq.cn/Article/details/gtofdacah.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/gwcjhwffz.sHtML

pat = re.compile(r"\d+")
来源：http://blog.hesvh.cn/Article/details/gxtdnprbr.sHtML

[U19] Py：正则替换带回调
来源：http://wap.zdbjq.cn/Article/details/ghqvtepcm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/ghnmbogqo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gorsytkfz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gssctbynb.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.zdbjq.cn/Article/details/gfuhxnquv.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/gkrdotskv.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gfwestwnm.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gxypmxmyv.sHtML

[U23] Py：分块读取大文件
来源：http://blog.hesvh.cn/Article/details/geoconrwy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.zdbjq.cn/Article/details/gysguzkht.sHtML

[U24] Py：路径操作
来源：http://baike.zdbjq.cn/Article/details/gdkoxjrom.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gkigegxjf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/grgffknxd.sHtML

csv.DictReader(f)
来源：http://3g.zdbjq.cn/Article/details/glgepamza.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/grcentxdy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gwsrekhpu.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.hesvh.cn/Article/details/ggtaitcat.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.hesvh.cn/Article/details/gwggfvtya.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gfuwvertv.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gapqbgepw.sHtML

[U29] Py：属性校验
来源：http://read.share.fehbvm.com/Article/details/gpliacabx.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/glsjpqmxa.sHtML

[U30] Py：数据类
来源：http://mobile.zdbjq.cn/Article/details/gazkxtwgj.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/glldndfhj.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gfheqpwqj.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gmvymhsvk.sHtML

[U32] Py：代码格式化
来源：http://www.blog.hesvh.cn/Article/details/gonxuxkas.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gcjkvuyus.sHtML

[U33] Py：打包发布
来源：http://m.share.zdbjq.cn/Article/details/grqxeyvue.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gikxsubes.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gokqnmsrh.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gurhxuncz.sHtML

[U35] Py：发送邮件
来源：http://3g.hesvh.cn/Article/details/gwlguxaif.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.zdbjq.cn/Article/details/gfpfxjskm.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gwnihqduq.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gtqgvnzwn.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/gkcgxmmcu.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fehbvm.com/Article/details/gwrduwxhn.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gslhdinjf.sHtML

Path(__file__).resolve().parent
来源：http://read.share.hesvh.cn/Article/details/gfwceqtqu.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.fehbvm.com/Article/details/grgsnzwcs.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gnjnhdlre.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gkqvvcpyl.sHtML

print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gvbylmsrj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gizjayqyp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/gynospkrk.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.hesvh.cn/Article/details/gfsnvkdce.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/ghckblmkx.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gwveghgdv.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gvzczxuuy.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gpwyzmxhc.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gkdxuowsl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gkdbhtbfl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gesvxytwj.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gwznoeshv.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gugjffsya.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/gohvmdrus.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gzhhmfeqx.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gtbmbgaih.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gjudjfwye.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gewcztycd.sHtML

public readonly string $name
来源：http://read.share.zdbjq.cn/Article/details/gphrrwdki.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/gyfelrfxw.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gdghcyfvv.sHtML

[U51] PHP：数组解构
来源：http://www.blog.zdbjq.cn/Article/details/gbdpewjvb.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gtrryfsdl.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gswttludb.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.zdbjq.cn/Article/details/gqmubuyex.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gldntdlay.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gclrwctpe.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gihuyxqkq.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gclzzmjfp.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/gkqaebupy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/glyymswfq.sHtML

[U56] PHP：命名参数
来源：http://m.share.fehbvm.com/Article/details/gejrtruoa.sHtML

f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gcuotwzhx.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/givpfpdit.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gyidwnqfk.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gpgucdmav.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.hesvh.cn/Article/details/gocxstrjl.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gyocryake.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gspolvvvx.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gstckrcnz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gpmidjote.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/ghqcsdjjn.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnvnzqagt.sHtML

[U62] PHP：日期对象
来源：http://m.share.hesvh.cn/Article/details/gtagozngc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gonomszjl.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/gydfvshiu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gbreegpof.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gnwdhprqj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/giqkifbsj.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/ggbhzvrgm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gklrphkok.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/granhhjgq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbsicjqte.sHtML

[U67] PHP：处理文件上传
来源：http://wap.zdbjq.cn/Article/details/ggmhcnptr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/gbhqrwmts.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gihsizogp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gynkmwffp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.hesvh.cn/Article/details/ghsvriudw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gcyielfec.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gulzlreiy.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.zdbjq.cn/Article/details/gdaixldpi.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gettkqjlh.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.zdbjq.cn/Article/details/gbucnixii.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gdhihoxot.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fehbvm.com/Article/details/glcjmckgf.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gsmzurhqi.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.zdbjq.cn/Article/details/giosrjvny.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gyhusniyz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gajcmxxcn.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/getbdqizd.sHtML

composer require psr/container
来源：http://wap.zdbjq.cn/Article/details/gycjzevpt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/grxuwctqo.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gvlvzilas.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/geqdqrilz.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gzmkkmpea.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gnakrwfsf.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/ggcyonsxo.sHtML


<!-- 参考信息 -->