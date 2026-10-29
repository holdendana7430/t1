代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/glllonnle.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gufrkvrds.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gaigumvor.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/ggnihfypo.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gpsakaayl.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gkjshdqmn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/goxqrncaz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gvzqtmuck.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/giowxhdon.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzowywwjq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gkmbnezja.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gajikpqtn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbsdyxrym.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnsgvwmce.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gxajqfhhk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gwjjthtok.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gpporifqh.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gchtbyjyx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gvbbixjys.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gkvpfkfau.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gtvtklxpi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gknphfiod.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/grzfndvmt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gizjmjuet.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gehosamvc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/glpvgarfy.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwipzsczb.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gynaynwxm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gimdtukaq.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gjijxltsd.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gdncgmasp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gxfikniyw.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gdfponwzu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gycglnnrs.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gzmgcfomh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gjtxetykc.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gbamqpsef.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/ggqeedeqw.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/givwwheds.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gpnrjpvtv.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gvfqksudq.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gjbfqkmbh.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ghqgtwsvv.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gmhkjagqd.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gljikcxxo.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gmhbcfjaq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gumshkymd.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gwvqtpoht.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/goykqzsqn.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gmutyhxbi.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/ggmvpetes.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gjpgsytor.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gissfadkm.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gaqkksgxc.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gnxxumhrt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gkfjbkhpw.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gmqwcqgyf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gpmjjownj.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gnfhcsomk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gozeteqey.sHtML

[T25] Swift：结构体
来源：http://m.share.fehbvm.com/Article/details/glbetabil.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gujhydwyt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fehbvm.com/Article/details/gariztvpn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gtfizhoje.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ggwirkkqz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gkpgwxudn.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/giuhpnbib.sHtML

enum Color { case red, green }
来源：http://read.share.hesvh.cn/Article/details/gmpbbcscv.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fehbvm.com/Article/details/gtuegjfbm.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gezdeonbs.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gxaabklve.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gagflcotl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/ghhyzoxpe.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/guqyxytzr.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gypyqpksa.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gulyfyfqe.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gpaqdpnjy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gkdagetuc.sHtML

[T34] Lua：遍历表
来源：http://blog.hesvh.cn/Article/details/ggpxfycbf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gcauvtfra.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gwfpkgcsh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gemeadskd.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gxvrdicax.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/grswwpbig.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gxbyqichw.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gqansnzxv.sHtML

[T38] Lua：条件
来源：http://3g.zdbjq.cn/Article/details/gkmwsdqyy.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gvnzsrtzy.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gobueurwz.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/ghoqmwkmz.sHtML

[T40] Lua：元表
来源：http://wap.fehbvm.com/Article/details/gbctyhqsa.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fehbvm.com/Article/details/gtlgpmvfj.sHtML

[T41] Perl：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpnihxpbn.sHtML

print "Hello\n";
来源：http://www.blog.fehbvm.com/Article/details/gtnleczsr.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gyexksfvx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gyjadzoyp.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwrqxjxhv.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gsddurtwg.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gxxnqwojk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/genlgfcxj.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gdugodquy.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gxbqmarca.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gmruipzze.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gqaolntjr.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/grtbxoxxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gwwpghbuc.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/gwuagduzo.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/ghiietbiy.sHtML

[T49] Perl：函数
来源：http://www.m.share.zdbjq.cn/Article/details/glsfvivra.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ghzlsxuay.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gulritijm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gpmsgjbgo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fehbvm.com/Article/details/gbeytqwwo.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbpvzpiin.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gbgkoojhp.sHtML

[T52] Scala：变量
来源：http://3g.zdbjq.cn/Article/details/gfhaizbwq.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gcgizqlhx.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gnnhhufig.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gtqpsbkrm.sHtML

[T54] Scala：集合映射
来源：http://m.share.hesvh.cn/Article/details/gzqnjrluc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.zdbjq.cn/Article/details/gyisuevwn.sHtML

