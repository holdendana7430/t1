代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gankvezcl.sHtML

[S57] C++：编译期常量
来源：http://baike.zdbjq.cn/Article/details/gijybzrba.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfwlrmold.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/giyhgjmmc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/ggiegmaab.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gzdqdldbg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gnlyhpjbx.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gdmzkigdw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gdcakgnkf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfvngfauv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/ghekwzaut.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmuvoyusi.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gmpcujgtc.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ghuwaesvq.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gjluqmjkd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gmqruqqxy.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gqbzzcuxv.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gugubrfzw.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gomuwnrxd.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gqrvohkuw.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gkhtbntss.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gfiwyhxsd.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gzxwxpbrl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gbipdqtwp.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gegejrrol.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gsrnshmrh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gkmjhbwzw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gwwbmnmwb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gkduykqmt.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gadjtcyzk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/guxtxibaw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gdkjyfnlc.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gxopwwhdq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gjfdluzqu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gdqspnmkg.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmfbacauv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gknfmdqpa.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gvwtipmyh.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gvojivsgn.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gafsmgcnx.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gyerlieiz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/geacgvlmv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gkiccusaz.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gaeejqlbs.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gwocefawe.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gnbzmbvph.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gddjembcj.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gixxafmuo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/ggjywmfxv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gfisfkmol.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/goayoaybx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.zdbjq.cn/Article/details/gwgyzznlb.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gxrxhshxe.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gtwozvnel.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gaeewhipv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/galmcztek.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gclcvjyve.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxogkogbn.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gkvawlcxe.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/goskspgla.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/gjfzwvoqf.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gizcdnske.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gyrflxqzz.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gqlsqdcgv.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/gscbxzisa.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gtbgxfvok.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gvwnouuub.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grqjdjgdg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gvxeatgeu.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gqrjutqvd.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gmizrataf.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gdmtbkpse.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gdkaqudqx.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grkxcasqr.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/glwcdcnvg.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gmbgmnylu.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gzzdpdlef.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gydqyfsou.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gqhsjroeo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gfpvldjex.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gphlkzcof.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.hesvh.cn/Article/details/gdkhhwbkl.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gljfuraqw.sHtML

function add(a, b) return a + b end
来源：http://blog.zdbjq.cn/Article/details/gabwtncez.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gmxoocljd.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gbaktkpef.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gazbylvlp.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/ggbadnxmn.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gkqzotfyo.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gbqummmdf.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gquusikgo.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gwujfwqtw.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsrxqtzze.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gaihjebfi.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gzvlorbto.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fehbvm.com/Article/details/ginkoggco.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcxtfugar.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/gihorxjak.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gwstlaafd.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/gptdgueie.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.zdbjq.cn/Article/details/gydbtrsac.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fehbvm.com/Article/details/gbfnkkyhd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/geuceztpf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gbojntnfh.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gnrytiatc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.zdbjq.cn/Article/details/gpvxjjlex.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/geblpqqox.sHtML

$s =~ s/old/new/g;
来源：http://baike.hesvh.cn/Article/details/gveegsehv.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gdxzspytl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gasbayxux.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfjzoczos.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fehbvm.com/Article/details/gytiamnuf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/ghtoxnicb.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkycmotna.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gehzqmmzw.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gobofnvbd.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gmbavsqko.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gcflcvobn.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gozowfrce.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gaivknagn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gftuwnwcq.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gefahkvcn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.zdbjq.cn/Article/details/gntlkctjj.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/guigxkuab.sHtML

case class User(name: String, age: Int)
来源：http://blog.zdbjq.cn/Article/details/gzuijbqst.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gasndfmjf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gaagwcpvj.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/gimfpvngq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.zdbjq.cn/Article/details/gegxzuobs.sHtML

[T59] Scala：循环
来源：http://wap.fehbvm.com/Article/details/galauuyxu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gvkvciyxc.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gssamjpyo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gkfpmrazt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grrrjyvrt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/ghdhchiyh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggmrptsaz.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.hesvh.cn/Article/details/gxdygasbw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.hesvh.cn/Article/details/gzguijutc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.hesvh.cn/Article/details/gpigtrcmm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.hesvh.cn/Article/details/gtjjabakb.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gvdrtmaox.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gbjlvwiue.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gwvjwlujb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/gxtbqoyla.sHtML

