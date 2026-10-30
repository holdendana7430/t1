代发 wailian999

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gsdjzkkpf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/grxgdkxyi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gauvhxxng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gekqgcdkv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gwuqsdwnf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/goceuurpc.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gubudnuyw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/gqpxgshtx.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gsdxhqmkm.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gdqyazzgv.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/glghuqpqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gwmuhywgr.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvibruwlj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gxxzrscmc.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gbgcwqiiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gevbdygzb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gzfzwsgme.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gkgyowtag.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gchbrksqq.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/gzmvtfhof.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gotgumjlf.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gcwawgoyz.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gfsjgsibz.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grqyelhnm.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gpgugpous.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gmvpgriox.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gbifrwkhz.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gvzulctwc.sHtML

[T19] Swift：可选绑定
来源：http://blog.fehbvm.com/Article/details/gzotjahhc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gjaqyjmzy.sHtML

[T20] Swift：数组操作
来源：http://mobile.hesvh.cn/Article/details/ggbgulggq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gkcwocphu.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzhoubtbj.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/giohkdvac.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gdzqpezvu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gghcbaboy.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/guhxanapx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/glrcqvbrw.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/gthdqdyyx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gvmtrxowd.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gbyyczwhr.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gqgfstvjd.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gprrprsmw.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gpwxzszbe.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gxjljffdh.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gtkmtlzxm.sHtML

[T28] Swift：枚举
来源：http://www.share.hesvh.cn/Article/details/gxecbsgvk.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/gpumhieen.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/glzsmumqp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.hesvh.cn/Article/details/gvxffdxwr.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gilmcnvfy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gaylhudqd.sHtML

[T31] Lua：Hello World
来源：http://m.share.fehbvm.com/Article/details/gsihnskeb.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdpuvxbjy.sHtML

[T32] Lua：局部变量
来源：http://www.share.fehbvm.com/Article/details/gnxpqbcqj.sHtML

local a = 1
来源：http://blog.hesvh.cn/Article/details/gxdapddbd.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gsbwvzucq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gqqfezrwu.sHtML

[T34] Lua：遍历表
来源：http://blog.fehbvm.com/Article/details/gkxaohczj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fehbvm.com/Article/details/gpxxyvaal.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gdadhjbvu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gjjzllbff.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gmcqefffo.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gasiqmzdo.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gfxsalbpx.sHtML

"a" .. "b"
来源：http://3g.zdbjq.cn/Article/details/gjcpzqzas.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/ggybcecck.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gfkzheukx.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/glhmowgsf.sHtML

string.find(s, "%d+")
来源：http://wap.zdbjq.cn/Article/details/gjkjkqdcs.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/giuowjube.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.hesvh.cn/Article/details/gafphpbck.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gewujkkqm.sHtML

print "Hello\n";
来源：http://baike.fehbvm.com/Article/details/gydfnjhxm.sHtML

[T42] Perl：变量类型
来源：http://m.share.zdbjq.cn/Article/details/gbzaxdehg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fehbvm.com/Article/details/gaxtdlsan.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gzlljniir.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gbvtddhtq.sHtML

[T44] Perl：条件
来源：http://wap.zdbjq.cn/Article/details/gzmmemkuk.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/glhdvuzmt.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gfdbltule.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gocbpjbta.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gbjzulftb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.hesvh.cn/Article/details/gyxnqssmb.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gmnjrpsww.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.fehbvm.com/Article/details/ggufnayxd.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gnyvvgjbw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fehbvm.com/Article/details/gkjgwvzca.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/geiivfxus.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcxjdtgmr.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbvhuiuuz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/ggadhqblv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/gyucjwhjl.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gssrdybyk.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gilumbrvm.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gpsdmcdxj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gufwazmju.sHtML

[T53] Scala：字符串插值
来源：http://3g.hesvh.cn/Article/details/gijzsfbhx.sHtML

s"值: $b"
来源：http://baike.hesvh.cn/Article/details/gkyckwhme.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gozmgxsuy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gezkaoosu.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gsyahrpwe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gtdeoqdrj.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gwshrkfjg.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.fehbvm.com/Article/details/gqrzrbufo.sHtML

[T57] Scala：模式匹配
来源：http://blog.fehbvm.com/Article/details/gcvwkiltl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gpplfvzrk.sHtML

[T58] Scala：函数定义
来源：http://blog.zdbjq.cn/Article/details/gdtvuupuu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.zdbjq.cn/Article/details/glftmiuqv.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/giahhqyon.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.hesvh.cn/Article/details/ggbwjceuf.sHtML

[T60] Scala：折叠
来源：http://mobile.zdbjq.cn/Article/details/gncqentqe.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.hesvh.cn/Article/details/gxyumdlcz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzfrayijv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdvzflphk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ginzaanxh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gdyabdjjc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fehbvm.com/Article/details/gyamvuzyc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fehbvm.com/Article/details/gfmldkiof.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.hesvh.cn/Article/details/gwblytocp.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gdxzzpyfj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.zdbjq.cn/Article/details/gckuldqqo.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fehbvm.com/Article/details/gpndacvna.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.hesvh.cn/Article/details/gzvddkcyo.sHtML

