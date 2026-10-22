代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmhiixkw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2vkuxtzyv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qjiateah.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nilddgqp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kbwmqooj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjnovzct.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2oazwsqnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgbkvpjk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bkrzovtr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2scivxryg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xuotaboi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2pvlnbnyn.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2yxfqjhqc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2bpegbzvj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2bezrdtdu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wrvhcedz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2nhwjkghh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nbwlpncj.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sgvqfmkg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvuomojt.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2lmempisu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tjjhmcac.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ceaanamy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2igcigmzl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2ikqaijml.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2bwapbnhf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2taaarpto.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2urriehqh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2wndvdqii.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2skoamija.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lrtuquem.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ppbokhwn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2axxwqhut.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmuhnetb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2yaiigeva.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2abtpdpyb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2zhgalkrk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2skmqdjwp.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2whytkzhu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fpgtolpo.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2eazgyvrt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2vyjtqszc.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qusdurdn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2yrjqixsz.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2msxkkmce.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bolsxytk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2oljzlapq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffrncomt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gwjqrzgb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2pgyhjiyq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2ukoktsvv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2znfdadgg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ujxqxbbb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2swlpmuxs.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2colckxpx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xaegjwot.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nxeacqia.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2ftkoqmhe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qbvhcbuq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vwdsyadi.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2valzxlna.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pvzjtwwp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cewhehpc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qcuzbgbu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ieeqbofp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nddlcmgg.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2djhheomy.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mrvfagct.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xqwyldlp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2pgbkirri.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rentjyfh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2rhnpksxa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mhlfgxhh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2coejaoku.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2uwjfuzzn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pfbxnxge.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2wmhtlhph.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rodxumoe.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2wxcgpvpd.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rhvndfvd.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yhvuuuqb.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ftyxqhre.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ruqenyzo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ciojrnrd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2wuzuiexo.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2veredgxt.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2avumjgam.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2sbkefzwr.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2elojzvck.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xaamnrlo.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2cdykszha.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2tiqgfxgv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2sytxldei.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2qjppjuxr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ylzazkqc.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2uqdjefel.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2dmkiuqzi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcviwvpj.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2rgcqbxxt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2yzzelftg.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2rfgtonpv.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbgunphy.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2yzzipjfc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcieqd.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvhcrzbf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqaeomaa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxcdnlzq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wvjnvlzl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfsifsus.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mksbexmz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zypwteya.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2sqztbmhl.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2uooclahl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vjnudwyi.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nucshxgn.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2wgaplzor.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dnlhnpwx.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cmpppose.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2bjnlgolf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2qanzsazq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2wwwpwtkk.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2eajdwlvy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tgypdrwo.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gefcdmfg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2iujupezq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2dnkfuhrg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tjypeyoo.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2evsugzxc.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2revfucnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdclqeby.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ycjejgsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtzdrqtn.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2ccvxeaqk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2eivobxug.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2ohrljuxv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2lumfimlo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2juelwsoi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2azmwwpab.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2koerqvoh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2fxljokqy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2lltbhhiv.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2codhifju.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2qcrnfwxv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2nkwmxmvr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2uyzrqaec.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2susrqzmb.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2knvktfje.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2wyxvvzgr.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2znmtmnbf.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpoegeu.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2nafkpjhe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2qwhdxgpo.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt2fbhjkxcq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpzkjmgl.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2bphioanw.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2avzilwkv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2lienccvn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2gpxamexu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2jtopgqln.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmzkbno.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2fgrdwpws.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2owmsltif.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2tabuyzfg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2wwwlmcrj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2uhbnhfhq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2sqdzzjct.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2hziywbgi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aoujkmab.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2fhzxczgq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyptlifo.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2qrwmedpl.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2gzocitvr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2fiqonnck.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ojpwtxkb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2aejygzwg.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2zlvicjsq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2tameejmk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2dxstjujd.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2usqjscal.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gtpwoslv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2epjrlqmm.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2xrtovqxd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2hhwrvuua.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2motmpkvt.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2avnvkmji.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tptxcypg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2knioqqcc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2dfbbkoby.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2dlstsozh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2lhljpzqd.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2whpgdcgz.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ohniqrub.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2rglscapc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2mhefpica.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2fkyfmxzn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2nqqblwoe.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2wrvpungt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2vleqcdrq.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2oojooogo.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2shypfuuf.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2hokoarqk.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kulcedmw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ffavhqla.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2zorvcmmn.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rtwkasri.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2iybjkhxu.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2folgssfv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tfqraacn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2edqpoozw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jlpsoovy.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lhifhbqc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vpzfqonc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2muawtiip.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2tnjqngsi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2szsjimfu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lustvphb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2vjrlgpuu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2rkouruij.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2uwtvyeyr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2segtphwh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gnjjlqnr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gksyzplt.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2niepmbtz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lrilidge.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcdaqswn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ktnjhxdt.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2hnqetxub.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbqoenjr.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2yuuqsrbq.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2luotqbeg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2iqcmnnkw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nubjuwsv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2urrltosi.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ovdvlbbw.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rfojljuk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zkenjeeo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ornvrffn.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2qtfhbpnp.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2bzxcqcta.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2tfvbfrpa.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wybnzvlb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bnfkyvfx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2tntpabgb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2unfpwnyb.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2fuzvrjke.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2wdlwfmws.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2kreadber.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2yphhumkm.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2ysszsiqc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lholymff.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2yqsoslsn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ufvvxznh.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wycrwyku.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kjsxuydk.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2lbgnvdwo.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mfbvlbyk.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dswqjkpr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2yzdzedez.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ococjgjq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2xzfadozw.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2krnkbgut.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhdoza.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2xatemzho.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmtdmiux.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2xwyxoelm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2zilefwse.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2wikxucqq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2nrczsmec.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2gjgytunb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2khyhwhix.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gzitedvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ehpztezn.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2huzlaxkr.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wlmyogxf.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2uygpbsna.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2buhwqgqu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2vnrvpcvs.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ukjwkfno.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cfmuykxj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wkawpsya.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2lhtxzzzx.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2lhxehoia.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2tslgjyqa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dsyciuwl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2vcxyoplg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ianninmm.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2kgucydic.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dlmdnseu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2myrpubai.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2zbbygiwn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2hlszhgdz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2avuxpmdx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zwgpwfja.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jgopezth.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fnwwkqav.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yumvjkli.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ychfcciq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uymvacbk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ghlvmihp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2oxcucznm.html


<!-- 参考信息 -->