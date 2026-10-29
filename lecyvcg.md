代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gebuqvqdx.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqhinllhl.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gqmrbufqe.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gsrnjjsjw.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/getjpgntz.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gntpijyes.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gvxfrjhyv.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gsqmuecms.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gcxfgxtsn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfavberxo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gfumeiitf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gazopjmlu.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gnjssuvcv.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gcazgfusc.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gpeflyezr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gbfxnradf.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gnsxzxojc.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gbokatkcw.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gsgesgccj.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gutznlblk.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gnkxapxpb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/giwlgumji.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gkjyjsqmr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gygrtkdlj.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gmdzqfwwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gcxdoengu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gnfemxscp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gcpwzsygv.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gfghbsjsq.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gdhnqqbtb.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/glfjxffre.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/grmlexekh.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gepkzuhqt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gulyksacf.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gorbmjylb.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/guijrdewn.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/giarscxnr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/gbxsfvilw.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gpmjcfutj.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gpskrtbje.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gjzydiozx.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gtqvsjyby.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gbtntaeol.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvpdtpfsb.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/glonjkxeg.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/grikecxgu.sHtML

[T18] Swift：字符串插值
来源：http://3g.fehbvm.com/Article/details/goxgjflsu.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/guwkbbhkt.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gkjnqpeey.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/guwqflwbe.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gsaruneir.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.hesvh.cn/Article/details/gbtqydtvd.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gahehrbuw.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gtoyhaecr.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gijsuivss.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gsavewbjm.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gpwiwlmot.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/gfpghkszo.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/giepsghqp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gzbvwvoip.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gswhpozbp.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gpnfqmzzb.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gixfkohbq.sHtML

class A: Base { override func f() {} }
来源：http://3g.fehbvm.com/Article/details/gpsutkkvh.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gohiiwrnr.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gssjktjjw.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/ghzmqjmej.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gmdhyyciw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/gfihmfnyc.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gwbcwfaom.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gbpjwwvvd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gfqnkgqma.sHtML

[T31] Lua：Hello World
来源：http://3g.hesvh.cn/Article/details/gvotzjyva.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gnziojimr.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/gxwnmrais.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gqdiqdqtm.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/geeimtdwh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gkgbmkxci.sHtML

[T34] Lua：遍历表
来源：http://www.share.zdbjq.cn/Article/details/gtbrcscrs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gohyhamsx.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gcpdvrnzn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gojvkkblz.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gvjsshhwg.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gowppblss.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gfrmtmbch.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gfsyqqinn.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gbbmxkush.sHtML

if x > 0 then print("正") end
来源：http://baike.zdbjq.cn/Article/details/gsiiroqek.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gsljqxtor.sHtML

string.find(s, "%d+")
来源：http://www.blog.hesvh.cn/Article/details/glmiovdjm.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gwildjzhr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gkrwpqnrg.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/garbuomgn.sHtML

print "Hello\n";
来源：http://3g.fehbvm.com/Article/details/gfoaizpwb.sHtML

[T42] Perl：变量类型
来源：http://baike.fehbvm.com/Article/details/gdgkcjzqn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gkdhhatvr.sHtML

[T43] Perl：字符串插值
来源：http://wap.hesvh.cn/Article/details/ggikgtpok.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gplsnqmqt.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gqcudgfoz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gymgcwgab.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/grcrayick.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gyrxflqbo.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gvidnlkni.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/ghsrfrjnp.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gpzzyvyqu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gspjkzutn.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gjtrdlwzj.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gohxmrefc.sHtML

[T49] Perl：函数
来源：http://m.share.hesvh.cn/Article/details/gxhmsvbnh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gqgbhttxp.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gcxgmlqvl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.zdbjq.cn/Article/details/giwzyezrz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gynlizflr.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/gaxnufxof.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/ggwztjvll.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/ghynabglm.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gzhkzopwl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gnvmlrpmm.sHtML

