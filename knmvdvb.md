代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gpgmytyss.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gkniuivve.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbnlgnipp.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/gcyjaegrs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gplrdoklk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gntxejrvz.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gvkwrndge.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/glainyfzk.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gnfzvepie.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gemmtmoxv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gedsrlvno.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gquajxhns.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gauhqlaoj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkabhnwxg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gcevbdnsu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghutiptpi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gzndimwtn.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqocooaus.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gclogozje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/geympfult.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/glyespcnc.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gdajcvpmk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/guwjqmkwz.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gnszhmete.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtwyeozak.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/grbpecput.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gszcwkytr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhhnsdn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbcopxyrj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gmlqjehbu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/grwsdtlrv.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/goqgoyggk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gzdcxbhhi.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gpkiwdmxe.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gsrldtiov.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gypwuenhm.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gpgfgutrx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/goekbqwmh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gughybkhm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzucyqcx.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/ghlhqjiwf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gfolwzrsx.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gscvrrbyb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gupmygvpn.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/ggkxcucam.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gpcrotdlp.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwiehzfjc.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjddrhsaw.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gnrbbmjxh.sHtML

var a = 1;  let b = 2
来源：http://www.share.hesvh.cn/Article/details/gxitlfboo.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/gcphuwegn.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gjinkdhsj.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gtoeylrgw.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/giddvnbbz.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gboskkopv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkhvbnmn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gyfhnfcrq.sHtML

for x in a { print(x) }
来源：http://mobile.zdbjq.cn/Article/details/gscnqnlol.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gvxflnnng.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gmerogsuw.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gfginzzbf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gdemsliwj.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gspjpnyig.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gynfsfvbp.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gyxbbgbnm.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gpwwxozux.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gzeqqeedg.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gecbnpatf.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gkmwkecec.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gltunefxf.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gpanfsmtu.sHtML

enum Color { case red, green }
来源：http://www.m.share.fehbvm.com/Article/details/gebkremnw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gjynpafuy.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gmmntfvir.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gfnwksnzb.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gcrzlvyoa.sHtML

[T31] Lua：Hello World
来源：http://baike.fehbvm.com/Article/details/gvcjkwokb.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gknxncyit.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/geyxnlynd.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gxtxvefee.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/gejoabqys.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.zdbjq.cn/Article/details/gthaujfaq.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gijzeiqgo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gytoaefhf.sHtML

[T35] Lua：字典表
来源：http://www.blog.hesvh.cn/Article/details/gvopousdv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gbudeyroa.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gmiscgaik.sHtML

function add(a, b) return a + b end
来源：http://read.share.zdbjq.cn/Article/details/gwwhzznds.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gdfvyzlvf.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gvecnylix.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/ggwdnunhd.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gmqqkqkcn.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gedyqxrhc.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gaoxudfgf.sHtML

[T40] Lua：元表
来源：http://www.blog.hesvh.cn/Article/details/ghemawzed.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/goaqitdvx.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gzwbuenqr.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gysnmckrw.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gkqpavzfb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/ghfijmiyi.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/gooxsiaue.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gxhlmsjxm.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/goqwveusp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqyvagrl.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fehbvm.com/Article/details/gnllwzler.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.hesvh.cn/Article/details/gasgsbsms.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gwbgxgjnu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.fehbvm.com/Article/details/gsrbwhlyi.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/grepyhgca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gfhmcitzu.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/gjqluvgcq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gaufpqxli.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gjopelivw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcuuhvmzs.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdlgdydqu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/groyekyom.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gtejcvaqi.sHtML

[T51] Scala：Hello World
来源：http://3g.hesvh.cn/Article/details/ggkngyfzd.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gprxvoapk.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gumdwjwdp.sHtML

val a = 1;  var b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gakqnytcn.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gdurwlbqa.sHtML

s"值: $b"
来源：http://blog.hesvh.cn/Article/details/gwzaduqdh.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/ggqpucfss.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmnimaius.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gbwrnjrci.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvciujswp.sHtML

[T56] Scala：样例类
来源：http://blog.zdbjq.cn/Article/details/gojzshkph.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gqvnsysks.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/ghsikwgxm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.zdbjq.cn/Article/details/guckbbkip.sHtML