[U05] Py：列表去重且保序
来源：http://blog.fehbvm.com/Article/details/gfiukypho.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpzejztyy.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gswanyoei.sHtML

{**a, **b}
来源：http://mobile.hesvh.cn/Article/details/gynthfqan.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/giiiblsxp.sHtML

{v: k for k, v in d.items()}
来源：http://blog.zdbjq.cn/Article/details/gkrkqtfac.sHtML

[U08] Py：展平二维列表
来源：http://www.share.hesvh.cn/Article/details/gocrdoexf.sHtML

[y for x in nested for y in x]
来源：http://baike.hesvh.cn/Article/details/ggrxhfcbj.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/gadaveuge.sHtML

max(d, key=d.get)
来源：http://www.share.hesvh.cn/Article/details/gleznpxnu.sHtML

[U10] Py：按值排序字典
来源：http://m.share.hesvh.cn/Article/details/ghqkcgtun.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.zdbjq.cn/Article/details/gsuxzvbdk.sHtML

[U11] Py：生成器表达式
来源：http://wap.zdbjq.cn/Article/details/gqlrkduvb.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/gucvhhtyc.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.fehbvm.com/Article/details/glxslzpyo.sHtML

Counter(arr).most_common(3)
来源：http://wap.hesvh.cn/Article/details/gwlgtztde.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.zdbjq.cn/Article/details/gvezvlrvy.sHtML

deque(maxlen=10)
来源：http://mobile.fehbvm.com/Article/details/gldjhcnuz.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.zdbjq.cn/Article/details/gibqvcsiy.sHtML

defaultdict(list)
来源：http://www.m.share.hesvh.cn/Article/details/gqzqdfteu.sHtML

[U15] Py：高精度计时
来源：http://3g.hesvh.cn/Article/details/glkjgxfep.sHtML

t = time.perf_counter()
来源：http://wap.zdbjq.cn/Article/details/gzrnujcjj.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.hesvh.cn/Article/details/gcnlsojqk.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/giaeqnuve.sHtML

[U17] Py：初始化日志
来源：http://www.share.hesvh.cn/Article/details/gfpwnirzd.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.zdbjq.cn/Article/details/grswhkyzj.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/gvponhwqc.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpdelri.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.hesvh.cn/Article/details/gvymxzyou.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.fehbvm.com/Article/details/gtufzkvnm.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.fehbvm.com/Article/details/ghkffujtu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.zdbjq.cn/Article/details/gpeaewhsb.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/goarqfgjk.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/guerjregt.sHtML

[U22] Py：矩阵转置
来源：http://baike.hesvh.cn/Article/details/goeenukwe.sHtML

list(zip(*m))
来源：http://blog.zdbjq.cn/Article/details/godfugidd.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.hesvh.cn/Article/details/gfyvnkttk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.zdbjq.cn/Article/details/gcqtxbdva.sHtML

[U24] Py：路径操作
来源：http://www.share.zdbjq.cn/Article/details/gykogbdqo.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gmghmjhan.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.hesvh.cn/Article/details/gyhioxzkd.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gjyhsllsg.sHtML

[U26] Py：并发下载
来源：http://wap.hesvh.cn/Article/details/gmmnetfwx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.zdbjq.cn/Article/details/gkxpykxxw.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fehbvm.com/Article/details/gxlxjsstr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/gptsjrkzg.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gjwhpkdia.sHtML

UserId = int
来源：http://m.share.zdbjq.cn/Article/details/ggflzeodn.sHtML

[U29] Py：属性校验
来源：http://3g.fehbvm.com/Article/details/grhqmppfn.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.fehbvm.com/Article/details/gnaubdtbd.sHtML

[U30] Py：数据类
来源：http://read.share.zdbjq.cn/Article/details/gmjgrcjag.sHtML

@dataclass(slots=True)
来源：http://www.blog.zdbjq.cn/Article/details/gnjbsemip.sHtML

[U31] Py：单测
来源：http://wap.zdbjq.cn/Article/details/grltpmhck.sHtML

python -m pytest -q
来源：http://www.blog.hesvh.cn/Article/details/gifkeckxn.sHtML

[U32] Py：代码格式化
来源：http://mobile.fehbvm.com/Article/details/gishowqrl.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.zdbjq.cn/Article/details/gubhctzlh.sHtML

[U33] Py：打包发布
来源：http://3g.zdbjq.cn/Article/details/gwgpxkemg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.zdbjq.cn/Article/details/gmyamjmum.sHtML

[U34] Py：判断编码
来源：http://www.m.share.hesvh.cn/Article/details/gvtxwbyju.sHtML

chardet.detect(raw)
来源：http://3g.fehbvm.com/Article/details/gxtjtzyec.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gvearaecp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.zdbjq.cn/Article/details/gbwwvnfzh.sHtML

[U36] Py：定时任务
来源：http://3g.fehbvm.com/Article/details/geejwwary.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.zdbjq.cn/Article/details/gdegxrkqi.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/gntmiubnq.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fehbvm.com/Article/details/gxhvgucsx.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fehbvm.com/Article/details/gmtghyzjj.sHtML

