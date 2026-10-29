代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gczjunzxz.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/ghovddvit.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/glohiurqa.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gxfvihfeo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/ghxxjnvie.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gdxehsvhs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gzhpunlxc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gwnrytzei.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhceveu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyqoheatq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gyiwkddlv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grunrenas.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gxadhtqyz.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gtweocawy.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gsvsegbeu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gkzakchtp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gomdapngv.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gwtpezouw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gtufdwqut.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gcvcliuqt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gugyxooui.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gijmpwref.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gjcitqjam.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gvwylvpns.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gixiwxcnh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gtoivcjeo.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gndunepfv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/ghrubbehk.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gjjvhqcfm.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gzmwfevtk.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fehbvm.com/Article/details/gvnhxobrj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.hesvh.cn/Article/details/gxkafqllh.sHtML

[T11] Kotlin：协程
来源：http://3g.zdbjq.cn/Article/details/gdwyyowvw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gsstfdmlg.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gfnrodqdb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gokbjnsbk.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gddwfxdgy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gfkkyajev.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/grhtiricn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/grzcnrovn.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gddcueubg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/ggbdgxbty.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gzlakesfj.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gmudknyut.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/ggvyhndux.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gsouszezo.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbcbzudeo.sHtML

"值: \(b)"
来源：http://mobile.fehbvm.com/Article/details/gaeoteqrw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/gzlhgcien.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/glhtpahqu.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gnnizeamf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gtyrgoytg.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gsvwrfapo.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gmjfpfkig.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gphtbgxql.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gzutfaifx.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/grgkamugp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gbyrcyhia.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gmndxrffh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gmzjozvtz.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gjcsjpumv.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gaazazghs.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gurgjwrrz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.hesvh.cn/Article/details/gwfdfqchf.sHtML

[T27] Swift：错误处理
来源：http://www.blog.zdbjq.cn/Article/details/grweyiusx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gtjszcsaq.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/guetppdru.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gmpbstfmm.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gngengjri.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gicfgdbew.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gluizimkm.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/grzzbcnrg.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gpjbnmiku.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gbefiicnc.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gbogmatrj.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gxxbvynpw.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gyqdhsccn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gsosyjqzi.sHtML

[T34] Lua：遍历表
来源：http://m.share.fehbvm.com/Article/details/gftselqaa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/ggijahlpg.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/grzzhllsj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gyvfbwsnw.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gygbdsche.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gqejpzlih.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gpjgtbczm.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gkdablmyv.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gibghucby.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gynhqlhyf.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmdlgztgv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/glpaivwuy.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/glhqkkmla.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gzcjkjtxv.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwbzsymov.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gbktrpeni.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gjcvvipko.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gwnrminuw.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcmqufuys.sHtML

"值: $a"
来源：http://www.share.hesvh.cn/Article/details/guemzygpu.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gjuslmpng.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gecmujvmq.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fehbvm.com/Article/details/guifruwqz.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/gatxjtorm.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gwzcvlrdq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gnckvqbjo.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/giooondjb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gvbyzkhgh.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gmoenxxpy.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gtnvznmei.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gtmjmkjlc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gziohstpj.sHtML

[T50] Perl：逐行读文件
来源：http://wap.hesvh.cn/Article/details/ggazkaxcr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gflxswjxv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gpjhecohs.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvznnivbx.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/grcmgtuqm.sHtML

[T52] Scala：变量
来源：http://blog.hesvh.cn/Article/details/gwgvszdqd.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gpikwjuzu.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gdulczrfe.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gjmhkexlt.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/glgnohptx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfxlkxvan.sHtML

[T55] Scala：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gqsmfcrfd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gtjzzktme.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gtcalgkab.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/ggftkzafb.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghkfbudam.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gayyfcsmj.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/glutwdopv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gfcwrwszs.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/glrmvwniy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gcufqljuv.sHtML

[T60] Scala：折叠
来源：http://m.share.fehbvm.com/Article/details/gjvfnzjnb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.hesvh.cn/Article/details/ganrbhmly.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guezonbxh.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gvyilrplg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gepygulay.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.hesvh.cn/Article/details/gjuqfljzc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/grugkptdg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.zdbjq.cn/Article/details/gpfmgdbeh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gykmnwkjo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.hesvh.cn/Article/details/gxsldlfhm.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.zdbjq.cn/Article/details/ggvjefuye.sHtML

