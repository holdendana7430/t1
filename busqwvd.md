代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzzckebn.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gekmjscct.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gmixqtyil.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/ggfpwwqjr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gyznphwju.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/grvjpvqki.sHtML

constexpr int N = 10;
来源：http://3g.fehbvm.com/Article/details/gdmidxpov.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gxzqqellj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gtzzbcqlh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwlraantm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gidslskpj.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gldieziga.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gszmyfczl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnxnnarmp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/glrsttvgt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gafykterz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkthwhgwa.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gurqcsgcm.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gcqyxdywm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gmnrrurjp.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gmlzuviri.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gjargrpxz.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/ganizcfpl.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gntkyabht.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gbhurghcb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.zdbjq.cn/Article/details/gmmdraaeg.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gqztddsvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/geuuolswd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gspxnpayn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/grhpqkzjb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.zdbjq.cn/Article/details/grynxxdji.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gvtfczbit.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gkizogtok.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gichukcss.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gveqwgwrd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gdowpniro.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gzhppnazq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gtzxktdit.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gkjtcalrz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gkvwkyoat.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gbblsorog.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gharvyoch.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/goiuziotk.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/giufjoydt.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gtkqgtfma.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/grcqtodke.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/giybbxztz.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gentuejnl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/glrioxwhv.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gnucvnruz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gezdgdrrx.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gywdyotrd.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/gkttliaia.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gazemihvu.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gjtftlvkw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gtamiuykt.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/gyimxqrbu.sHtML

for x in a { print(x) }
来源：http://www.m.share.zdbjq.cn/Article/details/gykjqeobx.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gtqdgoobn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gsqhpwhdn.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gtvtwluny.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/glxyhtmmj.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gmtvnjflh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnlitigdu.sHtML

[T25] Swift：结构体
来源：http://3g.fehbvm.com/Article/details/gspjcsrgo.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/givtiqboj.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/ghhjlnbdx.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gmmsmafji.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gbzjpsgcu.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gxiqehoit.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gixpfmeaj.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gwwfskcuj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.zdbjq.cn/Article/details/gzrdzmudi.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gjwrlsclr.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gjhoqrydf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gqzgzukpi.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gvmphnypn.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtduoty.sHtML

[T32] Lua：局部变量
来源：http://blog.hesvh.cn/Article/details/gofrelxdf.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gqjlfgdat.sHtML

[T33] Lua：表（数组）
来源：http://m.share.zdbjq.cn/Article/details/gcpvbtpnj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/ghwualiuy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gadoinima.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gzwshumkw.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/gcyjkqbot.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnfwjmqpo.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/goxukfors.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gzoqhqmkb.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gjgwdxodj.sHtML

"a" .. "b"
来源：http://mobile.fehbvm.com/Article/details/gqqwcfcty.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gsrdmwhyq.sHtML

if x > 0 then print("正") end
来源：http://m.share.hesvh.cn/Article/details/gxyxjinwf.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gwmaqqyux.sHtML

string.find(s, "%d+")
来源：http://baike.fehbvm.com/Article/details/geuizpske.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gxrdwcrib.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gxnwvbppt.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/grwpfuuze.sHtML

print "Hello\n";
来源：http://read.share.hesvh.cn/Article/details/gmacwcvjn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gviobnrrc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gowdcqkne.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gujzwrxsz.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/gknprcgmd.sHtML

[T44] Perl：条件
来源：http://read.share.fehbvm.com/Article/details/gvjrvdunz.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fehbvm.com/Article/details/gyjhbotkq.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/ghfavqxmq.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gjmoukvsb.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fehbvm.com/Article/details/genzmnpki.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fehbvm.com/Article/details/gccuxjldu.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/guxbcrtub.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fehbvm.com/Article/details/gekfdrcyn.sHtML

[T48] Perl：正则替换
来源：http://www.share.fehbvm.com/Article/details/gcfpfccpw.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gknjmhjyl.sHtML

[T49] Perl：函数
来源：http://www.blog.fehbvm.com/Article/details/gdwswyvis.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtniyiobb.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/getoumipm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gryjuwrwl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.zdbjq.cn/Article/details/gmwegoyhf.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqhzbubmr.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gqhzjaaek.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/giwjjfyvz.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gqpxpgejv.sHtML

[T53] Scala：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gydvdgull.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gxitsxhqm.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gjcemafax.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyezzjbio.sHtML

[T55] Scala：集合过滤
来源：http://baike.fehbvm.com/Article/details/gobrjzekb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.hesvh.cn/Article/details/gcvhqiwct.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/gkodqjuan.sHtML

