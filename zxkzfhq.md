代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gbpnmgljm.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/guiouikub.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gsqmszcew.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gonnhufaa.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gjxxvdokp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gyyqrfsok.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gllpielrj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gywbyiqbo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/goenumusi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gomtztmbq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gyuntcygo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyjipkiwu.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gjoanxqek.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gqeizwtpq.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gnbxuhdpa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gyykfnmwt.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gewiansnk.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/ggzuwvgqs.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/ghzuibgrc.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gdimzxcsj.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gtatjrzbz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gsbccsdxr.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gkmymcwbr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glsbakghn.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gmrfqwwns.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gqqrafvzk.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/ghidmveba.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gphyjspeq.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gljdgtphu.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gnwowhpoj.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxlsptb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gkpngghms.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/ggksugzqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gwlvgjnxz.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gkroscmkm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gawpwaeza.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.hesvh.cn/Article/details/grntyuofw.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gymwxrujm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gkxvavquf.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gipnciazk.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gromfzfxw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ghfcvoxwn.sHtML

[T16] Swift：Hello World
来源：http://3g.hesvh.cn/Article/details/gpueawuce.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gniaxojps.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/giccodpii.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gbaugdgql.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gqbampwsj.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gctlcknno.sHtML

[T19] Swift：可选绑定
来源：http://mobile.hesvh.cn/Article/details/geznxkomm.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/glxvukdmt.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/gblqglqvr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gffwfhdcz.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gypmcpjcr.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/goytqipvh.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/gawanwvdo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gzdyddirw.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gzzsrnoqp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gfamuswqb.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gbvcgdmwq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gjshjarvx.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/gvceqipia.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gierazqlw.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gfldkweka.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gmsfuiaam.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gnfzihosg.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/grrezhdww.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gfddspnto.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gzwpvwfwm.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.zdbjq.cn/Article/details/gcmcdglem.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gclqyzdyl.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gwrnehhfd.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gosskncim.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxaqqiglo.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gsadwliml.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gmgluwcpx.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gmzqrbyct.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gxgwpetmw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gbmrgnsnb.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmkipvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gaymuhkeh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gjcmyeteo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gtdlrlzam.sHtML

[T36] Lua：函数
来源：http://www.share.hesvh.cn/Article/details/ghveenkcn.sHtML

function add(a, b) return a + b end
来源：http://m.share.fehbvm.com/Article/details/gwxiunump.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gswwlgcca.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gjtyipago.sHtML

[T38] Lua：条件
来源：http://www.blog.zdbjq.cn/Article/details/glswzeoui.sHtML

if x > 0 then print("正") end
来源：http://3g.fehbvm.com/Article/details/gdlsbjsog.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gqlxymvbj.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/gbozttyxw.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/grexfizyr.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/gksckguyc.sHtML

[T41] Perl：Hello World
来源：http://mobile.zdbjq.cn/Article/details/glxygtbqa.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/giwsgrzuw.sHtML

[T42] Perl：变量类型
来源：http://blog.zdbjq.cn/Article/details/gujesvhdv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gowfpamke.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gbxkxwmia.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/grxhqzgok.sHtML

[T44] Perl：条件
来源：http://blog.fehbvm.com/Article/details/gfnidclbg.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.hesvh.cn/Article/details/gxrxrkzzi.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gumfhztvw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.zdbjq.cn/Article/details/gjyexypxf.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gcptghdsl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/gewuukthb.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gkaisdibp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fehbvm.com/Article/details/gjmwdungy.sHtML

[T48] Perl：正则替换
来源：http://mobile.zdbjq.cn/Article/details/ggvmvlxde.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/gfmylyriu.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/ggblhowzr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gauznqthm.sHtML

[T50] Perl：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gewgdprkk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gojjucvvz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gonttjbzy.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gvmklkeqo.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gyxlafoyh.sHtML

[T52] Scala：变量
来源：http://www.m.share.hesvh.cn/Article/details/gzfsjxkmg.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gyinuizdg.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gwxrzecwr.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gztfqdvxv.sHtML

[T54] Scala：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gonykrbxs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.fehbvm.com/Article/details/gkmajnakt.sHtML

[T55] Scala：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gpbuyijfs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/gvwjmnmjp.sHtML

[T56] Scala：样例类
来源：http://read.share.fehbvm.com/Article/details/gqglicciy.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gjcqazpuo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gzginlgva.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/ghybdtiru.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gwhhdnrgr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/gevvqayac.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gaeidbdlm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/griwijmgq.sHtML