s"值: $b"
来源：http://baike.fehbvm.com/Article/details/gjwlocmda.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/glnnrytch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.zdbjq.cn/Article/details/gppmhohsm.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gelzqvujb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpzmjnmon.sHtML

[T56] Scala：样例类
来源：http://mobile.zdbjq.cn/Article/details/gojbofdep.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gehnfsgrb.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvmjgdipw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/glgovisjf.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gqgmrigug.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fehbvm.com/Article/details/gjdnomsaj.sHtML

[T59] Scala：循环
来源：http://blog.zdbjq.cn/Article/details/gklhbnnce.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gwiattzeo.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gcouibczc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gnqsdgfov.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlnqlgnp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gbgdcvvqp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyexzachn.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.zdbjq.cn/Article/details/gvnfknpwv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.zdbjq.cn/Article/details/gdubqmzhy.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gcifpdabk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsscsvbsy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.hesvh.cn/Article/details/gygtugxug.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fehbvm.com/Article/details/gwfrkxzbc.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gapshevkn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/gwnfhtecm.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.hesvh.cn/Article/details/gfteitejr.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gldeszfgf.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gecqyuadv.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gkyrknrfh.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/goqlvtjzp.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.fehbvm.com/Article/details/ghnlqevrx.sHtML

[U08] Py：展平二维列表
来源：http://wap.hesvh.cn/Article/details/gnuihemdk.sHtML

[y for x in nested for y in x]
来源：http://www.share.hesvh.cn/Article/details/gotoqxpbp.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.hesvh.cn/Article/details/gufmuxlyf.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gnulsdokl.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gsclwypvq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.fehbvm.com/Article/details/gtmfgsngd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.hesvh.cn/Article/details/geaumwqip.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gmycyfoni.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.zdbjq.cn/Article/details/gvmtrvksc.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gczthopau.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gubyhmfaq.sHtML

deque(maxlen=10)
来源：http://www.blog.zdbjq.cn/Article/details/gfrjhefrh.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gatkkdbvd.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gbhetqxlu.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gbhuqzixd.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/guhxexsmz.sHtML

[U16] Py：命令行参数解析
来源：http://baike.hesvh.cn/Article/details/gfjqvngnf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/ggtbxipvv.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gzayofqsk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.hesvh.cn/Article/details/gfraziigy.sHtML

[U18] Py：预编译正则
来源：http://m.share.hesvh.cn/Article/details/gwawtsoje.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fehbvm.com/Article/details/gqyvyvpew.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/ghzhficfh.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fehbvm.com/Article/details/gtbzwnsmd.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/giyunwvjq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/gdxlqpxsf.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.hesvh.cn/Article/details/gosqvbeji.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/grdymamlb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/gkkrzbifp.sHtML

list(zip(*m))
来源：http://mobile.zdbjq.cn/Article/details/gcgvwqpxh.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/gkwrguosa.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.zdbjq.cn/Article/details/grojygcop.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gfqiesqcq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gwspsqtjf.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gmaiaccus.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gjnfxqjfm.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gcapznssq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fehbvm.com/Article/details/grgzfiyat.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gmastpldz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gyijuhept.sHtML

[U28] Py：类型别名
来源：http://read.share.hesvh.cn/Article/details/gdrjkppoy.sHtML

UserId = int
来源：http://wap.fehbvm.com/Article/details/gqjxhhonz.sHtML

[U29] Py：属性校验
来源：http://www.share.hesvh.cn/Article/details/gnujjumui.sHtML

@property 与 @x.setter 配合
来源：http://blog.hesvh.cn/Article/details/gfxclomzn.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/giihppsjf.sHtML

@dataclass(slots=True)
来源：http://baike.zdbjq.cn/Article/details/gafjcfwpl.sHtML

[U31] Py：单测
来源：http://www.share.zdbjq.cn/Article/details/gmbordaqc.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/guhbuiieh.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gtqhppaef.sHtML

ruff format . && ruff check --fix .
来源：http://blog.zdbjq.cn/Article/details/gwilliakc.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gvexpynmd.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gxdjneipz.sHtML

