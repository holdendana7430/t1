代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gilxtytau.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxbopoftt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvplisz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzhisacg.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gywzzwnoi.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/grucpihch.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/guexemlmx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gnndxwrtz.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/glrdqinso.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gsaknfstk.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gguwcsdln.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/galtsqhqg.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gpdoodwzo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/ggiacchzj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gmoilxhgx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwesvalue.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gawtsufrj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gylqbzmdp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gkiluhsiq.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqjggylie.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gspexnajb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gnpjqgsxq.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gsyjeqlnv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gxbbmkyze.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvyqhfzkx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gwmsexnhb.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gfvbmffwg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gfyshyppk.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gxjwsbhjn.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gzjntlrqe.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gsobygzfh.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gmfmlobzl.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gphcizppq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/glbfqgdje.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gvkvunusf.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gbikosxyb.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gdajzxbvx.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtmrqyu.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gqhkkkkrb.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gcpjweife.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/ggpfsajzg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gntvxvkje.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gdjnycpze.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gqkmqvouz.sHtML

[T21] Swift：遍历
来源：http://wap.hesvh.cn/Article/details/goxpcnyxo.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gfyskvujr.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gqcjgpsio.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gpoggqmuk.sHtML

[T23] Swift：函数
来源：http://3g.fehbvm.com/Article/details/gweaiswts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ghpmlcknp.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gvgezuctg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gccyfoyjc.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gtqpaqehx.sHtML

struct P { var x: Int }
来源：http://3g.zdbjq.cn/Article/details/gkkrmzuim.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gadchsuzp.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gwjkfnwwn.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ghxdkzwmt.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gjvfamiol.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gmucamxln.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gyflxtzay.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/glggfyfos.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gcnqkkpxt.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gclgktyts.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gsqvitlbj.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdwhmjeit.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gxnnaxrpn.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/grxhtlshj.sHtML

local a = 1
来源：http://mobile.hesvh.cn/Article/details/gzsoohnmk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gegaqfccs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/goggmzkmb.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gcmwdyeuf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/gqlrupjnd.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gxpagijue.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gimivhsqc.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/ghesbubxl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/glmbbtxyq.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gssdeaaqb.sHtML

"a" .. "b"
来源：http://3g.hesvh.cn/Article/details/ggtegajuz.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/ghcwznkrk.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gvwioycvo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/grvkygiav.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/giuezqxvm.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gxbrowevj.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.zdbjq.cn/Article/details/glblfxnoa.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gzgfhrbco.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/gqofphssu.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gsxftewep.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gikzgplgh.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gkujudshn.sHtML

"值: $a"
来源：http://www.m.share.fehbvm.com/Article/details/gkfhgznnu.sHtML

[T44] Perl：条件
来源：http://www.share.fehbvm.com/Article/details/gctzqoapv.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gqyrnrqkt.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/geptzyryg.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gxwzkkexv.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gmlzmgfsb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fehbvm.com/Article/details/gnikedfjx.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gufiasoof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/ganjnjfta.sHtML

[T48] Perl：正则替换
来源：http://m.share.hesvh.cn/Article/details/glkvjlzrl.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gmzhpfjmn.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gjqzijnml.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbwruwlai.sHtML

[T50] Perl：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gawixouox.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gzjyaysqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.zdbjq.cn/Article/details/gfhmlotig.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/ghcjylfyr.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gwurvnlnf.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/gikqbwefp.sHtML

val a = 1;  var b = 2
来源：http://3g.fehbvm.com/Article/details/glpoiqhhq.sHtML

[T53] Scala：字符串插值
来源：http://wap.hesvh.cn/Article/details/gvorljzsy.sHtML

s"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gnpnsxnia.sHtML

[T54] Scala：集合映射
来源：http://blog.hesvh.cn/Article/details/gkuyumtmr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gvzbcsepb.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxcwqpeqx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.hesvh.cn/Article/details/givykuxxe.sHtML

[T56] Scala：样例类
来源：http://wap.hesvh.cn/Article/details/ghogejdps.sHtML

