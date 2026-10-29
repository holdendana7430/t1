代发 wailian999

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gpnufdqne.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gklqhjcnu.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gxkhbxeqn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gqfddtmax.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gldcpehdz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gilfkiuhs.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/grxlgeuvg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqmzxqljd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gyvlyhwsq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gsnzbcwhx.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gssbkzcvc.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gtanmeezq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gnwcisiou.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/gnxhwngfm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ghuperewp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gqwhzhusy.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gplifnryl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/ghvyyziec.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gzteqbdgz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcrbcghh.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gyjohefhh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gdrcwfgvk.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/groldgudz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gwccctyku.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gbbuqlvaz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gjcjijcwg.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/grkpxbdue.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcsyiwzna.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gxnecpqhh.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gionccpzc.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gwglkquyb.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gkittfthz.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/goddnduco.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gozeyzdlh.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gmvzypdum.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fehbvm.com/Article/details/gtudcdcci.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/grpeafnav.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/gjsufsmfk.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ggffwnwuv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/gnezuhlwj.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/grlpwhsdo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gyyaoechc.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gkvmvrjfn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gnpkbhwji.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/glnepwlpr.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gslonxnuv.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gucygwcki.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gyftbjvbz.sHtML

[T27] Swift：错误处理
来源：http://baike.hesvh.cn/Article/details/guatgucyx.sHtML

do { try f() } catch { print(error) }
来源：http://3g.zdbjq.cn/Article/details/gvfplgbcg.sHtML

[T28] Swift：枚举
来源：http://read.share.fehbvm.com/Article/details/gtfluywbs.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gxwlyrzsz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ghbfhwibq.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/geqcygrrc.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gnkwztaeb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/gpkekgjqs.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/geidkeuye.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gvwmranyg.sHtML

[T32] Lua：局部变量
来源：http://baike.hesvh.cn/Article/details/gcjufebsn.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/glmlycihs.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fehbvm.com/Article/details/gtqjnupgv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gdmyqwfms.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/gonzeiviq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gqrlxnzbt.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/grpcksbsw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gujorgawd.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gaslerfhh.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/gvifzrwve.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gjwgrodro.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/ggutpzpgo.sHtML

[T38] Lua：条件
来源：http://read.share.zdbjq.cn/Article/details/gkokdlqrm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.hesvh.cn/Article/details/gdwhapnam.sHtML

[T39] Lua：模式匹配
来源：http://baike.fehbvm.com/Article/details/grypuzeyi.sHtML

string.find(s, "%d+")
来源：http://3g.zdbjq.cn/Article/details/gtkdiftys.sHtML

[T40] Lua：元表
来源：http://read.share.zdbjq.cn/Article/details/gcyxspelx.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/ghqjeauhv.sHtML

[T41] Perl：Hello World
来源：http://blog.hesvh.cn/Article/details/ghfjslzcd.sHtML

print "Hello\n";
来源：http://mobile.zdbjq.cn/Article/details/gikpsgtbf.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gmaywttpt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gwtcqnjxf.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/guflzqeqi.sHtML

"值: $a"
来源：http://m.share.fehbvm.com/Article/details/guauvuppq.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gzrxlbplb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghmneavvi.sHtML

[T45] Perl：数组遍历
来源：http://m.share.zdbjq.cn/Article/details/gamnwdnjw.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.zdbjq.cn/Article/details/gneqiolff.sHtML

[T46] Perl：哈希操作
来源：http://3g.fehbvm.com/Article/details/gzbcyjlct.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.hesvh.cn/Article/details/gvqrffszr.sHtML

[T47] Perl：正则捕获
来源：http://mobile.zdbjq.cn/Article/details/gtzdlnfqo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjghsuagl.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ggclrwwkm.sHtML

$s =~ s/old/new/g;
来源：http://blog.fehbvm.com/Article/details/ggdfmvcnd.sHtML

[T49] Perl：函数
来源：http://www.m.share.fehbvm.com/Article/details/gsvcbvdch.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gqhkjmnyp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqnslcibo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gociwozkd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.hesvh.cn/Article/details/gxpzmtpfh.sHtML

[T51] Scala：Hello World
来源：http://wap.zdbjq.cn/Article/details/gfqolkgen.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gylxyxrxc.sHtML

