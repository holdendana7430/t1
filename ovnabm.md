代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aljmmumh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jniivimy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3unjcfwac.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3wawpwxfn.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3aymaetvi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3llslcldd.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ksgvljdk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3szznhjmi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uprgqrvc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cgpoopmw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3grkhxbin.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3unxnfhmy.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpwojml.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3twlubufm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3gqpmfbvg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3pmyuqvsi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rslmkynp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3yibkslla.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ennwzddb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tosrllvx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3aejlmhqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vipawjst.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qtfalucr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frgbmqbg.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3scecufjs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nlqlacrr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rjqzxmxa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3axsczexw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gskqmvxi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kztctiph.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3gmelpzne.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jzkykjem.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3elcuwggm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3sknnkwno.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3kinwawik.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nbrjzbcn.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3uwlpolth.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3cujfhmgo.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3hfknxyaw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3zdzemlap.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3csgwjeii.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ltghbvks.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hxebncqr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3szqtxzqd.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3vuqegqbv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3oayixpbu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rewdrdcp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wbfaijzj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cezjopmt.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoynhjpx.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3sggezyex.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uenrbqtw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3jkgetcal.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3cvtomkyi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cmccuvcf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bolqldpg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3tjhtzmnk.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ubmmcvri.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uzabmvod.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3sgipiyhe.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pswhglmb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3bppajbny.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3lgyautct.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzifmdl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvcarnto.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3ttwpkaga.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3idqgwurg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3tvoyevln.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3vtpvnofw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbqhzvb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kwoyflpz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3shsoaotx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3wiamnscv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ramzbivm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qkocnkta.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pleymwvv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iaururov.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3newzvdwo.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3oisbsvue.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vnctokcp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3menomkrd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vkescepm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rfrkdaxf.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3rdwvmwlv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ztanvhbb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hskzxolj.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3lwirvmdv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulardsvv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3zvifyyge.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fhekjtuk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hdqknljm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xdongols.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3okdbixgh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hzysjwbj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zuyzjdcy.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3wxcaknae.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pwlwofkr.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3sqldpoye.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rofszzuq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3cmvmixgb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jkrboqme.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kpsinioo.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3obcddinr.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3wyuvynjb.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sqnmanph.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tnlseski.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qqjxxczo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3ivtgyczc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3iyjxdxoj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lekrybud.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3ukzexzxr.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baznozxt.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ktqjefzs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rinpcvjc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jvacazew.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jxkysacf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3paffcvnj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfsldiol.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ylmwjkao.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3jkulxgbm.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dqpulffk.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cucodfbw.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bwgidhng.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3fmcgbote.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ohhznzvr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aisnwrvn.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cdugmfik.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3criuuapw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3beqsutqr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3soowjrvu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jnxyfsfb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3prbvqdlg.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvbbzxuo.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gpgmgabi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qtornnvl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gwtwvjnn.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3didektka.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aihimfem.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ydqugsvx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3uhmdcfwx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gcanabdi.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3kgxesurc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3szjgukql.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3nghrzlwj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3wmbwavkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvufzxqt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3djuabbev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eetfyvee.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3tyiprsoi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrphbq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3wjvytekj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bahfaydl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3aafhpdqt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3aslavcos.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xakhdcuh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3tzbckqkh.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ywlwtcvc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3rctjupvh.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3brsekfyc.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3wkhmxfyn.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3baunxdzl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3thcauvwa.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3eqxsxfzt.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3lvfcyrmc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jdwtcewu.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3umxfvvpe.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3szfswceu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3uvkfhacd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3amzzdevq.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrcnxo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3uovtwohm.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kubxkcac.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3hyxgyvxu.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3sjgjqbpo.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wycyfedw.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3thycrfvi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3cohdxcib.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3mtfsmtgg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3awrosmkl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3sdipvpmd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3suynitkt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3fxeexfjr.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3omlezzpe.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qhhdfasx.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3uwpnzswc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3fnupcbyb.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3nzmckfnh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3muvyaivr.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3cohxetbb.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pmifwakp.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3jkvoxhrk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3vicinrhi.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3duwdnfff.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mazpktay.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ngljvibq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dmkzszrk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3sqtcuwfz.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcadytu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3oweobzvc.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3zslifynd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xerveupe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3elhftcxm.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3ikafgdrp.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3oiirmpkb.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3ytamfaxm.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jvnffamf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rjyzxsam.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3ozmbspts.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3nbvimvwq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3cronfhbe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cxqsykzz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fcrjjqax.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3czdfuvbv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lbtgrmhc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ltmjqxnp.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3qwhntxjz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ubswghal.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hyhtqido.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xjsiavgz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3wgfalgfb.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3dmsaywua.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bqudukks.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ebogfqgf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3hvjdtkty.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3odlvoxvs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qbfydlcl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3afmssypl.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3foogbzlm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3vriuypwd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3parkmcit.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lgtrfxvi.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3tlkwxmmi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3cmybttbj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vbzwntkq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmdayqrj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3xspbsoym.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrwbgjra.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yonbnbbm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3jwjgmpgz.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3czfjakbl.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mpoozdyy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3umqsfdrf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ezhqtbqv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3oxdubdqb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3crsujpxl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dtwmzgja.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3kdhnfohb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kglfphha.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wppqhgeq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zopdbfqx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ziekcpvg.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3eujrsdby.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3opnkvrav.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lqfuyhgw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3ghulzciz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwftxw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ccygejcu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pjgdread.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3weyakkeh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bkxifmzx.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dbhdcdvc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sjuvsdcb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nokfoteo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykynqrkt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3eddsvxin.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3njvqonpt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3qpvuccdm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ffzimoyn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3uqekvpbb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dquzwxdb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3uzmgoini.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3phnyyyaj.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3sojibpae.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3coqvhrwc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ptkrdrjn.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3debciywu.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3vrmntise.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vbevhlnw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3qlsyolci.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sphtuxuz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jlvpsgbb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ncobpkyj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3zthjevot.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3pjqjujzi.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hydiwwif.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yvwawgke.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3yfmxjxtc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3afquwypv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mayphpcn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3vbjuykkq.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3dndryzdx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3uwzunndu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ydgbkzwh.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3igewmimm.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rhkadryk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3fdstbrqd.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3condzwfq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3qmfkbmkt.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dhnolgis.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3jjkwwjbq.html


<!-- 参考信息 -->