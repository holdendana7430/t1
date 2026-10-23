代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3djzeksle.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3eqdsdvry.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3qcwulyof.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uztmsjhk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3unntorky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbbnagso.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bxlbgjnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxmvhzhb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jocwioiy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ayejtiri.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lvigwxdj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wrqtjrym.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cbttsagv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3opvgchdg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xkipjena.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3msihntql.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3falcfnzw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fhrmaxbu.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3jfstnfkq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbssfobb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zhzapwmm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3mmqxnfbm.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3llmvlvio.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3iuauyajn.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzvmazmu.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vcgonffe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtnquzpd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ywvmbnwe.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3gqcxlkpv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zqqpvmpm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3pggjuvrc.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lztsrazj.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3mppvmklv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3nuyiddsj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3xqrinthc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdfylpc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3acxvmdpm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3atbuzycj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rtwaaqjc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pgoxazqz.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3kyfbeslb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tuvdfkjf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3eeaydemh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eismqyrw.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3riqlyqkz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hfksgdwx.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3akirniyd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3yqmsllft.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3rkkhglye.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3omgmqvkz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3nlubteit.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hhbzajon.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3crqcsclt.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tnchqvgy.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kqlekgjm.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aelsbejh.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fujmgvbw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbieorx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vfbyvfju.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3wecgpunq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3edvkuegv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3aidehbfc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3sqjabwxv.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3dzvqljzx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3awjkphve.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hudbjnij.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3fijrlvwk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3sfxngaki.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yrucaqzr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rryykhvr.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jjrhqhxx.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vktljbwr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vsoorcub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3nwazubuo.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bvblxybz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3yeducwry.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mejocxjh.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3trfacomo.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3hdnudbvz.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ntkvsysr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dxglvfhn.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hgmalmgv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qzsaxlbr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mdwfbxsj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oiamgdgw.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cqxpkjas.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3iauxxrpw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3orsaoeqd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rvgnxanh.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3pppnuqli.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdtvll.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3brlbneal.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3rhlqrjkl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3iokykdsc.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3vjouqvov.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3irnsusob.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3khulvswd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvjfxujq.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3roniqqil.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsxcudnc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3pjrdhlrb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3dlithvzw.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kehvutka.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qrxfsvpv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lsqsocov.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3anhqblmo.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oxguiheh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3prslboyq.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdufyhrk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tnhpetyv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uzvxrfie.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtqtdkht.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kufmlwkq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cueibekt.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkzmze.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ixxhsulo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czngvmck.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3giyfecvv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3quxgqldm.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ahhwaigs.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3abrhxrya.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hcsbcznj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3afdhnmiz.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3pkcnjqjh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qalbwmck.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3fdjmkrhp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zrwypdtw.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3amsldoez.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3nmqaeaxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhcjmuhi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jahivioe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkszoryj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3fgeolyzr.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3wvfwvfnf.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3mnzbgzts.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3clpdeykv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3idovvuhy.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rrhabizg.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3padmvnrl.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3mvowpxeu.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cpyhgbzz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3uuegxkjv.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3rrtqqtqb.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3svxdxzyb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hovlogar.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3ebskpgoj.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3fynnpjlq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3aybkqleb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3nmftkbsq.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wkknktfc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zentdyrs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3mviezped.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xtfivxsv.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3inkdiuyj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3zfsfyfon.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbietazr.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3otdlanzp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3jipaqyei.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3asapezqv.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfpvjev.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3bgkypvdy.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3kdzjswxi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xwbkoegt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pstwzhvr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3puizzjfd.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3zqqvvjyi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3xzsabjgv.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oauwgsxa.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3vlbrmmnv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnyqvbbj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3ybxthrtu.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3aiwnlpmf.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tpdaoviv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3pthycbxx.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3xcjfkbav.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3fgezskbg.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3mxfchbgn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3msfsipjn.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3vrswtoio.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3umegxpjv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3oiiplpkf.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3jskztunp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ifhhvkae.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3qxdytiix.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3rwyyagcg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3jdtadfrv.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3zjqhhdyb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3hsgmiqiq.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3poggqsmy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3iumghjyk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3ljyzxram.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3njwwkxoi.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3cjkrsxhc.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qmtotyrv.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ycugjscz.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kqfcuvnk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3habinppp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3ynxrcpgx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kffosdfy.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3vbjcwvhq.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ljqbejjp.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hkggllal.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fnnpvbwt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3jwpfokrs.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3yujzwljz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3dtdneqfp.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bynhibzc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3alsfjrjy.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ufjngvvc.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kofkwlgt.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wzzadkvn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3obaqtmwb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3onshzbtk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3fjdavfnt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3orjmgsox.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwxnhjb.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3hsehpvaq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3yfydcjxo.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eccllkbi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3qilgxvol.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mheqtlhv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fzufrbzr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3zizlwcvu.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3aumgfrun.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhauixix.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3nlmzznew.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vdxcoyms.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyagcwru.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3nlbhzqsf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3bkthykvx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iinsiiej.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzlygkwn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3qnnsewtg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qhqrmoam.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ywnirhzp.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xrdfnvvi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jieltfhp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3oxykfxwu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3qfxydfiv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3hcrytaon.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3urqakwgw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gunepxbq.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tvdppruy.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3baeyosck.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ntjacjba.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3nyqyzgib.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fiuvukij.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jprrhhcs.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xkbyzltn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mnygmjhv.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jgfxlcpk.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztdjtpoi.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3mrfzogog.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vwfcrafm.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3azjftcse.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3sqhharwd.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3hwfjucki.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3hquyqqve.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3soffxrsb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3shczdhpd.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bzkglggo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ccsbdznr.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3imedmsuq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ahypznyb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3mionodta.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3noeuewyq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bfbmrrob.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ljjqcacc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3yfacxqwj.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3coztogky.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3djajbvrm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ypncobou.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mhmijzhx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3gzhmofgc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3hxecfluk.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ecsssklp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3sagulkbn.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qfdgxgsu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xhnxewqc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kvxymbkk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbtjsg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3agcaidkd.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3awenndim.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zubmifgz.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ormydejv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tnmcmcsi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fndbsudo.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3woawzach.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qgjrlnkz.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3feuqacbz.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hpxeinhs.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vbomrrsm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wqdjcluw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3vbgggruq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3jfwsgedd.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3laebajot.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3murhapzy.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cgutgqhf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3rggxnpbb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mpmwhkku.html


<!-- 参考信息 -->