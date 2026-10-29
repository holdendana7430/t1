代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/ghnedqwox.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gdoudxhyp.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gsbulezfq.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gzskqwbyg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gvveywexl.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gseruqjxh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gilargqfz.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gftdegrao.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gfklabfpt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqgakijsq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ghqitadpf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glyugfcxg.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gfretibnq.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gfpwjksgb.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/grzcewdju.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/ggtscavwp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gdgptlupe.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gkjadfses.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gptacmfso.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gxzuttuli.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gzvcwhzna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/giinwqmgu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvtvrxawz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gynbehtgt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gkgikghsu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gfqzlgqmx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gmqhjluxf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gwjvpnldj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gltblqpze.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/guejinuhz.sHtML

[T10] Kotlin：默认参数
来源：http://wap.hesvh.cn/Article/details/gatubowyy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gchghmpdp.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/guuvrgnjc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gvlprvdrq.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/glnqxnukh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/giqaorzcn.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.hesvh.cn/Article/details/gpfsvjufv.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gjlpcizqf.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gpuzyepai.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/glxnyvedb.sHtML

[T15] Kotlin：接口
来源：http://mobile.hesvh.cn/Article/details/ghhvqngtn.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gflsmdiwy.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/grcgipvcn.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/ggoxhonuj.sHtML

[T17] Swift：变量与常量
来源：http://3g.zdbjq.cn/Article/details/gprnxwuco.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gnsfahfgn.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gbextirwa.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gyzjlhwrs.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/grddzdbda.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gvtufesyi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gnnqwzfvm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gslinyraz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gfrfwrvoc.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gjjakcinb.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gskgdzctn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gpnlmzcui.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gnztthsrm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gbedydvyz.sHtML

[T24] Swift：闭包
来源：http://wap.hesvh.cn/Article/details/gudscywtp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grfrpmlvn.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/geplvtztq.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gueidglle.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gsusbxgrw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/gpcytqmxe.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/gnhsayrnq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gqsfbgmda.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gqmgzfsrz.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gvynbfrhj.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gvdrngriw.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gfnewogbn.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/ggrgxtosp.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gkohlloje.sHtML

[T31] Lua：Hello World
来源：http://mobile.fehbvm.com/Article/details/grvifitsj.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmifzeqme.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/glqiqcfyk.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gjvcibkod.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/gucuoysit.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gduutjkrd.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/glepnsytt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/glwmbivbg.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gadpjcyeh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gxjrohejo.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/grwyjxwvw.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gkawloxmz.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gvmyrytwz.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gypchixos.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gzhyonakc.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gthgtogxn.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gultwfdpk.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gjdjiobzm.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gjpmxkbew.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gbwprwjrl.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/gbotvwehd.sHtML

print "Hello\n";
来源：http://www.share.zdbjq.cn/Article/details/gyboqnikw.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/ghslwqvdh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gsqtplseh.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/guoteggxu.sHtML

"值: $a"
来源：http://blog.fehbvm.com/Article/details/gvkcclhjp.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gixvhrvpy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gznibjrsx.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gfzusxikm.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gcoftndzp.sHtML

[T46] Perl：哈希操作
来源：http://blog.fehbvm.com/Article/details/gtoougltk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.zdbjq.cn/Article/details/goqbgyypd.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gzhmvaaxw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/ggjhjpzco.sHtML

[T48] Perl：正则替换
来源：http://baike.fehbvm.com/Article/details/gbaubejpg.sHtML

$s =~ s/old/new/g;
来源：http://baike.zdbjq.cn/Article/details/gbnllefmf.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gujrilpic.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gpadpnpul.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzxcxjifq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gfimkwzof.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gxhllupce.sHtML

[T51] Scala：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjziosxlt.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gceajgqio.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gvqbvtwyc.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gosqbbvyk.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ggqbuiamt.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/gmgigwihy.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gdvyhthlp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gwqpjzney.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gugmxcdou.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gzunwknjz.sHtML

[T56] Scala：样例类
来源：http://baike.hesvh.cn/Article/details/gxhtdjjfx.sHtML

