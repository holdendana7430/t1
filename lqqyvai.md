代发 wailian999

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/grqphveus.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gkubrweaw.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gegznhgyt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/ginraximm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gitrhpeqi.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gipvzjkwh.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/ghjwtjslo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gjuyhlgcl.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gzacgctos.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/gqprtopcg.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gsmymqjeo.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gvbtpfkxn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/galumbsxq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gbedmoebi.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gliixnhfv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gwoygrwyl.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gciicwjta.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/ggxkmmqag.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gifbapwup.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gfqurkzld.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gxrqboafv.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gfihofeoi.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gfrwvztkc.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/ghkqgnxic.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gyzouewkv.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/glnzlezeb.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxwzlsrna.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/getpazlvq.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gibpyuioh.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gkrpvfiqg.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/giikzxbti.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gjurqsjyp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/ggxzfclla.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gcxhguczw.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gipmohwoe.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gnhtqxagf.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gpvanlrkw.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/glbfmwndh.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/geegutpso.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fehbvm.com/Article/details/gtbqhfivn.sHtML

[T23] Swift：函数
来源：http://m.share.fehbvm.com/Article/details/gshlfmbxu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/giyvpawie.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gmtsjxctp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpdgdfvag.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/ggodytxnp.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/goqcjbtuq.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gabxyklsq.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gxcipcdow.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/grjvgsklc.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gldgfsikg.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gyfwchxme.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gzsozbccu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.hesvh.cn/Article/details/gjudnbhlj.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gqedhfxes.sHtML

[T30] Swift：协议
来源：http://www.blog.hesvh.cn/Article/details/gzcorntbo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gfldlnrig.sHtML

[T31] Lua：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfoosobcn.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvzjnjowu.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gyhatxyki.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gkbwrgmyo.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gmpgfavxl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/ghswupcut.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gofsjjlnl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fehbvm.com/Article/details/gnhvzqrmh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gxodafoid.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.hesvh.cn/Article/details/gyvufkquv.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/gbrtlbkcn.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gifubseve.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gkjwgwiuc.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gqinfvytt.sHtML

[T38] Lua：条件
来源：http://www.blog.fehbvm.com/Article/details/gvdefnslf.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gbubjezfd.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gjrbrjcvy.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/guwvgmusa.sHtML

[T40] Lua：元表
来源：http://blog.hesvh.cn/Article/details/ghhautegd.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.hesvh.cn/Article/details/gvxyquxcd.sHtML

[T41] Perl：Hello World
来源：http://baike.fehbvm.com/Article/details/gwehgvhnf.sHtML

print "Hello\n";
来源：http://mobile.hesvh.cn/Article/details/gzpgecrwd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/glyxyoivu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.zdbjq.cn/Article/details/gbmdffppz.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gwatfownk.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gsugyuhdk.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/glhoujcbi.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gdiwchlhh.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gsgljlcbk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/glhpoqfus.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/goyzgmntq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gpnbgsslf.sHtML

[T47] Perl：正则捕获
来源：http://m.share.hesvh.cn/Article/details/gmlxnmnln.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gxshhvyev.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gatbiwbdy.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.hesvh.cn/Article/details/gjzymfilr.sHtML

[T49] Perl：函数
来源：http://www.blog.hesvh.cn/Article/details/gpsfkfaas.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggmvfubkl.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvaxvitwi.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fehbvm.com/Article/details/gecvthmgh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gbieyrlad.sHtML

[T51] Scala：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjovkyvoi.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gnwnmnjww.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gwgekzkmm.sHtML

val a = 1;  var b = 2
来源：http://read.share.fehbvm.com/Article/details/gtsneoiol.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gisnltsai.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/genlfqyfu.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/goxegpdeb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyijddo.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gsolycezz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gqbudplgk.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gkaoxybuj.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gusosqiaf.sHtML

[T57] Scala：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gdecozfll.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fehbvm.com/Article/details/gwqmoseqi.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gbmnmpllk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gmxytctwe.sHtML

