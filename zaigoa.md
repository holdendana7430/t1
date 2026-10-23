代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvagrgkm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gzaiemcz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tapltlpi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ewngknsd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3svrhqjwh.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mjzgciuw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pmujenrj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3exokbexv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jpiqpcop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgzeyfgu.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pgrtflhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mozsasbu.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fkwgxnhe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ityeegov.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gaodxohu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3vdaknekf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3puqrfbwi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nxppvbwo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qbzfemcr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3byyvfebu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lueqauqd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3flwlumam.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3wqltjwln.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uedqexul.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mzyhaaao.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkptrbim.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zrhumvuu.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3hzsbwalj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzsxtlva.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3apgkyesg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xerbgahr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3sqmwfkrh.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3tbfxenql.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3drglwvhy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3dalyircn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zsljzxvn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ppzptqcq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3kvomsyyf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3qephcjpj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvweafz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kqozcifv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3nmpijzyf.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3suddmdkx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mrnggujf.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3eqmsvhfn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mlmrdraz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3imovtpau.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3afvckzdt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nopvhwzh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3wybebpaa.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3xfbrcipe.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzalapt.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3bsokyrbt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdpekvou.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3anhuekkc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3dewrxkgb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3anxychbs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lipqogrg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cojuzmjy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gledmtph.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3eproipcl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxrbxff.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3uxxllmgn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jqwvozsb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mwvezzhd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vugpwoaj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3dnplqvnv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dclnhgwx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3tergylqi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vlhnzfed.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3zulwxrby.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3shxnzlim.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gstillcv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3jsjodzwo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ouoajege.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kimzznxk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3qqsxmhfw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3vakilkzh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3tvcofnpi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3htaetghc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pycggjra.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3kdoizhgi.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3gescuedn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3fwemjrix.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aeodelbo.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vdcxuniw.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfepmegw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3pwbdspmg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wlsbvyfn.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vepzbxbb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3iyehrwfs.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ihvnvsly.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvrzqzzt.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fuvlfaiy.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxlzcnkq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xsdringy.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3xxwcpset.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vlusbujr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lxqpmsyp.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziotrycx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jpgxhebl.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqbfudx.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3eplfvbya.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3jhiecwap.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sdxamjwy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioikozbh.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ukfjyhfy.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3wjlsjptq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3njmtrxha.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3faslguhr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fkzkzben.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3xesxmltl.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3kqwgyrwh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uixoiaca.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3nunpaesr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3egbbyquh.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3okxnzzqq.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nwfbkoxf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3desqcpkp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3symjayjp.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3olizftgv.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ezuoprte.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3nmoaliod.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3knalyzkx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fcyltfyv.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qxdxpgip.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3dhlsmkns.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3sznmknes.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3iosbfpai.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3pyyhugvh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fcqfvvvi.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3awhzxfzv.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhghlzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmneaqbo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fcfrxdpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seceiuwp.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3nlieadwz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wwkqnsgw.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3rxhyyvas.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjadfsdp.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gcvbhdyt.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3fingvovv.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3owutcrcu.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3wvaccyxk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3sdatghbw.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yfdlqtke.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3erftiziz.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3mizjaliu.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3sopeygiw.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3xolvsphe.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3oaiftbyn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jsnxknin.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3fklvxcig.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fchspjuu.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qyofhjbe.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3bcftxeyy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pirbvppa.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hxmvfrbz.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmhgxhpi.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdexjlct.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3nyuupqjm.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3kdvebtmv.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3phimobci.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3alcaqnqp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rorwoadl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gxjeymvn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3csbwbsoc.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hytkseql.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3jifmtali.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3lpnwjmlq.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mjlacjuv.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cekrjlkl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3szddcobk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgunixha.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3erlcpvnx.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3hrcyeemc.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3irlvawhk.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3fifbsnqr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3ggcwbgla.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3eycdzyma.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjptlrno.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3fxnccmic.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3glaczipd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3avgwuiuy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ekquhpbo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3qmbejoqv.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3gqjyqmwn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ugwvjdvn.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3jwkhoicz.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mxrrlyvg.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3kybpchob.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3vnezcofi.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3heravquu.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3hapirqea.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3tfabpxdm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3aanfqjur.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3ktipoubt.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ifsznfds.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wsdkfwvi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3kaooyefc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3foagsunt.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3pongzhrz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3kerhrhpk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3zrxxcgru.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3yomyplau.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3zncwapvd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3tljcmjcw.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3szmuclua.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3acnabfpf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3joozbapa.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3irflrxmp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3horzlfdm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3cmaexwxs.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3tsvxbbrv.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3oktptocd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aunnkzis.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3rrnxecum.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3nivdlolf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3chxvvexm.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mcfkvkqw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jfrcwzke.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3amvvgcxa.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ipjkvjgo.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3fzxvlzqu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3crxcevdu.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fmdcyuub.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3tahfasjc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3uapwesbf.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jtcocvao.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3snfvzehc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tmvriuis.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbkawaah.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3uqagmhxl.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3vopqxbss.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3fzieycbi.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsisoxgy.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3cxddenlu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jbnoqrev.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsmhdoqt.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3daewkpmb.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jqdocddi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3aeubwfxc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3wlqwfnkx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3uaeuorli.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3lgbbxajy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lepsymqb.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytrgjtcc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ishwxhly.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cklfynxa.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3gmwkwvqh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3izcpogwy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uewugbhw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3uidtiouf.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xvgzlldm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qfibrrho.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3xodvdnbt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pqlsvmzg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mabvefnw.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ruzndzmm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ihtjhghg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gyxgcgyp.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3fllexlga.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ftgvdmfz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yjoloqao.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3rkjwahzj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oqloobts.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3isdhuzuc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kaacnfur.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jlwmnqtm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3gpkpbumu.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hfyjnqll.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3kjozairm.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3gvfesasm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3ehfzjnfl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wahiegkz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3nilrihik.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3opwemoln.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3mhowqnmn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3tklbhusy.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3xtswfmxg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3lqvrmmeq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3foheqdzk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kmeajwon.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ggjrstwz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3seqgkavv.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3czzwjnbe.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3ohlkniqg.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3fstllhqw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ioxtdfum.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3zvfpbrhi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3chrcgzai.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bpkcosra.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ophchbub.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3bczwfpff.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dsngzwyv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ivfpprhp.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nrbipfxn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qxufyami.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3omzppwne.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fvhwmxnf.html


<!-- 参考信息 -->