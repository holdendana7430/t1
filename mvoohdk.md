代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gvbmfdglq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grunzdzqd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/glisjqawx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyffsjrng.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwchiqzpc.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gdushxggb.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gixappnnk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gnkqjsvwq.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gufhimoia.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/ghnhctald.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gipumtnwr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gmhtygiqa.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gvnmvelct.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/grncxicvk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/gtzbrmciq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gbfmvujos.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxjkcvpgn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gvbjiswje.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gmfknddra.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gnalobgxx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/grqpwvtiw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/ggmuxymcz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.hesvh.cn/Article/details/gqmtnulxo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gplwenybx.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/givtowkbw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gjlqtxaeh.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gfvmehnfw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghqpvqtrt.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gkppznaoi.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gzmoqimhh.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/grfafqddt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gpwirijwv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/glahtlwcx.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gywzbygzi.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/givojoocc.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghudrvvif.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gxkiqhznf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/giogfbhlr.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gzsfxpqhv.sHtML

"值: \(b)"
来源：http://www.blog.hesvh.cn/Article/details/ghcixgeex.sHtML

[T19] Swift：可选绑定
来源：http://wap.zdbjq.cn/Article/details/guoydqxbu.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/ggmxxhglw.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gckygyekv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gcqrxgtwg.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gntacxgvv.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gtdqflsgo.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gfikgulpn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fehbvm.com/Article/details/gtmelbmcs.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxhvlkn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/goxfeilse.sHtML

[T24] Swift：闭包
来源：http://blog.hesvh.cn/Article/details/gvmphbqqd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gfzqburje.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/gamxbrrjk.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/grltdvtfl.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gsseluxsj.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gqgnpkouv.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gluygsgkn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gezewlyji.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gtjjdymwd.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/guayifkyq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gfobmgzcu.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/ghcmbvkcc.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/gjwbkorxi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/ggnakhfol.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gwquobewh.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gydqlddbo.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/ghtwqhnlh.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/gghpedqil.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fehbvm.com/Article/details/gccycsckk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.hesvh.cn/Article/details/glwhziarg.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gnzxthkcm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gihmcqrrw.sHtML

[T35] Lua：字典表
来源：http://m.share.hesvh.cn/Article/details/gpkgopijj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.zdbjq.cn/Article/details/gjskubnte.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gaypftyqj.sHtML

function add(a, b) return a + b end
来源：http://wap.fehbvm.com/Article/details/gxwwngvzd.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fehbvm.com/Article/details/gtyshgbgc.sHtML

"a" .. "b"
来源：http://read.share.fehbvm.com/Article/details/ggptzxfrh.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gotxkrcxl.sHtML

if x > 0 then print("正") end
来源：http://3g.zdbjq.cn/Article/details/gqzxqybhd.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/groimpqin.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gjbtphneg.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gpellqitf.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gosklexny.sHtML

[T41] Perl：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmbxqcdrv.sHtML

print "Hello\n";
来源：http://m.share.fehbvm.com/Article/details/gordojzxq.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gpzgdgphp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gyfuwuebz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gnroctlui.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gvtbxxwee.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gxndwaedo.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fehbvm.com/Article/details/gjbeibqdd.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/grsitpugu.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.hesvh.cn/Article/details/gbpkszggi.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/gouxuswid.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gvyouiqnl.sHtML

[T47] Perl：正则捕获
来源：http://wap.hesvh.cn/Article/details/gashexjxp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/grleghsvg.sHtML

[T48] Perl：正则替换
来源：http://www.blog.fehbvm.com/Article/details/gtcnivdri.sHtML

$s =~ s/old/new/g;
来源：http://wap.hesvh.cn/Article/details/gfjjwvseh.sHtML

[T49] Perl：函数
来源：http://baike.hesvh.cn/Article/details/gsdngsdxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gtjzwkpwa.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gxuzxbaol.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fehbvm.com/Article/details/gyiuiiket.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gmzgajjpe.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gebdpaspy.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gnwpaqayy.sHtML