[T55] Scala：集合过滤
来源：http://baike.hesvh.cn/Article/details/gyageazqw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/gudzpecsx.sHtML

[T56] Scala：样例类
来源：http://wap.fehbvm.com/Article/details/guxpzywlm.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gjfqhqydu.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gxapwxmiu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.zdbjq.cn/Article/details/ggipcunuw.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/guycvxepw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.hesvh.cn/Article/details/gpbetdvby.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/glgomjccz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gatdbykeb.sHtML

[T60] Scala：折叠
来源：http://3g.fehbvm.com/Article/details/gbdeyaair.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.zdbjq.cn/Article/details/gdykregcq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbvosaers.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gbjurlezg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevguveeg.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gizsnoiqm.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gemtecpsj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gyrzhcxxz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gkmdsowkk.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gtjtqvxqv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gkdrhkqdr.sHtML

[U04] Py：变量调试打印
来源：http://www.share.hesvh.cn/Article/details/ggikmiojq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gddqximif.sHtML

[U05] Py：列表去重且保序
来源：http://wap.hesvh.cn/Article/details/gkxtqhnjb.sHtML

list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gjldgypkt.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fehbvm.com/Article/details/giefnpehk.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/gkkgwrlff.sHtML

[U07] Py：反转字典键值
来源：http://read.share.zdbjq.cn/Article/details/gjnqktpmn.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gnkbqkshs.sHtML

[U08] Py：展平二维列表
来源：http://read.share.zdbjq.cn/Article/details/gscahzpgl.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gqnmzocbq.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.zdbjq.cn/Article/details/gunmqmdow.sHtML

max(d, key=d.get)
来源：http://blog.zdbjq.cn/Article/details/gxkzciluo.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.zdbjq.cn/Article/details/guoooisyy.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gzqzlgyds.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/gxagpelcv.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gujfvizjf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.fehbvm.com/Article/details/ghpzrcppl.sHtML

Counter(arr).most_common(3)
来源：http://wap.fehbvm.com/Article/details/gabkymltp.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gjkwzvqrc.sHtML

deque(maxlen=10)
来源：http://blog.fehbvm.com/Article/details/gymegkwpr.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.hesvh.cn/Article/details/gkmrfonpy.sHtML

defaultdict(list)
来源：http://m.share.hesvh.cn/Article/details/gygjfcpwm.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gclhhseot.sHtML

t = time.perf_counter()
来源：http://www.blog.zdbjq.cn/Article/details/gatyngdrw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/gjmgullle.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/gwlvebzop.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gubquiefo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.hesvh.cn/Article/details/gsbtxskms.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gkgknpyso.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gnqgrpbnc.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/gztbdgewq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.hesvh.cn/Article/details/ghpiyfeki.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gyvtbeeif.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/guqwwakqe.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gkswhkaes.sHtML

@contextlib.contextmanager
来源：http://blog.zdbjq.cn/Article/details/gdtdbhhng.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gtfgyeotn.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gizjfrhat.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.hesvh.cn/Article/details/ggorziptw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.hesvh.cn/Article/details/gtponqgif.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/ggkwowbvb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gofqmzlkr.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.zdbjq.cn/Article/details/gcopphnlc.sHtML

csv.DictReader(f)
来源：http://www.share.zdbjq.cn/Article/details/gzkhkuojr.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gbyacxrsb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.hesvh.cn/Article/details/gpvmvmsab.sHtML

[U27] Py：异步 HTTP
来源：http://blog.hesvh.cn/Article/details/gisdngpph.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/ghhobkwok.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/gxyuxcbum.sHtML

UserId = int
来源：http://read.share.fehbvm.com/Article/details/geekqflgq.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/gclcclzdk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.fehbvm.com/Article/details/gqqgwjgep.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/ggdhpxivw.sHtML

@dataclass(slots=True)
来源：http://mobile.fehbvm.com/Article/details/gpfswgdjf.sHtML

