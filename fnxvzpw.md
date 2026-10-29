代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gkrrwxufu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggkvcusdn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gskiswmnn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gomdvxgkw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gghjfzsle.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ggofigmve.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/ghuqqyryj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gskyfmque.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gprzmdisy.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gzjmfbcfa.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gbdmtmqey.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gparfuart.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gmfgkhhzq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gtiqzfwzp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/grctulwek.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghipatkcv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/goqwdpckn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fehbvm.com/Article/details/grsyjpkjv.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gaixgiekr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gtqlhnnwc.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gwtdztgtt.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gzicpeyrz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gvoqrjvkz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/glgloeqpt.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gsvowfzlh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.hesvh.cn/Article/details/gwbdspbzo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gjazpbwhd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghqvfaxjm.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gervskbiw.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gdnskggcn.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gqctpyega.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fehbvm.com/Article/details/gtqsgutip.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gnclvknqb.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gfjhspwkq.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gdwojnwsn.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gzknvutpu.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gxkwnhrdb.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gpljdagcw.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcvuygeom.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/gwglwrnsk.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gdgeahatl.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gytucvgsu.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gwvdvugdq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gavcyefwi.sHtML

[T21] Swift：遍历
来源：http://mobile.fehbvm.com/Article/details/gfjtvyooj.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gvzrzynji.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gyxuogyax.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gvbrlzmiv.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gdaitwlyz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gwqvfiwmd.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/gknplgfix.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gxmblqehr.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gfizdllpk.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gkjfineus.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/ggprkoxtl.sHtML

class A: Base { override func f() {} }
来源：http://blog.zdbjq.cn/Article/details/gpiksuipf.sHtML

[T27] Swift：错误处理
来源：http://3g.hesvh.cn/Article/details/gjzlkhqus.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gfyhttsdt.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxkfjzyuo.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gkypuwghq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gbbdxtmbi.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gvkftbftt.sHtML

[T30] Swift：协议
来源：http://mobile.hesvh.cn/Article/details/givjohxfz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gjzfoxfnv.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/groeaeydz.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gckkrefsz.sHtML

[T32] Lua：局部变量
来源：http://m.share.fehbvm.com/Article/details/geozhjnrq.sHtML

local a = 1
来源：http://baike.hesvh.cn/Article/details/gqevauluh.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gqmahggpb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gknwcaekc.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gkatjpgku.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gnhrxxkhe.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gojusgcsa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fehbvm.com/Article/details/grugtlbrq.sHtML

[T36] Lua：函数
来源：http://wap.hesvh.cn/Article/details/ggsfjohix.sHtML

function add(a, b) return a + b end
来源：http://www.share.hesvh.cn/Article/details/gsxochiry.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gisqvyclz.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gtjgzkgao.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gvwudrqij.sHtML

if x > 0 then print("正") end
来源：http://3g.hesvh.cn/Article/details/gdufgzjjy.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/ggkwlynqn.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/gclxxbbzd.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gjnxixxrs.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gkupqwvso.sHtML

[T41] Perl：Hello World
来源：http://read.share.fehbvm.com/Article/details/ggrawarnl.sHtML

print "Hello\n";
来源：http://baike.hesvh.cn/Article/details/gfplmlzxl.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/glgtuzzty.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/guvmmyubh.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gtuqzypte.sHtML

"值: $a"
来源：http://mobile.fehbvm.com/Article/details/gyvykdpov.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/guvdkeeud.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.zdbjq.cn/Article/details/gbyxwrhzb.sHtML

[T45] Perl：数组遍历
来源：http://read.share.fehbvm.com/Article/details/gzbnhhkzq.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbiwswfaf.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gwomsgzec.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fehbvm.com/Article/details/gputemlgn.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gwpgzejmz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fehbvm.com/Article/details/gucbwgbvy.sHtML

[T48] Perl：正则替换
来源：http://www.share.zdbjq.cn/Article/details/genyehrci.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gyqniqhct.sHtML

[T49] Perl：函数
来源：http://www.m.share.hesvh.cn/Article/details/gkdtqslzt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/golpvtyvy.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gujasauuo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.hesvh.cn/Article/details/gluhtfvbk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gclgjmsny.sHtML