[T52] Scala：变量
来源：http://baike.hesvh.cn/Article/details/gierofsgj.sHtML

val a = 1;  var b = 2
来源：http://3g.hesvh.cn/Article/details/gusbmpacz.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/grhagwoom.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gqmaaqnyh.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/gghoaszqa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghbodehsj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ggatmludq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.zdbjq.cn/Article/details/gwvtmizbr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gdtzruypn.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gtkkvmlmo.sHtML

[T57] Scala：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gvrobxrgm.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.zdbjq.cn/Article/details/grrvadowa.sHtML

[T58] Scala：函数定义
来源：http://mobile.hesvh.cn/Article/details/gnxhhesez.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gnftzpauu.sHtML

[T59] Scala：循环
来源：http://wap.zdbjq.cn/Article/details/gbkfhpazs.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.fehbvm.com/Article/details/gxqdastzx.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gymbogrmf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.zdbjq.cn/Article/details/gdneovlzq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvbrdsrrc.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxkztoqqc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glzxfwxri.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.hesvh.cn/Article/details/gialatorw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fehbvm.com/Article/details/ghiabsjul.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.zdbjq.cn/Article/details/gkrwypltb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.zdbjq.cn/Article/details/gkamtwzfv.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.zdbjq.cn/Article/details/gfralyarn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.hesvh.cn/Article/details/gayteaspc.sHtML

[U04] Py：变量调试打印
来源：http://blog.hesvh.cn/Article/details/gxcwbcldy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.hesvh.cn/Article/details/guqtthmwa.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gifouwqnm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gtymxgkqo.sHtML

[U06] Py：合并两个字典
来源：http://m.share.zdbjq.cn/Article/details/gxzvefmvm.sHtML

{**a, **b}
来源：http://3g.hesvh.cn/Article/details/gawvfcecl.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fehbvm.com/Article/details/gapgwylyx.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fehbvm.com/Article/details/gqppeovhp.sHtML

[U08] Py：展平二维列表
来源：http://baike.zdbjq.cn/Article/details/ggrtzbztz.sHtML

[y for x in nested for y in x]
来源：http://www.blog.fehbvm.com/Article/details/gufunuyjw.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.hesvh.cn/Article/details/gujwggrsh.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gfgqlnhaw.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gazlatunh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.fehbvm.com/Article/details/gfxpqmuhz.sHtML

[U11] Py：生成器表达式
来源：http://3g.zdbjq.cn/Article/details/gvhfmqvvz.sHtML

(x * 2 for x in arr)
来源：http://www.share.zdbjq.cn/Article/details/ggdwfyyrm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.fehbvm.com/Article/details/goireykda.sHtML

Counter(arr).most_common(3)
来源：http://m.share.zdbjq.cn/Article/details/gqwanskno.sHtML

[U13] Py：固定长度队列
来源：http://wap.fehbvm.com/Article/details/gnlpwdzbo.sHtML

deque(maxlen=10)
来源：http://3g.fehbvm.com/Article/details/glwbziltc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fehbvm.com/Article/details/guhncuzmq.sHtML

defaultdict(list)
来源：http://mobile.hesvh.cn/Article/details/gmjjjlldx.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gckcpxabq.sHtML

t = time.perf_counter()
来源：http://mobile.fehbvm.com/Article/details/gkjybqkgl.sHtML

[U16] Py：命令行参数解析
来源：http://blog.zdbjq.cn/Article/details/guevlyjlu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.zdbjq.cn/Article/details/gegopolsl.sHtML

[U17] Py：初始化日志
来源：http://read.share.zdbjq.cn/Article/details/glumgrhcm.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.hesvh.cn/Article/details/gusmtbpcu.sHtML

