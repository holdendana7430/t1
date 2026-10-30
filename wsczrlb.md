代发 wailian999

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gjelqaukl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxhsqhzv.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrtcfkup.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfviehxh.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ggowxtqyt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghajcwoqh.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gqmawyvzu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gvaoyzeru.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxnjqess.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/gjoexwnwb.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/gocehjmjy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjocovkfa.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/gcszgtuia.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbogcpvvv.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gsfegvkps.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guotjyfag.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpxanuir.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaipffmb.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvheauafz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafjhwqrg.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gdgzmwszw.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcljrplg.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glrnkmgjo.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdamnktxo.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gtnphnxmf.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnkkaaqds.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gdbnqgaih.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqthccls.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklsalnjf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govccbrsm.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gleduhdrl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fanxiaobao.xyz/Article/details/guobfqkhp.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgjriiza.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzvatjdr.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdmfrnwoq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhxzzsax.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkrmhucnj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmazwwrbf.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwdrsiue.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gozirmnge.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glibkhioq.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslmsjfup.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gbotkjics.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gjlkdilwo.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoiykdff.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gguicoltc.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gpmjbkddv.sHtML

enum Color { case red, green }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpxpkfqu.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gbocryncc.sHtML

guard let x = opt else { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/glcefhqma.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gibmsczbv.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyhvdraq.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvizceuz.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfcahboi.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glejlsqcl.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/grwzladiv.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqsimsby.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gsibhbxnq.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjyxxwjq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/glmyzdacv.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfzwvtvm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjuymhmd.sHtML

[T36] Lua：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gndjklqqb.sHtML

function add(a, b) return a + b end
来源：http://mobile.fanxiaobao.xyz/Article/details/gooyuhhlj.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gleokivcj.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gpkpropfl.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvukfhthn.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gvntchtmr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvdoeoxt.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/goktrprka.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gortfanpn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fanxiaobao.xyz/Article/details/gseaxeqrd.sHtML

[T41] Perl：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gefjysacm.sHtML

print "Hello\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvkaozep.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxmpusl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpnakgwq.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrhdlbel.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/ghozorhle.sHtML

[T44] Perl：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gvtsbjjbj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gejaqkxcu.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gljeyisko.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydxnpczl.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gobstwqpa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gykpyterg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/grrurogwa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdkhicndl.sHtML

[T48] Perl：正则替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdgkywb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzptmuer.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbbjekxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpioulnyz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtgkgrgwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcirvuhg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtunbvsrm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotidreea.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gneggdzkm.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvntmclz.sHtML

val a = 1;  var b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gojhpdmry.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glppxpmqf.sHtML

s"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gelxrtzml.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqssxvd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqayhdhyk.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gctnxlbyi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/getqnhsmi.sHtML

[T56] Scala：样例类
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbskwynr.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gffcudukd.sHtML

[T57] Scala：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gzffhojch.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnlptrsm.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gicxqajkg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/glejowkgd.sHtML

[T59] Scala：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gyudtdsgf.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gdgwceboq.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvaypfzr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxxeesck.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gfyvasfck.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gflxhvjto.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlhvetmc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynjcwfbx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gkmtkflyx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogueluzc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxylxrxqm.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.fanxiaobao.xyz/Article/details/gpbqhtdky.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmapfuph.sHtML

[U04] Py：变量调试打印
来源：http://m.share.fanxiaobao.xyz/Article/details/gpobkhaoi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fanxiaobao.xyz/Article/details/gefzfsdwb.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbadtsfdp.sHtML

list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gjhukhdme.sHtML

[U06] Py：合并两个字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgquyhva.sHtML

{**a, **b}
来源：http://wap.fanxiaobao.xyz/Article/details/gpysxkbdm.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflsrxdv.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmejibe.sHtML

[U08] Py：展平二维列表
来源：http://blog.fanxiaobao.xyz/Article/details/gonuuncgb.sHtML

[y for x in nested for y in x]
来源：http://wap.fanxiaobao.xyz/Article/details/gbpmbxcmo.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fanxiaobao.xyz/Article/details/gwryzwuhd.sHtML

max(d, key=d.get)
来源：http://baike.fanxiaobao.xyz/Article/details/gfprldyuj.sHtML

[U10] Py：按值排序字典
来源：http://wap.fanxiaobao.xyz/Article/details/gigmgyvyn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fanxiaobao.xyz/Article/details/gsedsejej.sHtML

[U11] Py：生成器表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gbtyxvqsx.sHtML

(x * 2 for x in arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpoojuyd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grtgxcamp.sHtML

Counter(arr).most_common(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkyudezd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrnpbnoa.sHtML

deque(maxlen=10)
来源：http://wap.fanxiaobao.xyz/Article/details/gnuzzkdbu.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fanxiaobao.xyz/Article/details/gnlfglbdd.sHtML

defaultdict(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwaxpepu.sHtML

[U15] Py：高精度计时
来源：http://blog.fanxiaobao.xyz/Article/details/gjgvemtou.sHtML

t = time.perf_counter()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuwclgxm.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnmonxrq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wap.fanxiaobao.xyz/Article/details/gwwhiifoe.sHtML

[U17] Py：初始化日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrddbkk.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjmrzbym.sHtML

[U18] Py：预编译正则
来源：http://read.share.fanxiaobao.xyz/Article/details/gkntomjst.sHtML

pat = re.compile(r"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gkpzqmobz.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fanxiaobao.xyz/Article/details/geppcarmi.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynahesvm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fanxiaobao.xyz/Article/details/ggrartapj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvofaorir.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyqetofr.sHtML

@contextlib.contextmanager
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxzneca.sHtML

[U22] Py：矩阵转置
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwlvveiv.sHtML

list(zip(*m))
来源：http://wap.fanxiaobao.xyz/Article/details/gmcjviyly.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsvggjey.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxqhwzu.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrcners.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/geydnvhdi.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwhxzjhi.sHtML

csv.DictReader(f)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcwgcvsl.sHtML

[U26] Py：并发下载
来源：http://m.share.fanxiaobao.xyz/Article/details/gdghqesbx.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexyvtsag.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccmoejp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fanxiaobao.xyz/Article/details/grpqhfcfv.sHtML

[U28] Py：类型别名
来源：http://wap.fanxiaobao.xyz/Article/details/gmevuvsks.sHtML

UserId = int
来源：http://baike.fanxiaobao.xyz/Article/details/gvnrcayii.sHtML

[U29] Py：属性校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqqqjbap.sHtML

@property 与 @x.setter 配合
来源：http://blog.fanxiaobao.xyz/Article/details/ggndusfau.sHtML

[U30] Py：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwjzzhc.sHtML

@dataclass(slots=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxcmcnez.sHtML

[U31] Py：单测
来源：http://www.share.fanxiaobao.xyz/Article/details/gczhoaoxy.sHtML

python -m pytest -q
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmlvwgi.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpozelhx.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmfsodhk.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpqejuom.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.fanxiaobao.xyz/Article/details/gdbhdjtwu.sHtML

[U34] Py：判断编码
来源：http://wap.fanxiaobao.xyz/Article/details/geisjgqbf.sHtML

chardet.detect(raw)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrrhxerf.sHtML

[U35] Py：发送邮件
来源：http://wap.fanxiaobao.xyz/Article/details/gcufzhxpv.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmjzirbu.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwivvyyqb.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqsdgenb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/grpelywdy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gevurrews.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fanxiaobao.xyz/Article/details/gftanoylu.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/guxsiilvy.sHtML

[U39] Py：判断是否在交互环境
来源：http://3g.fanxiaobao.xyz/Article/details/guctkgmcx.sHtML

sys.stdout.isatty()
来源：http://blog.fanxiaobao.xyz/Article/details/gsvpqsvpr.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gslpfznec.sHtML

print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdalfziu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fanxiaobao.xyz/Article/details/gippgigfs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqjusqkb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fanxiaobao.xyz/Article/details/glmbqvsve.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjevgzmw.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gzotukyyk.sHtML

namespace App\Http;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmwdgrlv.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghakwsapm.sHtML

declare(strict_types=1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhzxpplf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaiensft.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxmmjhoo.sHtML

[U46] PHP：可空类型
来源：http://blog.fanxiaobao.xyz/Article/details/ghyzfvlmv.sHtML

?string $name = null
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmmnjbfr.sHtML

[U47] PHP：联合类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcmelhfd.sHtML

int|string $id
来源：http://3g.fanxiaobao.xyz/Article/details/gbiudsfft.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/grazialmi.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gniujqnal.sHtML

[U49] PHP：只读属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbhmjqak.sHtML

public readonly string $name
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfrffanz.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.fanxiaobao.xyz/Article/details/ggiwfidcl.sHtML

public function __construct(private int $id) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjbvmlgio.sHtML

[U51] PHP：数组解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gzchejbuk.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhqvaifz.sHtML

[U52] PHP：箭头函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbiswzlay.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnlfqtkr.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fanxiaobao.xyz/Article/details/gatvsuugn.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fanxiaobao.xyz/Article/details/grafhsvhq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaapwvrpb.sHtML

$obj?->method()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwhrapw.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gbernfter.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpdcowvb.sHtML

[U56] PHP：命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gelyenzzn.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjjhtvqk.sHtML

[U57] PHP：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gplubhewx.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gteenubjd.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fanxiaobao.xyz/Article/details/gykldeedi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gjtzpwfoy.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfsdspiw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/glryvvxdl.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaunoaww.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gugmiryky.sHtML

[U61] PHP：正则
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiocqcmg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gckunisjs.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfzugzmt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdwxcfr.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gbujnllxf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqoidytw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtocgpeme.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvapwpkmo.sHtML

[U65] PHP：会话
来源：http://baike.fanxiaobao.xyz/Article/details/gpulooykg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytszyon.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatiaglia.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/grabasdzh.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/gsdscbvhp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdmaxjws.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhccuvw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgsrsvbs.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjiprxds.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhlwwvpq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fanxiaobao.xyz/Article/details/ggjzltihm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.fanxiaobao.xyz/Article/details/gmnhbgztt.sHtML

[U71] PHP：抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbetnnub.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaajyjbed.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwexgndx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcdudofl.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/gnpmsezcf.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fanxiaobao.xyz/Article/details/gepsszbrv.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtxfgpfk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvasvhv.sHtML

[U75] PHP：依赖注入
来源：http://baike.fanxiaobao.xyz/Article/details/gzfruhwkh.sHtML

composer require psr/container
来源：http://mobile.fanxiaobao.xyz/Article/details/gusyxnmuk.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gfhnzzcxd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvplgglpf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fanxiaobao.xyz/Article/details/gimlygiwz.sHtML

composer require twig/twig
来源：http://3g.fanxiaobao.xyz/Article/details/gpznghnxx.sHtML

[U78] PHP：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeesejxs.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihmnsbm.sHtML

[U79] PHP：静态分析
来源：http://blog.fanxiaobao.xyz/Article/details/gxbojgvbv.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcfulncv.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/gzagavhfi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gundjgnpn.sHtML

[U81] JS：初始化项目
来源：http://blog.fanxiaobao.xyz/Article/details/gzyswouup.sHtML

npm init -y;  npm i express
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstvpmxz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fanxiaobao.xyz/Article/details/gcetwshgm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gvhwmuhcm.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.fanxiaobao.xyz/Article/details/ghgkqglfa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gpbcqrfne.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gunkmijis.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvowvkni.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/giwaubimx.sHtML

a?.b?.c
来源：http://baike.fanxiaobao.xyz/Article/details/ggxzuvlzt.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gebhyqasq.sHtML

a ?? b
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfilini.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gejxcudfu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuodylqz.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gvzuvohyc.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gxmjxnguu.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/grvvkissf.sHtML

[...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgowvmag.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmksnbqke.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/geaqxlvri.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gasinskmf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdcayvtq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefwmtout.sHtML

structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goglhfphq.sHtML


<!-- 参考信息 -->