[T59] Scala：循环
来源：http://www.blog.fehbvm.com/Article/details/gwsckwwqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gukzkvdqq.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gkdyvkyrj.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.fehbvm.com/Article/details/gmjxcmbnj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwnzlwtgq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gmhpennrw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaycqtsnl.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.zdbjq.cn/Article/details/gzmsprjew.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.hesvh.cn/Article/details/gyurymlag.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.hesvh.cn/Article/details/gydojvmds.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.hesvh.cn/Article/details/gyrngrkhr.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.zdbjq.cn/Article/details/gjxhijdrd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.fehbvm.com/Article/details/grmpnhkeb.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fehbvm.com/Article/details/gnjnztrgl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.hesvh.cn/Article/details/grwbxtbgd.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fehbvm.com/Article/details/gicdtimok.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gzlmbregw.sHtML

[U06] Py：合并两个字典
来源：http://m.share.hesvh.cn/Article/details/gsduxbsfm.sHtML

{**a, **b}
来源：http://3g.fehbvm.com/Article/details/gobakylig.sHtML

[U07] Py：反转字典键值
来源：http://m.share.zdbjq.cn/Article/details/gwxcnkjpt.sHtML

{v: k for k, v in d.items()}
来源：http://wap.hesvh.cn/Article/details/gnukvlcgm.sHtML

[U08] Py：展平二维列表
来源：http://3g.zdbjq.cn/Article/details/gjujlbefu.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/gzprzxosi.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.zdbjq.cn/Article/details/ghfxcruht.sHtML

max(d, key=d.get)
来源：http://baike.fehbvm.com/Article/details/ggcmpmbza.sHtML

[U10] Py：按值排序字典
来源：http://wap.hesvh.cn/Article/details/gkjapzucs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.fehbvm.com/Article/details/gxbwymjcv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.fehbvm.com/Article/details/gsmqinhsy.sHtML

(x * 2 for x in arr)
来源：http://blog.hesvh.cn/Article/details/gmnfpqned.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.zdbjq.cn/Article/details/geydajnij.sHtML

Counter(arr).most_common(3)
来源：http://baike.fehbvm.com/Article/details/gelispjkc.sHtML

[U13] Py：固定长度队列
来源：http://read.share.fehbvm.com/Article/details/gxqwvvryv.sHtML

deque(maxlen=10)
来源：http://baike.zdbjq.cn/Article/details/gmenlqyxq.sHtML

[U14] Py：分组收集到列表
来源：http://3g.fehbvm.com/Article/details/gqzsmkiyo.sHtML

defaultdict(list)
来源：http://wap.hesvh.cn/Article/details/gbruidgen.sHtML

[U15] Py：高精度计时
来源：http://www.share.hesvh.cn/Article/details/gdavmkaww.sHtML

t = time.perf_counter()
来源：http://m.share.fehbvm.com/Article/details/gfjaxnaku.sHtML

[U16] Py：命令行参数解析
来源：http://blog.fehbvm.com/Article/details/gpbvjmlpd.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.hesvh.cn/Article/details/gunzzczxm.sHtML

[U17] Py：初始化日志
来源：http://3g.zdbjq.cn/Article/details/gnsrkqdye.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fehbvm.com/Article/details/grpkfnkbv.sHtML

[U18] Py：预编译正则
来源：http://baike.hesvh.cn/Article/details/grosegzvt.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gjwdtjmgm.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.fehbvm.com/Article/details/gopzhvdgm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.hesvh.cn/Article/details/gtcqgjzuz.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.zdbjq.cn/Article/details/gyysfjhgu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.zdbjq.cn/Article/details/govxumaod.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.fehbvm.com/Article/details/ggdrmntkq.sHtML

@contextlib.contextmanager
来源：http://m.share.zdbjq.cn/Article/details/glphnbagr.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.zdbjq.cn/Article/details/gogdbspeo.sHtML

list(zip(*m))
来源：http://read.share.hesvh.cn/Article/details/gvxelartc.sHtML

