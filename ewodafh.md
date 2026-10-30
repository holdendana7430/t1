代发 wailian999

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gduzutphc.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/guxnakjpi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gjhivhpwd.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gbdrladmj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gqzlopaoq.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gayyctfyh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gdvroalrn.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gmxvicubf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gqqqtqhkm.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gucsrxtgv.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gcergwxgp.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gshejiddb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gknpmrysc.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gmjdlljbw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gtdsndfky.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gxckpwtxi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/guupxfsyp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjjvqfeec.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbdghxz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gomqaswvx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gnkkglyfn.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gjbwmqhsp.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gluaphguv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gxsdswoqp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gtbvmkfmt.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gcglnwxwb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gjyqphvsd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gufodtpoo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.zdbjq.cn/Article/details/guaqkztlh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/ghzszxsgl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gqvhltouh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtrhanpcs.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gzkzyylav.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/guatayntq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/gfpdzmtwl.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gfmexewat.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gcjnvstzc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gpxredbcl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gevlkrpny.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gnjyrrcys.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gxzwwyzry.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gwipnfjoh.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/gkqehztjx.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gtstyhyvu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gvnvyqlpq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/gysclexxb.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gpbtgjgxk.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gcwalgsfn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/goohsphdk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gmudeaslx.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/ggbevdyof.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/guvimyblc.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gmalatglp.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gdeblepjm.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gcvtasunb.sHtML

"值: \(b)"
来源：http://read.share.zdbjq.cn/Article/details/gsecubxzv.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fehbvm.com/Article/details/gkdfdzifa.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gwjkxbsfp.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/ggbknwyxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gpkvyzyuj.sHtML

[T21] Swift：遍历
来源：http://baike.zdbjq.cn/Article/details/glojzfips.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gemkrnagh.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gdeuuqawx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gemltcfyu.sHtML

[T23] Swift：函数
来源：http://blog.hesvh.cn/Article/details/guazveztp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/gerzybvvd.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gaoyahetw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/guflwjjso.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gmdzvosuo.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gfurfbgwh.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/guneoklsa.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gibgpqfqj.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gnmwrzhnr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gsbnzkfkq.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gsyawkmkx.sHtML

enum Color { case red, green }
来源：http://baike.hesvh.cn/Article/details/gzpbycerr.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/grbcihgdv.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gxuciunwt.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gitipwpek.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gfumractk.sHtML

[T31] Lua：Hello World
来源：http://baike.zdbjq.cn/Article/details/glbdmrxen.sHtML

print("Hello")
来源：http://m.share.zdbjq.cn/Article/details/ggltqmeuz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.hesvh.cn/Article/details/gayncdlug.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gqawktaww.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gyefgrqsz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.fehbvm.com/Article/details/guouuaxjn.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gaskxgcsl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gwadmqgai.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gcofuxxif.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.zdbjq.cn/Article/details/gncuzwnrt.sHtML

[T36] Lua：函数
来源：http://www.blog.hesvh.cn/Article/details/gwdcugvxy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gnuvqmotm.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gknpnurup.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gtngyveae.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gdkpsdukz.sHtML

if x > 0 then print("正") end
来源：http://blog.fehbvm.com/Article/details/grdblwmpd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gfiuxtbyf.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggrehuhdk.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gaioikhtg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ghansrcfi.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gajmwtajy.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gktffmeoi.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gfcbgpncu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gyryuekio.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gcgjukpnt.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gpyjncuua.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/ggoougixb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gawujgmlo.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gzgltbiqv.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fehbvm.com/Article/details/gfgtukykq.sHtML

[T46] Perl：哈希操作
来源：http://baike.hesvh.cn/Article/details/gsuhuzmdt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gbqyclrlh.sHtML

[T47] Perl：正则捕获
来源：http://mobile.hesvh.cn/Article/details/gkblxsxdm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.zdbjq.cn/Article/details/guaxwkgjb.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/gkhqyizrq.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gblllajjz.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/ggjxdaefs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gekncvyim.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gcsrepdzq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.zdbjq.cn/Article/details/gshvkcwxv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.hesvh.cn/Article/details/gyilldxmy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gtugbojac.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/grlkffbvn.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/ghnwrcbmq.sHtML

val a = 1;  var b = 2
来源：http://www.share.fehbvm.com/Article/details/grtooqcpt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gofvtbpgw.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/ghmaeassj.sHtML

