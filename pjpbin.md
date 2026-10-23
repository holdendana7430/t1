代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3coebepdq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3fxjyrqae.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tldgdmkr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3edodatex.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdizfmt.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vganbimm.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixydoldx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3douvrnbt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnftska.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eakewecl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vvxmuxos.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zxfmxthi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3frojskqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfbmxdja.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ewwcthbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unugdfvh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xqnmdthc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rgpflgla.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3udkdkych.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3zagfhuhi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zlgzeoqf.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3iiptylyq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3utzypkzh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3czmtdecl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3gkoabysf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uhvhehyv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3uwxtfybh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3phmeclql.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rvnbqhet.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3xurnqseq.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3wxnuyjkn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nshsgplk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zzzvstmd.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3yvimlzvn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3byhqukjm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pcgbxwbi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gdcschrr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3cdbneltf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oaprqbke.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xncjhsfm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vlkjewjh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mdypxssz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mjnpnmeh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fcieohxg.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pzrghhhu.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xgcuqntx.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mivloexi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3djjejktx.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3gutlptyo.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dfmxzxde.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ibesfoja.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3owvteyhq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3aydluidk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3dmkdkvpq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xqdnqgzl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zwabmbwu.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nxxipgyk.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3lyrgxfhz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3epzmzqym.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qhytldmg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qswmqhlv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtxovqu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3cnwozbxj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uiahondx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tptqphml.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wuzqnbjk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nrhxaory.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3kxtpvpky.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nrocwaee.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hfdpiodw.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pyakecis.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sjluiqoi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jbuhacid.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3kpqisfjq.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fzhblffc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zcalrnqm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gachemlj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qsyratfw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jofdhcnw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zgpfuilu.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hmuauowt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3weunbqwm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gqkaldea.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3hcszwjlx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3gueucrhj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tlpzacyt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3twklpiiu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3zdhpojij.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uoqcifqf.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lerphrel.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3npoidrhs.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3moozfyit.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cirizymx.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wddkuthe.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3whvylcib.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3vjuhrxdf.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3azouxjqv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3pfhvxwre.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3concvzme.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mipxzgwp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hgvhubkn.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ilntjlfz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ytrnvdnz.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytjvuvpz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3ojzxzpxh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3iudfxugh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bonorhjr.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvxjgkks.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uwspgliu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3syhwixqc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xarxfsug.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3toawslsv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3kksdwnql.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gxiyjhoo.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwwgfq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3vevxzkjh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwwssrzb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3svgprhft.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kitgncik.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3yrutamhz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3patvcgdk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3cxxkevti.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3swflouky.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3bimbdhnu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oaemijdp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3sannvogb.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkqkqqpn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nubamprj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dxzrzpxf.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wmzqcuoq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3epdxvveg.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3aexyzdxg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wonhtvgq.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ctwmtngh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3fsdxvgxp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fftfuibg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3pofgxvfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbnfmumq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3sjuvmsxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywxlboui.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3ysuogmdl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3mholzzxk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3dbgdwzuh.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3tfaztvnc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3xxawkxxz.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3nlbylvfr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3txucyogc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3jlznujah.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3apkrofmh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vrocavdo.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3pmdracep.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3uokfyfvi.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hcauqvfd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pasaembr.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3piwpiesf.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3jkwrjdfg.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3htfvfdbm.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xebpisqc.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3hvknzruu.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ifzhtcqt.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ifsnieux.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdybolkd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vubqnivg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtfwfwe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3lkreozof.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ucjjxlii.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmxeqfdy.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mmvegkwd.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lconfjos.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3qtesopbt.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3pgwvestc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3msgkphvf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3xgkkekkn.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bdpgahwu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3izhooail.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3npkciizf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3xsfhlflh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3xlqaxlyc.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ofbtyqfe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3fzgenlrz.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3brozjfjr.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3cmmwkhih.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3drhqhixx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rrqvsdik.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3gpjpryeu.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3uxbpbdzj.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ouiglgoa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pwarlqvb.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3cshkfdnh.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3vmkdomlx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lbvsdjot.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnmddys.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3ysmlespz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3hfccshoe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mzskcwex.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fxhtqpqf.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3ckfrtvpd.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3sgbfmjhp.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qqjsnbng.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mafzynuj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uwacrlcx.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3jswwijaj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hxquzfhh.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3leprjhzb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hatqokpc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3rhmbvheo.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fdswlzpj.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3igkvrwsu.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3syktycmr.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3qcppssgi.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iegdtckp.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3ttnjfqba.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqwqoi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gnzxvnqi.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3mydxuhhp.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ytavjrob.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3cumfajmc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3bgjoowsl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3hbarssgq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3thbbtzdt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3yqbcbuos.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3joyvppxa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ezxfedmk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3udtxevsm.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sfheuhlo.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3zbgefdra.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3ziozdxzg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3ywejjcqh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hfbuckfy.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pqdcumnf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vtpndzas.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yfdybrno.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3wbxheqeb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kmrgjsks.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vldkhfln.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwpwrlb.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3nlzkwscg.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3hcmxlhcb.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3isbonfsi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxgjbeat.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3eupxuhwj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3whprdlzo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bvkvduir.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3apyrnnwu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3sfhpdalr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wcotxhol.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3fnoxdiyr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3sfkslaon.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3qrdrcxkz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ycrrhhjm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3kmbhwoqn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxehxifk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fowshqkf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3slstgnjz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3perzajpa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3kfbeiyym.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3forilkxq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3obkebipt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ztmnoyks.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xeuidqok.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gonogdfn.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ehjddibq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3cnlwcpbq.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zexhldrx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3aeevbcsb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3noxylohm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nkoxkblv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3gbgdknye.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3plwkmjsd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgpyoxf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vfbtfult.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dkktwjwg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3yehovcmd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3rwpatcbk.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sedagrtu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jwsownwe.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bbwyabui.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqoazzxx.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3eyosnlfi.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3cmzuhtrm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3beuvdvzs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vtofunov.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kxslyvms.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qrkuzkxu.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kupqqwor.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnxiuce.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wdnxizdf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3wlxwfril.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3uuqcqgnr.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3comineat.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3aipbgflp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3mtoaelsh.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3buyseakr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mxqmfxth.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ykymfjjv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3kdgljdnu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3iyctcwty.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3edvmvhue.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ushjhgpl.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3sqrklffx.html


<!-- 参考信息 -->