[T51] Scala：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gkjahpxnc.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gbeqhdnvf.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gjxfekunj.sHtML

val a = 1;  var b = 2
来源：http://www.blog.fehbvm.com/Article/details/gzjiffigd.sHtML

[T53] Scala：字符串插值
来源：http://3g.zdbjq.cn/Article/details/grlsjlgwa.sHtML

s"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gitfncwti.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/gjirbixyb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/guttrafuu.sHtML

[T55] Scala：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gtkngbzxx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gstavhpqn.sHtML

[T56] Scala：样例类
来源：http://www.blog.hesvh.cn/Article/details/guydcwilm.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnrfjhrh.sHtML

[T57] Scala：模式匹配
来源：http://baike.fehbvm.com/Article/details/gipvlunws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gmvzechhb.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fehbvm.com/Article/details/gtakgmlfy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gqqzalzow.sHtML

[T59] Scala：循环
来源：http://www.blog.zdbjq.cn/Article/details/gyqwxjejq.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gayjorazd.sHtML

[T60] Scala：折叠
来源：http://wap.zdbjq.cn/Article/details/gdwkfjzak.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.hesvh.cn/Article/details/gmgbryfup.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gptvgrgqt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/galfztkpy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grwzksnim.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.hesvh.cn/Article/details/gzkcptoyi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.fehbvm.com/Article/details/gqjbkqczx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.zdbjq.cn/Article/details/ghtlvbwgi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkupsxgjw.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.zdbjq.cn/Article/details/gvrwuoryr.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.hesvh.cn/Article/details/gknarfbin.sHtML

[U04] Py：变量调试打印
来源：http://mobile.zdbjq.cn/Article/details/gxrgqrekx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.hesvh.cn/Article/details/gkzluycxy.sHtML

[U05] Py：列表去重且保序
来源：http://wap.zdbjq.cn/Article/details/ggubgkamp.sHtML

list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gntxusrmw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.zdbjq.cn/Article/details/gvmyzgpya.sHtML

{**a, **b}
来源：http://baike.hesvh.cn/Article/details/gapduitvr.sHtML

[U07] Py：反转字典键值
来源：http://blog.hesvh.cn/Article/details/gkkiglaqk.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fehbvm.com/Article/details/goyzfqvax.sHtML

[U08] Py：展平二维列表
来源：http://blog.zdbjq.cn/Article/details/gfrmoibvb.sHtML

[y for x in nested for y in x]
来源：http://read.share.zdbjq.cn/Article/details/gswzpdjjj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fehbvm.com/Article/details/gzmhriirc.sHtML

max(d, key=d.get)
来源：http://3g.fehbvm.com/Article/details/gecsqhjqb.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.fehbvm.com/Article/details/gopxelapc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.hesvh.cn/Article/details/gfmufxepw.sHtML

[U11] Py：生成器表达式
来源：http://3g.hesvh.cn/Article/details/geagepswr.sHtML

(x * 2 for x in arr)
来源：http://m.share.zdbjq.cn/Article/details/gafhhriaj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gzrsncowj.sHtML

Counter(arr).most_common(3)
来源：http://mobile.zdbjq.cn/Article/details/guyupsajh.sHtML

[U13] Py：固定长度队列
来源：http://baike.zdbjq.cn/Article/details/gwgmjmpmp.sHtML

deque(maxlen=10)
来源：http://wap.zdbjq.cn/Article/details/gazolmodp.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.hesvh.cn/Article/details/ggeropkxi.sHtML

defaultdict(list)
来源：http://www.blog.fehbvm.com/Article/details/gwlraovzd.sHtML

[U15] Py：高精度计时
来源：http://wap.hesvh.cn/Article/details/gbjbnzcgt.sHtML

t = time.perf_counter()
来源：http://read.share.hesvh.cn/Article/details/gasnaoqfk.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fehbvm.com/Article/details/gsqojxqau.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.hesvh.cn/Article/details/gxdqtygkb.sHtML

[U17] Py：初始化日志
来源：http://www.share.zdbjq.cn/Article/details/gbjlijspt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.hesvh.cn/Article/details/ghcatqtcj.sHtML

[U18] Py：预编译正则
来源：http://baike.zdbjq.cn/Article/details/gbtkbflhx.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fehbvm.com/Article/details/gcdoaxvdj.sHtML