[U23] Py：分块读取大文件
来源：http://wap.fehbvm.com/Article/details/gdabngnvy.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://baike.zdbjq.cn/Article/details/gvrkzxjrc.sHtML

[U24] Py：路径操作
来源：http://m.share.fehbvm.com/Article/details/gyrvggdvv.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gufjjxoqi.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.hesvh.cn/Article/details/gwecchrmi.sHtML

csv.DictReader(f)
来源：http://mobile.zdbjq.cn/Article/details/gxpgdfvqd.sHtML

[U26] Py：并发下载
来源：http://blog.zdbjq.cn/Article/details/gbfvjwcuw.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.fehbvm.com/Article/details/gawsqzsvs.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fehbvm.com/Article/details/gszqcrpmh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.fehbvm.com/Article/details/glnjsuapy.sHtML

[U28] Py：类型别名
来源：http://www.share.zdbjq.cn/Article/details/gwjanlcdv.sHtML

UserId = int
来源：http://www.share.hesvh.cn/Article/details/gylrrmwcp.sHtML

[U29] Py：属性校验
来源：http://baike.fehbvm.com/Article/details/gtsevqflz.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.zdbjq.cn/Article/details/gjioxernr.sHtML

[U30] Py：数据类
来源：http://mobile.hesvh.cn/Article/details/gekxcmijj.sHtML

@dataclass(slots=True)
来源：http://m.share.zdbjq.cn/Article/details/ghugjmzxy.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/gbozifvvk.sHtML

python -m pytest -q
来源：http://mobile.fehbvm.com/Article/details/guagpgarn.sHtML

[U32] Py：代码格式化
来源：http://blog.zdbjq.cn/Article/details/gonviwmjl.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.zdbjq.cn/Article/details/gslibaoef.sHtML

[U33] Py：打包发布
来源：http://mobile.hesvh.cn/Article/details/gxzieoyhb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.hesvh.cn/Article/details/ghaydlwhf.sHtML

[U34] Py：判断编码
来源：http://wap.zdbjq.cn/Article/details/gnzgkmfjs.sHtML

chardet.detect(raw)
来源：http://3g.zdbjq.cn/Article/details/gbgkgvltf.sHtML

[U35] Py：发送邮件
来源：http://www.share.zdbjq.cn/Article/details/gxwtjhmku.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.hesvh.cn/Article/details/gdkrksubc.sHtML

[U36] Py：定时任务
来源：http://baike.fehbvm.com/Article/details/gnsnzlrxm.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fehbvm.com/Article/details/gabbqjmko.sHtML

[U37] Py：读写 Excel
来源：http://3g.fehbvm.com/Article/details/glqcntyjd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.zdbjq.cn/Article/details/guusbwomc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gwnhrhvkp.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fehbvm.com/Article/details/gmntwsfjb.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.hesvh.cn/Article/details/ghfgswkjc.sHtML

sys.stdout.isatty()
来源：http://wap.zdbjq.cn/Article/details/gufniaenn.sHtML

[U40] Py：打印到标准错误
来源：http://baike.zdbjq.cn/Article/details/gebxchlpj.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/ggvuhrpzd.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.hesvh.cn/Article/details/gksgdgjms.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.fehbvm.com/Article/details/gruzpbbig.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fehbvm.com/Article/details/gkckyffor.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gzygdgovk.sHtML

[U43] PHP：声明命名空间
来源：http://wap.fehbvm.com/Article/details/guoqpnobs.sHtML

namespace App\Http;
来源：http://www.blog.hesvh.cn/Article/details/garvldoop.sHtML

[U44] PHP：开启严格类型
来源：http://baike.hesvh.cn/Article/details/ggohdldba.sHtML

declare(strict_types=1);
来源：http://3g.hesvh.cn/Article/details/gkbthcvlz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.zdbjq.cn/Article/details/gaboilhkn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/grzchbzic.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/glahelcwg.sHtML

?string $name = null
来源：http://baike.zdbjq.cn/Article/details/gqgjshfdh.sHtML

[U47] PHP：联合类型
来源：http://blog.hesvh.cn/Article/details/ghshdhwns.sHtML

