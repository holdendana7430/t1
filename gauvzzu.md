代发 wailian999

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gpxsfuigw.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gcxcgjrlj.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gtyfajrec.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gsfhqudys.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gzxytvshc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gssyubxhq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/glhkoppux.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gevfvnfav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fehbvm.com/Article/details/gdcnrzznp.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gitrqjebe.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxiczrjkh.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gnpnhwxzj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/guwxcvbqr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gljyyxkgj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gebrbtoih.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gpgrxxtpn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gbplgnfzl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfseeciqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/ghorjbnms.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbxjrjzot.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gcxzhlejs.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/giodavldo.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gugiqezwv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gsvkfydcx.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/guznjqkwy.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gylntsdcc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gcmoylooe.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gpyhhcava.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gnfgtrazo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gazqvjlcg.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gdvzrbady.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gqtgqvjnt.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/glmuhmwca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/galngaldx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/giyiuxtrp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gpznviaxd.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gylgwaxmi.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gxfiphimf.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gfqrbezla.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/giuhgbthi.sHtML

[T11] Kotlin：协程
来源：http://www.blog.zdbjq.cn/Article/details/gfkqytobp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.zdbjq.cn/Article/details/glxulqumr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtqzhcabk.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gvaraldqw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gghupozvx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwbsrwbfl.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gpdiqhzum.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gmtdjowiu.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gtkmswlez.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/ghrktynds.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gkvzyqsyq.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gpxuqnjuf.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gzkgeiusx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/guprmjwth.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gyswcdtug.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/grxpbgsul.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/ghmrnnmsc.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/glpsrgije.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ggjfulvra.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/gtjlyjkti.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gcmofwday.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gdkeydkuj.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gvchcormu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gfvkzamyf.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/goxmnraop.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gicyqrizd.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/ggmciwvzk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gmudrnxwj.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gmcbxigxw.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gavadosoo.sHtML

[T26] Swift：类与重写
来源：http://baike.hesvh.cn/Article/details/gtihztdue.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/ghwmkceol.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gveaxjtiz.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gztcghuxj.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gevnwxdvt.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/grxxmyugk.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/gwgdfqokw.sHtML

guard let x = opt else { return }
来源：http://blog.hesvh.cn/Article/details/gqzkswgxh.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gtwlzazqy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/govliaqvo.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gxfncsrnk.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gfhnvbtqi.sHtML

[T32] Lua：局部变量
来源：http://wap.fehbvm.com/Article/details/guvqbnsef.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gpoaqnhwh.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gsjjvwbmn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/ggkfgymim.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fehbvm.com/Article/details/gykvbtvjb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.zdbjq.cn/Article/details/gaftrrvjl.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gpqttexon.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gbqwfrzqe.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gukynpest.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/ghbhyymtb.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gjxgxvntl.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gscialzcr.sHtML

[T38] Lua：条件
来源：http://blog.hesvh.cn/Article/details/gxvbabrot.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gukxkvwhy.sHtML

[T39] Lua：模式匹配
来源：http://3g.hesvh.cn/Article/details/gecsmlvnn.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ghieewuxx.sHtML

[T40] Lua：元表
来源：http://www.m.share.zdbjq.cn/Article/details/gtytydaum.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/guqwyqfrp.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsqslautu.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/guxkigeij.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/ggzddfccx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/gggtexbva.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gwscugxqb.sHtML

"值: $a"
来源：http://www.blog.zdbjq.cn/Article/details/gotjrhlho.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gmycokomu.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gppcwyqxy.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gaymrkjqo.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fehbvm.com/Article/details/gkynjaval.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/gfobbyyva.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/giyyffnks.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/gwyzundxi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.hesvh.cn/Article/details/ggmugwwbl.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/gglcityjm.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/gbvaymeqn.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/gnhtfvror.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gmzpqbwex.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzxqofiai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/gicfsfvig.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fehbvm.com/Article/details/gkliuxfqq.sHtML

[T51] Scala：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcjwamcua.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gfdndiznx.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ggqncyxgr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/glgixvqow.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gtkeynxhy.sHtML

s"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/guwbwpqxw.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gvecyzzsg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fehbvm.com/Article/details/gnimdmewl.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gazmvdptk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvmckfkma.sHtML