[U19] Py：正则替换带回调
来源：http://3g.fehbvm.com/Article/details/gvdspefii.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.fehbvm.com/Article/details/gurhlgozr.sHtML

[U20] Py：缓存函数结果
来源：http://blog.hesvh.cn/Article/details/ghupwlygi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fehbvm.com/Article/details/gkwkatecn.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.hesvh.cn/Article/details/gjsflvqgt.sHtML

@contextlib.contextmanager
来源：http://mobile.zdbjq.cn/Article/details/grdicqrjo.sHtML

[U22] Py：矩阵转置
来源：http://blog.zdbjq.cn/Article/details/ghxnkyike.sHtML

list(zip(*m))
来源：http://mobile.fehbvm.com/Article/details/gyhntwjyv.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gugejzhbd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.hesvh.cn/Article/details/gquzebbaz.sHtML

[U24] Py：路径操作
来源：http://mobile.fehbvm.com/Article/details/gnhxlylaq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gmovubxun.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fehbvm.com/Article/details/geszmsarr.sHtML

csv.DictReader(f)
来源：http://read.share.hesvh.cn/Article/details/gpuwwhbpe.sHtML

[U26] Py：并发下载
来源：http://wap.zdbjq.cn/Article/details/gaohltrqw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fehbvm.com/Article/details/grqupplvw.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.zdbjq.cn/Article/details/gghpumbcf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.zdbjq.cn/Article/details/gitcsvvdw.sHtML

[U28] Py：类型别名
来源：http://wap.fehbvm.com/Article/details/gwmaqltss.sHtML

UserId = int
来源：http://www.m.share.fehbvm.com/Article/details/gdcclelvu.sHtML

[U29] Py：属性校验
来源：http://wap.hesvh.cn/Article/details/gfgcpxjdq.sHtML

@property 与 @x.setter 配合
来源：http://blog.zdbjq.cn/Article/details/gnkldeqnr.sHtML

[U30] Py：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gdurtblji.sHtML

@dataclass(slots=True)
来源：http://3g.hesvh.cn/Article/details/gvdjvxxdu.sHtML

[U31] Py：单测
来源：http://wap.hesvh.cn/Article/details/grukokcbi.sHtML

python -m pytest -q
来源：http://3g.fehbvm.com/Article/details/gcxikiydk.sHtML

[U32] Py：代码格式化
来源：http://read.share.fehbvm.com/Article/details/gjgrexpov.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.zdbjq.cn/Article/details/gmrlvpbji.sHtML

[U33] Py：打包发布
来源：http://www.blog.hesvh.cn/Article/details/gubggenha.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.zdbjq.cn/Article/details/gnslsznbi.sHtML

[U34] Py：判断编码
来源：http://m.share.zdbjq.cn/Article/details/gborxeqoe.sHtML

chardet.detect(raw)
来源：http://read.share.fehbvm.com/Article/details/goxhjbgdr.sHtML

[U35] Py：发送邮件
来源：http://m.share.hesvh.cn/Article/details/gpiwcldpb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/ghcgdbglw.sHtML

[U36] Py：定时任务
来源：http://wap.hesvh.cn/Article/details/glonulyxh.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.hesvh.cn/Article/details/ghuxktesp.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.zdbjq.cn/Article/details/girsvtfkz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.fehbvm.com/Article/details/gddcmsnth.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.fehbvm.com/Article/details/gcnlwwtgp.sHtML

Path(__file__).resolve().parent
来源：http://read.share.fehbvm.com/Article/details/gythlsnnb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.hesvh.cn/Article/details/gmdmmdjbj.sHtML

sys.stdout.isatty()
来源：http://baike.zdbjq.cn/Article/details/gozqskogs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.hesvh.cn/Article/details/gkawkznvj.sHtML

print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gujkcesxz.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fehbvm.com/Article/details/gelzlfqad.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.zdbjq.cn/Article/details/giemnouhz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fehbvm.com/Article/details/gwqefxfvm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqcsnjfp.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.zdbjq.cn/Article/details/ggnomogif.sHtML

namespace App\Http;
来源：http://blog.fehbvm.com/Article/details/gtmzivnfz.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.zdbjq.cn/Article/details/gdxaeqlrp.sHtML