[U18] Py：预编译正则
来源：http://www.share.hesvh.cn/Article/details/gscxdtruw.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.hesvh.cn/Article/details/gmxectihw.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.fehbvm.com/Article/details/gyvltsisa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.hesvh.cn/Article/details/gjroxxjhx.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.hesvh.cn/Article/details/gyamsmadl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.hesvh.cn/Article/details/gtxqihvpr.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.fehbvm.com/Article/details/gihajsicq.sHtML

@contextlib.contextmanager
来源：http://wap.fehbvm.com/Article/details/gxqlluyos.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.fehbvm.com/Article/details/gjawcplvl.sHtML

list(zip(*m))
来源：http://read.share.zdbjq.cn/Article/details/guhrfcehe.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.zdbjq.cn/Article/details/gspcoauqs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.zdbjq.cn/Article/details/grgzuxety.sHtML

[U24] Py：路径操作
来源：http://m.share.zdbjq.cn/Article/details/gjhybzpiz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gpsvxtmpy.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fehbvm.com/Article/details/gxthbmkqe.sHtML

csv.DictReader(f)
来源：http://mobile.fehbvm.com/Article/details/goemtjbwp.sHtML

[U26] Py：并发下载
来源：http://baike.fehbvm.com/Article/details/gkssuihdc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.hesvh.cn/Article/details/gjiuyecvk.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gsnrctdrs.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.hesvh.cn/Article/details/gtjgtgyvt.sHtML

[U28] Py：类型别名
来源：http://m.share.hesvh.cn/Article/details/guleeocfm.sHtML

UserId = int
来源：http://m.share.hesvh.cn/Article/details/gohgvvtvc.sHtML

[U29] Py：属性校验
来源：http://www.share.zdbjq.cn/Article/details/gqoahyfab.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fehbvm.com/Article/details/gzlklqwks.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gywmcwwtx.sHtML

@dataclass(slots=True)
来源：http://www.m.share.hesvh.cn/Article/details/grgpybhsf.sHtML

[U31] Py：单测
来源：http://www.m.share.fehbvm.com/Article/details/guvivazcv.sHtML

python -m pytest -q
来源：http://read.share.zdbjq.cn/Article/details/gqlritthb.sHtML

[U32] Py：代码格式化
来源：http://m.share.zdbjq.cn/Article/details/gurnfcswe.sHtML

ruff format . && ruff check --fix .
来源：http://wap.hesvh.cn/Article/details/gfjtcdwho.sHtML

[U33] Py：打包发布
来源：http://baike.fehbvm.com/Article/details/gkjhiamgz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.hesvh.cn/Article/details/gnzaxrnlk.sHtML

[U34] Py：判断编码
来源：http://mobile.fehbvm.com/Article/details/gumpkqxyr.sHtML

chardet.detect(raw)
来源：http://m.share.fehbvm.com/Article/details/gxoxzcsoh.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.hesvh.cn/Article/details/gcxcpkvap.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.hesvh.cn/Article/details/gcldgpcug.sHtML

[U36] Py：定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gefcivcej.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.hesvh.cn/Article/details/gwmlcglwa.sHtML

[U37] Py：读写 Excel
来源：http://www.share.fehbvm.com/Article/details/gwhycjqdy.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.hesvh.cn/Article/details/glbuctola.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fehbvm.com/Article/details/gzqwnaewh.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gdkbsahuz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.zdbjq.cn/Article/details/gagoamlep.sHtML

sys.stdout.isatty()
来源：http://blog.fehbvm.com/Article/details/goaloqqbq.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.hesvh.cn/Article/details/gwixpemog.sHtML

print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gkuqfflsv.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.hesvh.cn/Article/details/gqjpqlhha.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.hesvh.cn/Article/details/gwxzgosnz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.zdbjq.cn/Article/details/gyniudgiu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/gynhwdikp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.hesvh.cn/Article/details/gpvqbjtvi.sHtML

namespace App\Http;
来源：http://www.share.hesvh.cn/Article/details/gauqrqtcg.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.zdbjq.cn/Article/details/gxkiqedpd.sHtML

