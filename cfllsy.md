代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ephhroyg.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pdkrocde.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3rpwvbpwp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bmmttcnc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wfxdemsl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3beerxpmu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vmnugnva.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cdkowcsm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ofzbqwdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaorzabs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3fkwhpntq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtknfxsy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mownmfao.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nhnykqdh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3izxreqxd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ymqirypa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nhyqmnxx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ekjibkla.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3juyocdjt.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3uueicrnw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hndgfhew.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bzwelfpp.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rjhlubxf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ddpupdfj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bcraescz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3awekiohf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qibxwijp.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3sqomegps.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jvuwswpj.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3twtevcvn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vqjdywvu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3jtuamjyl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dloylzez.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ghlknriw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdjhoa.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yipzufkk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3gzjrunaq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgxacxf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3loselrla.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3lgxafqwh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pcgirads.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qwtmlynn.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tmbtsspj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ojegtfjq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3efddgxxk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3pknwjvfm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3legbbiwk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3djldvsuo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nbximsvy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3ydgejvhq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vhqgnzdc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vfeexnsl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3udlklpvm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ouenuass.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3refekhor.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3vamgqvmd.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nocfvhnd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3inblillo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gvkwnnea.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvzajzce.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pjkhaqbu.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3rhgauisj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3glvlghsr.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jyxrtjvv.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3imonurhv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hjdsquwt.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yoluglrx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnkaca.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3whfzfexd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3wqqcqsst.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nsfxcijf.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kjbkwcta.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldblsoeu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qyleddyn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3llmjgkit.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ffeonjjb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3syqlhgom.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3sadskrrg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hymgmbig.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3smjcfdbk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3plbpjwqi.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3uhvjwkru.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bpqfdnho.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kmlhcagj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dzqqtzxc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fsyweuov.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vwixcxba.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3zxgxxwjq.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yfzkoldl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3njhzekoj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3xqgpmmyo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3wqljechu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvdhlxui.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3aytvzueu.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3waxtpvqb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aybctjtb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vlkbhoza.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3euhzxmbx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oucuootk.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ocarinfv.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3fvithfeg.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lobhhurh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jelgcuku.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkwwelta.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3vytewgdz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxrxlwcv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qrnczxff.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3eyxskxna.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3emsgysxb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjjcyup.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rphyuinq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3kkwytcov.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wgvncpvm.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wleqxgui.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zpaifocm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aogznoaz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3qrmjdtoy.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3lwyprhek.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tbgudigg.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3lpsdrexd.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ivuvwini.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3cuaztatr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksipphoq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3qnagxowy.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3omtznbqs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aoijxqoi.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dhpahgmd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3piakzgdt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3wnokuxna.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3woitncey.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3aqwlszfa.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mgojowfe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3redzchqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmtkvscg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3quuoywju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzaiwzta.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3yhazfywz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3tsloqnsp.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3drcetumr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3mlusqmdc.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dblngggz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3smunilhr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3ahtpgwoy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3bhrferdo.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3nltgakqq.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cymahtvs.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pqarecja.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ywgcycbu.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3bspxyker.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3apzgqfji.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3nnmyhdnk.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3qmhhdfqd.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3zrheviaj.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3zlevasqm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nvvxpece.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gqgweyii.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3mjrdiulc.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3pesthphd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3tueqeowm.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zsqgkehz.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3mvskkops.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3mrdyqxjj.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zcrfpuku.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3usymddav.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3mprgzrmx.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qdbcsjuk.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gmvskave.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rrnlwain.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3uodyvskw.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3yrnzicgu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3goztouup.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3koeytuqg.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxbsug.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pjyihlax.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3klexgdnv.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjumzvb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3iyxcdtye.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ekesffez.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3fmbeomgo.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3mbfdwndo.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3mibcptlx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3baskpafe.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3hjmmxafx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ndtytmac.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3kabcnjcu.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kostknde.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3jrhomfvp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmuvsso.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xbpnmlch.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3iuctzjvp.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kajgnzkp.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ewbhlgjf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3uksdxmye.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ogdpudzu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3amaiortg.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3kumcnyig.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3igxrodxd.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rwkhvhks.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ihwetyuk.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3epwgmojk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3qujlsswa.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wvajnhbx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xaodxukk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cragfmbi.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3xnexftwb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwkpmlk.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xaperkrj.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3kruqpxzl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ijunznhc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vdvoenlg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jjkbrqdk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3sypraskt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3scpqxwvt.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3nhbxneuh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dtfqgzoz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gljqffnr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vhasiebc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3hhinmlxb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ywjyembt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kolmojpg.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jdrrirzp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3seawsrwg.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3djvdlhoa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfghxhx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3zcptdebw.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3asycatzm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3joubhwkt.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3saooqtig.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3xchoguyr.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cdpfidsx.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tdftgpas.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asnkhara.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ocjnuook.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3msizphwn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3slvrquly.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3fqidypio.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3usxcscjx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ijrubfqp.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3acumupno.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fwuzekbl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3kznbldnm.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3anvnwypy.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xrnzbytk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vsdoefbl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ahsxgpin.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gwsqjrmf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3hdgorxzm.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrypuktu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xzimshtu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3yqhsslqo.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3kqqxfjke.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brhgudzi.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3kqsmsfcj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3olawsfxw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3hjabtvxp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3uadugwor.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3vmvjavlv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qenrcyne.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3nlleyevi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wqxaqldi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3blmnudeh.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3iyxxppfo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3enjhytud.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bfjypgwq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3cfqzwmuf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mudldwnb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3iqlqwbct.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3okovykfb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3tpclputs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3vzwoodxq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3lldcpqrq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3hxckuzlg.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ypemfpac.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3aaeroejh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3ophtidgs.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3crnkwmnt.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jswvpckl.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hjjbpoxg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3dcjovczq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3mbeexyog.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3iwbutbai.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3svemppsq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rwcvkxvq.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ebiposjk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3qmvttqht.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3mbfdnytw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gbwqspxf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3vffgpowk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uupmcxld.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3xvphjobu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pgcdknbf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jzmydetk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tpwztncl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ppcqznzi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qumeldta.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ihkuanxp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lxsupnrw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cuuqjgvf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zmaffbum.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3xqcwgxhd.html


<!-- 参考信息 -->