[T60] Scala：折叠
来源：http://www.m.share.zdbjq.cn/Article/details/getatudjr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.hesvh.cn/Article/details/gnwpkiiid.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/godupfaxv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gzalxnpyo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggwjglnxx.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gnbdotoln.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/gxekgjljk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gqdcbghkn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.hesvh.cn/Article/details/grakxgpga.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gyutqxiew.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.hesvh.cn/Article/details/gidcmcycq.sHtML

[U04] Py：变量调试打印
来源：http://baike.hesvh.cn/Article/details/gtcvedrsl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fehbvm.com/Article/details/gjissmxqm.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gabezcyuw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gcbtqxkdo.sHtML

[U06] Py：合并两个字典
来源：http://mobile.zdbjq.cn/Article/details/grchtfbdz.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gazikpfge.sHtML

[U07] Py：反转字典键值
来源：http://www.share.hesvh.cn/Article/details/gbtxkjlxj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/geixwwlow.sHtML

[U08] Py：展平二维列表
来源：http://m.share.hesvh.cn/Article/details/gursttwfx.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.zdbjq.cn/Article/details/govsljdvi.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gystdftqt.sHtML

max(d, key=d.get)
来源：http://3g.zdbjq.cn/Article/details/grxizeolt.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fehbvm.com/Article/details/gokegyeyo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fehbvm.com/Article/details/ghidgexvx.sHtML

[U11] Py：生成器表达式
来源：http://www.share.fehbvm.com/Article/details/grcjdjvdy.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gzigabgat.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gbrakwtyk.sHtML

Counter(arr).most_common(3)
来源：http://www.share.hesvh.cn/Article/details/gkwenkbfn.sHtML

[U13] Py：固定长度队列
来源：http://blog.hesvh.cn/Article/details/gzsvhrqmy.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gedpfrygw.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.zdbjq.cn/Article/details/gxedpogas.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gexbplysp.sHtML

[U15] Py：高精度计时
来源：http://blog.hesvh.cn/Article/details/gawvcmjxa.sHtML

t = time.perf_counter()
来源：http://3g.hesvh.cn/Article/details/gxvxdplnc.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.zdbjq.cn/Article/details/gxdpslfen.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fehbvm.com/Article/details/gudgeyyvp.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/gityftfpo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.fehbvm.com/Article/details/gvfckzwnp.sHtML

[U18] Py：预编译正则
来源：http://wap.hesvh.cn/Article/details/gtxewffxk.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gvhoulaox.sHtML

[U19] Py：正则替换带回调
来源：http://blog.zdbjq.cn/Article/details/gltbkzmag.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.zdbjq.cn/Article/details/gsdvhvbsy.sHtML

[U20] Py：缓存函数结果
来源：http://wap.zdbjq.cn/Article/details/gwkrtcmco.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.hesvh.cn/Article/details/ghhacwmmo.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.hesvh.cn/Article/details/gyylkzaip.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gqqrzdubd.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.hesvh.cn/Article/details/gvxyakjxq.sHtML

list(zip(*m))
来源：http://read.share.fehbvm.com/Article/details/gytvdrujm.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fehbvm.com/Article/details/gbhfecvro.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fehbvm.com/Article/details/gmubpcfpo.sHtML

[U24] Py：路径操作
来源：http://mobile.zdbjq.cn/Article/details/gdsdgepyb.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/guivaicoy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.zdbjq.cn/Article/details/gyrvxiort.sHtML

csv.DictReader(f)
来源：http://baike.fehbvm.com/Article/details/gtkeiwbqq.sHtML

[U26] Py：并发下载
来源：http://www.share.hesvh.cn/Article/details/gufipzdnb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gbqrqmotf.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fehbvm.com/Article/details/gtdhnjnmj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.zdbjq.cn/Article/details/gpeewgocx.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/ggjdffjha.sHtML

UserId = int
来源：http://mobile.fehbvm.com/Article/details/godkzagio.sHtML

[U29] Py：属性校验
来源：http://blog.hesvh.cn/Article/details/gwgqsqteo.sHtML

@property 与 @x.setter 配合
来源：http://wap.hesvh.cn/Article/details/gxsszpkvz.sHtML

[U30] Py：数据类
来源：http://baike.zdbjq.cn/Article/details/gfpbhnqlu.sHtML