int|string $id
来源：http://wap.zdbjq.cn/Article/details/gwnncgnrc.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gwaqjowtl.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gurtyztio.sHtML

[U49] PHP：只读属性
来源：http://mobile.hesvh.cn/Article/details/glodznksl.sHtML

public readonly string $name
来源：http://3g.fehbvm.com/Article/details/grbqhuady.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.zdbjq.cn/Article/details/gklbjxyru.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/ghkoaccqd.sHtML

[U51] PHP：数组解构
来源：http://m.share.zdbjq.cn/Article/details/gtsfmdxre.sHtML

[$a, $b] = $arr;
来源：http://wap.hesvh.cn/Article/details/gqsspklub.sHtML

[U52] PHP：箭头函数
来源：http://3g.zdbjq.cn/Article/details/grdumyawx.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.zdbjq.cn/Article/details/gqhykukse.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/gigpgdics.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.hesvh.cn/Article/details/gkyrzszmf.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/ginnmkwyi.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/guapvnzlp.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnidngxfg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gqskcqoia.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gwimvkzph.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gbpimpsgw.sHtML

[U57] PHP：字符串插值
来源：http://blog.fehbvm.com/Article/details/gcxrmuuwx.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gahrwevyb.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gwgomsfvd.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gcnbkqlcf.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gqegrwjeu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gzvfuepyl.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.fehbvm.com/Article/details/goytvawfr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/gdbyeuwxr.sHtML

[U61] PHP：正则
来源：http://www.share.hesvh.cn/Article/details/gleiepiri.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/ggexdajvn.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gtswuzktk.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.hesvh.cn/Article/details/gqlfxyusp.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gvlafrrcz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gipwzzvci.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gwzsatrpm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gouufizas.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/gufcdvcpc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.hesvh.cn/Article/details/gssqgspmz.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.hesvh.cn/Article/details/gywlyatwo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gahgcgdem.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gfdtukqjw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/gkgzsfjnz.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fehbvm.com/Article/details/ggzqmembh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/guplobhyo.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/garpvtsyq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/guplkjyep.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gbwxqtbpg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gpaphsmlf.sHtML

[U71] PHP：抛出异常
来源：http://baike.zdbjq.cn/Article/details/gvwogdmwb.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.zdbjq.cn/Article/details/glsomuqpt.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gpostoopg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/ghsqcqhgs.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.zdbjq.cn/Article/details/gnjqxlpzs.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fehbvm.com/Article/details/gvvdzsyer.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gxmnsiwvp.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fehbvm.com/Article/details/gpllsvfmc.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gzgjdvjzj.sHtML

composer require psr/container
来源：http://m.share.fehbvm.com/Article/details/ghswxcyjv.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gzkfdezio.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gtnwfeetm.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/ghhyyccld.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gcduzsjnj.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/geutczzff.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/gxqzpxzpg.sHtML

[U79] PHP：静态分析
来源：http://blog.hesvh.cn/Article/details/gqdxoctjh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gdipdxrqe.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/gmuwkrlrj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/gvalnwcyl.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gbaksglkc.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gwobssvkk.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gpuimpjar.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fehbvm.com/Article/details/ggvbgxizq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gthvglixw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/ghdzsgxyl.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/goinjzibg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.hesvh.cn/Article/details/gdgthhrwl.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gbofndepg.sHtML

a?.b?.c
来源：http://mobile.zdbjq.cn/Article/details/goqtkemop.sHtML

[U86] JS：空值合并
来源：http://read.share.fehbvm.com/Article/details/gfadkyota.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gjfvownzi.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/gpadllhvm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/gyhaxcltx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gvuhoizlh.sHtML

{ ...a, ...b }
来源：http://mobile.zdbjq.cn/Article/details/gywjlssap.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gmjepwkjx.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gbspfmjwt.sHtML

[U90] JS：数字数组排序
来源：http://mobile.hesvh.cn/Article/details/gsqoxjbjg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gxppbbxmj.sHtML


<!-- 参考信息 -->