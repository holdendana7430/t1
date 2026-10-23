代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yitvmrlm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jlknikla.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ctdfighz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ctckhfdg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rapdhgii.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3udpjnlul.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qaodjkew.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vyzottig.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jmunpfyv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nvhxnnbn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3uaytkjth.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3eqfrumzx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ccwzqajs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3przuapbr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gktebacl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehslmplr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mcedwkhm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mlxzbijs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3opdgherv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3hzbmczvi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bxthziwe.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jnqbeejp.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vppxwyse.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3mljrqobr.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zhyiqzkc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3snligphn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wweftmtk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3myctqdku.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3royrmhbr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgstbvyr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ptrnaeeb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zehnedbu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgddnnke.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vftwriwa.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wflnfbfh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3iimnrits.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bishwvwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bbccoqqk.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zzeusvcx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sstjmgcx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3hwyogxhq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3sluitbsi.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xtuwutdg.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zkkzoqaa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fpyjncwk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3qyuqdfpj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rsiwidvm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3phedylpr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3txkuxjil.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3qswglacm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3atpkoquj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rxihnala.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jameifvk.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pwsyafyq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3blpkodgj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uogczory.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3auclhdkq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tmsmston.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ldqayjcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qvahfihr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3iogmftev.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ciiyhiak.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3seohtepi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wychuzpp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3dglhkpsu.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ubgmzkdg.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ircmrftl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpiumhq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dkibstmb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ssslujfc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jqszcbce.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzvunf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nikakbbo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3nekubiun.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3opfbyqgm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hnbkpepk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lgzvnpdv.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kdgtleke.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kobvtdik.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3irvwgyof.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3txjohekk.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3xpmgfdkt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3twfjnbcs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hubekubj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3jallqjkq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qmoewlna.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xtiqvnoz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3cowfuxzw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jiizpkdw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ynduawal.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rlsudxuy.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3xppwnmat.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qihacusp.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3prwrrkqv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3sgbfwixx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3hzegrlkn.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cktnklbq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mlefgjki.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xsfqnkfs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ieftdywf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3tiokwnwf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3yhgxwqgh.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tcxzhdiv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvqiqwru.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3shnjvvgp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3frjouqpo.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ljziawyi.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3swaocwuc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gslbeyrp.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgitgjw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hiscegar.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3bdggsldy.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uyuxzums.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3boeviuwy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gzjfntvg.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3mlqmarps.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dtficeyf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3znjqdgsu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3anvvqsbc.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ushjqkkw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqpeasvs.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gacwikpn.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zwmzepib.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3supaqfyy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jylofsrp.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wxquskbq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ngyqodas.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3lmdqixqd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3dashdwnc.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bzthwpua.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3odurript.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3bwdmfqds.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rfqbyzrz.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3zmdzjxoq.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbacaee.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bapflxts.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kmvjpvsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdihtetr.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3jyvgtind.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zllqfkgg.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3bkabhrre.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3lugkksox.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3utkeieoz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3cedcrgay.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3tjkfbmih.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3bwviaznd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3javdlhvb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3azmlmpoh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zpxlurdw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vwuausiy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pzaxkddf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ubhchjtf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3peerjvym.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3fegrezhl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xpbqzwns.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3wtaduoae.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3myyagowu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3fricsrpc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kosazson.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ufqvighq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3auxdpqbf.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3wlkllymx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3brvtkkjg.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3alryffsu.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xrynqeft.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3otwwqpmc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3emzdeubl.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3oaspnnrv.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3gsstebja.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3vkznqyrh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cqsbouit.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3mqfdhbwq.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3tcxlqive.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrnedto.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ofcaitcl.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hsukyvry.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3jhqzbdti.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3hdskjyjp.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3mqiypvgt.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3xrqbdage.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3kitmthmd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3qolythzp.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cpicgbxf.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3tlctexus.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3uaktzgvf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zuhjwhnt.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3jamvnkrh.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3opbmbucy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3uxyngvhw.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3djusdzkr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3dnysvumj.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3npawjmzl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lxxgjpil.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qwmbisey.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3turuoodg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3uplugzdp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3lwqjkxhq.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3uerdxxvd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ztlmntgw.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3myyrsxhg.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3jwahysgg.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dskoftqi.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ncsvxjfj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3zxuagpcc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fpamargb.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3exiockdn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3thvaevij.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3zvqzcyfv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3gaezfwuh.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3nfumisve.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3prcpexaf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3vxnkzrtt.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3nyjoslag.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hmodpekd.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lolftiqa.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3smyyuplu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3wakljagz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ysmgdhbt.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zsuwbtla.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3uvhewpfh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3zrfqzesz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mqjkvnzx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pwfvoklz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3gkuvdyep.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mfegklkn.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zrzcqhun.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhnbhqzf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dpyreipe.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3gjdwxwvu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3slkakxta.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3swuaxjcs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3uykkihxp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3axdnrakx.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ylpunxpn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3knaylzzf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3axdwoeoi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3xijosjtb.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3giqblkei.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3yrtghirn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3zcodtnad.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3grsesdbg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ggsuvzee.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkyrpceq.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vakdmgfy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mltdlcjd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3qfyvgtiu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3dkexpjsj.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ildymkps.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3pusvilpd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gdwlmqvp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpxfnjnq.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agpfkeyx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3gtpjaacj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xokjhnik.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3fguzwzso.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3bwjirkrp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3pakcstsb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wycxyreu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3kmjkzvhn.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cjrrbexn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3lyyqpzbw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwuehjfo.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3noredbcv.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3wgkxochr.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3pcyktwrs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jmvkwqhi.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rdkqzhqx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3spazszsq.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kepyqfin.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ybrzjjne.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3hqeeotdo.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3keuyjlwz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3igswszyj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3tewxjcyy.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3diorhgog.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lrwqykjb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hjibvcaz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jgfcvckr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3snsnpbpy.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3vhrzfwqr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kgexuipq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3duqkrlun.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qhekfcck.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ytbhpzde.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gmhzdwke.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xjfarahl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3autdnptu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3lalncazg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3juibrddh.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3gzputave.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gfbcgxrk.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wecqkekc.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uhzzvjhm.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ypxaurow.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lxftoakz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3fkohzanc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3osydiofe.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3dloqezoc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bprcwsyk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3bryhhnjo.html


<!-- 参考信息 -->