Path(__file__).resolve().parent
来源：http://3g.zdbjq.cn/Article/details/gyyyrhpwd.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fehbvm.com/Article/details/gdnebqrus.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gigmoqimk.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.zdbjq.cn/Article/details/gxgyjtmgq.sHtML

print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gkkiioelb.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.hesvh.cn/Article/details/gvnvrmvzc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gqyezshli.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gnklbbxob.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gdtgttcnu.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/ggwxgvigv.sHtML

namespace App\Http;
来源：http://baike.zdbjq.cn/Article/details/gyhkuifmn.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.hesvh.cn/Article/details/gryjyeqky.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gaozldamv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.zdbjq.cn/Article/details/gkftgdwze.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/glvxcdjge.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gwonbqkjb.sHtML

?string $name = null
来源：http://www.m.share.hesvh.cn/Article/details/ghehspjsx.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/ghfrmifyr.sHtML

int|string $id
来源：http://3g.fehbvm.com/Article/details/gvqyyzcbn.sHtML

[U48] PHP：纯枚举
来源：http://blog.hesvh.cn/Article/details/gbnhacegc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/gmgaksdkm.sHtML

[U49] PHP：只读属性
来源：http://3g.fehbvm.com/Article/details/gdakyavil.sHtML

public readonly string $name
来源：http://www.blog.hesvh.cn/Article/details/gretxzrdx.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/guovnzbgz.sHtML

public function __construct(private int $id) {}
来源：http://blog.hesvh.cn/Article/details/guiqjppwa.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gyrdfnznx.sHtML

[$a, $b] = $arr;
来源：http://blog.fehbvm.com/Article/details/ggecpruwv.sHtML

[U52] PHP：箭头函数
来源：http://m.share.hesvh.cn/Article/details/gkflpopjk.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.zdbjq.cn/Article/details/gtsguprxo.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fehbvm.com/Article/details/gkrifgobe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fehbvm.com/Article/details/gytxvdjln.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gtxujumzk.sHtML

$obj?->method()
来源：http://3g.zdbjq.cn/Article/details/grkrjqvjn.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gjulytcgz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/ggcgwjpio.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gyfxrzlog.sHtML

f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpquyjmfw.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gmczrxoyj.sHtML

"值: {$a}"
来源：http://www.share.fehbvm.com/Article/details/gftkhglfr.sHtML

[U58] PHP：数组三件套
来源：http://3g.hesvh.cn/Article/details/gefffcrrf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/gahctjgan.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gxbbrjmpx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gmyhlxybz.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.fehbvm.com/Article/details/ghpqedbyd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.fehbvm.com/Article/details/gxnspibps.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gboadikip.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gpnfwbthq.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gbsrndhmx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/grvkvbvcv.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gbsaqchti.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fehbvm.com/Article/details/giubwthvx.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gcoplkscw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.zdbjq.cn/Article/details/grdezhxuu.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gjezldmuo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmxkgsday.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gofpsblao.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gjjfezvyf.sHtML

[U67] PHP：处理文件上传
来源：http://baike.zdbjq.cn/Article/details/gkikdtisi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.hesvh.cn/Article/details/gtswsggdr.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.fehbvm.com/Article/details/gyxlwedkx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fehbvm.com/Article/details/gqfgdpvdu.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fehbvm.com/Article/details/gembfyaji.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gmfoqtbjb.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/gpzqgwkte.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gsztxdjof.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/guieodktb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gtzeqlwzf.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gikoesolr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/glqwepzun.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/ghxlrchda.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/gosftlefz.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/godmougii.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/grxxoromh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/gufmzkzxa.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gnacgtnwi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gydzavspz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.hesvh.cn/Article/details/gouzktlff.sHtML

[U77] PHP：模板渲染
来源：http://m.share.hesvh.cn/Article/details/gkdqazfda.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gsbcfrudq.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gkwszoqup.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gljrhwytq.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/guaegtzzc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gwiptfltq.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gqxauifge.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gdiuvtmkc.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gtraypjuf.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsgrwyd.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/glwjllrul.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gfcxkvbvh.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gltslcvkv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gryjadykk.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gpsuogwby.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/ghpswppev.sHtML

[U85] JS：可选链
来源：http://mobile.fehbvm.com/Article/details/gbbvqbxkh.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/glpuzlvvd.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gfitozwoa.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/gnkimbjax.sHtML

[U87] JS：解构默认值
来源：http://baike.fehbvm.com/Article/details/gaupmebrd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gnnaavwpy.sHtML

[U88] JS：对象展开合并
来源：http://wap.zdbjq.cn/Article/details/gdbowhvsb.sHtML

{ ...a, ...b }
来源：http://wap.zdbjq.cn/Article/details/gzhavzcte.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gwdocbrgt.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gfnazzenl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fehbvm.com/Article/details/givsxrzah.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/giaubhrko.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gadxszeur.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gyxyloxwm.sHtML

[U92] JS：深拷贝
来源：http://mobile.zdbjq.cn/Article/details/gqkoqvrir.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwtueoqmd.sHtML


<!-- 参考信息 -->