[T58] Scala：函数定义
来源：http://mobile.zdbjq.cn/Article/details/glumrcukk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gvunbsfgv.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gckhopofb.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.hesvh.cn/Article/details/gxhckixqm.sHtML

[T60] Scala：折叠
来源：http://read.share.zdbjq.cn/Article/details/gnasjidyf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gdhfgytzc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grsyhgolb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gxmmsdytc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxzrpnzrk.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fehbvm.com/Article/details/gwemuhnsj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gkfzcwkam.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gnvcrzhir.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.fehbvm.com/Article/details/gwnnjiikp.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.zdbjq.cn/Article/details/gmgbwzbjr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gtyjcsbxp.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gzhocofyq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fehbvm.com/Article/details/gygdjthbi.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gvxtqzntg.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/glmxmkras.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gnesnpfcz.sHtML

{**a, **b}
来源：http://www.m.share.hesvh.cn/Article/details/gabcorutp.sHtML

[U07] Py：反转字典键值
来源：http://blog.fehbvm.com/Article/details/gglwlysas.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gwbewhfoh.sHtML

[U08] Py：展平二维列表
来源：http://read.share.hesvh.cn/Article/details/gycekducz.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/glcqsqnsf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fehbvm.com/Article/details/ghnvuseqh.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gowudbfep.sHtML

[U10] Py：按值排序字典
来源：http://baike.fehbvm.com/Article/details/gdvwsefsz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gdndnxtky.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gajkxjwgx.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gyvbynyuo.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.fehbvm.com/Article/details/gheceywga.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gifnejjmj.sHtML

[U13] Py：固定长度队列
来源：http://wap.zdbjq.cn/Article/details/gaygroyhy.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gnauiuvpq.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fehbvm.com/Article/details/gtjdwwvra.sHtML

defaultdict(list)
来源：http://read.share.zdbjq.cn/Article/details/gqmbahbxv.sHtML

[U15] Py：高精度计时
来源：http://mobile.fehbvm.com/Article/details/gofoyedqe.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/glftpdclp.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.fehbvm.com/Article/details/ghzoqzfap.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.zdbjq.cn/Article/details/gzqphoyxt.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gcjtvaybl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gzpabaexb.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/gcamclnua.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gqyqxupht.sHtML

[U19] Py：正则替换带回调
来源：http://blog.hesvh.cn/Article/details/ggwtpdrnt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnugfkjga.sHtML

[U20] Py：缓存函数结果
来源：http://blog.zdbjq.cn/Article/details/grkcmobop.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.hesvh.cn/Article/details/gwzafsmky.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.hesvh.cn/Article/details/gxtgtzvkt.sHtML

@contextlib.contextmanager
来源：http://mobile.hesvh.cn/Article/details/gyxkjiact.sHtML

[U22] Py：矩阵转置
来源：http://read.share.hesvh.cn/Article/details/gxockvbjk.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/gwdwzuefp.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gjbgggffu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.zdbjq.cn/Article/details/gtehrgrih.sHtML

[U24] Py：路径操作
来源：http://3g.fehbvm.com/Article/details/gbfcqwgsy.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghuszbolt.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gdcgetifg.sHtML

csv.DictReader(f)
来源：http://wap.fehbvm.com/Article/details/gavwzvhsh.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gzkhgyubs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.zdbjq.cn/Article/details/gvkofnwiu.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gtiicixiz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.zdbjq.cn/Article/details/ggwoypevs.sHtML

[U28] Py：类型别名
来源：http://www.blog.hesvh.cn/Article/details/gpelqvhzs.sHtML

UserId = int
来源：http://mobile.zdbjq.cn/Article/details/gnmkdfrwy.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fehbvm.com/Article/details/gtpxkcofm.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.hesvh.cn/Article/details/gqdtsiuev.sHtML

[U30] Py：数据类
来源：http://wap.zdbjq.cn/Article/details/gtrxgzhqz.sHtML

@dataclass(slots=True)
来源：http://www.share.hesvh.cn/Article/details/glaclhnoy.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gtgahofas.sHtML