[T54] Scala：集合映射
来源：http://mobile.fehbvm.com/Article/details/gcjbrkzgj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.hesvh.cn/Article/details/gpmudjzno.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gthahbcwv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/ggtklqqfi.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/geujfaoyw.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gpnjcxceg.sHtML

[T57] Scala：模式匹配
来源：http://wap.hesvh.cn/Article/details/gpeqajrah.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fehbvm.com/Article/details/godofqkyh.sHtML

[T58] Scala：函数定义
来源：http://wap.fehbvm.com/Article/details/gfsbpnzij.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gdhkkhvul.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/geknqexcy.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/gobfnlehz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.hesvh.cn/Article/details/ghxkaapvj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/ghzxmnqnh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gziqpkyqp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gzbxvffjo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gidxbtvwn.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gpmqbjdiy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.hesvh.cn/Article/details/gtjtilyao.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.zdbjq.cn/Article/details/gyaculamg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/gejjorgui.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gtwpqnvri.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.hesvh.cn/Article/details/gosplhfrv.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gmpsojwiw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gxterkwbd.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.zdbjq.cn/Article/details/gipjernry.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjlkvsbqj.sHtML

[U06] Py：合并两个字典
来源：http://read.share.hesvh.cn/Article/details/ggjmhufav.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/grhrrdilr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.zdbjq.cn/Article/details/gngjldpau.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.fehbvm.com/Article/details/gktnvshuc.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gvifgmnjy.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gyjwbqfum.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gysppwquo.sHtML

max(d, key=d.get)
来源：http://mobile.fehbvm.com/Article/details/galtyiurk.sHtML

[U10] Py：按值排序字典
来源：http://www.share.fehbvm.com/Article/details/gwfdwnguq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/grjfysqkl.sHtML

[U11] Py：生成器表达式
来源：http://mobile.hesvh.cn/Article/details/ghdfunotk.sHtML

(x * 2 for x in arr)
来源：http://baike.fehbvm.com/Article/details/gctvdaxaq.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gpuvuzahc.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gydhoaxhk.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gvxbooiyy.sHtML

deque(maxlen=10)
来源：http://mobile.hesvh.cn/Article/details/gsfdhrdgf.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.zdbjq.cn/Article/details/gnsdaajrz.sHtML

defaultdict(list)
来源：http://mobile.zdbjq.cn/Article/details/gbjejjbra.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/glonymedv.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gysegrchk.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.zdbjq.cn/Article/details/gvziwnqck.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/gjutmuuup.sHtML

[U17] Py：初始化日志
来源：http://baike.zdbjq.cn/Article/details/gbxyhfara.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.hesvh.cn/Article/details/gekqbdjpn.sHtML

[U18] Py：预编译正则
来源：http://www.blog.zdbjq.cn/Article/details/ggppviakx.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.hesvh.cn/Article/details/gciuaugvb.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gmljzssbl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gkmknacej.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/gmptchltr.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gfucrvtef.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/gwcwptjfs.sHtML

@contextlib.contextmanager
来源：http://www.share.hesvh.cn/Article/details/gmiihzica.sHtML

[U22] Py：矩阵转置
来源：http://read.share.fehbvm.com/Article/details/ghjvaulwb.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gsrunrwpp.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gtxsawjxw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.hesvh.cn/Article/details/gkqqksenv.sHtML

[U24] Py：路径操作
来源：http://3g.hesvh.cn/Article/details/gnpeasysp.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gorhqqnwn.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/gvtjvlcze.sHtML

csv.DictReader(f)
来源：http://baike.zdbjq.cn/Article/details/gnsaoltoo.sHtML

[U26] Py：并发下载
来源：http://blog.fehbvm.com/Article/details/gguapgjob.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gkrorkjwp.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fehbvm.com/Article/details/gkvnxqjgm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gtldjfmxe.sHtML

[U28] Py：类型别名
来源：http://blog.zdbjq.cn/Article/details/gujfuvvwr.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gyxojjbka.sHtML

[U29] Py：属性校验
来源：http://www.blog.zdbjq.cn/Article/details/gxpiayrmx.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gruuggbav.sHtML

[U30] Py：数据类
来源：http://m.share.zdbjq.cn/Article/details/gqqfsjjip.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gecuxojow.sHtML

[U31] Py：单测
来源：http://3g.fehbvm.com/Article/details/gdttemjnr.sHtML

python -m pytest -q
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcylsmb.sHtML

[U32] Py：代码格式化
来源：http://wap.hesvh.cn/Article/details/gmmsrowcj.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gywbmrexf.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gylfyayec.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.hesvh.cn/Article/details/gtggodunp.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/gcykvpgbp.sHtML

