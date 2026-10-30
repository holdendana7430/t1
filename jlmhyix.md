代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gnpjcwrdn.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gmdnaesld.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/ggcxrtfho.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.zdbjq.cn/Article/details/gncongpka.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gnaqnqbib.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwxytjpqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gwtdgwxne.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbjpymuvu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gpeoqoxoe.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gjusmgsvx.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gzflymxax.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gvtetuvly.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gjorptkyh.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/geashlmyr.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gpvjhswpt.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gaellouoh.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/ghaeabhij.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gpxvrnrvx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gyymbvias.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gmkgyhuyh.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/grafbonxd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gvflikrwc.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gpssrnxrh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzdmjriaw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gnxlrfkuu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gtdrgcbry.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gpvhjuigu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gdinylylb.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gpyotjmmo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gefviufhy.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gkrgllech.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gclajxvzx.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gkhzyhnbm.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/goqchpwvu.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gfjaaeznv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gwlelwdwq.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gbktgczdx.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gdanswqog.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/grkbaqvvx.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gpnbntdzs.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gmiylwmgj.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gnmaprozd.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gywbezxek.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gmycbnoac.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/gkarqoptw.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gzzjhxspa.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gljvoimjk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/glqqsehgi.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gpcffchti.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/gluuroghw.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gmtaavmmp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gyvhltocv.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gvjmonytl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gmmukkwwe.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/galegvdel.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqrfzrxyt.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gughqfhzb.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/gcljqglyr.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/guembpali.sHtML

class A: Base { override func f() {} }
来源：http://m.share.zdbjq.cn/Article/details/gxnzwtgau.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/gfipmbvpr.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gzxpzrkuj.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gjsdjwgqp.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/ggnwotlvs.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gzcgrwmam.sHtML

guard let x = opt else { return }
来源：http://m.share.zdbjq.cn/Article/details/gifdmvlob.sHtML

[T30] Swift：协议
来源：http://baike.zdbjq.cn/Article/details/gduvipbyu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gvhetoaop.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjpezcdyy.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gtvwcpwft.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gwxoblncn.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gfdblipyf.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gxiwfwmzj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gfndtqzly.sHtML

[T34] Lua：遍历表
来源：http://read.share.zdbjq.cn/Article/details/gkkkcixkb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.hesvh.cn/Article/details/gabmibgai.sHtML

[T35] Lua：字典表
来源：http://read.share.fehbvm.com/Article/details/gcnuhiupa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gasfhjfjp.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gtttvokjh.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gquzibjbi.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gvtxzvyeb.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gfmdllynv.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grxzfchoj.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/guculjdui.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gnmbysqrw.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/giccyspuc.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gncyawibj.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gednfalan.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/guwewaaor.sHtML

print "Hello\n";
来源：http://blog.zdbjq.cn/Article/details/gdpgswhlx.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gdohitkyw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fehbvm.com/Article/details/gtocjlqge.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/ggzwyqlhd.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gjkqwssqg.sHtML

[T44] Perl：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzckuosqk.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/gfwptryzi.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gogcgrajq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.zdbjq.cn/Article/details/gqjljinje.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.zdbjq.cn/Article/details/gzygnsddv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gpsnthvyc.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/ghuopmdnf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fehbvm.com/Article/details/gynalkokn.sHtML

[T48] Perl：正则替换
来源：http://3g.zdbjq.cn/Article/details/gheenutcx.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gljqwkafi.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gesmuirhr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gsxnvgjwl.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/greibutiz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gyxfdtizb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.hesvh.cn/Article/details/gcwdnlnqu.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxtaixsqt.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gduwjazgb.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/gmqpflueo.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/gycniwlrw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gisfpuzni.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/guisveoan.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gykofmxys.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/ghtxrgdla.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/glplxqiux.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/glsnuqdbb.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gjenjkmno.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gykzgqppt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gkrswurax.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpakeqnkh.sHtML

[T58] Scala：函数定义
来源：http://wap.zdbjq.cn/Article/details/gxegnmzfz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.hesvh.cn/Article/details/gebopskzs.sHtML

[T59] Scala：循环
来源：http://m.share.fehbvm.com/Article/details/gpekqgeyt.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gtaqugvew.sHtML