[U04] Py：变量调试打印
来源：http://read.share.zdbjq.cn/Article/details/gnntcodzu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.hesvh.cn/Article/details/gdebundza.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fehbvm.com/Article/details/gvjkvtrmw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gzyurncvz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/gjpavenik.sHtML

{**a, **b}
来源：http://3g.zdbjq.cn/Article/details/gzcxlhcuj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gbvveslfg.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.zdbjq.cn/Article/details/gfzjexonk.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.fehbvm.com/Article/details/gtrnetvqc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gkembqpmv.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/ggvxezgvy.sHtML

max(d, key=d.get)
来源：http://read.share.zdbjq.cn/Article/details/gxlgtymii.sHtML

[U10] Py：按值排序字典
来源：http://www.share.hesvh.cn/Article/details/gqvcdcxxv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.hesvh.cn/Article/details/gkijrtqle.sHtML

[U11] Py：生成器表达式
来源：http://baike.fehbvm.com/Article/details/gqlvacdtk.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/geshwzwig.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.hesvh.cn/Article/details/gtxsvihjy.sHtML

Counter(arr).most_common(3)
来源：http://m.share.fehbvm.com/Article/details/gjhlhjctr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gltrqdemz.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gfcdwazjy.sHtML

[U14] Py：分组收集到列表
来源：http://3g.zdbjq.cn/Article/details/ggxloxsgi.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gfpnxfjhq.sHtML

[U15] Py：高精度计时
来源：http://baike.fehbvm.com/Article/details/gdzvmbpne.sHtML

t = time.perf_counter()
来源：http://m.share.zdbjq.cn/Article/details/giqbgqtas.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gsjsevggi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fehbvm.com/Article/details/gjzdicvrp.sHtML

[U17] Py：初始化日志
来源：http://m.share.fehbvm.com/Article/details/gjpvxgwkr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.fehbvm.com/Article/details/gbtwnwcza.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/ginyhkest.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/ggqoturcx.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.zdbjq.cn/Article/details/gtuwitgyv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fehbvm.com/Article/details/glvqrdfsw.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.zdbjq.cn/Article/details/gwnenjndw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.hesvh.cn/Article/details/gafguhnfp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/glsfiqxsd.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gqvdpvneb.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gsxwgxvma.sHtML

list(zip(*m))
来源：http://m.share.hesvh.cn/Article/details/gmtiyqhet.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.zdbjq.cn/Article/details/gjxebcrci.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzskxxw.sHtML

[U24] Py：路径操作
来源：http://www.blog.zdbjq.cn/Article/details/gzuhibjpz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/grjnsfsfu.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.hesvh.cn/Article/details/geqmeqbtm.sHtML

csv.DictReader(f)
来源：http://read.share.fehbvm.com/Article/details/gobdkpcno.sHtML

[U26] Py：并发下载
来源：http://www.m.share.zdbjq.cn/Article/details/grpabmowy.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.fehbvm.com/Article/details/ganbgisck.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gcaimedkh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.hesvh.cn/Article/details/gbnnpeyjr.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gyemwlhjd.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gnyltjoor.sHtML

[U29] Py：属性校验
来源：http://3g.zdbjq.cn/Article/details/gqpsyeboz.sHtML

@property 与 @x.setter 配合
来源：http://baike.fehbvm.com/Article/details/gqnprcojd.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gpvlgylzo.sHtML

@dataclass(slots=True)
来源：http://www.share.fehbvm.com/Article/details/ghcrjlqwo.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gclawakvl.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gppdvqktd.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/glcaqfxow.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/ggbhmbfwq.sHtML

[U33] Py：打包发布
来源：http://3g.fehbvm.com/Article/details/gmeskfayc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.zdbjq.cn/Article/details/gthglewhm.sHtML

[U34] Py：判断编码
来源：http://read.share.hesvh.cn/Article/details/gqvrgtffa.sHtML

chardet.detect(raw)
来源：http://mobile.hesvh.cn/Article/details/gmmlncgyz.sHtML

