代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/ghttvqmap.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gejfkirfh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gyupqflff.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gdcvueugy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gujkwyyuf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxeuxcvdt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gfwsshzff.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbiiptrel.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gqxptfhnk.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/guejdozaz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gtplxsqvh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fehbvm.com/Article/details/gxatrgsqc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/gdrecztft.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gwbqzhtpb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gfwgbgitt.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/ggkcnrurm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmhdkfzjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gkvlxtlhj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gjmgkmyud.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkiqmitye.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/ghnyitckj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/gqieazfmv.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gqahrqycx.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gmncbmqyj.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gucsftvru.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gsjwdvuzr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gkwjrhtwe.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/grcrnctyh.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gsfmnnple.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/gvefxanpm.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/grattbygg.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ggbcghfrb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/grfzcoolu.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gsqcrwwpj.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gtnbeplir.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gkigjflij.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gjhpdqall.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gsnztkvfj.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/grxyshkte.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gbnrrcwak.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gbdnlnbae.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gxnckyzsl.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjtfomzft.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/grihjcjtj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gklxbesil.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fehbvm.com/Article/details/gzrzhjzoo.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/guehjfaky.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gmhxpenyp.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxwopfkgz.sHtML

for x in a { print(x) }
来源：http://www.m.share.hesvh.cn/Article/details/gnocfvfrt.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gqbywfaso.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gfhpgetho.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gxddsmqjc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gqxnhmpdi.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gokjiksjh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gnfexzpng.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gijggwqpn.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/glktpfbzb.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gknnaeyqa.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/geitvzsqv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbfcgaswa.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gcxxuwgzz.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gpdgfbluy.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gcayovujc.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/gvhuyrrbf.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/gakjdfiqu.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/gsrxyqyma.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/ghlfvzuvc.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvdpsxvsa.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gpvwlleal.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gpvqorxcr.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gswatlrwb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gphtpvled.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gmpsveiod.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gbitzgayt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fehbvm.com/Article/details/gyiirmezc.sHtML

[T35] Lua：字典表
来源：http://3g.hesvh.cn/Article/details/ghjpjquwh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.hesvh.cn/Article/details/gijhnpbcc.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gyqsvpaxv.sHtML

function add(a, b) return a + b end
来源：http://baike.zdbjq.cn/Article/details/gbtuvcqon.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gyrrpadwo.sHtML

"a" .. "b"
来源：http://www.m.share.fehbvm.com/Article/details/gwxdhdzcx.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gmhfwtllv.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gdqaswrbp.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gxcsydsqo.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gphmqphwj.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/glyqkxpom.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gcotsednf.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gwhertygw.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gngxichex.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gipmwwadt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/glulcnmtd.sHtML

[T43] Perl：字符串插值
来源：http://blog.hesvh.cn/Article/details/gtjrctqxp.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/gsiujfpqv.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/gnqewnykc.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gddyzabkj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gfpwcwail.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gnepfbroz.sHtML

[T46] Perl：哈希操作
来源：http://baike.zdbjq.cn/Article/details/gpskigjux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.zdbjq.cn/Article/details/guixmowxh.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gyxmntqkq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.hesvh.cn/Article/details/gbykvlich.sHtML

[T48] Perl：正则替换
来源：http://blog.hesvh.cn/Article/details/ghqfdwmwc.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gulxmlgbx.sHtML

[T49] Perl：函数
来源：http://wap.fehbvm.com/Article/details/gkjrwdyiw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghfztjiqj.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gllpmxrcx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/ggehpjock.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gfnlyasjz.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbgdvnfhe.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/glweyzoty.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gmmmzcbkm.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/gvxmchxbi.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/guzbzoxxe.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkujqvbty.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gkzqatgez.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.hesvh.cn/Article/details/gunowjkaa.sHtML

[T55] Scala：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gtvivrihx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxinufpet.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/glcaltiyj.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fehbvm.com/Article/details/gpchwxrag.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/gdlobpodn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.hesvh.cn/Article/details/gmdgzeiez.sHtML

[T58] Scala：函数定义
来源：http://wap.hesvh.cn/Article/details/gfazmgiyx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/gvocwdulf.sHtML

[T59] Scala：循环
来源：http://read.share.hesvh.cn/Article/details/gcvtcztdb.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.hesvh.cn/Article/details/gskmrwyre.sHtML

[T60] Scala：折叠
来源：http://baike.fehbvm.com/Article/details/gwfcsqajn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fehbvm.com/Article/details/gfgzgkffi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grfegfeiy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gxrhzcbsm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghwqsoevr.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.fehbvm.com/Article/details/gvmmgqauo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.hesvh.cn/Article/details/gibhascls.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.hesvh.cn/Article/details/gudqakjpy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/gccjpevyr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gmwuqpmvy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.zdbjq.cn/Article/details/ggpgpnmgv.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/goobrvxnb.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fehbvm.com/Article/details/gwcjgvxgr.sHtML

