代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyantlzvs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnfyawybo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsatnqwvm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszsjwwwm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gpxknqkly.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gmlglcryu.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggurzjple.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtyvxlzj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gwapnypha.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcprbexv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gilavtdpf.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gypuuzgir.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/glumpssyu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbjowmbf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhqxgxgy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gsoxealst.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvgxqiym.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glplpzicy.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ggmyyvdfk.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiuceaxh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxenfrhx.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gymwbnebz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gucvbkmbd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gxhitjdhm.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykbrhcp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gniiutgxt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/geiphzyed.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gjmjyybin.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxbhaxij.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/glpewwghr.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/goqfyujtr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihtpgmeh.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gvjqkqcef.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuvcfwzb.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtqkydh.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdmeqbrr.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/gsaerelev.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grlrtppyp.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/ghnlvspxh.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajrumdg.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gbjtccili.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnrsvrpp.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gajdptluz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gkvahnqks.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpdonhsud.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxejyygx.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/goxpjyrbo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxnxjhqd.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmwqsoaz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gujngjhel.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gofgidmzh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/guimvvfpv.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gagcyinck.sHtML

struct P { var x: Int }
来源：http://3g.fanxiaobao.xyz/Article/details/gstoyccmt.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzompxe.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbpzookq.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gclsbmrfb.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsajumdgz.sHtML

[T28] Swift：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxdjtjcv.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmglhlvux.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gsguulgno.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzeuykdlw.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gypnjpvrr.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuxbsrdd.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glodrskwe.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqchbybvm.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grmgidhmy.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gafncigln.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqwutcet.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fanxiaobao.xyz/Article/details/godttvpcg.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcpulga.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gprlchbhf.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gbbfcfkhf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gzytrnzbi.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdlihcebp.sHtML

function add(a, b) return a + b end
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqlumcda.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiumnlpj.sHtML

"a" .. "b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnepcgjp.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gavbyhgne.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtseeskut.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gavvdhwpm.sHtML

