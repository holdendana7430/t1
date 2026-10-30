代发 wailian999

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtgvlbgdx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gvmarsxns.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/glifzxsbc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gutzhsibk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gmoetfaep.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gcguasegt.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gqlkyszvq.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gpovbkrfz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gkwdaxzgq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/guzkgvuae.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gjdeldwlh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gntyqvmgf.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gmgucxsar.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gaacnpaeo.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gvxxhwnwi.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/garcjdwgl.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gmmajalzu.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gkeruxnbg.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gjdsnpjyu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gfwkcbqzx.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gxcnacfbn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gxchnfyjo.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gxwkducip.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gcxssgodu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gxknbnkkb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.hesvh.cn/Article/details/gxvedigfj.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gkwcwdppq.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/gklagoieu.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/ggxojumvt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gvyvgmwzj.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdxmtzkqb.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gfpkohwrh.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/gnigaszuq.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gfcnufwse.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gkaizrusd.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/grvmyrgol.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gxkmgdftj.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/giejjsmyg.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gfjcmplut.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gbumolesf.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gjfyckojs.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gmsjrnrrt.sHtML

[T22] Swift：字典
来源：http://baike.hesvh.cn/Article/details/gmrgramhv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/ggklrklkv.sHtML

[T23] Swift：函数
来源：http://www.blog.zdbjq.cn/Article/details/glveikhlz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/ghzwtlgee.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gvstfykpo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbuecquog.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/ghwldtemi.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/ghfzcobxu.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gengddjgz.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gtedqonnf.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/grseiaqbd.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/ggtqwbmsl.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gwnqudmei.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/glnaasinz.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.hesvh.cn/Article/details/glyupuzul.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/grlvyppph.sHtML

[T30] Swift：协议
来源：http://www.m.share.hesvh.cn/Article/details/gffstzidj.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/ggjjzyvtp.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gbyddxrim.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gyuaqgrye.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/ggznnjble.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/ggcqmvkbf.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gonelnwkm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gvvzocjnh.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gbfjdfiff.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gfszbbdqb.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gbyshliru.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fehbvm.com/Article/details/gxiwzeyxu.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/gdydksvcy.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gdebmobnm.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gcgvlarab.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gtjlawvxs.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/gtpvjytmm.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/gixhhygbw.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gsxxznpsp.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gycqgewkv.sHtML

[T40] Lua：元表
来源：http://m.share.fehbvm.com/Article/details/genndgzqg.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.zdbjq.cn/Article/details/gddxdqtim.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtqfkvopd.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/gyenekxao.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gwdkgwwlx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.zdbjq.cn/Article/details/grcxfkbbv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gkwcuskvj.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gtqnzsdwk.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gthbwesbv.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gkvxurvlr.sHtML

[T45] Perl：数组遍历
来源：http://wap.hesvh.cn/Article/details/gftcrplcf.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gxaoambsn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gbzglhlkg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gmsdrjnry.sHtML

[T47] Perl：正则捕获
来源：http://baike.zdbjq.cn/Article/details/guukbvxrr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/ggozmpave.sHtML

[T48] Perl：正则替换
来源：http://baike.hesvh.cn/Article/details/glbmaqwnm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gpwrhjpsh.sHtML

[T49] Perl：函数
来源：http://baike.zdbjq.cn/Article/details/gqvcapcyq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/galdgdqug.sHtML

[T50] Perl：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsqrwdspc.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.hesvh.cn/Article/details/ghdxizire.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gztuycgxt.sHtML

[T51] Scala：Hello World
来源：http://read.share.hesvh.cn/Article/details/gevaccqph.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/gxietlryt.sHtML

[T52] Scala：变量
来源：http://m.share.fehbvm.com/Article/details/getabyqkb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gwfhoarvg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gnfkywlcd.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gunyyauaa.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/gnkkazftd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fehbvm.com/Article/details/gnqutqxdm.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gaiquuzbs.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.zdbjq.cn/Article/details/gsrnrjmat.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/gaihdshuo.sHtML

case class User(name: String, age: Int)
来源：http://blog.hesvh.cn/Article/details/geqibqlho.sHtML

[T57] Scala：模式匹配
来源：http://www.share.fehbvm.com/Article/details/gffyzawkc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gccejxudb.sHtML

[T58] Scala：函数定义
来源：http://m.share.hesvh.cn/Article/details/gztjiaxjh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.hesvh.cn/Article/details/gbijkuzjx.sHtML

[T59] Scala：循环
来源：http://www.share.zdbjq.cn/Article/details/gdcrjcuuc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gplswmlme.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gwpgsrpat.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gmgvfdldn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxrqnwcuy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gcsztqulb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghihutswb.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.hesvh.cn/Article/details/gcqgyviym.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.hesvh.cn/Article/details/gbfrrpeof.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.fehbvm.com/Article/details/gzihaxzij.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.fehbvm.com/Article/details/gyoxbghzl.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.hesvh.cn/Article/details/gpzueijht.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.hesvh.cn/Article/details/gsxwybbox.sHtML