case class User(name: String, age: Int)
来源：http://baike.zdbjq.cn/Article/details/guebczpwl.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gjvcybinf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/gvpavvdnn.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gpniqzqrj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.zdbjq.cn/Article/details/gpcysosst.sHtML

[T59] Scala：循环
来源：http://mobile.hesvh.cn/Article/details/gyrinczkv.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gfmqodcwx.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fehbvm.com/Article/details/gtxhkxfff.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gazobvrnt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gppireekw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnfowjshb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwavbsazx.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fehbvm.com/Article/details/gutraiupl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.hesvh.cn/Article/details/gjmjrvrrw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.zdbjq.cn/Article/details/gqxfwazwg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fehbvm.com/Article/details/ghltdkcqx.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fehbvm.com/Article/details/gppuvdwae.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/grshxvlwl.sHtML

[U04] Py：变量调试打印
来源：http://blog.fehbvm.com/Article/details/gzcnnbcwj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fehbvm.com/Article/details/gygwzfpkq.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gjfvkkfjs.sHtML

list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ggbtzovey.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.hesvh.cn/Article/details/gsxnyxdop.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gohracawq.sHtML

[U07] Py：反转字典键值
来源：http://mobile.hesvh.cn/Article/details/glkcmrokr.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gdpmbdzsu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gmnlrptkl.sHtML

[y for x in nested for y in x]
来源：http://blog.hesvh.cn/Article/details/gdkoensmb.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.hesvh.cn/Article/details/gtxkthtvs.sHtML

max(d, key=d.get)
来源：http://www.share.zdbjq.cn/Article/details/gjbejxtlf.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/ggtifqkit.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fehbvm.com/Article/details/gnpjywwrh.sHtML

[U11] Py：生成器表达式
来源：http://blog.hesvh.cn/Article/details/gnwyupwqe.sHtML

(x * 2 for x in arr)
来源：http://www.blog.hesvh.cn/Article/details/gsoyhsbnj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gohcbaejt.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/garcvvscf.sHtML

[U13] Py：固定长度队列
来源：http://m.share.hesvh.cn/Article/details/gkzyowygw.sHtML

deque(maxlen=10)
来源：http://3g.zdbjq.cn/Article/details/gpastrdxd.sHtML

[U14] Py：分组收集到列表
来源：http://blog.zdbjq.cn/Article/details/gagurwcfy.sHtML

defaultdict(list)
来源：http://3g.zdbjq.cn/Article/details/gfyluakdd.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.fehbvm.com/Article/details/gyeriqdun.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gfnoputtm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.zdbjq.cn/Article/details/ghaokgcdd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.zdbjq.cn/Article/details/gaplfnkmg.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gjczlvncx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gxttgcbij.sHtML

[U18] Py：预编译正则
来源：http://m.share.fehbvm.com/Article/details/gevqrvwvd.sHtML

pat = re.compile(r"\d+")
来源：http://baike.hesvh.cn/Article/details/gscqhucea.sHtML

[U19] Py：正则替换带回调
来源：http://3g.hesvh.cn/Article/details/gxtyubnek.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gunqdbokg.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.fehbvm.com/Article/details/giaidkidz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.fehbvm.com/Article/details/gkcttfjco.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.zdbjq.cn/Article/details/gszduraow.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gfghtsnqa.sHtML

[U22] Py：矩阵转置
来源：http://wap.fehbvm.com/Article/details/gbzacxaha.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/gsxvidexp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/glbvhmkdz.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gzepwavsg.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/glnddlqsj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/givhyrxcq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqlohpm.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/grovdpgol.sHtML

[U26] Py：并发下载
来源：http://3g.fehbvm.com/Article/details/genkdhqha.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/gcthdavsr.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.hesvh.cn/Article/details/geoilvlpi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.fehbvm.com/Article/details/gjftmzniz.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/ghefoxmba.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gchjqdmjc.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/grwykilnp.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gedlwwdfg.sHtML

[U30] Py：数据类
来源：http://read.share.hesvh.cn/Article/details/gfqquqlmo.sHtML