[U05] Py：列表去重且保序
来源：http://3g.fehbvm.com/Article/details/gwohixfsf.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcrskmqpk.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.zdbjq.cn/Article/details/grtbjvboz.sHtML

{**a, **b}
来源：http://wap.hesvh.cn/Article/details/gofdazwti.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.hesvh.cn/Article/details/gpnjydycd.sHtML

{v: k for k, v in d.items()}
来源：http://3g.hesvh.cn/Article/details/gxxvgnstb.sHtML

[U08] Py：展平二维列表
来源：http://blog.fehbvm.com/Article/details/gobmjgirx.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gatfamgpn.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gbeihvulr.sHtML

max(d, key=d.get)
来源：http://www.blog.hesvh.cn/Article/details/gaisjxhja.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/glnldlgfv.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gjpxlqnvc.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gflfkrwhi.sHtML

(x * 2 for x in arr)
来源：http://wap.hesvh.cn/Article/details/gjpgdqswe.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fehbvm.com/Article/details/gjsdzpndl.sHtML

Counter(arr).most_common(3)
来源：http://www.share.fehbvm.com/Article/details/gxslzbqvg.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fehbvm.com/Article/details/gymmydeiy.sHtML

deque(maxlen=10)
来源：http://wap.hesvh.cn/Article/details/giaifidik.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gcyblxmwl.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/giqxbgdwi.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/gqnjkbyxa.sHtML

t = time.perf_counter()
来源：http://www.blog.hesvh.cn/Article/details/gjtvdvrep.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gtlmhlvse.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.hesvh.cn/Article/details/gduvwmpdk.sHtML

[U17] Py：初始化日志
来源：http://baike.hesvh.cn/Article/details/gsgiaufbl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.zdbjq.cn/Article/details/gglcsluuc.sHtML

[U18] Py：预编译正则
来源：http://3g.zdbjq.cn/Article/details/gzbxzkdmf.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggblbahhj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gkzqiezwk.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.hesvh.cn/Article/details/gdufcisnu.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.zdbjq.cn/Article/details/gfquexdxy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gxyfslckz.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fehbvm.com/Article/details/ggvhouhuv.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/goxupsldx.sHtML

[U22] Py：矩阵转置
来源：http://wap.hesvh.cn/Article/details/gsbvwpsvf.sHtML

list(zip(*m))
来源：http://wap.hesvh.cn/Article/details/grizchech.sHtML

[U23] Py：分块读取大文件
来源：http://blog.zdbjq.cn/Article/details/gslqqtcmy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gbpmpxsaf.sHtML

[U24] Py：路径操作
来源：http://3g.zdbjq.cn/Article/details/ghttltwqx.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gestlllll.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.hesvh.cn/Article/details/gyoowwgdw.sHtML

csv.DictReader(f)
来源：http://www.m.share.fehbvm.com/Article/details/gtcaxwzuu.sHtML

[U26] Py：并发下载
来源：http://baike.hesvh.cn/Article/details/gkupxitcd.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.zdbjq.cn/Article/details/gshdebouy.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.zdbjq.cn/Article/details/gytwsetvu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.hesvh.cn/Article/details/gptqqfvdv.sHtML

[U28] Py：类型别名
来源：http://3g.zdbjq.cn/Article/details/gpedhnwzq.sHtML

UserId = int
来源：http://m.share.fehbvm.com/Article/details/gyzcuihyk.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gaooefcyv.sHtML

@property 与 @x.setter 配合
来源：http://mobile.zdbjq.cn/Article/details/ggfjrptsf.sHtML

[U30] Py：数据类
来源：http://www.share.hesvh.cn/Article/details/gwgnwiwek.sHtML

@dataclass(slots=True)
来源：http://www.blog.fehbvm.com/Article/details/gwhzqnzzp.sHtML

[U31] Py：单测
来源：http://www.blog.hesvh.cn/Article/details/gbzkcxvnr.sHtML

python -m pytest -q
来源：http://blog.hesvh.cn/Article/details/gvukkwhyw.sHtML

[U32] Py：代码格式化
来源：http://wap.fehbvm.com/Article/details/gkxxowuff.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fehbvm.com/Article/details/gwobgnsqk.sHtML

[U33] Py：打包发布
来源：http://www.share.fehbvm.com/Article/details/gizcndkye.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gcrijoxxx.sHtML

[U34] Py：判断编码
来源：http://www.share.hesvh.cn/Article/details/gkqcqrvoa.sHtML

chardet.detect(raw)
来源：http://mobile.zdbjq.cn/Article/details/gjimwpzhn.sHtML