[U35] Py：发送邮件
来源：http://m.share.zdbjq.cn/Article/details/gfjxzpddw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.hesvh.cn/Article/details/gfarquhsa.sHtML

[U36] Py：定时任务
来源：http://mobile.hesvh.cn/Article/details/gssbufhoo.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/gidrttkpj.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gusaipeik.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.hesvh.cn/Article/details/ghgmqrqwb.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.fehbvm.com/Article/details/gxnobinwf.sHtML

Path(__file__).resolve().parent
来源：http://wap.zdbjq.cn/Article/details/gswhncvzd.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkolxqfpn.sHtML

sys.stdout.isatty()
来源：http://baike.fehbvm.com/Article/details/gglbrxisw.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fehbvm.com/Article/details/ghucdrjnw.sHtML

print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gycbrzfaa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.hesvh.cn/Article/details/gicflvxti.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/grjrvmehu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.zdbjq.cn/Article/details/gnbzvpeva.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.hesvh.cn/Article/details/gsxgozrnx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gugmukffc.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gtictfjox.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gngnghowe.sHtML

declare(strict_types=1);
来源：http://3g.fehbvm.com/Article/details/gdhkiwfpd.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fehbvm.com/Article/details/gmcmxbkfs.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gbtjwpbld.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/gkipanaru.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gjxvdoivq.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fehbvm.com/Article/details/gfgtythor.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/gygxiwxvi.sHtML

[U48] PHP：纯枚举
来源：http://www.share.zdbjq.cn/Article/details/gmtxkpaee.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.hesvh.cn/Article/details/gyxbyzgjd.sHtML

[U49] PHP：只读属性
来源：http://baike.fehbvm.com/Article/details/gmeurpufl.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/grogwtnwk.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fehbvm.com/Article/details/gjtjskcdl.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gxzjiifig.sHtML

[U51] PHP：数组解构
来源：http://www.share.zdbjq.cn/Article/details/gdvlivhab.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.fehbvm.com/Article/details/gtfkpijdi.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gvsxgmmsj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gbqwlmqbx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.zdbjq.cn/Article/details/gkzvzimac.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gudnlpcia.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gvvldnpgh.sHtML

$obj?->method()
来源：http://baike.zdbjq.cn/Article/details/gxvqcufod.sHtML

[U55] PHP：match 表达式
来源：http://wap.zdbjq.cn/Article/details/gaqsyaiim.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gppffdsul.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gefenutlc.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gkzcxlhtu.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gznpramsa.sHtML

"值: {$a}"
来源：http://mobile.zdbjq.cn/Article/details/gxkifgfal.sHtML

[U58] PHP：数组三件套
来源：http://www.share.zdbjq.cn/Article/details/ghtniljou.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fehbvm.com/Article/details/geavbjhrr.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gwpybyvpd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gabvrpcwy.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gpthuvrtx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gsqknjdkw.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gltuirbnw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gwzbzacqj.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/grgtaesiy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.zdbjq.cn/Article/details/gvqjxwgwk.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gbslpjoue.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gsurvyqjh.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gwnzkhyni.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/ggnglfsfc.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gwptmdmgt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gwkadjgsm.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gfqwappvk.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.zdbjq.cn/Article/details/gonmzhsrn.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gogjrriae.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/giyxwlzbm.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/ghcrtcpps.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/gplnnhaea.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gpflqbduw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/gcemtnbsf.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gqgddksuz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gfcxazgxz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gknxlzuud.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gkyyjmvvx.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fehbvm.com/Article/details/gmaipqhls.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/gwwsswhtl.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/giotpywnq.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/grqczizpr.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gmduexcru.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gkyjaazor.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gcxpzqsvs.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/gydvzxfrz.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gpkbgzcma.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.zdbjq.cn/Article/details/gdkyjkdik.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gqojfuije.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/gobgqxvkv.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gwiojxlbw.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.hesvh.cn/Article/details/gdslpjsak.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gqoaejxaq.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gdisnxojt.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gwrfdfbof.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/ggzimqhkp.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gexrzencd.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/grhtrylej.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gwuykdakd.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/guhefcznd.sHtML


<!-- 参考信息 -->