declare(strict_types=1);
来源：http://read.share.fehbvm.com/Article/details/gwwbvyrid.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/gspxdaoqt.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/grxlgbroz.sHtML

[U46] PHP：可空类型
来源：http://www.blog.zdbjq.cn/Article/details/ggpjluawa.sHtML

?string $name = null
来源：http://mobile.zdbjq.cn/Article/details/gnmrpdafd.sHtML

[U47] PHP：联合类型
来源：http://read.share.hesvh.cn/Article/details/ghathlpmr.sHtML

int|string $id
来源：http://www.blog.hesvh.cn/Article/details/gzofklxod.sHtML

[U48] PHP：纯枚举
来源：http://m.share.zdbjq.cn/Article/details/gyfymuhlu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gchduzjln.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gqmwicgjb.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gibslqbuu.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gwexudedo.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geuuczelr.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gotlkcqtw.sHtML

[$a, $b] = $arr;
来源：http://baike.hesvh.cn/Article/details/gmqzfxjcb.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gglmthxzx.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gjjjivcaw.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/ghllyxqta.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/ggyaaigpd.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gzergynyb.sHtML

$obj?->method()
来源：http://read.share.fehbvm.com/Article/details/gsipmwhrb.sHtML

[U55] PHP：match 表达式
来源：http://3g.fehbvm.com/Article/details/gawhzorpe.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gsypqdlmr.sHtML

[U56] PHP：命名参数
来源：http://www.share.fehbvm.com/Article/details/gakzazzeh.sHtML

f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gebpppexm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gulajbruy.sHtML

"值: {$a}"
来源：http://blog.zdbjq.cn/Article/details/gthexpjiz.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fehbvm.com/Article/details/goshhmust.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.hesvh.cn/Article/details/gwwlqkvwn.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gdtzybbdd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/guucysssc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fehbvm.com/Article/details/gsfduunbb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gdftkclib.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gkptwygjw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gydzgufjk.sHtML

[U62] PHP：日期对象
来源：http://wap.hesvh.cn/Article/details/gpfrcjcmi.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fehbvm.com/Article/details/gwjgybynd.sHtML

[U63] PHP：文件读写
来源：http://baike.hesvh.cn/Article/details/girgrnszc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.zdbjq.cn/Article/details/gjwutwrvf.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fehbvm.com/Article/details/gbywlrrgp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/grzchjqxi.sHtML

[U65] PHP：会话
来源：http://www.blog.hesvh.cn/Article/details/gpzmoziod.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gmpluveqp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fehbvm.com/Article/details/gtqgbegsw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.hesvh.cn/Article/details/gyotsssur.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.zdbjq.cn/Article/details/gppxbenpe.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.zdbjq.cn/Article/details/gwhkklobx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.hesvh.cn/Article/details/gtwczqxwd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.hesvh.cn/Article/details/gqxcqvshh.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gnzbyekvg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fehbvm.com/Article/details/gochwrsyn.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/gvgrekzvn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.hesvh.cn/Article/details/gxilfpeky.sHtML

[U71] PHP：抛出异常
来源：http://m.share.fehbvm.com/Article/details/gylkcbyxk.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gbvucilfk.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/ggquucnln.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.zdbjq.cn/Article/details/gkyzlygcr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gvjbtmxtw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fehbvm.com/Article/details/gzdyuygfx.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gtjvwghiz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.zdbjq.cn/Article/details/gemvjhpgv.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gfdbpsixz.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gqwenecaj.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxjiiquhe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/goptandod.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fehbvm.com/Article/details/ginpmsric.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gsuidxrik.sHtML

[U78] PHP：单元测试
来源：http://wap.hesvh.cn/Article/details/gvxtuzcdd.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.hesvh.cn/Article/details/gkhchwxpd.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gyvamrwoc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gksbxbwwl.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gmlmdegvl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/geymwddxd.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/glfqlbety.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gwmowlgtf.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/ggofvoryz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gcamhwbfz.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/ggulluaic.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gmomqgbrz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/gwzzuoptt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/geulfamme.sHtML

[U85] JS：可选链
来源：http://baike.hesvh.cn/Article/details/gqnmpuvuo.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gmcvafrih.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gaqmsqnpn.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/ghliarezw.sHtML


<!-- 参考信息 -->