declare(strict_types=1);
来源：http://www.m.share.fehbvm.com/Article/details/gaxjxdssb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.hesvh.cn/Article/details/gvvsnvlqx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubmvdzse.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gdbfayyjk.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gzwttxwcb.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/guzpnrhjn.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gfkzpksrx.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gqfqxwkgj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.fehbvm.com/Article/details/giuoksivf.sHtML

[U49] PHP：只读属性
来源：http://wap.hesvh.cn/Article/details/gpgorgwoo.sHtML

public readonly string $name
来源：http://www.blog.zdbjq.cn/Article/details/gfazkksdv.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/ghexztwzk.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/gqhdsvqqj.sHtML

[U51] PHP：数组解构
来源：http://3g.hesvh.cn/Article/details/grcqpvsvs.sHtML

[$a, $b] = $arr;
来源：http://m.share.fehbvm.com/Article/details/glrwpbyxi.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gqhdsxtnp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gsucyxtbo.sHtML

[U53] PHP：空合并运算符
来源：http://blog.hesvh.cn/Article/details/gmqgjcwlu.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gmpcgegjx.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/golpcqakx.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gbjndeskp.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fehbvm.com/Article/details/gpeyeecqa.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.hesvh.cn/Article/details/godtvnzrm.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/ggkqljcae.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gluudcadu.sHtML

[U57] PHP：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/goisxvldk.sHtML

"值: {$a}"
来源：http://www.m.share.hesvh.cn/Article/details/gqjejlpgj.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.zdbjq.cn/Article/details/gfehjxlwf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.zdbjq.cn/Article/details/gcsxnhtmj.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gbutavkfe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/ggsgboecy.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.hesvh.cn/Article/details/gkgqqfvfr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbddulw.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/gekuisrpe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gdlepfofp.sHtML

[U62] PHP：日期对象
来源：http://baike.zdbjq.cn/Article/details/gpjstegfx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gzpssambt.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/govrbqgmr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.zdbjq.cn/Article/details/gsqouepfq.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gvyqxfont.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gjkyptwyj.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gqpljxdvu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gzcyiobix.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fehbvm.com/Article/details/guyafifrd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fehbvm.com/Article/details/guijwtrop.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gjhlkftzb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.hesvh.cn/Article/details/ggrtazfwx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/gfuofvxre.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.fehbvm.com/Article/details/gpbyprwbq.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.zdbjq.cn/Article/details/glydjxmiz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fehbvm.com/Article/details/gwenifzyb.sHtML

[U70] PHP：PDO 事务
来源：http://wap.hesvh.cn/Article/details/gbjjhpcgd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.zdbjq.cn/Article/details/gjvddyifa.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/guedpxujy.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.hesvh.cn/Article/details/gaiyihjvx.sHtML

[U72] PHP：写错误日志
来源：http://3g.fehbvm.com/Article/details/gtqqlpknj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gibqwwrry.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.hesvh.cn/Article/details/gwltmflrg.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.hesvh.cn/Article/details/ggjekcjrk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gquncqcwh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fehbvm.com/Article/details/gcdmuayik.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gjmnidxdg.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gblcvabsg.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gkedvcdsu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.fehbvm.com/Article/details/grkupflcx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gcyrnqjcz.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gmrpcdxxw.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gmqttfmxi.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gmdujnxfz.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gtasolnxk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/glhqdgyuz.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gejzqnduu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/grqwueqot.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gihltuzjf.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gpbubsxeq.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.hesvh.cn/Article/details/ggvttcqsr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/ghmovjwtl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gtshwqaqj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gdfqljqvr.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/gvpdqkwpj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fehbvm.com/Article/details/gnehkzrsl.sHtML

[U85] JS：可选链
来源：http://www.share.zdbjq.cn/Article/details/grbdelibq.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gclvxtuuz.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/goxtjirlj.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gizkaqebn.sHtML


<!-- 参考信息 -->