代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hugpnrdh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sjnhevxp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vafivqgs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3spqdbvbv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hdjrotfd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nqisuquh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3wnfmnzkv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mshxmuiy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rgrqzacx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wuijquax.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3lahrcler.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rvdhjnbx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3unveqawm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acmcaldw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rbfuxurq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcsdpwuz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aefzgwof.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3phchayxp.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lfjrqyft.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lqzfotia.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vounkocq.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kkwlgccg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pqjgbcjk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3thrjeonz.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3itjhvcrb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fthjomek.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3cbiadpfo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3anvzjrpu.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3psyfnutn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3znuildnn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3tqskzwsd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmyulpy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jvmapmux.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jhhadkjb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rjgdyirh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3rcqdstio.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3svaqkgdw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3eqrbdzkb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zobwfyof.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwefpihp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3evfeemsk.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnecpkfd.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mllyxivy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oyyynosh.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3zrrgormu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdjsftv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vycayoux.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hlaxkoht.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3iowunqah.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lsbsubzp.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zwcoqxqh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3thvqqjby.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rmfiglgq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pkctzlay.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3cdiplzvt.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3cynabxte.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vlecyqee.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3glcrkksw.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3fwnsxpyp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3eqjvlljw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3hriqgrfk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hfnfccwi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3sypcyhhr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3obnznmxx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xnszqqfn.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3aumvaozs.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ufffbwrq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bijtmwnr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qocjcocu.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ejvdkdhj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3kzwfwaww.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3lroejkxw.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3blevcxdu.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pkdrviqr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3lnqpsqtp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mkkoyasl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kgyqbiei.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kucrkvyi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zuzamcoe.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivibqdbc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fimqpdce.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zhmjdjdf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3kyuvevjs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3flzabbff.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3updymtxh.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lungpihr.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lnhdvdeg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wmyjnuow.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fxfntaib.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3tfbprxiu.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jysijuzj.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3roybgfhv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3odfpczui.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3jfvxwvqk.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xbqrxngx.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ubjvkzrt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qbrldrbt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3cxxbgxbe.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qzxofltk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dockppcz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kddhqysx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3msojorjr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3leoodhgm.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqcnpud.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rvhympsh.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dskqxdbw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zzeqoekm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3puxcsdcc.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pfbnwyoh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrejzstg.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3xlctjevx.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ijsgyodi.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3xxjsoybl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbihfxtt.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oujaanhh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3gvvuiwom.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nausqyav.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jbepwxao.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhckhxgs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vnyxuiua.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vpfmqnwp.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gthfondf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3udskvtvt.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zfhbpmtj.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wegwyvfe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3enadaqrr.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3cdvuvwen.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mhuwuyop.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3igxbasvp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hkghlckq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sbkfxvyz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3xlvhrecu.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yogliaeg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tpdaqoya.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ntbfuvpw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3fnzmmiyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbmugmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvwvtbpk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dvitnehk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rclqcegc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kheyqifb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3hncezwvp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3tahlhrsu.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3yaxkmsgr.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ayrewzgd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ymeozcvr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3jyhdpdkd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ngtisgoa.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3beltaiww.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3sngdkdzc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ufebvpzw.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3fixuwyls.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3veqwtkjm.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3lgajkrgd.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3jnqtizlr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3swymjmoa.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3kxjdxfxk.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cgortokr.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3nfmervny.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3ijhurqhn.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3lnkymlrs.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqukvwhd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3bhwxtivy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fbntbevb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3sktieyjl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3omfxllcq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ftgaaplm.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3uxucfmqe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3oicwnqkn.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3qouuaovs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rgeoyqbq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ljfehciz.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3aeehylut.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3hmlbmynn.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3nfxccccs.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3szajtarn.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3zfokkuns.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3aodumfrr.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3naisjhad.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3vkcdwrwx.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3bfpvdnrv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3garjyuvr.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3dnghvsjh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3xdgwdjdt.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3plipecuu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3hfhnmnjf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3sswndskn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kxvdkdtw.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3xmkwqjvy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3jchewyhw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ajnxkpmz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3xkfmqcuu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3lrgphkxk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3qhxcshmf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3xkwqgdwp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ywnubgpn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3vxqcopif.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3wnizqulz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ikkwmqnx.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ejmbfgkr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3wmndxuaa.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yjwplsai.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3atjxrpel.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3jlogqesi.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rqadqzdz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3dhlegbzi.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3hziexugy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vkeoqhgp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3wjfeiieq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3mktomfmu.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3moccwera.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3sorkcdpi.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3dfxohuzm.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3xcpcbvzm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ztxrntxg.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vxyrmydc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3imosowyv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ifcoqwtj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wuzjijnp.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oqpxfzuf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3llfjzdzr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vaayztcs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3reaiqmjg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ylcbbfep.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3wvpwvubr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3bncrkahr.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3chrpgyyy.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfszlfef.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3smzouiqo.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ajrxzeub.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3crgcxzuh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3blmrppvl.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3vgisctll.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3oaeixova.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iycyanwa.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acmncvmf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uaurmhsy.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3wqocwahv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3gpfprxud.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfpnjznk.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yibiapuf.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3owttklco.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cnhzapgr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3sxakwqrj.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3htyeuwyu.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wmggipsg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3camsvrpr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3pgaenjki.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wevgylho.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wlfyvoih.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lhhaagce.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qrbuvzlu.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3admlusfb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3jkvyzxqh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3eqiqqegx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fofqzkfe.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qokavfpz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3twvrunbw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yamtaddw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3oabqdyrx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yzyyazxh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3owyvusza.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3masmogsz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3vclrndvt.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3hddtbgro.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mbodcbps.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nkdfsjbs.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3jupkbatt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3jcdudlro.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3feouhxea.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3qwrjntmr.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3roljdjps.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zogjraue.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3inlhumqe.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3nieginei.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ljfyppye.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jhhqfyyg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3pkwyesig.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gzvykbbc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3dskxqnlk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cmyitixi.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3enabspyb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3mqnsytok.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ktcqsydz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3zggifcqj.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3wmputrte.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wojpcwzp.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gvbuexih.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3cxunhroy.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qngltruc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zvncotbw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3yxtcrqfi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3udiefnbl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3ofgqlqnd.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3wygilmvn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3gjwpiqyy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jgwphusr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3harofvof.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hdamnikr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ugygslwc.html


<!-- 参考信息 -->