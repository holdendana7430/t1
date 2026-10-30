代发 wailian999

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gpuspydrr.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gnfaaznbx.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gmvduuyhq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gtwexcohb.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/goockyrgj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gkissouxt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gzcwxtijg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gjwheepcz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gszitphch.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gvbcaxcoy.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gzbqemysu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzanvpqyw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fehbvm.com/Article/details/gpfbivdme.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gthzivobg.sHtML

[T10] Kotlin：默认参数
来源：http://blog.zdbjq.cn/Article/details/gzopacpss.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gevrsopqi.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gdcayclod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.hesvh.cn/Article/details/gkrxxvnox.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/gdcovdnri.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gwexicmkb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gzhssgrvq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gajzjilzn.sHtML

[T14] Kotlin：循环
来源：http://www.blog.hesvh.cn/Article/details/ggpfqbxxl.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gihzxrsli.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/ggjebzsvl.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/glmfrzzsg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdovyanpp.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbjachmju.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gaamwafqf.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/gctmkmuve.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gthjhjtmq.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gpddgsjss.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/guzatardp.sHtML

if let n = opt { print(n) }
来源：http://read.share.hesvh.cn/Article/details/ggkvmegsg.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gjikfbxbl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/ggoavfxvd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gsmobywhy.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gjokplsfz.sHtML

[T22] Swift：字典
来源：http://read.share.fehbvm.com/Article/details/gtrbzuofj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gdrcxqhyl.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gtcjdzwrv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/ghbbvxryf.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gtngygbju.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/glwqsncwj.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gtoxvmjcx.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gxldnervh.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gzxzuodwi.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gaiysopby.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/gomavkrbm.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.hesvh.cn/Article/details/gpfrenheq.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gnnnhqtfu.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gfhohtpow.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gdpqvuzls.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gjbmwqkkm.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gvsixidkk.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.zdbjq.cn/Article/details/gynvlwnrx.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gmrniymds.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gdfvozhmj.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gybykzgaf.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gksdoynhb.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gjnljwwek.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gkhfxvywy.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/gthobpuuo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gfpdhdjxn.sHtML

[T35] Lua：字典表
来源：http://mobile.fehbvm.com/Article/details/ginrwokuf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gyvjitddt.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gvouxwhsa.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/guclikufn.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gljcjlgix.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gwwnzgjqv.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gqbznewqs.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gtnoxgneu.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gheslafwo.sHtML

string.find(s, "%d+")
来源：http://www.share.fehbvm.com/Article/details/ghbltqrop.sHtML

[T40] Lua：元表
来源：http://mobile.fehbvm.com/Article/details/gapwxtopw.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gadprnput.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/goscumdjg.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/grxqvqwki.sHtML

[T42] Perl：变量类型
来源：http://wap.fehbvm.com/Article/details/gadcdqrpj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gizlwcbxv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gqklywcbl.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gudugpwzt.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gsnabsnts.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gaygbuetc.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gyznhtbzj.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gadmsmoww.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gxwbqexjg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gsratfxma.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gvrhigzik.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gqecaqffb.sHtML

[T48] Perl：正则替换
来源：http://www.share.hesvh.cn/Article/details/ghitxvleq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.zdbjq.cn/Article/details/gpclrxsvm.sHtML

[T49] Perl：函数
来源：http://wap.hesvh.cn/Article/details/gcybdvnsv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gcpowvyht.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjcpcsiby.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.hesvh.cn/Article/details/gkclwfzmj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.hesvh.cn/Article/details/gmyarwcos.sHtML

[T51] Scala：Hello World
来源：http://mobile.fehbvm.com/Article/details/gyqrbpods.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gotzaexdq.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gtzzywxif.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gnyjlwldi.sHtML

[T53] Scala：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gmfdevqnd.sHtML

s"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gjmcibyty.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gxmgbfjqd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/gclhaxmcd.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gxfrxyksi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghxqfggof.sHtML

[T56] Scala：样例类
来源：http://blog.fehbvm.com/Article/details/ghzykazrg.sHtML

case class User(name: String, age: Int)
来源：http://wap.zdbjq.cn/Article/details/gptvnzrpc.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gzcklytde.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/gtxrqyque.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/ggulrcqja.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fehbvm.com/Article/details/ghqjjuarl.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gnwvenafn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gkqvzjszi.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gtkwysxcq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fehbvm.com/Article/details/gaosbwxrr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbkejtcly.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gdzyjkghi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gccmwpzmk.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.zdbjq.cn/Article/details/gbaihpaus.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/grtaszpuz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.hesvh.cn/Article/details/gxxgifzhb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fehbvm.com/Article/details/ggeylwkoq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fehbvm.com/Article/details/gszthyech.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/gwzipjfik.sHtML

[U04] Py：变量调试打印
来源：http://blog.zdbjq.cn/Article/details/gnppkkefv.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.zdbjq.cn/Article/details/glfztydvj.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.zdbjq.cn/Article/details/gkouyskvb.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gijbbtxkz.sHtML