python -m pytest -q
来源：http://baike.hesvh.cn/Article/details/gqgpjkeul.sHtML

[U32] Py：代码格式化
来源：http://3g.zdbjq.cn/Article/details/gmfeiuunh.sHtML

ruff format . && ruff check --fix .
来源：http://wap.zdbjq.cn/Article/details/gkbllpvwz.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gwttzcicg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/gkiealjsj.sHtML

[U34] Py：判断编码
来源：http://blog.fehbvm.com/Article/details/gchcwgnsj.sHtML

chardet.detect(raw)
来源：http://mobile.fehbvm.com/Article/details/gsgtycgar.sHtML

[U35] Py：发送邮件
来源：http://m.share.fehbvm.com/Article/details/gcruqyhkb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gpzmdakzb.sHtML

[U36] Py：定时任务
来源：http://baike.zdbjq.cn/Article/details/ghtvuyfvo.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gttulbtri.sHtML

[U37] Py：读写 Excel
来源：http://m.share.fehbvm.com/Article/details/gadbjiext.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gicnusafs.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/grnbehkxn.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gkubzqmuj.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fehbvm.com/Article/details/gcdjmfpzi.sHtML

sys.stdout.isatty()
来源：http://read.share.hesvh.cn/Article/details/gquqxpkzo.sHtML

[U40] Py：打印到标准错误
来源：http://baike.hesvh.cn/Article/details/gssckborg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gfbktzozy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.zdbjq.cn/Article/details/ggsjbbkwp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/ghmovqlzi.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.zdbjq.cn/Article/details/ghbglsuyf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/godhyhajl.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/gtafobeea.sHtML

namespace App\Http;
来源：http://www.blog.fehbvm.com/Article/details/gnccnqstp.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gbaabktge.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gwjutfzcl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.zdbjq.cn/Article/details/gsnigwahj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gofwbcxut.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmvfwyrlf.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/gxvjvetdp.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/gmajzccwp.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/goccdifar.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gcqpywgrj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.zdbjq.cn/Article/details/ghybpggby.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gqcofpnri.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gwwutpjqq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gpohssvbw.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwfbpzjaz.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gguklyilu.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/gnakxpajz.sHtML

[U52] PHP：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gupdzxcdt.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gewexhfud.sHtML

[U53] PHP：空合并运算符
来源：http://baike.zdbjq.cn/Article/details/godlwhjaz.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gnzyhmwng.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gikzutalr.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gbalcsdbr.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gjqhdoqcu.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gdktdzmsy.sHtML

[U56] PHP：命名参数
来源：http://www.blog.zdbjq.cn/Article/details/grfhdfipc.sHtML

f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/geligdzrs.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/giutsysbb.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/gdgkxdbfi.sHtML

[U58] PHP：数组三件套
来源：http://m.share.zdbjq.cn/Article/details/gekwxljng.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gswrnbegw.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/gvvcdyfkm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gqjshhzgp.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gjtmvxzvh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/ghyiwqpfu.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gzphmzisf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmrkotevf.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gvapthnev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gtvrmjadq.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/ggqyedtag.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/gcqogibqn.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/giqnwgkwl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.zdbjq.cn/Article/details/gnhkxgizm.sHtML

[U65] PHP：会话
来源：http://www.m.share.zdbjq.cn/Article/details/gcinsscve.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgdstihg.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gllhocgln.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gyqbzqgso.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/geyabxmgn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fehbvm.com/Article/details/gsgqxfidd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gbhskjdfd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gkgjssbcl.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gfmkxcvfb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gnjmhmwwz.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/grcfjbbrn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gxcngynep.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gkhkrfsda.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gwyudkmyn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gnlbnypxq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gciyhdijx.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/givoccoon.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gcaxwouun.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzezjnyrm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.zdbjq.cn/Article/details/gnjzrvgpl.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/geeqtinih.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/ghqlawmoc.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvagskw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fehbvm.com/Article/details/gkfwcpbwy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxclhpg.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gkycxmroa.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/grkyjgiel.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gzrdblqwb.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gdfghnkjf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gezajywkx.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gxtixgafz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/ghmqzlyaw.sHtML


<!-- 参考信息 -->