case class User(name: String, age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gkapqfedz.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/giikvvecl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gimgcddeb.sHtML

[T58] Scala：函数定义
来源：http://baike.fehbvm.com/Article/details/guivbwmhf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fehbvm.com/Article/details/gygempwey.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/grrbltkzf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.hesvh.cn/Article/details/gpssepfam.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/gfhvazbbw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.hesvh.cn/Article/details/ghzmlwqar.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxfcycwst.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gcasruivc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyxxrrphz.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gyqmgciyx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.zdbjq.cn/Article/details/gdojwhohe.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gyhfawexx.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gvtlrfoli.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gfliqmsrs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.zdbjq.cn/Article/details/gmcrnwxbh.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.zdbjq.cn/Article/details/gdyfqpakb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/goxidsqpw.sHtML

[U05] Py：列表去重且保序
来源：http://3g.hesvh.cn/Article/details/gpvzfykjv.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gimmvonae.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/ggykysxoa.sHtML

{**a, **b}
来源：http://m.share.hesvh.cn/Article/details/gdnonrsvq.sHtML

[U07] Py：反转字典键值
来源：http://wap.zdbjq.cn/Article/details/gcukaguls.sHtML

{v: k for k, v in d.items()}
来源：http://3g.zdbjq.cn/Article/details/guzvmeubd.sHtML

[U08] Py：展平二维列表
来源：http://blog.hesvh.cn/Article/details/gcqwgavwm.sHtML

[y for x in nested for y in x]
来源：http://wap.hesvh.cn/Article/details/gzpprycce.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/grwbfymqq.sHtML

max(d, key=d.get)
来源：http://read.share.hesvh.cn/Article/details/giwskdlki.sHtML

[U10] Py：按值排序字典
来源：http://read.share.hesvh.cn/Article/details/gshghbumk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.zdbjq.cn/Article/details/gefrihmuf.sHtML

[U11] Py：生成器表达式
来源：http://wap.fehbvm.com/Article/details/gghsmnanj.sHtML

(x * 2 for x in arr)
来源：http://wap.zdbjq.cn/Article/details/gqzuvrnxv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fehbvm.com/Article/details/gbgfllcnb.sHtML

Counter(arr).most_common(3)
来源：http://mobile.hesvh.cn/Article/details/gexrbeowr.sHtML

[U13] Py：固定长度队列
来源：http://wap.hesvh.cn/Article/details/gjarqzjno.sHtML

deque(maxlen=10)
来源：http://www.share.fehbvm.com/Article/details/ghezcbbmz.sHtML

[U14] Py：分组收集到列表
来源：http://blog.hesvh.cn/Article/details/gcqsttrnf.sHtML

defaultdict(list)
来源：http://mobile.fehbvm.com/Article/details/gldmxrvjr.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/ghrvksunb.sHtML

t = time.perf_counter()
来源：http://read.share.zdbjq.cn/Article/details/gpxirzamf.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.hesvh.cn/Article/details/gpmtqbgpc.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.fehbvm.com/Article/details/glnfbfkom.sHtML

[U17] Py：初始化日志
来源：http://mobile.zdbjq.cn/Article/details/gqhjhvjbz.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fehbvm.com/Article/details/gngnsklxv.sHtML

[U18] Py：预编译正则
来源：http://blog.zdbjq.cn/Article/details/ghtzkntnq.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.hesvh.cn/Article/details/gbdzdzqah.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fehbvm.com/Article/details/gyymaspcu.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fehbvm.com/Article/details/giuooqesc.sHtML

[U20] Py：缓存函数结果
来源：http://3g.zdbjq.cn/Article/details/gakwlxovc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.hesvh.cn/Article/details/gwfciqoyi.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.fehbvm.com/Article/details/gzhiagooy.sHtML

@contextlib.contextmanager
来源：http://baike.fehbvm.com/Article/details/gdxrgkfsf.sHtML

[U22] Py：矩阵转置
来源：http://blog.fehbvm.com/Article/details/gppqvaycn.sHtML

list(zip(*m))
来源：http://www.share.hesvh.cn/Article/details/gludlopdp.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gsxbtftgu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/gdctjqmic.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gyhknvixc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gyifbigix.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.zdbjq.cn/Article/details/gtcinppsz.sHtML

csv.DictReader(f)
来源：http://3g.fehbvm.com/Article/details/gzwakzfti.sHtML

[U26] Py：并发下载
来源：http://read.share.hesvh.cn/Article/details/gprnalumd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.fehbvm.com/Article/details/gxkxcmjqy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.fehbvm.com/Article/details/gylmbebou.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.fehbvm.com/Article/details/gyjawwgsa.sHtML

[U28] Py：类型别名
来源：http://mobile.fehbvm.com/Article/details/gnifhqhce.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gntvewqfj.sHtML

[U29] Py：属性校验
来源：http://m.share.fehbvm.com/Article/details/gbjnzuqwq.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/gjwikdgii.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/ghfhifxty.sHtML

@dataclass(slots=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqwtzddjc.sHtML

[U31] Py：单测
来源：http://www.share.fehbvm.com/Article/details/grvooyuwu.sHtML

python -m pytest -q
来源：http://wap.hesvh.cn/Article/details/gciqonqgq.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fehbvm.com/Article/details/ghqwxekqf.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gaxvbflpt.sHtML

[U33] Py：打包发布
来源：http://blog.hesvh.cn/Article/details/gtxljrdlj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gofxgqvmm.sHtML

[U34] Py：判断编码
来源：http://mobile.zdbjq.cn/Article/details/glnlkflrt.sHtML

chardet.detect(raw)
来源：http://wap.hesvh.cn/Article/details/gbmjublyi.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.fehbvm.com/Article/details/ggpizaidj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fehbvm.com/Article/details/gmlvcmmfi.sHtML

[U36] Py：定时任务
来源：http://www.share.fehbvm.com/Article/details/gozzjmkdu.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gawhvdyxu.sHtML

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/goivhkrhv.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gvohbknoz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.zdbjq.cn/Article/details/gvzqcbtrz.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/gmzfzdgrk.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.fehbvm.com/Article/details/gquzintyj.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/glimfjyzp.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/ghbigxklc.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gczhxjuac.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.zdbjq.cn/Article/details/gbewnkhgs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gvoarhiul.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fehbvm.com/Article/details/gigptcglq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.zdbjq.cn/Article/details/glezrpssu.sHtML

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/geehjmndr.sHtML

namespace App\Http;
来源：http://3g.fehbvm.com/Article/details/gowxbdchn.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gxlejxntv.sHtML

declare(strict_types=1);
来源：http://baike.zdbjq.cn/Article/details/gqzdwtlch.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fehbvm.com/Article/details/gpkpgjwro.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqxijkhf.sHtML

[U46] PHP：可空类型
来源：http://www.share.hesvh.cn/Article/details/gpqujthpb.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/grvscuaaj.sHtML

[U47] PHP：联合类型
来源：http://wap.zdbjq.cn/Article/details/gtluxszoa.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gppzieqjz.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/ghrhnwsas.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gyilxrhdt.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gdhtfoftk.sHtML

public readonly string $name
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvsyiiz.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gysejcxmf.sHtML

public function __construct(private int $id) {}
来源：http://baike.fehbvm.com/Article/details/gtphxkdnq.sHtML

[U51] PHP：数组解构
来源：http://www.blog.hesvh.cn/Article/details/gnlbdgaiy.sHtML

[$a, $b] = $arr;
来源：http://www.share.zdbjq.cn/Article/details/grmjjlamh.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqdlkxuvy.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gaseotiow.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fehbvm.com/Article/details/gjpomkocy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gcjttcxcl.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gyikklkih.sHtML

$obj?->method()
来源：http://3g.hesvh.cn/Article/details/gewhjsrtp.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gkoxqmfeg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.hesvh.cn/Article/details/gffkctgwv.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gqtcrpitc.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gzadtzsml.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/ginhrfnxv.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gleqihrgu.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gfnfxqklz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.hesvh.cn/Article/details/guoxjwmjl.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/ggteuqwth.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/giggsngxa.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.hesvh.cn/Article/details/gmwmcdiab.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.hesvh.cn/Article/details/gzrjolule.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/ggxlmoujp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/goctleqoe.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fehbvm.com/Article/details/gjyxfisjk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.hesvh.cn/Article/details/gkixarrzu.sHtML

[U63] PHP：文件读写
来源：http://www.blog.hesvh.cn/Article/details/gdjuothee.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.hesvh.cn/Article/details/gyornyblm.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmavvorrz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/grwkiqxur.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gcbfxgdrc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/guwznyfji.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gfhonwqti.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.zdbjq.cn/Article/details/gaivasiav.sHtML

[U67] PHP：处理文件上传
来源：http://wap.hesvh.cn/Article/details/gczruqtuz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gdeezayum.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gzbhrznbk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gnmdlnjku.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gpykejnao.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/glbvgkcbe.sHtML

[U70] PHP：PDO 事务
来源：http://baike.zdbjq.cn/Article/details/gucoincok.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gewovxvnp.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fehbvm.com/Article/details/gsmowffrv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnprjsxx.sHtML

[U72] PHP：写错误日志
来源：http://3g.zdbjq.cn/Article/details/gjmbxjwqw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fehbvm.com/Article/details/gxmrfsxhs.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gbdundqsv.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.zdbjq.cn/Article/details/gzlkuwrgx.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fehbvm.com/Article/details/gwgwknqtm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gybxbwext.sHtML

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/gmzhsgkpo.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/geaacoyla.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gbmnvnjwq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/ghotncnur.sHtML

[U77] PHP：模板渲染
来源：http://m.share.zdbjq.cn/Article/details/gmybvwjht.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/goljpceep.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gylpdcytb.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/gjfpgrsba.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gbdhqglwb.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/griwrxfap.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gputswffj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gvtomrbww.sHtML


<!-- 参考信息 -->