case class User(name: String, age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzjpqzdjd.sHtML

[T57] Scala：模式匹配
来源：http://baike.hesvh.cn/Article/details/gojuuerof.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fehbvm.com/Article/details/gsjncaqzs.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gewhroghl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/gaocqzrpf.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/gtxvraioi.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.fehbvm.com/Article/details/gqrpqmdqd.sHtML

[T60] Scala：折叠
来源：http://blog.hesvh.cn/Article/details/gjyaaibcs.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.hesvh.cn/Article/details/gkagqycjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbdukycpj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gazeoginl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyrfnuyzz.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fehbvm.com/Article/details/gboywoqth.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fehbvm.com/Article/details/ganitkizp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/ggcvtagwh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fehbvm.com/Article/details/ghwpxmdgx.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.hesvh.cn/Article/details/glrngodii.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.zdbjq.cn/Article/details/gxwazmhag.sHtML

[U04] Py：变量调试打印
来源：http://baike.zdbjq.cn/Article/details/gfhzwmnmu.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.hesvh.cn/Article/details/gtfsxueza.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gkjzymtvx.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/ghkaicwzd.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gyprkwapk.sHtML

{**a, **b}
来源：http://www.blog.hesvh.cn/Article/details/gswtadwmc.sHtML

[U07] Py：反转字典键值
来源：http://blog.zdbjq.cn/Article/details/gqlfpazwl.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.zdbjq.cn/Article/details/gxxpisujh.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gjxltqyek.sHtML

[y for x in nested for y in x]
来源：http://mobile.hesvh.cn/Article/details/gvdfbcyix.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fehbvm.com/Article/details/ggzreykqq.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/grucjmgwm.sHtML

[U10] Py：按值排序字典
来源：http://baike.hesvh.cn/Article/details/grexnplei.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.hesvh.cn/Article/details/gcisjbubn.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gytkmtymy.sHtML

(x * 2 for x in arr)
来源：http://mobile.hesvh.cn/Article/details/gddjzjffc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/ggsfrsfac.sHtML

Counter(arr).most_common(3)
来源：http://mobile.fehbvm.com/Article/details/gxdrpytuq.sHtML

[U13] Py：固定长度队列
来源：http://baike.fehbvm.com/Article/details/gbezbadpp.sHtML

deque(maxlen=10)
来源：http://m.share.hesvh.cn/Article/details/gkddtfrgv.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.zdbjq.cn/Article/details/gecpbctgp.sHtML

defaultdict(list)
来源：http://baike.zdbjq.cn/Article/details/gjedrtzmi.sHtML

[U15] Py：高精度计时
来源：http://m.share.fehbvm.com/Article/details/ggdpopjoi.sHtML

t = time.perf_counter()
来源：http://wap.hesvh.cn/Article/details/gubixteqy.sHtML

[U16] Py：命令行参数解析
来源：http://wap.zdbjq.cn/Article/details/gdecfvhao.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.fehbvm.com/Article/details/grvxavzzx.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gjhvwwixl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.share.fehbvm.com/Article/details/gteiugkva.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gqufvmszf.sHtML

pat = re.compile(r"\d+")
来源：http://blog.zdbjq.cn/Article/details/guomkpioq.sHtML

[U19] Py：正则替换带回调
来源：http://baike.fehbvm.com/Article/details/gqnqttsgp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fehbvm.com/Article/details/gceyuteve.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.hesvh.cn/Article/details/gscczzmwp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fehbvm.com/Article/details/gopzkzuhd.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.hesvh.cn/Article/details/gfliscpqg.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gkvnwzzaj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.hesvh.cn/Article/details/gerdxlgma.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gwtfymfvd.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.hesvh.cn/Article/details/gzdwuujhs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.fehbvm.com/Article/details/glvgbsebb.sHtML

[U24] Py：路径操作
来源：http://wap.zdbjq.cn/Article/details/gtwvkbisj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gyntxpknz.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.hesvh.cn/Article/details/ghlpgsqoq.sHtML

csv.DictReader(f)
来源：http://wap.hesvh.cn/Article/details/geeddydua.sHtML

[U26] Py：并发下载
来源：http://wap.fehbvm.com/Article/details/gefcakdcu.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/grdzzuocd.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.hesvh.cn/Article/details/groegpmnb.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.fehbvm.com/Article/details/gkqqfeihm.sHtML

[U28] Py：类型别名
来源：http://read.share.zdbjq.cn/Article/details/gpnkugwuo.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/ghmfygxxh.sHtML

[U29] Py：属性校验
来源：http://mobile.fehbvm.com/Article/details/gvahyashx.sHtML

@property 与 @x.setter 配合
来源：http://mobile.hesvh.cn/Article/details/gbeqldddu.sHtML

[U30] Py：数据类
来源：http://3g.zdbjq.cn/Article/details/gnfhsczgo.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/gnuejdubz.sHtML

[U31] Py：单测
来源：http://baike.zdbjq.cn/Article/details/ghshtbxif.sHtML

python -m pytest -q
来源：http://www.share.zdbjq.cn/Article/details/gfujbgtmb.sHtML

[U32] Py：代码格式化
来源：http://m.share.hesvh.cn/Article/details/grlravarn.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.hesvh.cn/Article/details/gwzhhocry.sHtML

[U33] Py：打包发布
来源：http://www.blog.fehbvm.com/Article/details/gwhqeppsh.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.hesvh.cn/Article/details/ghmoplusw.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/ghmxxkirw.sHtML

chardet.detect(raw)
来源：http://baike.zdbjq.cn/Article/details/gjiqoojgj.sHtML

[U35] Py：发送邮件
来源：http://read.share.fehbvm.com/Article/details/gqfjrsztj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fehbvm.com/Article/details/gjzeshwwh.sHtML

[U36] Py：定时任务
来源：http://www.blog.fehbvm.com/Article/details/gdwzfipfm.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.zdbjq.cn/Article/details/gysmgfdar.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/gvjunztew.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.hesvh.cn/Article/details/gqddipwxe.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.hesvh.cn/Article/details/gnhmqzjzk.sHtML

Path(__file__).resolve().parent
来源：http://mobile.zdbjq.cn/Article/details/giztzobuf.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.hesvh.cn/Article/details/golzamuly.sHtML

sys.stdout.isatty()
来源：http://m.share.fehbvm.com/Article/details/gjemguarc.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gwegkcydn.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/ggniclnqz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gtdjvlpmp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.fehbvm.com/Article/details/gbliuanpo.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfpllpx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gwfhottwy.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.hesvh.cn/Article/details/gsjfsdoun.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gbomttggx.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fehbvm.com/Article/details/gibeuzxog.sHtML

declare(strict_types=1);
来源：http://blog.zdbjq.cn/Article/details/gvfpcewhw.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/gxmulvapi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmzabdlvu.sHtML

[U46] PHP：可空类型
来源：http://blog.zdbjq.cn/Article/details/gsmbjpkfy.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gcjmzihtd.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gepqmyank.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gtyrzfoyu.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gunhnxqci.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fehbvm.com/Article/details/gjnjmsuqt.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/gvysxpfat.sHtML

public readonly string $name
来源：http://wap.zdbjq.cn/Article/details/ggshwbvak.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.hesvh.cn/Article/details/gpxfuxzop.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fehbvm.com/Article/details/gbpahgtvv.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gvnaglszm.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/ghxkkgiiu.sHtML

[U52] PHP：箭头函数
来源：http://blog.fehbvm.com/Article/details/gpyfdqqpn.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gazhlvcck.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/gvyydbzoy.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.fehbvm.com/Article/details/gmwfplcfz.sHtML

[U54] PHP：空安全调用
来源：http://wap.hesvh.cn/Article/details/gayntfdyc.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/gbpwxfksn.sHtML

[U55] PHP：match 表达式
来源：http://wap.hesvh.cn/Article/details/gxhwunuyh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.fehbvm.com/Article/details/giofgymje.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gfafuzude.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gucontipp.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gmrosilhz.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gtpyjcuhr.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/gocklnuja.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfgnruyet.sHtML

[U59] PHP：自定义排序
来源：http://baike.fehbvm.com/Article/details/gflqtxwcw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gpmkckxuo.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gtwfrgptn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/giavcmhfz.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gzlzrponk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gzplftlot.sHtML

[U62] PHP：日期对象
来源：http://www.blog.hesvh.cn/Article/details/gwwthswsy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/guojqmlek.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/gmahjbdxc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gaetymbpn.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gtszwkbqy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gtaulbbkp.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/ggsubmuxh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/goroftpfx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gjjxvwbhx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gnjozbolj.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gpjyzxwpr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gvefebcrx.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gpynqdlrf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gzhihwltj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gghgqnluz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gyqulgwqy.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/gxulgclzq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.fehbvm.com/Article/details/gvuvmqfbe.sHtML

[U71] PHP：抛出异常
来源：http://blog.hesvh.cn/Article/details/gjaxbewhc.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.hesvh.cn/Article/details/goevwaocw.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gejajuwcs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/geigfgyln.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gtissnhal.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fehbvm.com/Article/details/gbspdncjk.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gqwrekscq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gybwaigpy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fehbvm.com/Article/details/gebirqqly.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/giiycyldo.sHtML

[U76] PHP：简单路由
来源：http://read.share.hesvh.cn/Article/details/gxcvrsiso.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/goxsikzod.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gatspzqwq.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gwfijfzpn.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gdttgpaxv.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gitxsoong.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/gtnpnltud.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gzyocxbad.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gvzpruqtl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/ghhnwpbum.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gctmmyfep.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/ghyleebti.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gwikcbyhh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fehbvm.com/Article/details/gilxigqly.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gxbjzrskd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gvlstmbxj.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gnhkmowtd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gipygsaqw.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gpzikwzps.sHtML

a?.b?.c
来源：http://m.share.fehbvm.com/Article/details/gedpotdfu.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/goeweocko.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gfxnwdgye.sHtML


<!-- 参考信息 -->