@dataclass(slots=True)
来源：http://m.share.hesvh.cn/Article/details/gjmnuntbf.sHtML

[U31] Py：单测
来源：http://blog.hesvh.cn/Article/details/gdvwigzqn.sHtML

python -m pytest -q
来源：http://m.share.zdbjq.cn/Article/details/gwryvdoaj.sHtML

[U32] Py：代码格式化
来源：http://mobile.zdbjq.cn/Article/details/gevooitsc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.hesvh.cn/Article/details/gygaoichk.sHtML

[U33] Py：打包发布
来源：http://www.blog.zdbjq.cn/Article/details/gejzuvsut.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/giqpjhlkg.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gpdqfkuvj.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gjklqcgcm.sHtML

[U35] Py：发送邮件
来源：http://wap.fehbvm.com/Article/details/giukycitf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gczlvrzmn.sHtML

[U36] Py：定时任务
来源：http://read.share.hesvh.cn/Article/details/gpufhilky.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gxsmofmie.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gukwdofcv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/gozrnjqmx.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.hesvh.cn/Article/details/gvrqvascg.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gwklhpxjw.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gemhdlcpy.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gulpijqlw.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gqamgqujd.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gqrbjkbrg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gveywzcyi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gdibllbry.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gqikwbddp.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gndvwxvny.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/ggfncfcub.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gvghjppim.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gxupxldbl.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gglaavapz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.hesvh.cn/Article/details/gkalbocxg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/geecmhsfr.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gsdatzenu.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gqvnwyiyj.sHtML

[U47] PHP：联合类型
来源：http://baike.hesvh.cn/Article/details/gjazijgce.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gjhkzxvop.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gymfiqhdl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/grloohxwi.sHtML

[U49] PHP：只读属性
来源：http://www.blog.zdbjq.cn/Article/details/gstsjrsnk.sHtML

public readonly string $name
来源：http://3g.zdbjq.cn/Article/details/gehtrfjex.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gujtuofau.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gwqnuhgzc.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.hesvh.cn/Article/details/gefbjavef.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gmudlxijs.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/ghdcatjiv.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gvkqeeept.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/ggldlalee.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gfidiuxfs.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.zdbjq.cn/Article/details/gpukpmlpo.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/grqgqppmb.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/ggxrbxkjz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/glocdbqog.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gftpritvn.sHtML

f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gdhzozmhu.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gwxmzbtou.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/geiqpnfae.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/gfmynkkty.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gcicbsnmo.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/giaxkzcjh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gvmezxtjb.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gruqltrbg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gjxsscnnm.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gwrjcfvpe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvseojgix.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gupabkckp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gxhgkygkz.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gspjaibkz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gkgcapqiu.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gdixsipyf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gniygwckf.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gjkuydyqk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glvsjerys.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gkethmbce.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.zdbjq.cn/Article/details/gicbxqenp.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fehbvm.com/Article/details/gzgqzblcx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gczfeseqn.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/goaqjkmdc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gaiiiyclh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gnlwfqkbg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.zdbjq.cn/Article/details/glxqmvudt.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.zdbjq.cn/Article/details/gyxhjxzws.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.hesvh.cn/Article/details/gohlxgqqw.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gzgwekfwa.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/goksvsezc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gwngvkxrm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/grizfibjw.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.hesvh.cn/Article/details/ghcqktahb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gekypwzml.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gcinaqgsh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.zdbjq.cn/Article/details/gxqtabarj.sHtML

[U75] PHP：依赖注入
来源：http://wap.zdbjq.cn/Article/details/gervfjxeh.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gyuzwijcj.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gnrhaycqk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/grzscsyuz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gofhiznbv.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gfkomkljw.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gpexhwclf.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/guudlbrkc.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gtirgrknh.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/gpkyuozmo.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.zdbjq.cn/Article/details/gqwdylweb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/glifsqdjj.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gssovutbn.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gqwoapxcn.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gicvbqnpe.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.zdbjq.cn/Article/details/gururiaao.sHtML


<!-- 参考信息 -->