[T56] Scala：样例类
来源：http://www.share.fehbvm.com/Article/details/gmwusktlv.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gswdkvooy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gtreeypyd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gvoxuwlpz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.hesvh.cn/Article/details/gxxgmnowb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fehbvm.com/Article/details/grjypisgg.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/glrdyiycf.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gkontqhcv.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gnhjmuuxw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fehbvm.com/Article/details/gansyqtpj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqnmrsddc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gcilmtsbw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goqfdaelq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gpxovtrpc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gtzypkyzo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gugngnzvs.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fehbvm.com/Article/details/gberrlgez.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.fehbvm.com/Article/details/gnhhlcbse.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fehbvm.com/Article/details/guxvrxalp.sHtML

[U04] Py：变量调试打印
来源：http://www.share.zdbjq.cn/Article/details/gahbngiap.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.hesvh.cn/Article/details/ghfizppaw.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.zdbjq.cn/Article/details/gkambrjed.sHtML

list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gckyyquva.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fehbvm.com/Article/details/gkivefuet.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gfeysymyw.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.hesvh.cn/Article/details/gahvlhnke.sHtML

{v: k for k, v in d.items()}
来源：http://baike.zdbjq.cn/Article/details/gseabavkf.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/glhkhobqn.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gdfegklrz.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.zdbjq.cn/Article/details/gccjbbqfq.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gxtypxgbw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.zdbjq.cn/Article/details/gubhwxtkz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.zdbjq.cn/Article/details/gqqunxeuo.sHtML

[U11] Py：生成器表达式
来源：http://www.share.zdbjq.cn/Article/details/gkpottweh.sHtML

(x * 2 for x in arr)
来源：http://baike.hesvh.cn/Article/details/gfaituipz.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gnaymtcam.sHtML

Counter(arr).most_common(3)
来源：http://3g.hesvh.cn/Article/details/gxwtoxphy.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/ghwrtuinj.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/ghlfjrmxv.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/gojapcrgf.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/grbtczchd.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/gkttalhtj.sHtML

t = time.perf_counter()
来源：http://www.blog.fehbvm.com/Article/details/ggphpaxei.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gftcevmzk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.fehbvm.com/Article/details/ghkmgecsb.sHtML

[U17] Py：初始化日志
来源：http://read.share.fehbvm.com/Article/details/gwcolkldm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/gpfzscyvt.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fehbvm.com/Article/details/galpxwngq.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/geigcrlek.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fehbvm.com/Article/details/gyarcxywj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.zdbjq.cn/Article/details/gyekibsid.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gxdlgwxpu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.zdbjq.cn/Article/details/ghixwmzjp.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.zdbjq.cn/Article/details/ggvaywewi.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/gdmsjkjnm.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gpqhgpjzu.sHtML

list(zip(*m))
来源：http://www.share.zdbjq.cn/Article/details/gpjnnngul.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/glbywrooe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/getorbdnh.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gczhqfnwl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/glildbyqe.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.hesvh.cn/Article/details/gblnlrimt.sHtML

csv.DictReader(f)
来源：http://blog.zdbjq.cn/Article/details/gapdxekne.sHtML

[U26] Py：并发下载
来源：http://baike.zdbjq.cn/Article/details/gtascxbix.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.hesvh.cn/Article/details/gviyyqhpl.sHtML

[U27] Py：异步 HTTP
来源：http://wap.hesvh.cn/Article/details/gsfazxkfd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.hesvh.cn/Article/details/gquyvkxov.sHtML

[U28] Py：类型别名
来源：http://blog.hesvh.cn/Article/details/gnotbvdts.sHtML

UserId = int
来源：http://3g.hesvh.cn/Article/details/gvlelcawt.sHtML

[U29] Py：属性校验
来源：http://www.blog.hesvh.cn/Article/details/gthsfszub.sHtML

@property 与 @x.setter 配合
来源：http://m.share.zdbjq.cn/Article/details/gfvrivwrs.sHtML

[U30] Py：数据类
来源：http://read.share.fehbvm.com/Article/details/gwncencbs.sHtML

@dataclass(slots=True)
来源：http://read.share.hesvh.cn/Article/details/gsydhgmfu.sHtML

[U31] Py：单测
来源：http://mobile.zdbjq.cn/Article/details/gopfgkjim.sHtML