[T60] Scala：折叠
来源：http://wap.hesvh.cn/Article/details/gtfhwvocs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fehbvm.com/Article/details/geelouecf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpzkvbgbc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gasmcqeej.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gswmscklj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gkntvzuja.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gynjtqack.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/geigjnian.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gwpubiauc.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.zdbjq.cn/Article/details/gafgyngow.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.hesvh.cn/Article/details/gtrnyfwtf.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gfalgjhtu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.hesvh.cn/Article/details/gyrquniuq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fehbvm.com/Article/details/gcgfldsfb.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gcnfdaibe.sHtML

[U06] Py：合并两个字典
来源：http://blog.hesvh.cn/Article/details/gywxgfavz.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/gjabyrpdj.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.zdbjq.cn/Article/details/gjvjcjozj.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.hesvh.cn/Article/details/gzjwixujf.sHtML

[U08] Py：展平二维列表
来源：http://baike.hesvh.cn/Article/details/gcbcynyag.sHtML

[y for x in nested for y in x]
来源：http://www.blog.zdbjq.cn/Article/details/gwreeswhy.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/gwjgzbhja.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gwiyyqnxk.sHtML

[U10] Py：按值排序字典
来源：http://wap.zdbjq.cn/Article/details/gayjzobxu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.zdbjq.cn/Article/details/gtfpvdyya.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fehbvm.com/Article/details/gdvcxbcta.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/glkhckbrn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/gdgtcclhp.sHtML

Counter(arr).most_common(3)
来源：http://wap.zdbjq.cn/Article/details/gauiwxlih.sHtML

[U13] Py：固定长度队列
来源：http://www.share.zdbjq.cn/Article/details/gyqfxorrh.sHtML

deque(maxlen=10)
来源：http://www.blog.hesvh.cn/Article/details/gtjlmczhz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/grctgqjau.sHtML

defaultdict(list)
来源：http://www.m.share.fehbvm.com/Article/details/gzwkiclch.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/grdpzsysi.sHtML

t = time.perf_counter()
来源：http://mobile.zdbjq.cn/Article/details/goyqgiesw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.hesvh.cn/Article/details/glwzcmpyi.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gkyujoxub.sHtML

[U17] Py：初始化日志
来源：http://blog.hesvh.cn/Article/details/ggqjorlcu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.zdbjq.cn/Article/details/guwllvpjd.sHtML

[U18] Py：预编译正则
来源：http://www.share.fehbvm.com/Article/details/gyvxehizo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gkjngqqgs.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.zdbjq.cn/Article/details/grbwcocup.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/ghxtukxoo.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.zdbjq.cn/Article/details/gaplrpdgf.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.zdbjq.cn/Article/details/goxqtpsnj.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gqblwilae.sHtML

@contextlib.contextmanager
来源：http://read.share.zdbjq.cn/Article/details/gzcwmjsvs.sHtML

[U22] Py：矩阵转置
来源：http://read.share.zdbjq.cn/Article/details/ganglljnc.sHtML

list(zip(*m))
来源：http://m.share.fehbvm.com/Article/details/gfsctlits.sHtML

[U23] Py：分块读取大文件
来源：http://3g.hesvh.cn/Article/details/gyjnsxjwe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/ggyjxtrju.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/ggfckyuge.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gikrtckty.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.zdbjq.cn/Article/details/gxbjzqkhu.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gckvzppfn.sHtML

[U26] Py：并发下载
来源：http://www.share.zdbjq.cn/Article/details/gvgxxzfdw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.hesvh.cn/Article/details/grvklhnce.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gssyyaxjv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.hesvh.cn/Article/details/gvuntzwgu.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/gydsrnvml.sHtML

UserId = int
来源：http://wap.hesvh.cn/Article/details/ggqalyuxz.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gcqplmkvl.sHtML

@property 与 @x.setter 配合
来源：http://wap.zdbjq.cn/Article/details/godbkhppv.sHtML

[U30] Py：数据类
来源：http://mobile.fehbvm.com/Article/details/ggqnxking.sHtML

@dataclass(slots=True)
来源：http://m.share.fehbvm.com/Article/details/gcgdfdktn.sHtML

[U31] Py：单测
来源：http://www.share.hesvh.cn/Article/details/ghgjjhmcy.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gvmpekcka.sHtML

[U32] Py：代码格式化
来源：http://baike.fehbvm.com/Article/details/ggafupgjt.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.hesvh.cn/Article/details/gybpikhxm.sHtML