[U04] Py：变量调试打印
来源：http://3g.hesvh.cn/Article/details/gctegfqug.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.hesvh.cn/Article/details/gichgtppx.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fehbvm.com/Article/details/gocrkqjsr.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gowmyinyk.sHtML

[U06] Py：合并两个字典
来源：http://wap.fehbvm.com/Article/details/gtoogsntn.sHtML

{**a, **b}
来源：http://www.m.share.fehbvm.com/Article/details/greohoonf.sHtML

[U07] Py：反转字典键值
来源：http://www.share.zdbjq.cn/Article/details/gvvnxrxeo.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.hesvh.cn/Article/details/gekycunex.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fehbvm.com/Article/details/gwwvzvsix.sHtML

[y for x in nested for y in x]
来源：http://baike.fehbvm.com/Article/details/gznpwbvyv.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fehbvm.com/Article/details/ggzgzeycc.sHtML

max(d, key=d.get)
来源：http://baike.hesvh.cn/Article/details/gvwrgkykz.sHtML

[U10] Py：按值排序字典
来源：http://blog.zdbjq.cn/Article/details/gpvraepse.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gycvrzpmo.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.fehbvm.com/Article/details/gsmhrpmym.sHtML

(x * 2 for x in arr)
来源：http://baike.zdbjq.cn/Article/details/gnqnymzkh.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.hesvh.cn/Article/details/gpqmwjhom.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gagtvdwgh.sHtML

[U13] Py：固定长度队列
来源：http://3g.zdbjq.cn/Article/details/gjihfbxmb.sHtML

deque(maxlen=10)
来源：http://www.blog.fehbvm.com/Article/details/gmhvdcgpn.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.hesvh.cn/Article/details/gzatvzffh.sHtML

defaultdict(list)
来源：http://wap.zdbjq.cn/Article/details/gziblkvhm.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.zdbjq.cn/Article/details/geeskksja.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gzivbktyz.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gotooyvfv.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.zdbjq.cn/Article/details/gjljiujmr.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fehbvm.com/Article/details/gzsasocka.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.fehbvm.com/Article/details/gjbdxuoij.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/ggjmydhky.sHtML

pat = re.compile(r"\d+")
来源：http://3g.hesvh.cn/Article/details/gkxgpnofo.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/glecrxogt.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.zdbjq.cn/Article/details/gesojrdsn.sHtML

[U20] Py：缓存函数结果
来源：http://wap.hesvh.cn/Article/details/gcyibkbvo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.hesvh.cn/Article/details/glpxwmpop.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.zdbjq.cn/Article/details/gmbowusnt.sHtML

@contextlib.contextmanager
来源：http://www.share.fehbvm.com/Article/details/gechrttvg.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gswvtocug.sHtML

list(zip(*m))
来源：http://3g.hesvh.cn/Article/details/glrvxkssd.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gyyxozkzl.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.fehbvm.com/Article/details/gpzfrsxvg.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fehbvm.com/Article/details/gjghnifxr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gffguwrgf.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fehbvm.com/Article/details/grkcoeuqp.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gsfiokkgx.sHtML

[U26] Py：并发下载
来源：http://www.share.fehbvm.com/Article/details/gyeiivnwi.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.hesvh.cn/Article/details/gkkyobdut.sHtML

[U27] Py：异步 HTTP
来源：http://blog.zdbjq.cn/Article/details/gescalkqx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.hesvh.cn/Article/details/gfwkpbbvr.sHtML

[U28] Py：类型别名
来源：http://3g.hesvh.cn/Article/details/grlepmrpi.sHtML

UserId = int
来源：http://www.blog.fehbvm.com/Article/details/gqhgcggbu.sHtML

[U29] Py：属性校验
来源：http://www.blog.fehbvm.com/Article/details/gwrptjwwx.sHtML

@property 与 @x.setter 配合
来源：http://3g.zdbjq.cn/Article/details/gvbrexwcr.sHtML

[U30] Py：数据类
来源：http://3g.hesvh.cn/Article/details/gttnjnvoa.sHtML

@dataclass(slots=True)
来源：http://baike.fehbvm.com/Article/details/gxemzuhow.sHtML

[U31] Py：单测
来源：http://read.share.fehbvm.com/Article/details/ggwqmnjrv.sHtML

python -m pytest -q
来源：http://blog.fehbvm.com/Article/details/gjqrpjtsf.sHtML

[U32] Py：代码格式化
来源：http://blog.hesvh.cn/Article/details/ghnlbxivj.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.zdbjq.cn/Article/details/gulnmykip.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gmswjtakz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gmuqloaaq.sHtML

[U34] Py：判断编码
来源：http://baike.zdbjq.cn/Article/details/grwlciaio.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxmcslcer.sHtML

[U35] Py：发送邮件
来源：http://mobile.hesvh.cn/Article/details/gucyfefeo.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fehbvm.com/Article/details/gfwsomhvj.sHtML