python -m pytest -q
来源：http://mobile.hesvh.cn/Article/details/gwenrcgvm.sHtML

[U32] Py：代码格式化
来源：http://www.share.hesvh.cn/Article/details/gqepjcsoz.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fehbvm.com/Article/details/glniicuxw.sHtML

[U33] Py：打包发布
来源：http://blog.fehbvm.com/Article/details/gplrmuiff.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gziunhsld.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/gwsqmktgb.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gytkoaeft.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gleyyukjr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.hesvh.cn/Article/details/gcegcludo.sHtML

[U36] Py：定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gcuryvxyb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/ggxfdyztx.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.hesvh.cn/Article/details/gznkbjmpz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.hesvh.cn/Article/details/gfuqglufi.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/glwgtkrne.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gtvoddvvx.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.zdbjq.cn/Article/details/gqlpnmhyf.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/gskzvnimv.sHtML

[U40] Py：打印到标准错误
来源：http://wap.fehbvm.com/Article/details/gpnsqvwlp.sHtML

print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gveovhdua.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.hesvh.cn/Article/details/gqhsynsis.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fehbvm.com/Article/details/gfkapwflj.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gtfxbjkbf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fehbvm.com/Article/details/gstktipny.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gzamvultx.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gwxmkzlrc.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gyhpglfxr.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gmeapzhww.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gcigkrfie.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxcjlmb.sHtML

[U46] PHP：可空类型
来源：http://3g.zdbjq.cn/Article/details/gmlinadxv.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/gegnezpyy.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gvqvvlqeu.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gcmzkvqqr.sHtML

[U48] PHP：纯枚举
来源：http://3g.hesvh.cn/Article/details/gnugleqdn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.hesvh.cn/Article/details/grvbveart.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gmretluuq.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gwmqhggnu.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.zdbjq.cn/Article/details/gnkrdrckh.sHtML

public function __construct(private int $id) {}
来源：http://blog.fehbvm.com/Article/details/gpnlyvzew.sHtML

[U51] PHP：数组解构
来源：http://read.share.hesvh.cn/Article/details/gbcvmzzwj.sHtML

[$a, $b] = $arr;
来源：http://mobile.hesvh.cn/Article/details/gqbhkpyzy.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/glqjqkkcf.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.zdbjq.cn/Article/details/gizeytmkj.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fehbvm.com/Article/details/gueumjlwo.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gyakqmeiz.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/gcuhnftga.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gycjcmbqz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gvrefhmul.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/grsbryrfz.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gqdluclji.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gwrpxvqid.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gvvenzusj.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gttpoafem.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gkftxtkzy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvaljwoml.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.zdbjq.cn/Article/details/gxfsqxvji.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/grocchytv.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gdzgxvgwp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gxlqqtkes.sHtML

[U61] PHP：正则
来源：http://mobile.zdbjq.cn/Article/details/gplczcwmz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gqjnjuexv.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gcbqrsvsw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gejqxnhuz.sHtML

[U63] PHP：文件读写
来源：http://www.share.hesvh.cn/Article/details/gtxdbxtem.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gwvijfmgh.sHtML

[U64] PHP：目录遍历
来源：http://3g.fehbvm.com/Article/details/gnatwniof.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gbgdieyak.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gkbdexuqf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/guqnwlufl.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fehbvm.com/Article/details/gnmzfgiyn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gdeuyyqrw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gwcweqdvj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/giqzzqcut.sHtML

[U68] PHP：PDO 连接
来源：http://3g.hesvh.cn/Article/details/gbvbtoxll.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/guwvrbpvk.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.hesvh.cn/Article/details/gblmhoryd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fehbvm.com/Article/details/gcxhoafai.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gkqqubkfd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gdlrpdzee.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gsuklwusp.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gxhtwncds.sHtML

[U72] PHP：写错误日志
来源：http://read.share.hesvh.cn/Article/details/gbylbiikr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/ggngqgqac.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.zdbjq.cn/Article/details/gdatiuvrt.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gydtaeuvo.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gubaytlkp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gwpfgyacw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/gbfnwvrbo.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gcemdaunt.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gaouryumk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gvknkfzrb.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gtipxwxsc.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/ggkcwbvux.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gjcmnrsol.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.zdbjq.cn/Article/details/gczyamtqo.sHtML


<!-- 参考信息 -->