chardet.detect(raw)
来源：http://www.m.share.fehbvm.com/Article/details/gmklhhxhm.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/gavirclvv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fehbvm.com/Article/details/grtpiwcbd.sHtML

[U36] Py：定时任务
来源：http://blog.zdbjq.cn/Article/details/gdhserram.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.blog.zdbjq.cn/Article/details/gpqwbdkyf.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gaequoego.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.zdbjq.cn/Article/details/gadmppbwg.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gvmsmauts.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gnfczgwyt.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.hesvh.cn/Article/details/gpksnqocn.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/ggwzlghry.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gmexuiaff.sHtML

print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gnlyvwldk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gtevyyxbp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gfetrjwky.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/grhqeelhy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkaxmhd.sHtML

[U43] PHP：声明命名空间
来源：http://blog.hesvh.cn/Article/details/glnxhilpv.sHtML

namespace App\Http;
来源：http://3g.hesvh.cn/Article/details/gmffkebcb.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gzlkzckuv.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gsdwikhal.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/girwofhzr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/goswqqoip.sHtML

[U46] PHP：可空类型
来源：http://blog.hesvh.cn/Article/details/ghatyxlbb.sHtML

?string $name = null
来源：http://read.share.hesvh.cn/Article/details/gkypquqzx.sHtML

[U47] PHP：联合类型
来源：http://www.blog.zdbjq.cn/Article/details/gwrxaeqxx.sHtML

int|string $id
来源：http://mobile.hesvh.cn/Article/details/ghcmurlzu.sHtML

[U48] PHP：纯枚举
来源：http://read.share.fehbvm.com/Article/details/gtkvwdgwu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.hesvh.cn/Article/details/gidyfcfos.sHtML

[U49] PHP：只读属性
来源：http://read.share.zdbjq.cn/Article/details/gjoduwugc.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/gypsblugx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.hesvh.cn/Article/details/gbvwphrrc.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gcxerejch.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gromrxwnx.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gunajznvx.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gktxeyxmo.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gcpqxmdic.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.zdbjq.cn/Article/details/gvhwjebmb.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.hesvh.cn/Article/details/gmgwcqtia.sHtML

[U54] PHP：空安全调用
来源：http://3g.fehbvm.com/Article/details/gqjnniewm.sHtML

$obj?->method()
来源：http://blog.zdbjq.cn/Article/details/grdkizfqc.sHtML

[U55] PHP：match 表达式
来源：http://wap.fehbvm.com/Article/details/grsuezbgo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gelngmcal.sHtML

[U56] PHP：命名参数
来源：http://read.share.fehbvm.com/Article/details/gzopawwgb.sHtML

f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gtnzduzxh.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gudcwbtzr.sHtML

"值: {$a}"
来源：http://www.share.hesvh.cn/Article/details/gprwenspz.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ggmtvtyqo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gioxfeixr.sHtML

[U59] PHP：自定义排序
来源：http://blog.hesvh.cn/Article/details/gxnoqbsjf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gypmuvmmg.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/goqalrboz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gbfyzpltv.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gspovckny.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/guevsmdwz.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gykipkhxb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gjyzlncfl.sHtML

[U63] PHP：文件读写
来源：http://mobile.fehbvm.com/Article/details/gvomuyfnt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gdmduwaql.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/ggjhdoqwr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/glhydtzsu.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/ggxckiuxb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gucmedpwp.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fehbvm.com/Article/details/grqsvrdzh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/gancrlzpc.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gmbzvjdjc.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.hesvh.cn/Article/details/guwxevgwi.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gfdbqeuuj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/gmrsahpqc.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gcabajhyl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/geyscppzw.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.hesvh.cn/Article/details/gxibmuudm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gzwmofmjn.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gnamjueni.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.zdbjq.cn/Article/details/gqluoxppm.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gsiijkgdv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fehbvm.com/Article/details/gilpeambi.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gpwrpjhnn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gglhqblql.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/ghltcufzm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.zdbjq.cn/Article/details/gpuhrhgol.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/ggazvizle.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gbxttuves.sHtML

[U76] PHP：简单路由
来源：http://mobile.fehbvm.com/Article/details/gybqozzop.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/genzshtxg.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/grwidcvhd.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gigqhwnyg.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gvxiigtbp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.fehbvm.com/Article/details/gkcaxmtbw.sHtML


<!-- 参考信息 -->