[U33] Py：打包发布
来源：http://baike.zdbjq.cn/Article/details/gnbkirnar.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.zdbjq.cn/Article/details/gcasmlrsa.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gieraljmw.sHtML

chardet.detect(raw)
来源：http://www.blog.hesvh.cn/Article/details/gihdsyieq.sHtML

[U35] Py：发送邮件
来源：http://blog.zdbjq.cn/Article/details/gwvigxqyg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.zdbjq.cn/Article/details/gfzpwdova.sHtML

[U36] Py：定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwhscgnol.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.zdbjq.cn/Article/details/gunfpwqwl.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.zdbjq.cn/Article/details/gtyvrdjnn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.zdbjq.cn/Article/details/gnrjnprea.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fehbvm.com/Article/details/ghqanohdc.sHtML

Path(__file__).resolve().parent
来源：http://m.share.hesvh.cn/Article/details/glwrnfsmw.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fehbvm.com/Article/details/gfiwpniaz.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gvxgoyiuo.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.fehbvm.com/Article/details/grffvcraf.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/ggchiccom.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gujwyxpot.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fehbvm.com/Article/details/ginkttypr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gcjlyzrau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.zdbjq.cn/Article/details/gqzmtzlkl.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gniacaiug.sHtML

namespace App\Http;
来源：http://wap.fehbvm.com/Article/details/gfmstszpm.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gqansuaen.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gwyggwhkb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/ggicckztu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gpjhfroyh.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gqsacrbov.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gaepaoxxk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gjmdjnybv.sHtML

int|string $id
来源：http://blog.hesvh.cn/Article/details/goplbmkmc.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.hesvh.cn/Article/details/gruvenajd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.hesvh.cn/Article/details/gyhovhsvz.sHtML

[U49] PHP：只读属性
来源：http://www.share.fehbvm.com/Article/details/gvbyrivil.sHtML

public readonly string $name
来源：http://mobile.hesvh.cn/Article/details/gargyrsqh.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gjdoeqxvv.sHtML

public function __construct(private int $id) {}
来源：http://mobile.hesvh.cn/Article/details/gurnwzujz.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gyggcvejc.sHtML

[$a, $b] = $arr;
来源：http://read.share.hesvh.cn/Article/details/gcixwnsxl.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gszwugxsp.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.hesvh.cn/Article/details/gslivlyoq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/grgrwdjxt.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.zdbjq.cn/Article/details/gkjvimxkc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/gmygpffow.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gothyumgg.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/guhaqbmze.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/goqowzwbe.sHtML

[U56] PHP：命名参数
来源：http://blog.hesvh.cn/Article/details/guedrudnq.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/grktwueth.sHtML

[U57] PHP：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gtmliyasg.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gtfhdxtne.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gozuevbvn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gclwnygfj.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gwkwwmypb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gvwlbonwt.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gewmhimui.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gtyuucrzl.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gcsofsqym.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/glqtjriee.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/grqtmyafu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gugxezrrr.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/gztpupcuv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gqwaetish.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gfwfrvlkk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.zdbjq.cn/Article/details/goxrxcuab.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gxrqbzuul.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gdzfyuirn.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gcbwxqjyz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gqajsgsag.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fehbvm.com/Article/details/gasfpjqfi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gxnmkonzo.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gnsdzrkts.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fehbvm.com/Article/details/gckfqmbrd.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gcyjonxcv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/gjbwwlunu.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/gionpckvp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gezugickc.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gqixsvflz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gpecxzigu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fehbvm.com/Article/details/gejywcfhf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.hesvh.cn/Article/details/gujamhlei.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gdpsxdwbk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fehbvm.com/Article/details/gqsmodkny.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gpowxzlkt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gkdxomofk.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gncmewofv.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gwcpvhknd.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gumbcanmw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.fehbvm.com/Article/details/gcbqhoaev.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gjplzjjqm.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gzclmclnu.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gsnrefiwe.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gadmsjyai.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gkhbkleyp.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fehbvm.com/Article/details/gkqqrmqhe.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gfvkymzcq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gnjykpmna.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.hesvh.cn/Article/details/gmkxxlzph.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gshybpshp.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/glfuwrjek.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/gscfngded.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gijrzhomo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fehbvm.com/Article/details/grflhnueg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gmzfutkyi.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gvxxrkbuj.sHtML


<!-- 参考信息 -->