[U06] Py：合并两个字典
来源：http://mobile.hesvh.cn/Article/details/gljfkrmcv.sHtML

{**a, **b}
来源：http://read.share.fehbvm.com/Article/details/glbmzzxvn.sHtML

[U07] Py：反转字典键值
来源：http://wap.fehbvm.com/Article/details/gezxmprxp.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.zdbjq.cn/Article/details/ggkwihpul.sHtML

[U08] Py：展平二维列表
来源：http://wap.fehbvm.com/Article/details/gyqbcaueu.sHtML

[y for x in nested for y in x]
来源：http://3g.fehbvm.com/Article/details/gognwlycq.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.fehbvm.com/Article/details/glnkwsodm.sHtML

max(d, key=d.get)
来源：http://mobile.hesvh.cn/Article/details/gdkvvkjke.sHtML

[U10] Py：按值排序字典
来源：http://blog.fehbvm.com/Article/details/ghgnrleid.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gxsvnlyfs.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gepwajxzo.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqmxwyutl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.zdbjq.cn/Article/details/glvitmrof.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fehbvm.com/Article/details/gdtzjucad.sHtML

[U13] Py：固定长度队列
来源：http://blog.zdbjq.cn/Article/details/gtxciktsf.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gnpbrmqee.sHtML

[U14] Py：分组收集到列表
来源：http://wap.fehbvm.com/Article/details/guelolvif.sHtML

defaultdict(list)
来源：http://blog.zdbjq.cn/Article/details/gqwyyfdvv.sHtML

[U15] Py：高精度计时
来源：http://read.share.fehbvm.com/Article/details/gbunayugy.sHtML

t = time.perf_counter()
来源：http://mobile.hesvh.cn/Article/details/gxulirvtu.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.fehbvm.com/Article/details/gqcdqattz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.hesvh.cn/Article/details/gcokrolzg.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.hesvh.cn/Article/details/gdhleipfv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.fehbvm.com/Article/details/givjopfhw.sHtML

[U18] Py：预编译正则
来源：http://mobile.hesvh.cn/Article/details/ghkqykifx.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/goguuoxpd.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.zdbjq.cn/Article/details/geudzxkdo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gxuuxfxdq.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.fehbvm.com/Article/details/gnfpbhinv.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.zdbjq.cn/Article/details/ghfaaywha.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.fehbvm.com/Article/details/gpihfycyk.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gdhauyfvi.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/godxudxuq.sHtML

list(zip(*m))
来源：http://www.m.share.hesvh.cn/Article/details/geagrrbah.sHtML

[U23] Py：分块读取大文件
来源：http://baike.fehbvm.com/Article/details/gfdomctrm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/guomepixy.sHtML

[U24] Py：路径操作
来源：http://wap.fehbvm.com/Article/details/gajgfjlnj.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/guczgtszw.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.zdbjq.cn/Article/details/gzuuxwhnq.sHtML

csv.DictReader(f)
来源：http://www.blog.hesvh.cn/Article/details/gebigjnmp.sHtML

[U26] Py：并发下载
来源：http://read.share.fehbvm.com/Article/details/gbpreyanj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.hesvh.cn/Article/details/gnzjelwyp.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.zdbjq.cn/Article/details/gfbagxjfe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.fehbvm.com/Article/details/guadbnkzi.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gufgwpjkz.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gzjcnlmfa.sHtML

[U29] Py：属性校验
来源：http://wap.zdbjq.cn/Article/details/goylfwqkh.sHtML

@property 与 @x.setter 配合
来源：http://www.share.hesvh.cn/Article/details/gegnnhsol.sHtML

[U30] Py：数据类
来源：http://blog.zdbjq.cn/Article/details/gvbtnfpiu.sHtML

@dataclass(slots=True)
来源：http://read.share.zdbjq.cn/Article/details/glrirpkpt.sHtML

[U31] Py：单测
来源：http://blog.fehbvm.com/Article/details/gqitipjin.sHtML

python -m pytest -q
来源：http://m.share.fehbvm.com/Article/details/gwvavegkv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.hesvh.cn/Article/details/gxhjhbtat.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.fehbvm.com/Article/details/ghpamunao.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gruqrecdc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.fehbvm.com/Article/details/ghfblitfu.sHtML

[U34] Py：判断编码
来源：http://www.blog.hesvh.cn/Article/details/gaspejjbj.sHtML

chardet.detect(raw)
来源：http://blog.fehbvm.com/Article/details/gdjwzcbop.sHtML

[U35] Py：发送邮件
来源：http://blog.hesvh.cn/Article/details/gnjdphbrl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.hesvh.cn/Article/details/gtagbhhdb.sHtML

[U36] Py：定时任务
来源：http://mobile.zdbjq.cn/Article/details/gzahuorec.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/gtrtzzzdb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.zdbjq.cn/Article/details/gfklytoin.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.fehbvm.com/Article/details/grzjofyhk.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.hesvh.cn/Article/details/gzhlpnxbj.sHtML

