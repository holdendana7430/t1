代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfwoalar.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/giymqxixh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/ghfddtvum.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gqkcoowjg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gduxwzdnd.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gxsfmamfv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gtwkieqps.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gnxjwdlok.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gfpbgiedk.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gkuruthwz.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gxyrijnkd.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/gfpyhhxvb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gigqdgatq.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gptzxppcj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gqftawpiu.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gkdhhyjcm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ggdjlzbvk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvopnxzco.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/geicelpur.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghetuhslb.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gdnpcgvst.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpqozurzu.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gnnyeyjcf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gdtnbrdsj.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gahasghdj.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gbihvscqn.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gipxzjzfc.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gfdeiitcz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gsaqivizx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gpbqnkfnm.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/gncketmcn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gkdolfzoa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbmirxvyk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/glypudzdo.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/grdirtaum.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fehbvm.com/Article/details/gvoduwlxc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gjtkdjpuj.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gspcvibev.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gjnjogzbk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gcazsmtat.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gxpjiydku.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gttavkttp.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gobbcclpf.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gcvknflwh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/geunsezrp.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggigkyqnx.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gswpcxlgs.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gkajbmfnf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gynntzvbl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/garnnoizl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gwgbvlldk.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gagadwvkc.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gqpkkycfu.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gmjuvzyth.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gkwdnsblz.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/grrbtwrcg.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gtxohmrnf.sHtML

if let n = opt { print(n) }
来源：http://baike.hesvh.cn/Article/details/gwntpjreg.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gvyqstbub.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gjrzftkfo.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gjmiqfnch.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gncgwhtfx.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/ghxuzxdjv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gdhaxgcpc.sHtML

[T23] Swift：函数
来源：http://blog.zdbjq.cn/Article/details/ghlmxckqm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gxlhakszj.sHtML

[T24] Swift：闭包
来源：http://mobile.fehbvm.com/Article/details/gmkbbxpkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gjqqumkou.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gyauzycqc.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gkjxmmqci.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gvodwrxjl.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gtkfyeolb.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gtnwsdkeh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gomzcijuw.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/gbnbmopyl.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gwtexwlee.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gghnwiltj.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gudxkesvc.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gyfotvtzd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/geeamimim.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gjballazn.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvymlzrbk.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/ggvafmkwx.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/gapejfjiy.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/grjmjoiiw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gpdspvnno.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/guxiumkvi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fehbvm.com/Article/details/gdlbnopel.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gszttfwvy.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gdwcgfggo.sHtML

[T36] Lua：函数
来源：http://mobile.zdbjq.cn/Article/details/gbjgyeckw.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gjdgvrehx.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gaivkfzba.sHtML

"a" .. "b"
来源：http://www.blog.fehbvm.com/Article/details/giqshfbsb.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gdmyqcsos.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gwsghpxap.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/gffpzqpca.sHtML

string.find(s, "%d+")
来源：http://read.share.fehbvm.com/Article/details/gwolelriq.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/guafpxwjx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gkpjteisl.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gvcqgdxgr.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gcjlohhbs.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gptjlgpxw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gapwhmsuk.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gqxsplokv.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gbaixhhxa.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gelswijxy.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.hesvh.cn/Article/details/gzwwiysbq.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fehbvm.com/Article/details/gtcbcttvt.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gnvsrmwnq.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gjarrorxc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gsrxurzab.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fehbvm.com/Article/details/gvmdsbbcw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gxxyqmztt.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/glnqbotfv.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.zdbjq.cn/Article/details/gnxtekmpv.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gcelldrqm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gkitundge.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggtjuwyhc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fehbvm.com/Article/details/gcmyujgwg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.hesvh.cn/Article/details/gltwmencr.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gvmehsqkb.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/glqrpfqta.sHtML

[T52] Scala：变量
来源：http://blog.zdbjq.cn/Article/details/girglccsp.sHtML

val a = 1;  var b = 2
来源：http://mobile.zdbjq.cn/Article/details/gxpjadhdt.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gwyyrbgob.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/grxcpoxsg.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gktuyxeuo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/goneyvyvi.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzktbhjfa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkzkrtggw.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/grykuhuat.sHtML