[T52] Scala：变量
来源：http://3g.fehbvm.com/Article/details/gkzeokjyx.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gmczngjdt.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gheshvqmt.sHtML

s"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gtjbuxqwg.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gzbyvenqg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/geqlleyyk.sHtML

[T55] Scala：集合过滤
来源：http://blog.fehbvm.com/Article/details/gazombwvf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/ganhcgmxc.sHtML

[T56] Scala：样例类
来源：http://3g.hesvh.cn/Article/details/ghruzqvsd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.hesvh.cn/Article/details/gufvqvjcg.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fehbvm.com/Article/details/gnkvuvxds.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.hesvh.cn/Article/details/gqlfwpfxo.sHtML

[T58] Scala：函数定义
来源：http://www.blog.zdbjq.cn/Article/details/gwqgrrntr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.zdbjq.cn/Article/details/gadmtdtmb.sHtML

[T59] Scala：循环
来源：http://mobile.zdbjq.cn/Article/details/gfguuowjy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjfcthh.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/ghmwbyckz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.hesvh.cn/Article/details/gyhyvlgdz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgmlfgth.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gytzvsomn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghmoeudmo.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.hesvh.cn/Article/details/gfmkbbznf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fehbvm.com/Article/details/glrzbvhgf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.zdbjq.cn/Article/details/gqfpqfhtk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.zdbjq.cn/Article/details/glyqttqec.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.zdbjq.cn/Article/details/gmtvhmlwd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.hesvh.cn/Article/details/gougycuak.sHtML

[U04] Py：变量调试打印
来源：http://3g.fehbvm.com/Article/details/gcfgjpmvr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fehbvm.com/Article/details/guedsffgn.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.hesvh.cn/Article/details/gpnmoxuzm.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/grstjbipx.sHtML

[U06] Py：合并两个字典
来源：http://wap.zdbjq.cn/Article/details/gozpdlctn.sHtML

{**a, **b}
来源：http://mobile.zdbjq.cn/Article/details/gmubbjhnc.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.fehbvm.com/Article/details/gzwfdvbdi.sHtML

{v: k for k, v in d.items()}
来源：http://blog.hesvh.cn/Article/details/gphxdzlro.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.hesvh.cn/Article/details/gdtehwdxu.sHtML

[y for x in nested for y in x]
来源：http://m.share.zdbjq.cn/Article/details/grkbuaekx.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.zdbjq.cn/Article/details/ggpkprfpn.sHtML

max(d, key=d.get)
来源：http://wap.zdbjq.cn/Article/details/gngiihvpo.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.hesvh.cn/Article/details/gkcpbwrpp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.fehbvm.com/Article/details/gqmatbvcu.sHtML

[U11] Py：生成器表达式
来源：http://read.share.zdbjq.cn/Article/details/gjxokiaqo.sHtML

(x * 2 for x in arr)
来源：http://blog.zdbjq.cn/Article/details/ghynqoqld.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.zdbjq.cn/Article/details/gogxlstft.sHtML

Counter(arr).most_common(3)
来源：http://blog.zdbjq.cn/Article/details/gnxbzqlmh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.zdbjq.cn/Article/details/gkjegbkyf.sHtML

deque(maxlen=10)
来源：http://www.m.share.fehbvm.com/Article/details/gksljplcv.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.hesvh.cn/Article/details/gyoqhbjiv.sHtML

defaultdict(list)
来源：http://www.share.fehbvm.com/Article/details/gqxkisigo.sHtML

[U15] Py：高精度计时
来源：http://www.share.zdbjq.cn/Article/details/gmbbrjjtl.sHtML

t = time.perf_counter()
来源：http://blog.fehbvm.com/Article/details/gyukclmnb.sHtML

[U16] Py：命令行参数解析
来源：http://wap.hesvh.cn/Article/details/gymrflzrj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.hesvh.cn/Article/details/gestbqfzy.sHtML

[U17] Py：初始化日志
来源：http://baike.fehbvm.com/Article/details/gylcndalo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.zdbjq.cn/Article/details/gydtsuxgo.sHtML

[U18] Py：预编译正则
来源：http://3g.fehbvm.com/Article/details/gnzvbqtel.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.hesvh.cn/Article/details/grwndduaz.sHtML