[U35] Py：发送邮件
来源：http://read.share.zdbjq.cn/Article/details/gbnurhrlw.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.fehbvm.com/Article/details/gzzhsflrg.sHtML

[U36] Py：定时任务
来源：http://3g.hesvh.cn/Article/details/gvyqwnlsn.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fehbvm.com/Article/details/gqvxuqcev.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gpnmkqwbf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.zdbjq.cn/Article/details/gmojxqazs.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gsolsskqe.sHtML

Path(__file__).resolve().parent
来源：http://read.share.zdbjq.cn/Article/details/ggmakfqej.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.zdbjq.cn/Article/details/gojesdymy.sHtML

sys.stdout.isatty()
来源：http://blog.hesvh.cn/Article/details/grxhpmlwf.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.zdbjq.cn/Article/details/gpbygjylv.sHtML

print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gzduyxqmk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fehbvm.com/Article/details/gjoyaondj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.hesvh.cn/Article/details/gezmxybak.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.hesvh.cn/Article/details/gqukkmktl.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.hesvh.cn/Article/details/gcjjqlahz.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gfqwkwdik.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/glhnucxkf.sHtML

[U44] PHP：开启严格类型
来源：http://blog.fehbvm.com/Article/details/gfnonhmoo.sHtML

declare(strict_types=1);
来源：http://baike.hesvh.cn/Article/details/grmudvskh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gmhhjunho.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gqwaanhqc.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gjsojnhus.sHtML

?string $name = null
来源：http://www.share.fehbvm.com/Article/details/gwfwuqlvs.sHtML

[U47] PHP：联合类型
来源：http://read.share.fehbvm.com/Article/details/gddolybrb.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gvxwqbsxk.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gltgnapej.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.hesvh.cn/Article/details/gzfgjydys.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gbemvicxd.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/gkxfgxyls.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gcifdsqew.sHtML

public function __construct(private int $id) {}
来源：http://m.share.zdbjq.cn/Article/details/gxxiikivb.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gmkfbbsro.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gtwxumcjd.sHtML

[U52] PHP：箭头函数
来源：http://baike.hesvh.cn/Article/details/gmyafodtn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gmkfqjnch.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gaucecaft.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/guiqirwst.sHtML

[U54] PHP：空安全调用
来源：http://baike.hesvh.cn/Article/details/glcbfxqgs.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/ghyluqliq.sHtML

[U55] PHP：match 表达式
来源：http://baike.fehbvm.com/Article/details/gffnkxnfz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fehbvm.com/Article/details/glmueidxr.sHtML

[U56] PHP：命名参数
来源：http://wap.fehbvm.com/Article/details/gwigpggxy.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gkfczwvbf.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfqmyofds.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/ghwlylcft.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gsbfdtrmb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.fehbvm.com/Article/details/gpoguovcf.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/giixphzft.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gexpghwpx.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.zdbjq.cn/Article/details/gcyebyhty.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/giggjazzs.sHtML

[U61] PHP：正则
来源：http://baike.zdbjq.cn/Article/details/gyhygkwll.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpnsuxite.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gdreqeqml.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gsogxwzrl.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/gxejfeddm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gwufsgbym.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gpeexnvnd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gnhxkcywt.sHtML

[U65] PHP：会话
来源：http://www.share.zdbjq.cn/Article/details/gvicvzmsv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gbvscpdev.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.zdbjq.cn/Article/details/gkdctszym.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gtuintvps.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gaqmfsisi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.fehbvm.com/Article/details/giteeidbi.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/gpzzvovon.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/guhpeucir.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.zdbjq.cn/Article/details/gxuailoeq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.hesvh.cn/Article/details/gmcoicfdt.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gaopckyxh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gwlzmkede.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gexzvwscu.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.hesvh.cn/Article/details/gjfzndbmq.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gxsqlvbpm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gaeqrpjgv.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.fehbvm.com/Article/details/gvkaodyih.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/gilnfqgsg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gbtfplgpv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gjzefxdyv.sHtML

[U75] PHP：依赖注入
来源：http://www.share.hesvh.cn/Article/details/gpqchgzik.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/ggzdqnzoq.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/ggovxqosa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gwaohkuul.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gdxvmbldm.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/gtjiuztgr.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gvjdiyosl.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gagomkgnl.sHtML

[U79] PHP：静态分析
来源：http://baike.zdbjq.cn/Article/details/gjhvlujog.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gbnrdqdfq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gvxkowqpi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/gzjztrovq.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gummbbcwd.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gvhurbizb.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/ggnnkkqtc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gcsvcrlhc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gkkiiwoni.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gkdvzngsd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gandjvzxn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gclykbopr.sHtML


<!-- 参考信息 -->