case class User(name: String, age: Int)
来源：http://blog.fehbvm.com/Article/details/ghispvmof.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmuihzudj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gdhpjfoem.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gsjgcdpgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.hesvh.cn/Article/details/gcmqeuhnb.sHtML

[T59] Scala：循环
来源：http://www.blog.hesvh.cn/Article/details/gwfdnkavq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gosrcmrfl.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gbeipfmdg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.zdbjq.cn/Article/details/gabwajjrj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gszsxdcip.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gtqdrvzww.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmfjfcotm.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.hesvh.cn/Article/details/gmfqxrylx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.hesvh.cn/Article/details/ghtqjkvei.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.hesvh.cn/Article/details/gjpxatwjb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsnpipwyw.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.zdbjq.cn/Article/details/gnhauwfef.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gxxzvdljw.sHtML

[U04] Py：变量调试打印
来源：http://mobile.hesvh.cn/Article/details/gunpmugvg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fehbvm.com/Article/details/geyzzdccz.sHtML

[U05] Py：列表去重且保序
来源：http://3g.zdbjq.cn/Article/details/gnewkcvlf.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gdocbxoyz.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.hesvh.cn/Article/details/gbafdazdq.sHtML

{**a, **b}
来源：http://www.blog.zdbjq.cn/Article/details/gbtqrbmud.sHtML

[U07] Py：反转字典键值
来源：http://read.share.fehbvm.com/Article/details/ggbvftnzt.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.hesvh.cn/Article/details/ggppnjzfu.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.zdbjq.cn/Article/details/gsoapihry.sHtML

[y for x in nested for y in x]
来源：http://m.share.fehbvm.com/Article/details/ggcnasaza.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.zdbjq.cn/Article/details/gbabisllc.sHtML

max(d, key=d.get)
来源：http://wap.fehbvm.com/Article/details/grchqpplh.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gdetagymf.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/guvtmtogd.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/giumiucow.sHtML

(x * 2 for x in arr)
来源：http://3g.fehbvm.com/Article/details/gzlgidajw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.hesvh.cn/Article/details/gsiqnhgqk.sHtML

Counter(arr).most_common(3)
来源：http://blog.hesvh.cn/Article/details/gnmodlofy.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gvvfchspb.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gwnqgbjfl.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gjlisnhai.sHtML

defaultdict(list)
来源：http://www.share.zdbjq.cn/Article/details/gqvffbsmk.sHtML

[U15] Py：高精度计时
来源：http://baike.zdbjq.cn/Article/details/gdbzbstxb.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gsoynyccs.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.zdbjq.cn/Article/details/gcoykasih.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.fehbvm.com/Article/details/gzgrjxrec.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gyvbafwlb.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fehbvm.com/Article/details/gponijchs.sHtML

[U18] Py：预编译正则
来源：http://3g.hesvh.cn/Article/details/gghbjbtzv.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gslyjgsqf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.zdbjq.cn/Article/details/gfbkvpqhe.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.hesvh.cn/Article/details/gvnihxrli.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.fehbvm.com/Article/details/gcqxfkmag.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/gntaqmxje.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.zdbjq.cn/Article/details/gyqmjsdql.sHtML

@contextlib.contextmanager
来源：http://blog.fehbvm.com/Article/details/gdijgnocy.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gzmkylrpt.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/ghcjovyqs.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gazhelpyw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fehbvm.com/Article/details/gwtjfavgp.sHtML

[U24] Py：路径操作
来源：http://mobile.hesvh.cn/Article/details/grepgejej.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfhctnqlz.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.zdbjq.cn/Article/details/gkblkchgr.sHtML

csv.DictReader(f)
来源：http://www.m.share.hesvh.cn/Article/details/gcockdmrm.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/goscfqicm.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fehbvm.com/Article/details/gkifhfgos.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.zdbjq.cn/Article/details/gxongvdfk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/glljpkgck.sHtML

[U28] Py：类型别名
来源：http://www.share.hesvh.cn/Article/details/gzyhunbya.sHtML

UserId = int
来源：http://baike.zdbjq.cn/Article/details/geqyyeqgt.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gtnyfkpau.sHtML

@property 与 @x.setter 配合
来源：http://baike.zdbjq.cn/Article/details/gebmzvwvm.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gwjrmcuky.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/guifayswo.sHtML