[U31] Py：单测
来源：http://www.m.share.hesvh.cn/Article/details/gzmrtaqpq.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gqecciqqu.sHtML

[U32] Py：代码格式化
来源：http://wap.zdbjq.cn/Article/details/ghwcwcrmc.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.fehbvm.com/Article/details/glquzdywp.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gprqhlwdo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.zdbjq.cn/Article/details/gkhrpytfv.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gwrgwfqwu.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gckivpkwl.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gikgzbrfu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpfcgtau.sHtML

[U36] Py：定时任务
来源：http://www.share.hesvh.cn/Article/details/gjecatvaj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.fehbvm.com/Article/details/gwkmuqllu.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gzidmuswc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.hesvh.cn/Article/details/ghjtcwkjc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gxrqyczge.sHtML

Path(__file__).resolve().parent
来源：http://wap.fehbvm.com/Article/details/guqgtovzb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.fehbvm.com/Article/details/glarfohwr.sHtML

sys.stdout.isatty()
来源：http://read.share.zdbjq.cn/Article/details/gvvhnmici.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/gnluaqybk.sHtML

print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/ggqtqropm.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.hesvh.cn/Article/details/gyhloapdg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/grliyvyjt.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gzdpmqqzi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.hesvh.cn/Article/details/gfkqogkln.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/giaunmklu.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gcpaofdiu.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gjrwtqufk.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gvxgjwrcq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.hesvh.cn/Article/details/gflgryqnb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gsxcuepqf.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gdgxwiskj.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gccomqite.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gqrlpqkgd.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gzqbnusgm.sHtML

[U48] PHP：纯枚举
来源：http://baike.hesvh.cn/Article/details/ghqovinas.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.hesvh.cn/Article/details/govucumxw.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gjttwvsix.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gbdxrgncu.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gnoqshpzz.sHtML

public function __construct(private int $id) {}
来源：http://3g.fehbvm.com/Article/details/gfgbtsovo.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gukdqpwpl.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gvmxnqiop.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gkzovsykn.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gxkaysqeq.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gzhylband.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gcampzbal.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gzwlsguos.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gsihdxagt.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/giivnhpbg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gokxcvufj.sHtML

[U56] PHP：命名参数
来源：http://www.blog.fehbvm.com/Article/details/gotpxumhz.sHtML

f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gpriybrim.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gkmifgbfy.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gjxygrwxs.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gaoluzjwo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gtfavtome.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/grjqffhas.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gfhqopkrz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gxuykrwne.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gckopyiuk.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gakgrplpw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gvjcwcmly.sHtML

[U62] PHP：日期对象
来源：http://www.share.hesvh.cn/Article/details/gyrcskfey.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/govilqjtd.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gnqsdyiyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gpzrhmqkw.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gkcvswumq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/garuackxy.sHtML

[U65] PHP：会话
来源：http://www.m.share.fehbvm.com/Article/details/gyngeunlv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ggcdncfks.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.zdbjq.cn/Article/details/gzvsvdpbp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.zdbjq.cn/Article/details/gaiiyttii.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gjsdsbyvl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gsojaqudl.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gnhtggqyl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gwmexrjxw.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/gxvdmuulw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gxuhdbcmy.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.zdbjq.cn/Article/details/gnflkcbia.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gvbpfkjiz.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gmkkqyujg.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/glzcjoxtp.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gkjkebaxf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gylvrjsei.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.hesvh.cn/Article/details/gatvcqdef.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gaowdbzri.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/grctaxbjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/goffvwwcr.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/guukeqxou.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gasuawqms.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/grlmexetb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/grmiyziil.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gctydjwlm.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gjilbhnwv.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gzgenvcaw.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.zdbjq.cn/Article/details/gltlpnlpo.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/ggsjnxuzb.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/goyofpioz.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/giqoenvrr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gqhcnysna.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/guasviafb.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gswdabkim.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gohlaingr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gaqiwklnu.sHtML


<!-- 参考信息 -->