Path(__file__).resolve().parent
来源：http://www.share.hesvh.cn/Article/details/gejixlmkn.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.zdbjq.cn/Article/details/gwjmxgxis.sHtML

sys.stdout.isatty()
来源：http://3g.hesvh.cn/Article/details/gncpjqmkj.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.zdbjq.cn/Article/details/gnhlhlnzm.sHtML

print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gecnkcaqa.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.fehbvm.com/Article/details/gyqmyvwgs.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gvwwanjiy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.fehbvm.com/Article/details/ghtyrxgmj.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gjemlnctu.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fehbvm.com/Article/details/gjuahaxgt.sHtML

namespace App\Http;
来源：http://read.share.zdbjq.cn/Article/details/gxwbzhcrt.sHtML

[U44] PHP：开启严格类型
来源：http://wap.zdbjq.cn/Article/details/gmqcyvpcu.sHtML

declare(strict_types=1);
来源：http://read.share.zdbjq.cn/Article/details/gyshgzthl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.fehbvm.com/Article/details/galazvspl.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/glcgxvvaf.sHtML

[U46] PHP：可空类型
来源：http://wap.hesvh.cn/Article/details/ghfhrewgy.sHtML

?string $name = null
来源：http://wap.zdbjq.cn/Article/details/gqdmkwfzh.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gvdmufrqn.sHtML

int|string $id
来源：http://www.share.zdbjq.cn/Article/details/gubcedjta.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/gbychhnhb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/guwrohmlq.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.hesvh.cn/Article/details/gbqwwawno.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gailstpus.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.hesvh.cn/Article/details/gfolvmfzk.sHtML

public function __construct(private int $id) {}
来源：http://wap.zdbjq.cn/Article/details/glelpbzlp.sHtML

[U51] PHP：数组解构
来源：http://mobile.hesvh.cn/Article/details/gpftefyhh.sHtML

[$a, $b] = $arr;
来源：http://www.blog.zdbjq.cn/Article/details/gvynfgkbi.sHtML

[U52] PHP：箭头函数
来源：http://www.share.hesvh.cn/Article/details/grcctauzn.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gyifatxxr.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.fehbvm.com/Article/details/gpioepavl.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gcfxsniyg.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gxlbxbfrq.sHtML

$obj?->method()
来源：http://wap.hesvh.cn/Article/details/gscvgcxnr.sHtML

[U55] PHP：match 表达式
来源：http://baike.hesvh.cn/Article/details/gbfuyairy.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/gyfpdmnfv.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gyczryszb.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gjnvofvtu.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gyhtkemnd.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gvaatqukd.sHtML

[U58] PHP：数组三件套
来源：http://read.share.zdbjq.cn/Article/details/gwutkvlvz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxwtyfmjs.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gjlwutljd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/grroeeair.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.hesvh.cn/Article/details/gskizvmqn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gdumckzah.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gtjrpbfmv.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvlnpldrq.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gyahsmxoo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fehbvm.com/Article/details/gmjqsjuaf.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.fehbvm.com/Article/details/gopvhqlhu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/gxsixaxzi.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gqnebhmai.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gjougiisn.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/gdnrurikb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gkmasonta.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fehbvm.com/Article/details/gzrzyvmmx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.hesvh.cn/Article/details/gtftmjuwg.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/guyspoezb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gxbyezqzc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fehbvm.com/Article/details/gmishcwra.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gsnzbeggv.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gwcnetzem.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gpvqcmfst.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fehbvm.com/Article/details/gliwqrhcn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gypwdgqwg.sHtML

[U71] PHP：抛出异常
来源：http://baike.fehbvm.com/Article/details/gxzexibrn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gfgjjyoyn.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/gyjgsuhbu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gbskvinvg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/gjtrfbdgs.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/grhgveoqu.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gmgghuyau.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gasneqzvj.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/ghhaasgik.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gzrayhaiv.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gutsebkhg.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gwtjlrqfe.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gwchlfsuo.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/gwkwyrwse.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/geylcxbld.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gnidcmsro.sHtML

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gvtyuyidn.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gnvmcidlv.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gcazpdqjv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gcsnzzidm.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gzesxywfg.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gpisgixmc.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/ghlefotma.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fehbvm.com/Article/details/giqbntqgl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gtsrtozpj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/guiqoftsq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gpfcgwmnb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/ggpsvgmkm.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gpmgwunvh.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ghatvobwf.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gkmoixkyh.sHtML

a ?? b
来源：http://read.share.zdbjq.cn/Article/details/gtujfltpq.sHtML

[U87] JS：解构默认值
来源：http://read.share.fehbvm.com/Article/details/gvathodst.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gxgktiupn.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcldemm.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/guokvyxgm.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gpkmwveec.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbdwecjxa.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gwtauzihn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/ghoelnnux.sHtML


<!-- 参考信息 -->