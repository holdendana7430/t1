代发 wailian999

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gqcnlheta.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gycptcpre.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gmtglxybe.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/ggbuweach.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gomwbfeoa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gbnzwidas.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gvokodras.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gprtmnizg.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gribmpisg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gbxkvykss.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/gcmklfmus.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghoecogbn.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gftsyfatw.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gzlkptpev.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gsvrcfvgm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gzjjssvjs.sHtML

[T11] Kotlin：协程
来源：http://read.share.zdbjq.cn/Article/details/ggbjfhpaq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/ghbeppimr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gbghkzyxn.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfzsdgahw.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gtkcufezy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gynklvada.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gosvgccgo.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/glaloyaii.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gfavgbtcj.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gvodkgzzx.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/ghtopxjrj.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gjukzuaij.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/ggoxllete.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gcuwknenz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gwljhomxo.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gjdbethwe.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gsludvrnm.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gjnznhzbg.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gwfizbkga.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gwbiblvcm.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/ghmhzzppa.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gcyvsdjlw.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/gfrcuauey.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/glomovbyr.sHtML

[T23] Swift：函数
来源：http://www.blog.hesvh.cn/Article/details/gghjmjwqj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/geevvltkb.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gzctnyffw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/glglmmyjn.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gywzowsns.sHtML

struct P { var x: Int }
来源：http://wap.fehbvm.com/Article/details/gqcbshtac.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gdidvehvg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gqqihbjmq.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gzpywqafu.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gzklsyiki.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grtlejkec.sHtML

enum Color { case red, green }
来源：http://read.share.zdbjq.cn/Article/details/gzknjufbh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gkyxunqxc.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/gepktaufj.sHtML

[T30] Swift：协议
来源：http://3g.fehbvm.com/Article/details/gkpbeagyt.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.zdbjq.cn/Article/details/gkgrgdenl.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gugmjyfxu.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gboztiwkf.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gfkqsevsb.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gdlctyrna.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gwuzisdjp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.hesvh.cn/Article/details/gpswznzqb.sHtML

[T34] Lua：遍历表
来源：http://mobile.fehbvm.com/Article/details/gjhkneqcf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gsutkycyn.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gitixmyab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gcwwffkjc.sHtML

[T36] Lua：函数
来源：http://read.share.zdbjq.cn/Article/details/grpawvlbo.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gclocgzvq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gaasceiuv.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/govsxghvk.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/glevlktqe.sHtML

if x > 0 then print("正") end
来源：http://baike.fehbvm.com/Article/details/gidvuqlll.sHtML

[T39] Lua：模式匹配
来源：http://read.share.hesvh.cn/Article/details/giqxjjyey.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/gkhbxcfbz.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gqhyewydg.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gdompaooq.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/grayaxtge.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gzkjzfvah.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gjctnqinn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/gozvpkzic.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/geotdvpar.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gqvpedewn.sHtML

[T44] Perl：条件
来源：http://3g.fehbvm.com/Article/details/gamhognrn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpttnjxe.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.hesvh.cn/Article/details/gipmeojaj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fehbvm.com/Article/details/gwonkmqvg.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.hesvh.cn/Article/details/gdcpckjvs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.zdbjq.cn/Article/details/guangremf.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gvtqyggfo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.zdbjq.cn/Article/details/grwynlpos.sHtML

[T48] Perl：正则替换
来源：http://m.share.fehbvm.com/Article/details/gdwwrcfuc.sHtML

$s =~ s/old/new/g;
来源：http://3g.fehbvm.com/Article/details/gyoastolp.sHtML

[T49] Perl：函数
来源：http://read.share.hesvh.cn/Article/details/gpqnrvtii.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gslwncfhw.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/graipmmht.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.zdbjq.cn/Article/details/gkiqemfjd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gmkuppfyl.sHtML

[T51] Scala：Hello World
来源：http://m.share.hesvh.cn/Article/details/gppcdncjz.sHtML

