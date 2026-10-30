代发 wailian999

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gwqezbqyf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gqrwaxrhp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmguffjxx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/guwkqxryo.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gishqkjgd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavouuosp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gikgnwxcc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gngvjagnx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvllfvebl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaszfhrv.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnojldjwm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnpscdau.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsmifbvl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwbjycmt.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/grgykvvfa.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grcguziko.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtkslvlp.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/goslzrkti.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gidkjyjwx.sHtML

for (i in 1..10) println(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gnddsxghl.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpajgiwje.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtawmmppw.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gaerrfybf.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gxuxlwupk.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexnrdhbb.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/giqixqwpn.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gchrkmnvb.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqikaptpb.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwxjypo.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtctltscp.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gxrpvkngw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyqfprbe.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwocwfre.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grittymqk.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gklltfhab.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfuocvlsq.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxmkofht.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyakeoyjh.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoydulxx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbmuxvqf.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/graahwpar.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgbkoyso.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gchcabztv.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtehckhz.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gruccvuji.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjptpedy.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gykbbefpq.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gtwzoqmfu.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzbvzxwm.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grzoyocgo.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvuvazoc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjqnlhsa.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkyditg.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghesxmtvl.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gihgfibgi.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqeskcra.sHtML

[T33] Lua：表（数组）
来源：http://3g.fanxiaobao.xyz/Article/details/gzrjzsfei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxhnndvg.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/ggzmesups.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/goezoahji.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gcothzfjz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmdthfys.sHtML

[T36] Lua：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvwhhemne.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfhgana.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyeclfol.sHtML

"a" .. "b"
来源：http://3g.fanxiaobao.xyz/Article/details/givhopeup.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxvzvqhvm.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/gpljiejcd.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glppgngrg.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhfteac.sHtML

[T40] Lua：元表
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkzpkrwm.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gyiwevztx.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjjtklbva.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gnibodtvs.sHtML

[T42] Perl：变量类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpuwwcmp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gbajtlywq.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjdjifg.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gldlpscfv.sHtML

[T44] Perl：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gsbzlbxih.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxcjvxcgf.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfpxpycd.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtjdqgwr.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gaozmspxh.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfykmyjz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/giscevmvs.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrajmfto.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpbvxsii.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqimpdpxm.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnywdgqxk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/glhlmjanq.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeaskfmm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fanxiaobao.xyz/Article/details/gkilzmjhq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjdfsznq.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmelzkig.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngsafbyl.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guoproquc.sHtML

val a = 1;  var b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoeojzej.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtdmbjnl.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgfuxpmw.sHtML

[T54] Scala：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gccrhnowh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gqounpsku.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlnolhtt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvpcmobu.sHtML

[T56] Scala：样例类
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsohdnsg.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gbxoahvyk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/genbewgfo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlwdyeyc.sHtML

[T58] Scala：函数定义
来源：http://blog.fanxiaobao.xyz/Article/details/grrdvrbgq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgehjbo.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gbypysnak.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdecxzidk.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gscuwikhq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gojxccaxn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glsoihyye.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/guiskrrch.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqbdexsi.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fanxiaobao.xyz/Article/details/gywfzajtw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fanxiaobao.xyz/Article/details/gekuparlq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fanxiaobao.xyz/Article/details/gjzumbhqv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqthsmhx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.fanxiaobao.xyz/Article/details/geoskdqqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbactnhym.sHtML

[U04] Py：变量调试打印
来源：http://www.share.fanxiaobao.xyz/Article/details/gejtztocl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.fanxiaobao.xyz/Article/details/gnwaflfrz.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsfkxcad.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnqwoukm.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxdsatkn.sHtML

{**a, **b}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkebclstk.sHtML

[U07] Py：反转字典键值
来源：http://blog.fanxiaobao.xyz/Article/details/gicwciigj.sHtML

{v: k for k, v in d.items()}
来源：http://baike.fanxiaobao.xyz/Article/details/gdawiznhc.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gwinuifmv.sHtML

[y for x in nested for y in x]
来源：http://read.share.fanxiaobao.xyz/Article/details/gemvzulte.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fanxiaobao.xyz/Article/details/giqcobdsm.sHtML

max(d, key=d.get)
来源：http://www.share.fanxiaobao.xyz/Article/details/giofjcttg.sHtML

[U10] Py：按值排序字典
来源：http://3g.fanxiaobao.xyz/Article/details/gmzpbovmt.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbrxsdgq.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcovvcgev.sHtML

(x * 2 for x in arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrhxbecn.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fanxiaobao.xyz/Article/details/gilmxmlfw.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjddazgh.sHtML

[U13] Py：固定长度队列
来源：http://m.share.fanxiaobao.xyz/Article/details/glamsqaxm.sHtML

deque(maxlen=10)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdnnxbuf.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghubptnzh.sHtML

defaultdict(list)
来源：http://wap.fanxiaobao.xyz/Article/details/gksipgcij.sHtML

[U15] Py：高精度计时
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyjniknk.sHtML

t = time.perf_counter()
来源：http://wap.fanxiaobao.xyz/Article/details/gfkiaiyak.sHtML

[U16] Py：命令行参数解析
来源：http://wap.fanxiaobao.xyz/Article/details/gqvwzxmzr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkkvvhp.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdukhlqao.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqoupnc.sHtML

[U18] Py：预编译正则
来源：http://baike.fanxiaobao.xyz/Article/details/ghbwltihh.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfsvmnqr.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdpdpffp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.fanxiaobao.xyz/Article/details/guhzeyglt.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxyjcbwc.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplhjyym.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.fanxiaobao.xyz/Article/details/geqokfpxz.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrutkyzp.sHtML

[U22] Py：矩阵转置
来源：http://3g.fanxiaobao.xyz/Article/details/gnefnafuv.sHtML

list(zip(*m))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedyzivvz.sHtML

[U23] Py：分块读取大文件
来源：http://3g.fanxiaobao.xyz/Article/details/guaiesovs.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.fanxiaobao.xyz/Article/details/gwclhesms.sHtML

[U24] Py：路径操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsqjrolm.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gsgnpwjyx.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fanxiaobao.xyz/Article/details/gqcucbfql.sHtML

csv.DictReader(f)
来源：http://baike.fanxiaobao.xyz/Article/details/gayvyrggn.sHtML

[U26] Py：并发下载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlcevlvc.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.fanxiaobao.xyz/Article/details/gatavnpub.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmocixx.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fanxiaobao.xyz/Article/details/gncxdtrdn.sHtML

[U28] Py：类型别名
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwrjnbhu.sHtML

UserId = int
来源：http://blog.fanxiaobao.xyz/Article/details/gungdnvbc.sHtML

[U29] Py：属性校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjwftdaq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskkjraa.sHtML

[U30] Py：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/gbcgwdont.sHtML

@dataclass(slots=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gvglotuln.sHtML

[U31] Py：单测
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgprdjhh.sHtML

python -m pytest -q
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmnkrcl.sHtML

[U32] Py：代码格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gldyuxvut.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwnffzm.sHtML

[U33] Py：打包发布
来源：http://mobile.fanxiaobao.xyz/Article/details/gptyiodpj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnghelyfv.sHtML

[U34] Py：判断编码
来源：http://mobile.fanxiaobao.xyz/Article/details/gntdrgjcn.sHtML

chardet.detect(raw)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsitugmr.sHtML

[U35] Py：发送邮件
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqalowp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.fanxiaobao.xyz/Article/details/glkokeqmr.sHtML

[U36] Py：定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowvycpfb.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.fanxiaobao.xyz/Article/details/gzynnwebx.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyniqmdt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhbzdova.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxebblpd.sHtML

Path(__file__).resolve().parent
来源：http://baike.fanxiaobao.xyz/Article/details/gtwlznqvk.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fanxiaobao.xyz/Article/details/ggclwefpm.sHtML

sys.stdout.isatty()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvrxesih.sHtML

[U40] Py：打印到标准错误
来源：http://baike.fanxiaobao.xyz/Article/details/gzfjgovsr.sHtML

print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaigaqqhk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fanxiaobao.xyz/Article/details/goenwiybv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiibshrv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://wap.fanxiaobao.xyz/Article/details/ggolhfgau.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkmiswja.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/goofarfwm.sHtML

namespace App\Http;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvcvqgqd.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fanxiaobao.xyz/Article/details/gcqdlxngg.sHtML

declare(strict_types=1);
来源：http://baike.fanxiaobao.xyz/Article/details/gxisivraz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gzabnndes.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcuvkfhc.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geehkujtw.sHtML

?string $name = null
来源：http://wap.fanxiaobao.xyz/Article/details/gqucogomy.sHtML

[U47] PHP：联合类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gbenafnow.sHtML

int|string $id
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqehpnne.sHtML

[U48] PHP：纯枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gnuhrqcqq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyohjfrl.sHtML

[U49] PHP：只读属性
来源：http://baike.fanxiaobao.xyz/Article/details/gywrrqotm.sHtML

public readonly string $name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurpqofal.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gorcfxlrs.sHtML

public function __construct(private int $id) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvputblpd.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgojhxob.sHtML

[$a, $b] = $arr;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzndzjqem.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfozzfgsq.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdnqcrvu.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmcldpon.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykjmqhl.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqgeouuj.sHtML

$obj?->method()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfnsojos.sHtML

[U55] PHP：match 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glttlwyyp.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygxlpnur.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqusrznq.sHtML

f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlefhctc.sHtML

[U57] PHP：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/ggczuvevy.sHtML

"值: {$a}"
来源：http://mobile.fanxiaobao.xyz/Article/details/goqmykpom.sHtML

[U58] PHP：数组三件套
来源：http://baike.fanxiaobao.xyz/Article/details/gtwsamyjt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/godwcnnwq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmmgqbz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/ghfjpcxtc.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.fanxiaobao.xyz/Article/details/gxnrvsudc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjsmdxqt.sHtML

[U61] PHP：正则
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnelpeta.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsjazmwf.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboptfbkl.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssbmlvjk.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqymxcjk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgywyted.sHtML

[U64] PHP：目录遍历
来源：http://3g.fanxiaobao.xyz/Article/details/glfekdhht.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwrlymq.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gwpnavbed.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqbpjgkmn.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.fanxiaobao.xyz/Article/details/gcttmaynm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gihnsxybt.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapnkpza.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgpakave.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxhtywvm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfufffau.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glkduhhsg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fanxiaobao.xyz/Article/details/gigexzian.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/gqvqbmgqo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpljioou.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gzeswrhcc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlklzqcm.sHtML

[U72] PHP：写错误日志
来源：http://baike.fanxiaobao.xyz/Article/details/gkuwbllzq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.fanxiaobao.xyz/Article/details/gidpupgbj.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fanxiaobao.xyz/Article/details/ggapwqhpf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.fanxiaobao.xyz/Article/details/gxqtyavid.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeduouyd.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fanxiaobao.xyz/Article/details/goqgpcvsj.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyjytet.sHtML

composer require psr/container
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknswsref.sHtML

[U76] PHP：简单路由
来源：http://mobile.fanxiaobao.xyz/Article/details/gexsrbawl.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduyzkzsl.sHtML

[U77] PHP：模板渲染
来源：http://3g.fanxiaobao.xyz/Article/details/gjateebye.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gadhdumud.sHtML

[U78] PHP：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gahxkjyyk.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fanxiaobao.xyz/Article/details/gifgmkptw.sHtML

[U79] PHP：静态分析
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfhkncrr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/guwqbuprx.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fanxiaobao.xyz/Article/details/gfxdsicxd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fanxiaobao.xyz/Article/details/gntsjtrsx.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gdllexokj.sHtML

npm init -y;  npm i express
来源：http://mobile.fanxiaobao.xyz/Article/details/giexsujjt.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdiwlqop.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/glniswbbm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gejwskmdb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxlgkpjp.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fanxiaobao.xyz/Article/details/gulnfjfgx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefqhygqt.sHtML

[U85] JS：可选链
来源：http://3g.fanxiaobao.xyz/Article/details/gnawjkjwh.sHtML

a?.b?.c
来源：http://mobile.fanxiaobao.xyz/Article/details/glrrqzkjc.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdrhnfcw.sHtML

a ?? b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmovssfl.sHtML

[U87] JS：解构默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gydsvdugm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlncpdvg.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gaazibkku.sHtML

{ ...a, ...b }
来源：http://3g.fanxiaobao.xyz/Article/details/gxbtlztgk.sHtML

[U89] JS：数组去重
来源：http://wap.fanxiaobao.xyz/Article/details/gritphhwt.sHtML

[...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtouwpcwa.sHtML

[U90] JS：数字数组排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjjnludnm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gbbqzudzi.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gohcspjvj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fanxiaobao.xyz/Article/details/gndrwdlya.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjqjgjfia.sHtML

structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gminnjlig.sHtML


<!-- 参考信息 -->