[U34] Py：判断编码
来源：http://baike.hesvh.cn/Article/details/ghybgkzmp.sHtML

chardet.detect(raw)
来源：http://www.m.share.hesvh.cn/Article/details/gfkriskdo.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gpgbgxykv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gwnnkkipz.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gtllcjvvm.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.hesvh.cn/Article/details/gdfhhxbpt.sHtML

[U37] Py：读写 Excel
来源：http://wap.fehbvm.com/Article/details/ghifbcwcj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.fehbvm.com/Article/details/giqttrofe.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gabflpocl.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gotojspln.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.hesvh.cn/Article/details/goukayqde.sHtML

sys.stdout.isatty()
来源：http://wap.fehbvm.com/Article/details/gyyivrzoq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/gvkoakkvo.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gqgwexisf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/ggszkgalp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gtudsrtck.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.zdbjq.cn/Article/details/gsamgngbf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gagyfrizw.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gzpswbyyc.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqufiizid.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.hesvh.cn/Article/details/gplygkhfh.sHtML

declare(strict_types=1);
来源：http://www.blog.hesvh.cn/Article/details/ggfqqadob.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.hesvh.cn/Article/details/gcqtdqtix.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gpuqfrrfr.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gvipyxvex.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/gdrdxmzgq.sHtML

[U47] PHP：联合类型
来源：http://baike.fehbvm.com/Article/details/gmgriaiiz.sHtML

int|string $id
来源：http://www.blog.zdbjq.cn/Article/details/gvvhzpbws.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/ghamosqpx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.fehbvm.com/Article/details/gmckgorpf.sHtML

[U49] PHP：只读属性
来源：http://m.share.zdbjq.cn/Article/details/gyqywtcmj.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gladjupgk.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.fehbvm.com/Article/details/ghjjsmlaj.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/ggccrfwfz.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gmzwuncty.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/glqhsidgr.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/gxgtnxogh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fehbvm.com/Article/details/ggfmdusrt.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/guvikionl.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.zdbjq.cn/Article/details/gopuumljn.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.hesvh.cn/Article/details/grtodckgn.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/gjuzfbfcr.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gbqegckgj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gbzlmqokl.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gkuytwbfk.sHtML

f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gmgpcxmqz.sHtML

[U57] PHP：字符串插值
来源：http://blog.hesvh.cn/Article/details/gcioqkyjq.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxpipizei.sHtML

[U58] PHP：数组三件套
来源：http://3g.zdbjq.cn/Article/details/gmoilxiwa.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fehbvm.com/Article/details/ghzpixebq.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbfejtpbv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqbevpddv.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gnosowfre.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/glctadgrz.sHtML

[U61] PHP：正则
来源：http://www.m.share.fehbvm.com/Article/details/gbaljmgup.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gxvcoggfc.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gjhbvvcnv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gzlpbhklu.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gtcmbuvht.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gsdlbfycg.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gobxurtqd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/ghnpxlzue.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gkvopjcft.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/guygaegmv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gjvcenvyj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gieztdsps.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gfkooinpo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.fehbvm.com/Article/details/grjvwgjmd.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/ghrgkpjat.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gfeaxqhlx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/ggniwrcaw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gzpqkkoll.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gkndknxmh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gmayzprma.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gzviutwtb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/geevjypuw.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gmslluics.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gezfhjeea.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/grdypvnfp.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gljyfodox.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gixjiderm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gxnppevqt.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gpjhzgnwi.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/glyrxowld.sHtML

[U76] PHP：简单路由
来源：http://blog.zdbjq.cn/Article/details/ggokwulja.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/ghvqgjupf.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fehbvm.com/Article/details/gnhydfduf.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gnswgncbv.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gztnmwpns.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gxwwztnlr.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gzcvkvghg.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gcpapsvfl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gjlhhqeor.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gsxmptxup.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/guufmrxtt.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gzcapmslk.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/gzckfrhes.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gkuhfyiqg.sHtML


<!-- 参考信息 -->