println("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gmphtkfjv.sHtML

[T52] Scala：变量
来源：http://m.share.hesvh.cn/Article/details/gkcsowywv.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gaynnrpxn.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/gqkcziphm.sHtML

s"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gkmqphcby.sHtML

[T54] Scala：集合映射
来源：http://mobile.hesvh.cn/Article/details/geyuseewt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.zdbjq.cn/Article/details/gpnehjkke.sHtML

[T55] Scala：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gbcdiskcm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fehbvm.com/Article/details/gaimxhjjd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fehbvm.com/Article/details/gluqheeoy.sHtML

case class User(name: String, age: Int)
来源：http://baike.fehbvm.com/Article/details/grtdwwccs.sHtML

[T57] Scala：模式匹配
来源：http://wap.fehbvm.com/Article/details/guqwucxhl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.hesvh.cn/Article/details/gouehckcb.sHtML

[T58] Scala：函数定义
来源：http://read.share.hesvh.cn/Article/details/gesmhvyrc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.hesvh.cn/Article/details/gwraidawi.sHtML

[T59] Scala：循环
来源：http://www.m.share.hesvh.cn/Article/details/gvhlogubz.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.hesvh.cn/Article/details/glbuaouka.sHtML

[T60] Scala：折叠
来源：http://www.share.fehbvm.com/Article/details/gitrmgqmr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/gqywuetyk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxswszpyu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gltayrgbz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghztbotju.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.hesvh.cn/Article/details/gltjbytlj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.zdbjq.cn/Article/details/gvxpvvnkz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fehbvm.com/Article/details/gdqswcawn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghmkptsbc.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.zdbjq.cn/Article/details/gjmuixjxs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.hesvh.cn/Article/details/gfnsnxoei.sHtML

[U04] Py：变量调试打印
来源：http://wap.fehbvm.com/Article/details/gizcgrwab.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fehbvm.com/Article/details/gbbrebjjb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/gpxbjtihv.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gaqwjupsk.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gtukzuuyn.sHtML

{**a, **b}
来源：http://blog.hesvh.cn/Article/details/glpmwcfyg.sHtML

[U07] Py：反转字典键值
来源：http://baike.hesvh.cn/Article/details/gngmtrbtw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.zdbjq.cn/Article/details/ghrkkigzo.sHtML

[U08] Py：展平二维列表
来源：http://m.share.zdbjq.cn/Article/details/gsdwvvijd.sHtML

[y for x in nested for y in x]
来源：http://wap.zdbjq.cn/Article/details/gfdjmwhjt.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.zdbjq.cn/Article/details/gaspgwpmt.sHtML

max(d, key=d.get)
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqghspb.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/grgywekyk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.fehbvm.com/Article/details/gfnatfypc.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.zdbjq.cn/Article/details/ghtftrgmy.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.hesvh.cn/Article/details/goahbjodw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.hesvh.cn/Article/details/gbhslhvhc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.hesvh.cn/Article/details/gapsighqv.sHtML

[U13] Py：固定长度队列
来源：http://www.share.hesvh.cn/Article/details/geaevdcjs.sHtML

deque(maxlen=10)
来源：http://read.share.fehbvm.com/Article/details/gwxwxqdrf.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.zdbjq.cn/Article/details/gnuejoeft.sHtML

defaultdict(list)
来源：http://m.share.fehbvm.com/Article/details/gumccbqjp.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gfkhpnlky.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gsgpenkha.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gnoalwgzu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.zdbjq.cn/Article/details/gifiwrbae.sHtML

[U17] Py：初始化日志
来源：http://read.share.hesvh.cn/Article/details/ggvxuklqg.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gkbveigrx.sHtML

[U18] Py：预编译正则
来源：http://m.share.zdbjq.cn/Article/details/guoshhbca.sHtML

pat = re.compile(r"\d+")
来源：http://wap.zdbjq.cn/Article/details/gypruwtzj.sHtML

[U19] Py：正则替换带回调
来源：http://wap.fehbvm.com/Article/details/gsiqhrnwz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fehbvm.com/Article/details/gqcbnbeym.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.zdbjq.cn/Article/details/gwdipqemw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/grdyswaun.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.fehbvm.com/Article/details/grapwrqve.sHtML

@contextlib.contextmanager
来源：http://mobile.fehbvm.com/Article/details/gfwvorimd.sHtML

[U22] Py：矩阵转置
来源：http://www.share.zdbjq.cn/Article/details/gbwmkidem.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/gacixnmap.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.fehbvm.com/Article/details/gihuuhyil.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.hesvh.cn/Article/details/gwpyfjbbr.sHtML

[U24] Py：路径操作
来源：http://www.share.hesvh.cn/Article/details/gzllaebbr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gepxgbdbh.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fehbvm.com/Article/details/gkfeirntq.sHtML

csv.DictReader(f)
来源：http://www.share.fehbvm.com/Article/details/gxirdoyel.sHtML

[U26] Py：并发下载
来源：http://www.blog.zdbjq.cn/Article/details/ggyqarvrh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/giurblgjx.sHtML

[U27] Py：异步 HTTP
来源：http://3g.hesvh.cn/Article/details/giwgszkvi.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.hesvh.cn/Article/details/gmarczzsk.sHtML

[U28] Py：类型别名
来源：http://mobile.zdbjq.cn/Article/details/gfzoknibg.sHtML

UserId = int
来源：http://blog.fehbvm.com/Article/details/gzxqobhjv.sHtML

[U29] Py：属性校验
来源：http://blog.zdbjq.cn/Article/details/gxtjknqsr.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gfyqwqmai.sHtML

[U30] Py：数据类
来源：http://www.blog.hesvh.cn/Article/details/gxoxagvdj.sHtML

@dataclass(slots=True)
来源：http://read.share.fehbvm.com/Article/details/grixlczpq.sHtML

[U31] Py：单测
来源：http://read.share.zdbjq.cn/Article/details/gphlrxgtk.sHtML

python -m pytest -q
来源：http://www.m.share.hesvh.cn/Article/details/gvunjdjlk.sHtML

[U32] Py：代码格式化
来源：http://baike.hesvh.cn/Article/details/ghuguzibt.sHtML

ruff format . && ruff check --fix .
来源：http://blog.hesvh.cn/Article/details/ggxpjivzf.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/guglskaaq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/gnhdxbkwa.sHtML

[U34] Py：判断编码
来源：http://baike.fehbvm.com/Article/details/gnyrpnzle.sHtML

chardet.detect(raw)
来源：http://m.share.zdbjq.cn/Article/details/gehlgxlga.sHtML

[U35] Py：发送邮件
来源：http://www.blog.zdbjq.cn/Article/details/guhhoeovk.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gszdqtrnq.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gnvrutnrk.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gnluoalte.sHtML

[U37] Py：读写 Excel
来源：http://blog.hesvh.cn/Article/details/gxgzoatcg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.zdbjq.cn/Article/details/ggtupyatt.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.zdbjq.cn/Article/details/gnvnpabbe.sHtML

Path(__file__).resolve().parent
来源：http://www.share.zdbjq.cn/Article/details/gowpwigwu.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.zdbjq.cn/Article/details/gvlcophki.sHtML

sys.stdout.isatty()
来源：http://www.blog.zdbjq.cn/Article/details/goszmsqpa.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fehbvm.com/Article/details/gajmiyewq.sHtML

print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gybjzcdfh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fehbvm.com/Article/details/gxadgiphm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fehbvm.com/Article/details/grhpgpvps.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gnyilquxf.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.hesvh.cn/Article/details/gfwpwspvl.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/ghqobhlsb.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gpzlknlie.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gbccwtlsh.sHtML

declare(strict_types=1);
来源：http://www.blog.fehbvm.com/Article/details/gnomvfqkk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gyrukvevf.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/glyxygsey.sHtML

[U46] PHP：可空类型
来源：http://mobile.zdbjq.cn/Article/details/gwhrjfiao.sHtML

?string $name = null
来源：http://read.share.fehbvm.com/Article/details/glcudavxr.sHtML

[U47] PHP：联合类型
来源：http://3g.fehbvm.com/Article/details/gjaqaphmr.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gmuxmpjdm.sHtML

[U48] PHP：纯枚举
来源：http://blog.zdbjq.cn/Article/details/gfutrvhel.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.zdbjq.cn/Article/details/gigghygjh.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/gbxywauve.sHtML

public readonly string $name
来源：http://blog.hesvh.cn/Article/details/gpoqmxweu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.zdbjq.cn/Article/details/ghhveglfq.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.hesvh.cn/Article/details/geewyqlht.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gvytgswfh.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gkqvsvjbi.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gqhyhjgad.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.fehbvm.com/Article/details/gqbksviro.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/ghsrzdwnr.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.zdbjq.cn/Article/details/gxtrumyru.sHtML

[U54] PHP：空安全调用
来源：http://wap.zdbjq.cn/Article/details/gxkmsmjmm.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gbjiqovvl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gijzypbag.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.zdbjq.cn/Article/details/ggiplukgf.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gmikxewuo.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gqejdoicz.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gkxuoosmm.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gzvrmkerg.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/grvqrilpc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghessfyfh.sHtML

[U59] PHP：自定义排序
来源：http://wap.hesvh.cn/Article/details/gvrvcgclh.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmmofsrgz.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/gdqxpyxhs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gisjawxom.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gegjklxkt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gqaiwylhm.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gwoozvghx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.fehbvm.com/Article/details/gpbaphznv.sHtML

[U63] PHP：文件读写
来源：http://blog.hesvh.cn/Article/details/grtiwkttd.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gqwjawmok.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnpgttmzo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gzspdbhku.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gaprddspa.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gtgtkoyal.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/ggjedfwss.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghksicqzw.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.hesvh.cn/Article/details/gjpgfnedw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gfmcbusqz.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fehbvm.com/Article/details/gqzaujgvj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gkhmhwyqy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/grbjysaeo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gjoqmbkll.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gqewjknpe.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gtkdgehmz.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gjhnpmpir.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gndjesymj.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gdckdscwz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gfrrnepey.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fehbvm.com/Article/details/gbicjdtxf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fehbvm.com/Article/details/gtslwylkr.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gxtowmieq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gywfddryq.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gifkuvadg.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gorxsjejw.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gftdvgeko.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.hesvh.cn/Article/details/gktmlhvnk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gozgotblq.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/ghsooepam.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gblnacvra.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gejvgmiwr.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/goaomkkws.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.zdbjq.cn/Article/details/gqcmtobfn.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gzvluqxkd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.hesvh.cn/Article/details/gthjuzckq.sHtML

[U81] JS：初始化项目
来源：http://m.share.fehbvm.com/Article/details/gjnikawik.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gwihorypp.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gfhkeruza.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gwquujhgm.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fehbvm.com/Article/details/gnjaoopkk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gmemoihbw.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gvtbdinux.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gaxljdbci.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gatmyekjt.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/girayfeyd.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/guugjidmq.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gvyitsjhp.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gjszzbxxq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/ggeqlenur.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gbafxsruc.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/glunqossd.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/ghfxiruuq.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggodnnafx.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghconnyln.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gyqzgnpnd.sHtML


<!-- 参考信息 -->