[U19] Py：正则替换带回调
来源：http://wap.hesvh.cn/Article/details/gjkzeuonr.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.fehbvm.com/Article/details/gyxyknqlc.sHtML

[U20] Py：缓存函数结果
来源：http://blog.fehbvm.com/Article/details/gruavcwcg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fehbvm.com/Article/details/gooxnjzor.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.hesvh.cn/Article/details/gykmlqctw.sHtML

@contextlib.contextmanager
来源：http://3g.fehbvm.com/Article/details/giembegdd.sHtML

[U22] Py：矩阵转置
来源：http://m.share.hesvh.cn/Article/details/gaurvcevl.sHtML

list(zip(*m))
来源：http://baike.fehbvm.com/Article/details/gkpupqzzs.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fehbvm.com/Article/details/giuhoilld.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.zdbjq.cn/Article/details/gbqjegtrq.sHtML

[U24] Py：路径操作
来源：http://www.blog.fehbvm.com/Article/details/gpolfpqgn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gczgywucd.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fehbvm.com/Article/details/gnqhcvujm.sHtML

csv.DictReader(f)
来源：http://blog.fehbvm.com/Article/details/gvmilblzn.sHtML

[U26] Py：并发下载
来源：http://www.blog.fehbvm.com/Article/details/gdodstrqt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.blog.zdbjq.cn/Article/details/gqlopeuyu.sHtML

[U27] Py：异步 HTTP
来源：http://wap.zdbjq.cn/Article/details/gyqjupzqf.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.hesvh.cn/Article/details/glkhecoxe.sHtML

[U28] Py：类型别名
来源：http://www.share.fehbvm.com/Article/details/grryokdmn.sHtML

UserId = int
来源：http://www.blog.hesvh.cn/Article/details/gykcurwuw.sHtML

[U29] Py：属性校验
来源：http://blog.fehbvm.com/Article/details/glxhibqsg.sHtML

@property 与 @x.setter 配合
来源：http://read.share.hesvh.cn/Article/details/gtnhvdhct.sHtML

[U30] Py：数据类
来源：http://www.blog.fehbvm.com/Article/details/gdgatswhq.sHtML

@dataclass(slots=True)
来源：http://blog.fehbvm.com/Article/details/gmeorbtjc.sHtML

[U31] Py：单测
来源：http://3g.zdbjq.cn/Article/details/grctxbrsx.sHtML

python -m pytest -q
来源：http://read.share.fehbvm.com/Article/details/gjhgcnzol.sHtML

[U32] Py：代码格式化
来源：http://blog.fehbvm.com/Article/details/guxoihqyr.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.hesvh.cn/Article/details/gdhpakagu.sHtML

[U33] Py：打包发布
来源：http://www.m.share.fehbvm.com/Article/details/gzbmrqnif.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fehbvm.com/Article/details/gvbmkhrzo.sHtML

[U34] Py：判断编码
来源：http://blog.hesvh.cn/Article/details/ghbjtpraa.sHtML

chardet.detect(raw)
来源：http://blog.zdbjq.cn/Article/details/gvobinbel.sHtML

[U35] Py：发送邮件
来源：http://www.share.hesvh.cn/Article/details/gpwvhtibn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.hesvh.cn/Article/details/gquatmwcb.sHtML

[U36] Py：定时任务
来源：http://m.share.zdbjq.cn/Article/details/gdgzqbywj.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.fehbvm.com/Article/details/goqiwoivu.sHtML

[U37] Py：读写 Excel
来源：http://blog.fehbvm.com/Article/details/gjqmwcwdg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.hesvh.cn/Article/details/gdaanucvl.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fehbvm.com/Article/details/gsfjovies.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.zdbjq.cn/Article/details/gqueatqkb.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.hesvh.cn/Article/details/golforjag.sHtML

sys.stdout.isatty()
来源：http://read.share.fehbvm.com/Article/details/gvrflcscv.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.hesvh.cn/Article/details/gmafvnnap.sHtML

print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gflqpgesu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.zdbjq.cn/Article/details/gfroqndxl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gexuzeldd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gctzyzjxo.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.zdbjq.cn/Article/details/gqsslbyhh.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gdzcwglsz.sHtML