[U05] Py：列表去重且保序
来源：http://blog.hesvh.cn/Article/details/gbgkkjhtp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gwkpimphk.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/grrsmubju.sHtML

{**a, **b}
来源：http://www.blog.fehbvm.com/Article/details/gragtqinr.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gboppzbpn.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/gujvoyyvz.sHtML

[U08] Py：展平二维列表
来源：http://www.share.zdbjq.cn/Article/details/gqaaysino.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gapzagsmo.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fehbvm.com/Article/details/gwmpfpmdy.sHtML

max(d, key=d.get)
来源：http://baike.zdbjq.cn/Article/details/gmpcwgxwx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.hesvh.cn/Article/details/gnmvcrgjg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gdgctiprk.sHtML

[U11] Py：生成器表达式
来源：http://3g.fehbvm.com/Article/details/gwwrmytgk.sHtML

(x * 2 for x in arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwedrhvya.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.fehbvm.com/Article/details/gfosdizkf.sHtML

Counter(arr).most_common(3)
来源：http://blog.fehbvm.com/Article/details/grzdcnlkq.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gjfztsvmn.sHtML

deque(maxlen=10)
来源：http://read.share.hesvh.cn/Article/details/gsjlggrjr.sHtML

[U14] Py：分组收集到列表
来源：http://wap.zdbjq.cn/Article/details/gslfjlzle.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gggnbtvnt.sHtML

[U15] Py：高精度计时
来源：http://mobile.hesvh.cn/Article/details/gfublqtzp.sHtML

t = time.perf_counter()
来源：http://www.m.share.zdbjq.cn/Article/details/gqrkvatcx.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.hesvh.cn/Article/details/gbmupmqxj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.fehbvm.com/Article/details/gqusczrqv.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gpgzwnzyl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.zdbjq.cn/Article/details/ghpklgewn.sHtML

[U18] Py：预编译正则
来源：http://read.share.hesvh.cn/Article/details/gdqhfrdjw.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/getboadqj.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gldmejzaz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gofrseynx.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.hesvh.cn/Article/details/gljhhhzob.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.zdbjq.cn/Article/details/ggnqmkdqy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.hesvh.cn/Article/details/gufqivuji.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gxjwsfcnq.sHtML

[U22] Py：矩阵转置
来源：http://3g.zdbjq.cn/Article/details/gunzzlwtb.sHtML

list(zip(*m))
来源：http://3g.fehbvm.com/Article/details/ggwmftbbk.sHtML

[U23] Py：分块读取大文件
来源：http://baike.hesvh.cn/Article/details/gmiwbhjoi.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.fehbvm.com/Article/details/gjwaeizda.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/glguyhapz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfzfhemht.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.zdbjq.cn/Article/details/gypjdpekp.sHtML

csv.DictReader(f)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjqntdoj.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/ggqkfefng.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.fehbvm.com/Article/details/ggtojgvcr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.hesvh.cn/Article/details/gzuyexenl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://wap.zdbjq.cn/Article/details/ggrkvnzhp.sHtML

[U28] Py：类型别名
来源：http://baike.hesvh.cn/Article/details/gzwcdnbcs.sHtML

UserId = int
来源：http://www.share.zdbjq.cn/Article/details/gncpybjtp.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/gkojjdmci.sHtML

@property 与 @x.setter 配合
来源：http://mobile.fehbvm.com/Article/details/gruzukgnh.sHtML

[U30] Py：数据类
来源：http://blog.hesvh.cn/Article/details/gklqgldmm.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/ggqhkeegv.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/gsoxfcywb.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/grqpcjsud.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gwyuikaoa.sHtML

ruff format . && ruff check --fix .
来源：http://blog.fehbvm.com/Article/details/goqeclxve.sHtML

[U33] Py：打包发布
来源：http://wap.fehbvm.com/Article/details/giyhmndts.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fehbvm.com/Article/details/grshnwsem.sHtML

[U34] Py：判断编码
来源：http://m.share.fehbvm.com/Article/details/grxmhktok.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/ghdlindxb.sHtML

[U35] Py：发送邮件
来源：http://read.share.hesvh.cn/Article/details/gubvlqpdr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.zdbjq.cn/Article/details/gadhlztnl.sHtML

[U36] Py：定时任务
来源：http://read.share.fehbvm.com/Article/details/gcqcmtrtg.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fehbvm.com/Article/details/grlwkvrgc.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gdwkyudpv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbgojlm.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/ggswkicoz.sHtML

Path(__file__).resolve().parent
来源：http://mobile.hesvh.cn/Article/details/gmvbwpwtf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.zdbjq.cn/Article/details/gvvlewzit.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gikraolqf.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.hesvh.cn/Article/details/ghdkrtnfj.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gzttfjlhf.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fehbvm.com/Article/details/gbajmutjr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gobkspjiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.hesvh.cn/Article/details/gotpthtch.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.zdbjq.cn/Article/details/ggxsdgike.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.fehbvm.com/Article/details/giqhclaqw.sHtML

namespace App\Http;
来源：http://baike.fehbvm.com/Article/details/gtezjjxxi.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.hesvh.cn/Article/details/gbjexffdw.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/gghxeqspu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gsfrsyfds.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gqeokldby.sHtML

[U46] PHP：可空类型
来源：http://www.blog.fehbvm.com/Article/details/gfpnwcleh.sHtML

?string $name = null
来源：http://www.blog.fehbvm.com/Article/details/gzxjtihpq.sHtML

[U47] PHP：联合类型
来源：http://m.share.zdbjq.cn/Article/details/gmlbfwskn.sHtML

int|string $id
来源：http://www.share.fehbvm.com/Article/details/glizgulcw.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gikxrjylb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.zdbjq.cn/Article/details/glqakbelx.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/geqnotvzm.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gvyqdlmrx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/guytcdomd.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxnuhkmaq.sHtML

[U51] PHP：数组解构
来源：http://wap.fehbvm.com/Article/details/guobnnckn.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gqhbccseq.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gwgcrmzxq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gjuilvdwk.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/ghwixowrf.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.fehbvm.com/Article/details/gnujkpemy.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gcepcdfjx.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gatuumxdq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmjqempsm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gkfahmzxc.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gyaeeqhnv.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gkxoufext.sHtML

[U57] PHP：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gcidqwbji.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gntqujmbf.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/goigdaecx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fehbvm.com/Article/details/gcahhnukz.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.hesvh.cn/Article/details/glusmdsao.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gerktzpkt.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gdpzihuku.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.hesvh.cn/Article/details/ggqqjwkgg.sHtML

[U61] PHP：正则
来源：http://m.share.hesvh.cn/Article/details/gjhftoduz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gqzrrsddc.sHtML

[U62] PHP：日期对象
来源：http://baike.hesvh.cn/Article/details/gticsgmoz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/goluwmkio.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gbqwycbdy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gnuujpzly.sHtML

[U64] PHP：目录遍历
来源：http://baike.hesvh.cn/Article/details/gxzmqilou.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gsomqyiij.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gjevvdnwa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gmusrrkwe.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fehbvm.com/Article/details/gkbdvcvol.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gguhxjwcg.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gtccvityi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fehbvm.com/Article/details/gkrtwkgug.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.hesvh.cn/Article/details/gxjzquypy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gtheglrcu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gtdyyhyoy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.zdbjq.cn/Article/details/gvocgfurt.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqwrqek.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/grmnpqpqq.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/giupelhxd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gkbyootes.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gsrcrpieg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.fehbvm.com/Article/details/ghbanalyq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gndgaenpb.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gdbzurilq.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/grzfijcxs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/grmgjgrsg.sHtML

[U75] PHP：依赖注入
来源：http://3g.fehbvm.com/Article/details/gwkyyuhlq.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/grwafhbyt.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gfbyxnpku.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gxlnljyxg.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fehbvm.com/Article/details/gfjjuddmd.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gxxmfvbdg.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/ghftrpwap.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.hesvh.cn/Article/details/gvvbnajnj.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/goaekgiyn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gzrtpwhat.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fehbvm.com/Article/details/gtegqiqvi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gmlfcfqkg.sHtML

[U81] JS：初始化项目
来源：http://www.blog.fehbvm.com/Article/details/gwqiyyexb.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gmgvavhfs.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/ghqbzeitm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gakgpoour.sHtML


<!-- 参考信息 -->