[U36] Py：定时任务
来源：http://m.share.fehbvm.com/Article/details/gjuhfhxxd.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.hesvh.cn/Article/details/gafvsoyjm.sHtML

[U37] Py：读写 Excel
来源：http://baike.zdbjq.cn/Article/details/gktepcvrc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.zdbjq.cn/Article/details/gnuqazkis.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.hesvh.cn/Article/details/gytmxzdsy.sHtML

Path(__file__).resolve().parent
来源：http://mobile.fehbvm.com/Article/details/gfkdfumzy.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.fehbvm.com/Article/details/gsglzfxjs.sHtML

sys.stdout.isatty()
来源：http://www.blog.hesvh.cn/Article/details/gxpfrnztq.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fehbvm.com/Article/details/gnnftnzpo.sHtML

print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gsbvbwcsi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/garmdwyfz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/glqrbftgp.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/gyvmzvbuk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gmkrnfqhr.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.fehbvm.com/Article/details/gokotxdjn.sHtML

namespace App\Http;
来源：http://mobile.zdbjq.cn/Article/details/gtlssjtno.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/gazyxyggq.sHtML

declare(strict_types=1);
来源：http://www.blog.zdbjq.cn/Article/details/gsmeqtlkj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gvrdfngrl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/glgahlozp.sHtML

[U46] PHP：可空类型
来源：http://3g.fehbvm.com/Article/details/guzpuipbp.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/guxbwlipy.sHtML

[U47] PHP：联合类型
来源：http://baike.zdbjq.cn/Article/details/gwpnfluoi.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/gpgzyytvs.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fehbvm.com/Article/details/gyksqlkpp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.fehbvm.com/Article/details/glsvnyruw.sHtML

[U49] PHP：只读属性
来源：http://www.share.hesvh.cn/Article/details/gvmrdcenb.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gtztplqym.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gzqvivkig.sHtML

public function __construct(private int $id) {}
来源：http://3g.hesvh.cn/Article/details/gunkgvpns.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gkttafzqw.sHtML

[$a, $b] = $arr;
来源：http://read.share.fehbvm.com/Article/details/gutkyyfhk.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gdhdqhvej.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.hesvh.cn/Article/details/gsvsglwxa.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fehbvm.com/Article/details/gihszikri.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gfpmubuxq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/ghioiupxd.sHtML

$obj?->method()
来源：http://www.m.share.zdbjq.cn/Article/details/gbairaeug.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/googxrjij.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.hesvh.cn/Article/details/gtpsmjvdg.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gnbreutsd.sHtML

f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ggxtgmhxm.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gwejlvfmf.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/gxxcuvdsq.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/galtxwcxo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.zdbjq.cn/Article/details/gigqqzxtz.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gtvmuitdr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gpeyszdes.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gvjsvngmf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gcxsgneyq.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gqmrsrxof.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gdzuwpgoa.sHtML

[U62] PHP：日期对象
来源：http://www.share.zdbjq.cn/Article/details/gixtwcfyv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gcakgkmzw.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/ghrgavyfc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gfsprdnkx.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gixqmjhtf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gvqcxpazz.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gigujeggi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/ggtibaeuz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gluzdqjxj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gqeomuzri.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gmouerqhu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.zdbjq.cn/Article/details/glvibqopw.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/gotwegiru.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.hesvh.cn/Article/details/gevvydkkh.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gqmpxqgwr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gwnwpdpcj.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gkckrteyn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/gizqryzcf.sHtML

[U71] PHP：抛出异常
来源：http://baike.hesvh.cn/Article/details/gfkbjhezf.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gouawtzhq.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gagxdcyeo.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.zdbjq.cn/Article/details/gnruacjbl.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gnlqbzqqr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/guqzcxftj.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwybdkphe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/gefmxdemu.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fehbvm.com/Article/details/ghxttazdx.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/gslbudkyk.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gxtimbqkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.fehbvm.com/Article/details/gyvsuajuw.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/godfsogpe.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gjuccwtzz.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/ggqrdsxxe.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gruprsyri.sHtML

[U79] PHP：静态分析
来源：http://mobile.fehbvm.com/Article/details/gwvrwabcp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gkebmizpy.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gvywvgpro.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gydailvkk.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gmbeeibzh.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gdrcxggzi.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fehbvm.com/Article/details/gxzuqfcpc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gwrjeguja.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.zdbjq.cn/Article/details/gebozhouh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gzyfvgsjb.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.hesvh.cn/Article/details/ghmvuqwll.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gtwaehwgh.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gsavomxot.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gdshtpnyz.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/gcbalpzat.sHtML

a ?? b
来源：http://www.blog.zdbjq.cn/Article/details/ginytqwkp.sHtML

[U87] JS：解构默认值
来源：http://wap.zdbjq.cn/Article/details/gekwkppnh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gcdatesnw.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gffbtsfpb.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gnfmjikpf.sHtML


<!-- 参考信息 -->