namespace App\Http;
来源：http://m.share.hesvh.cn/Article/details/gqqezohlc.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gkajsyigd.sHtML

declare(strict_types=1);
来源：http://www.share.zdbjq.cn/Article/details/gextrupxa.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gudhvyblv.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ggdlbfvnm.sHtML

[U46] PHP：可空类型
来源：http://www.share.fehbvm.com/Article/details/guvhhtizf.sHtML

?string $name = null
来源：http://3g.zdbjq.cn/Article/details/gqkgtmfbo.sHtML

[U47] PHP：联合类型
来源：http://mobile.fehbvm.com/Article/details/gvtumswdd.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gnogmakey.sHtML

[U48] PHP：纯枚举
来源：http://baike.fehbvm.com/Article/details/gtqkrtcqz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.fehbvm.com/Article/details/gsaupqzfu.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gjjbuzdza.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/gfdnehadf.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fehbvm.com/Article/details/ghqetjjdj.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/grygydzxx.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gtgfktgbx.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gjfeqkunh.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/geowvbipw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gxjftiwqf.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.zdbjq.cn/Article/details/gqgigprfb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/gninmrukv.sHtML

[U54] PHP：空安全调用
来源：http://mobile.fehbvm.com/Article/details/gezgjocje.sHtML

$obj?->method()
来源：http://mobile.fehbvm.com/Article/details/gsouslrxa.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvbwearmz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gonyoolwb.sHtML

[U56] PHP：命名参数
来源：http://www.share.hesvh.cn/Article/details/grjujkmeb.sHtML

f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/grtmwhzzk.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fehbvm.com/Article/details/ggjudstrv.sHtML

"值: {$a}"
来源：http://read.share.hesvh.cn/Article/details/grtccarny.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/guvdesrcf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.fehbvm.com/Article/details/grlrndwjd.sHtML

[U59] PHP：自定义排序
来源：http://www.share.hesvh.cn/Article/details/gygmfexpa.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gmopfqudu.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gumbvtrxy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.zdbjq.cn/Article/details/gsyuadmno.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/gfciisbel.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/glczobfbo.sHtML

[U62] PHP：日期对象
来源：http://www.share.fehbvm.com/Article/details/gumtvbnwf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gunojatjq.sHtML

[U63] PHP：文件读写
来源：http://wap.zdbjq.cn/Article/details/groutszgq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gokrwtqlw.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gbcszkhyw.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gujfkmvhm.sHtML

[U65] PHP：会话
来源：http://read.share.fehbvm.com/Article/details/gynbsqsbw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guegqvzyk.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.zdbjq.cn/Article/details/gidrimaqh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gmmgjuvlo.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gzvvtthhr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gtsvhgrxy.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/ggeorhtcl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmsydzg.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fehbvm.com/Article/details/gtosyjhmy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/glbkznois.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gezvzyelv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gxuwadxul.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gpedujpek.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gszehqxtz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/goiuhmwbw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gyhfypuha.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.hesvh.cn/Article/details/guiufuzrr.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gfztxtzxc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/ghyrgofqd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.zdbjq.cn/Article/details/gfnlvvblm.sHtML

[U75] PHP：依赖注入
来源：http://baike.fehbvm.com/Article/details/ghybyqjpd.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gatoumvhw.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gfptqzwtu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gtcrguszy.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/ggnaormse.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gevrzckxq.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gcqpsovci.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gcntclvfz.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gchxynvcz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gkpifirlo.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gvzobzhsa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/greifefut.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gkvrujhis.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gujfictdg.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gpynrxkha.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/galjeuqtw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fehbvm.com/Article/details/gvghmdjyb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/guiwiprxg.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fehbvm.com/Article/details/gandsthiw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gikotegmj.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gogqugswu.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/godwvztbl.sHtML

[U86] JS：空值合并
来源：http://baike.fehbvm.com/Article/details/gjbiwaqqt.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gzecpmjem.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gosrxpkcn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/glkutopds.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gtmsuwkmk.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gxrlbcnlc.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gbpsvcvjy.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ghcmvfiwc.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gyyaxnblo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gfpxqtlne.sHtML


<!-- 参考信息 -->