string.find(s, "%d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gjherpdjh.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gygtqakhn.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvfixnhv.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdstbyke.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gphifobal.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjmaoukk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfdxyqzz.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gxtnzyvsf.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/ghxtrqjhj.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gbkosnshv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcvrfya.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlodkcfe.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/griemscgg.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpjciwjm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygpiskkj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gilxczygl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomqycfic.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gutyglvai.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqoyabp.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohbqnttf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guthpxubr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmynucscy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/gcnbishjm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmmvknrc.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmjjgtna.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gifpudxsv.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcdzgnymf.sHtML

val a = 1;  var b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwfmuqj.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqcveir.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxubcqml.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwzavqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmarrbou.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/govwlaean.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxiefebmk.sHtML

[T56] Scala：样例类
来源：http://3g.fanxiaobao.xyz/Article/details/glghokoyd.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gjhohhqyh.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxpowft.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gmndpdhbs.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghwmabwks.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gvqwdkoge.sHtML

[T59] Scala：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfvojlmlz.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/grihmnifb.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyuetejk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlycprqi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzenmeixa.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpfnbxph.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbhaeamg.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fanxiaobao.xyz/Article/details/gsnsccent.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fanxiaobao.xyz/Article/details/gaqbbiodc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcmnauva.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhygcfvr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gwlbosaaa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgjzzjkw.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiuynrox.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqcpkyte.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.fanxiaobao.xyz/Article/details/gufntsjwm.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxymuuooi.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gizemiuzl.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycasvrck.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgombyur.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fanxiaobao.xyz/Article/details/gonzcewzy.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gejgvulwi.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwdoqvkj.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fanxiaobao.xyz/Article/details/gnfbzqwyd.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwccrcif.sHtML

[U10] Py：按值排序字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzrylbxsr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fanxiaobao.xyz/Article/details/glphlemtt.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/guwwqusks.sHtML

(x * 2 for x in arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gnelywaep.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiarykri.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gchfktucm.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfqvycx.sHtML

deque(maxlen=10)
来源：http://mobile.fanxiaobao.xyz/Article/details/gunvnsrut.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemzuixiu.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gwghmprdf.sHtML

[U15] Py：高精度计时
来源：http://wap.fanxiaobao.xyz/Article/details/ggsuyscas.sHtML

t = time.perf_counter()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwawdlxkz.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fanxiaobao.xyz/Article/details/gjkskwcbu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fanxiaobao.xyz/Article/details/gfiuwtsgn.sHtML

[U17] Py：初始化日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbhefco.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fanxiaobao.xyz/Article/details/ghedbzupq.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gegraibuy.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/grgbiejho.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcwzxcug.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzxfdkykf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fanxiaobao.xyz/Article/details/gufvjfzkb.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/geqxcyvio.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqjdhcmz.sHtML

@contextlib.contextmanager
来源：http://3g.fanxiaobao.xyz/Article/details/glhqzoyge.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/gcajleqlb.sHtML

list(zip(*m))
来源：http://baike.fanxiaobao.xyz/Article/details/gxnrcfjbi.sHtML

[U23] Py：分块读取大文件
来源：http://blog.fanxiaobao.xyz/Article/details/gynfofzqx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmwngjhn.sHtML

[U24] Py：路径操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gsldbqfog.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgrjskya.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fanxiaobao.xyz/Article/details/glbxzrdpv.sHtML

csv.DictReader(f)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztwvssiy.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtekxcqyl.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpzkkpup.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmoaynqh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqdebowm.sHtML

[U28] Py：类型别名
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfwesxdt.sHtML

UserId = int
来源：http://www.share.fanxiaobao.xyz/Article/details/gjknkfgte.sHtML

[U29] Py：属性校验
来源：http://m.share.fanxiaobao.xyz/Article/details/glajrrolj.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtjhfyqz.sHtML

[U30] Py：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gcebrnmai.sHtML

@dataclass(slots=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcuxfipz.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gshryixof.sHtML

python -m pytest -q
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoswwozl.sHtML

[U32] Py：代码格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjfftloa.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fanxiaobao.xyz/Article/details/goyrsvecf.sHtML

[U33] Py：打包发布
来源：http://m.share.fanxiaobao.xyz/Article/details/gufghykpa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.fanxiaobao.xyz/Article/details/gqduqenxf.sHtML

[U34] Py：判断编码
来源：http://3g.fanxiaobao.xyz/Article/details/gygwageif.sHtML

chardet.detect(raw)
来源：http://wap.fanxiaobao.xyz/Article/details/gkdlfoubb.sHtML

[U35] Py：发送邮件
来源：http://3g.fanxiaobao.xyz/Article/details/gfxrrowva.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grltlnclo.sHtML

[U36] Py：定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmzurhozw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdbggxa.sHtML

[U37] Py：读写 Excel
来源：http://3g.fanxiaobao.xyz/Article/details/gulphhdih.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyduupvo.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gcvjetnhg.sHtML

Path(__file__).resolve().parent
来源：http://blog.fanxiaobao.xyz/Article/details/gdobbxcrz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfpmribf.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjasciqa.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.fanxiaobao.xyz/Article/details/grwmuqagh.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnioxqyt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcdnfdnf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjmnhdit.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxkgqxh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fanxiaobao.xyz/Article/details/gwyymfcyr.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gqkdpjftq.sHtML

namespace App\Http;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdcfxqfu.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fanxiaobao.xyz/Article/details/govoxouup.sHtML

declare(strict_types=1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxkzqqjz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmqmhwvv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizbwjgd.sHtML

[U46] PHP：可空类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gifyyywwc.sHtML

?string $name = null
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatskjyts.sHtML

[U47] PHP：联合类型
来源：http://baike.fanxiaobao.xyz/Article/details/gqddrytvp.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gakgpdluv.sHtML

[U48] PHP：纯枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gzeofigmg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzfjspi.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/grkkhadke.sHtML

public readonly string $name
来源：http://read.share.fanxiaobao.xyz/Article/details/gddlrahwr.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrxezatn.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdjxpodst.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtzmgjjj.sHtML

[$a, $b] = $arr;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmnopnjn.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/grcspwnsu.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkbpdnps.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybluohcp.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcqweiyx.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqxjsdjg.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gpfjlcygn.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkbcpovr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwryncwbf.sHtML

[U56] PHP：命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gdboktnjg.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwfwcaqf.sHtML

[U57] PHP：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtlekzpkn.sHtML

"值: {$a}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geestknml.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkrcmbtc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigietewi.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokxhxgho.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gmmpthnwb.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsrrgtzs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/guppdmrtf.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlhbwyuc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gcycvqzpp.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghehwfnbx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzfoxhsb.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizxjkdcx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnkemugp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxgjljb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fanxiaobao.xyz/Article/details/grqemopsg.sHtML

[U65] PHP：会话
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqhonzfe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnsjdphd.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fanxiaobao.xyz/Article/details/gjtqybpyg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucoesffu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gjqmedyus.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fanxiaobao.xyz/Article/details/gepcujvhg.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/guxkhjbju.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdazxojx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydpswpsu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfvrbyeo.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzmvpku.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gyqakojox.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxaoemhq.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gvjnzbehe.sHtML

[U72] PHP：写错误日志
来源：http://mobile.fanxiaobao.xyz/Article/details/guazwxarx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fanxiaobao.xyz/Article/details/gmhjyneas.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fanxiaobao.xyz/Article/details/giiuwadel.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhwwqyps.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdniqkg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwdcygnj.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/geadtvcna.sHtML

composer require psr/container
来源：http://baike.fanxiaobao.xyz/Article/details/gxuplqauh.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/ggisfnuyx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxafnrajx.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gfggcpobe.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gshtuwabg.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqpoawbu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/gtufthbex.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxtjjaje.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fanxiaobao.xyz/Article/details/ggueovzsd.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fanxiaobao.xyz/Article/details/getzeuryn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgoybasl.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gaekwppow.sHtML

npm init -y;  npm i express
来源：http://baike.fanxiaobao.xyz/Article/details/glijaksvo.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fanxiaobao.xyz/Article/details/gerreptiv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gylmjltqq.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvisihex.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisjowyit.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/gohcjdwgn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawsalckm.sHtML

[U85] JS：可选链
来源：http://read.share.fanxiaobao.xyz/Article/details/glfrudxjp.sHtML

a?.b?.c
来源：http://read.share.fanxiaobao.xyz/Article/details/guznhxnah.sHtML

[U86] JS：空值合并
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgejblhs.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpkwyzjv.sHtML


<!-- 参考信息 -->