[U31] Py：单测
来源：http://wap.fehbvm.com/Article/details/gwllrprut.sHtML

python -m pytest -q
来源：http://3g.hesvh.cn/Article/details/gnypjbcgn.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gtwdnspkn.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gpcxozzoq.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gpxtxfwdx.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.zdbjq.cn/Article/details/gkcfiqbjy.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gqoinhobh.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gxzqpablb.sHtML

[U35] Py：发送邮件
来源：http://baike.hesvh.cn/Article/details/gjxhwoxlf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gletkkcfz.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gpfyopfvs.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.zdbjq.cn/Article/details/gmpafcfcm.sHtML

[U37] Py：读写 Excel
来源：http://m.share.hesvh.cn/Article/details/gcsjtfrwl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.fehbvm.com/Article/details/giwyywghg.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.hesvh.cn/Article/details/gpiemgano.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gkaokzykv.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/genmmbtwv.sHtML

sys.stdout.isatty()
来源：http://www.share.fehbvm.com/Article/details/gmrijtjqg.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.hesvh.cn/Article/details/grmspkvke.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gxifrxzhg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.hesvh.cn/Article/details/gzxcyckld.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gitmuaheg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.fehbvm.com/Article/details/guhiqqesm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gfiyijlnv.sHtML

[U43] PHP：声明命名空间
来源：http://baike.fehbvm.com/Article/details/grzocjbqx.sHtML

namespace App\Http;
来源：http://www.m.share.zdbjq.cn/Article/details/gerlzmmfa.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.zdbjq.cn/Article/details/gbmwxejfm.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gchdxtcpf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gpuxyzwad.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gjrjuladl.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gmoxvoyyi.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/girbwqbpl.sHtML

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gjbhazpjf.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/gedtjlpzt.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gtincnpsw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvdpmsaes.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gqzvugbji.sHtML

public readonly string $name
来源：http://www.share.zdbjq.cn/Article/details/gosuhhdwe.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/gvrrmkdqu.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/guobvpktq.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcacplsfe.sHtML

[$a, $b] = $arr;
来源：http://baike.zdbjq.cn/Article/details/gywbvnocm.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gjomdmgbp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gdejrzeeu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gfnsvlgfh.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/gpjnnpmho.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gheahhhna.sHtML

$obj?->method()
来源：http://www.share.zdbjq.cn/Article/details/gtzjvneiz.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gpwexiipd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gpkrjrcjn.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/giebdlcwu.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gbnhbzxsy.sHtML

[U57] PHP：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvtabqett.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gbpvmrklu.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/glsxlfpga.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gkgtegtqt.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/ggwgzhqsf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ghfqugfbb.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gutapkuko.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/gvvlajspy.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gioiuqoks.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gjawkioun.sHtML

[U62] PHP：日期对象
来源：http://read.share.fehbvm.com/Article/details/gcbqhlarc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gstgbgdmg.sHtML

[U63] PHP：文件读写
来源：http://mobile.hesvh.cn/Article/details/gxpcppzdd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/grqclesmw.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/grwjubhqz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gleypebbp.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gawevnaqn.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gajtepwjn.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gusmizemn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.hesvh.cn/Article/details/gdcbztywl.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/gzbpijprz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gayinialx.sHtML

[U68] PHP：PDO 连接
来源：http://wap.fehbvm.com/Article/details/gaucgiwtx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gmrsgtpes.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/glomngevy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gjstrhfoc.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gwkjhkvmm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fehbvm.com/Article/details/gnlqdnrvf.sHtML

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/ggrmtijff.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gzbvvbvhh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.hesvh.cn/Article/details/ghpipzkem.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.hesvh.cn/Article/details/gqwjlythx.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gjxiyuojs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gzcgfjsnl.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gfprjxlty.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gqvlpufhd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.hesvh.cn/Article/details/gshrdyufy.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/geiyfpsvt.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/ggyhveodl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gfkmjirbu.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/gcdjoibht.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gqxkhaakm.sHtML

[U78] PHP：单元测试
来源：http://baike.hesvh.cn/Article/details/gbovuqwks.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gvxmnygnl.sHtML


<!-- 参考信息 -->