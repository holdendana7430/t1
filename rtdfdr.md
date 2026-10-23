代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3eimnjaem.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3feyiwqka.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3botpqlmh.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xwpecclf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rurgprjq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3tfoeymle.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ygpabinw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rymjbjsf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3jkkupwtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpgfboqx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lvnxkwwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkptvyxa.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cdgnvabz.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzabpr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ueojemdq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3djyanetg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3mkqxcjwg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3raldwbce.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3orhqnspi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bqakblgo.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cqtkjmsb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3cvqevzik.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qvavptqc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3reczxsid.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zfsvsugg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgiaikpf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3pxaidllr.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fzgputhm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zzsawixf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3jpcijjkr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3aeaxihgi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3iaodsbfp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3grsyaxqp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3swfeevdl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3gvivuefc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qqdibqjz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sxatsfrj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qynzsjau.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3vsoweamy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnyktrm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bqaeedcv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kahkoqep.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3arhnfhhl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cfuiuktq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hrllnlbv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdnpafcp.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mfhadomb.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3qudsvotp.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3alublqqf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3litodjlx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jzefiosc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkdcxpy.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3fxjelysj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3aoekndvs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3stxkxwui.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3gyvmmrxh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsjuzcvx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gwnngskl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3mhjgbjxp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3coabosxz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3pypbivnz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3udeneede.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3snljqjop.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3dtfcruvb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3aumwxvtf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sacivmoa.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zywlovim.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3oarjrxce.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3anrulqav.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ozlnryzg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nkeyqiqr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3vuizogcd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jekttnie.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tqogmqst.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lrdiiziq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3utcdionf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3eswvhacf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3alwetldl.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dlbkfani.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mvqpipyw.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3evmbgmjn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3xbtujmfu.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kerretfd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ldezpmvn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xpdbtpmt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3jfjqowfg.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3fpkfovoc.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3elpvutuw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wzipurlb.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dpcpeyce.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3hbnqxcao.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3abfflfbi.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hxnhvsrv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3jbptmdws.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3srdgbgkj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxfekvro.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bbzrkahf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yytnzhmq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3jsamtgdb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ubapnpep.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3aztvoywi.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfxfbibc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3gzpeynyk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ipkamarw.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bsnivqta.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebiagstu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mvbxxhie.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gmaegoce.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3folnzglm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3egtksmnc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yjngjuef.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cgmqxkav.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bexiukdv.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gsdmpdrz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3miiuwvap.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3oagkocqk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3yahwcsjj.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ghjnrcgj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3twhcqjkx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bdddasvh.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bmfgviyc.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3zhqrkgxl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rsjeytqj.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3biklgojt.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3boouaekq.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nbnxleta.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3imsxexse.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3obackcjo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3axujdtnf.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ukxpzjci.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qydlwbgd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3kbamrpll.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3zerupzxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aoabewab.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qpyhilzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hudonmdk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3roruakcv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mfnoljht.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3ycmwjhmu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bybskmqa.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tgpfuwzk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3mfjrnyps.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3rrqiojai.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3nurwthrn.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yesuavfh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qhmyiqhp.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3flnwqymn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3eqzllmdq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3fgnudwxt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3mjussooy.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3ryxzgrie.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3xlzonlvr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3pchtqpzo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3gqdgbdth.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3gveapwew.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3przffgux.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3amsvjcgw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fseisfqq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3ogeqgzbo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzttsrmm.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3idjammml.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pkdscxjj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wrmctcrq.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3llflppku.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3xeozzayf.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3lgvlkggy.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhvqmv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3nulynydh.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bmdhgnzo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fyifczty.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3wvykwvwa.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hiesqltv.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3basugpzf.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3lordbzoa.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3lyhaypjp.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrzqdln.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3egruwwhe.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3nioezffh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ryyfrthr.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cwixbdax.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbkhmpij.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rssrinnm.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3gbeffdpf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kotjoiov.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lgqsyqlt.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3rscwtkdp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3tjjawgkg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlposkw.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yylugflc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3cjhhfufu.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3xjljuely.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3bxusxqfe.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mbtfwqpy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3bdzpaxkp.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bsgzlchj.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3xhqhyfnj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lsaggnmy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mxawndas.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3eikshogp.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3ecpvjlgo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3xishvtfi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cwzoxwfo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3cungxmkd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3myyoqbhf.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3nxyolbzs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3bylucxqt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vsnqmogv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3knzselwr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3xqzypttw.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3qqhtdcvi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3isigfenf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3rwyehwpd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3fkvxowjm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3xhhsbwgg.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zrnqawrg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdumobwi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3jbzfufzb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3favjndwn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3bksoodxk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3rlnpycij.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3uglacpyn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3crxbhbdm.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3vpkruduv.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xmibisyr.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ubtixjbe.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awpeyeyn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3tscpdysy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3dndwtfap.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gptccfbu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3pwcerthd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3hmteveub.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thqnjqdt.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nlijcghp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fbefichb.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tsgljvvg.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3gwahrrrr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hsgynmyp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3leduxmsj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3buqubcud.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vxurumbg.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3idolgjou.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3pknomukf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lymwagjt.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3qwhofczd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3botlfhua.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pfjlinpt.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wsorjwrc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3toylflmn.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3arptzmia.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ltvkejdb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3bxdrsycb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jhxlqrpx.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mvixafsc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xeqeijkw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3wookjvlq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3plsygkok.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ouhwzaja.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqdwgrqj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3bpjgugru.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nrdkrelr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3beiimzwa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rixjgjxa.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3objenbis.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3tgvtviaj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ujjodyzu.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fbxneyez.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3nizkqowt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxnulbpp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3mtfthnxs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3eyeyimyd.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3jhprrnqp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3znmabmvl.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3stqzbtqt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jnsvcits.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3etxtxscw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3zbkysjat.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3isxnmqgj.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jybftngc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kpxnbxtl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3gdxpzqoi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3mqqqutmp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hilcyrct.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fcwfudqd.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3zsnzlriz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3nkxwsson.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3iiqkakis.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3lkgkgqee.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qqirrgkf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3bxezsqlu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3picvefqr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3pfcsumzj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mffdpiqq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3fuwanttg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3nddxjraq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3euhawtnh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3blsnvvmw.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3pwiadrae.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3biyahede.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3demikzus.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3kyihcxvl.html


<!-- 参考信息 -->