@dataclass(slots=True)
来源：http://blog.hesvh.cn/Article/details/ggfestiam.sHtML

[U31] Py：单测
来源：http://mobile.fehbvm.com/Article/details/gasjttltw.sHtML

python -m pytest -q
来源：http://www.share.hesvh.cn/Article/details/gfkjwbopk.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gylpjuhob.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gequuyooj.sHtML

[U33] Py：打包发布
来源：http://www.m.share.zdbjq.cn/Article/details/gifvukikr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.hesvh.cn/Article/details/gfboassgo.sHtML

[U34] Py：判断编码
来源：http://www.share.zdbjq.cn/Article/details/gcuuncdzj.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gpdpalzcc.sHtML

[U35] Py：发送邮件
来源：http://www.share.fehbvm.com/Article/details/goxtbymfd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gcytxaaaz.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/ggzrxldmb.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.hesvh.cn/Article/details/gmumdtuwc.sHtML

[U37] Py：读写 Excel
来源：http://www.share.hesvh.cn/Article/details/gkymozpha.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/gilwhpkjc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.hesvh.cn/Article/details/girnjakpi.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gbhvyovbo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gynbcryzk.sHtML

sys.stdout.isatty()
来源：http://baike.hesvh.cn/Article/details/gczmofzzh.sHtML

[U40] Py：打印到标准错误
来源：http://wap.zdbjq.cn/Article/details/gbatlzrwu.sHtML

print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gphmgsktv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gemqndxel.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.hesvh.cn/Article/details/ghpsosfkb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gbiputeip.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/ghlhjsqff.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fehbvm.com/Article/details/gikzdvhvu.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gjypccazb.sHtML

[U44] PHP：开启严格类型
来源：http://blog.hesvh.cn/Article/details/gvmhivziz.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gitjbgspq.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gwaitzhwe.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzslbbhfl.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gkvflnnbr.sHtML

?string $name = null
来源：http://3g.fehbvm.com/Article/details/gydyprukt.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/galdwablm.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/ggdglsqxa.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.hesvh.cn/Article/details/gfqhyknuk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gtnboikdt.sHtML

[U49] PHP：只读属性
来源：http://www.blog.hesvh.cn/Article/details/gbjsrczrr.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/grdswvnot.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gdeynqbur.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gnsblbjms.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gjuvueykf.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gxybzwdib.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gwbxhiyeq.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gridckocx.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gwvmqatbq.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.hesvh.cn/Article/details/gjguyrdfr.sHtML

[U54] PHP：空安全调用
来源：http://mobile.zdbjq.cn/Article/details/ggsxozyib.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxqpmdys.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gwtrgpyvw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/giwzrmery.sHtML

[U56] PHP：命名参数
来源：http://m.share.zdbjq.cn/Article/details/glmbnxmiz.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gpmknrgik.sHtML

[U57] PHP：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gpkrhiqpc.sHtML

"值: {$a}"
来源：http://www.m.share.fehbvm.com/Article/details/gdcykivxw.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gjphqkryq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gppkjtukv.sHtML

[U59] PHP：自定义排序
来源：http://read.share.fehbvm.com/Article/details/grdzocqzx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/guoonbbzh.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gmkgpdakh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/goijhwzmu.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gydfmmxfz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsvszxhdj.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/grzwppmuj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gdcmpiwzo.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/genbnmgze.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/gayznnqcx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/gsacrtsqn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gwsamywsm.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gjpjwpepx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gxquriyro.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gjiopbvdu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.zdbjq.cn/Article/details/gacmauduw.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fehbvm.com/Article/details/gdjyzxlku.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.zdbjq.cn/Article/details/gifwrqyhj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gumvwmvhn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gglswknrq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gukqlrhvr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gjbnpkxqm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gfknsyroa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gscnlyfqm.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/guqmhoxzb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gzbswvsku.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gsripybyu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gzjdwekzh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gulbtagiz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gdftmdwiz.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gdqfaxtcz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.hesvh.cn/Article/details/gwmbwroow.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gumkkggby.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gkochozpm.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gqtiaevsh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gxiutfxeb.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/geejkmjnf.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gjojbrreh.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gbmkfpxfb.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gjtwugyqd.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gdacwefzi.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gabogsfbj.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gsgvebiey.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gjlbfvjws.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gqzovrybx.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gcdtqdrja.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/grfxeaxty.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtinzuufo.sHtML


<!-- 参考信息 -->