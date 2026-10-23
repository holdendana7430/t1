代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqeeobnd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mhlzeedq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3xkgegvrm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3cqzvxsov.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3pkjmpoiz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ytisfpjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fajnzkjp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3levvvxfe.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3sxfljsxs.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hrrbhewc.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wfydmjvi.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3srnnwwqp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ngetphsu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fxicrmtj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3oemozasm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nqzazdgs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xkdqeczn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmfuouxh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3plqzmnhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfkujlyh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3djohmifv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ojtjwiwr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3rsutgkxn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gnxsrlph.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3zxsivsnj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3etkplbjk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ztlnflwr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivzrzvdo.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3idbxejpu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hmthnjaa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kqqaoiuz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3radpejuv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gpccasur.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3uoecwsch.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lfstjzuc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3oqlrhqfu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3rakneizn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3vsxssuqc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmukryeo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ctnefdbm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3kiezjcfn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3aiugfibr.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qunucrzg.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wggjbeew.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3insqrlxu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgenbivc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrfammew.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qdlyjpla.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3dfgtkqtx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lktinjaj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wzxbngrz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fowoflmk.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3azeibtbo.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jdjoavus.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3arbmsjzz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3wccqgevx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3grtotsmv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3telnsztj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ohphlxes.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3sicdeipx.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3esgqkyhx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uctlcswf.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ygpmzrcj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cplfnjai.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxhkkjbl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bqxfuqzw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lxidjvcx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ikcgwaig.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3oguatkjt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lylwxitk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ydyosjtm.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3blemalwf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pftksppx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3bgnenagz.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lxkngict.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3myylrvwc.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kwrekesq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwtqzqd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3sjvuqoaa.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3wvxazycl.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3enfummmw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xududmwu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pjwnqqxo.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnoudxyx.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xuvvzejs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3wiplffrl.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3pomyfmgp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3lgaesdwo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3kaxnxcel.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qussawls.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxwbha.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3coliylte.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zrieofhy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3hurwktly.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ykonitnm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3gxrbdzjt.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fchdgkyy.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fmnzafvl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tgwczimt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3erzbihdu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xpoafwtv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3xkcebmql.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3mhvxisoc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hnzsxwtc.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lgaqfqku.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3uafqnvtj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fulegizg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgmnkqiw.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hzcaucjs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wprrmqin.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3pkyfdwiy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3xkuvflxp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3gqkjvbux.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3zvhrtvqv.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3fawxftnt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3poxhbtdn.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qiopvkng.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eghbbqfz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzlgozhy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ivwzzwxr.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrnbclce.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fkticrzk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zrdyzugs.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ohncmklz.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wlujswjr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3apskqtln.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rnuoeszd.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3spmvsabv.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3xrmifoco.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3pfaghnxa.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3zdsdmbii.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3malnlljm.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vkmcgkni.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idshiail.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kwlnxkoi.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ryjkehnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lxltpryb.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pljnvnqp.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mvskzyxg.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wmkqgkvi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3kzhmlfdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ootapztn.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgtbtdcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dabjqoep.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3djyzzlsd.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3wfdjhztu.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3agzwrwhm.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dbhwhlqh.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dvewkznx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3jlljzqcr.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zwpbnrzi.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zmzhbgmp.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3cjutuwnu.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zrtxwhok.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3qjyklhce.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ywfjjbem.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3vlcwyicc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3znulbfat.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3bbhkjuwb.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3haxkqlkh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3dtgvzppc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtahfjy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3fzyzygkf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3krjsyaxe.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3copuotiu.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3nrikfcco.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3oshdvxfd.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tknxppco.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qucojkns.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxwcvod.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3rkadtkvi.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3sfujkbfi.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3rafnqyds.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3legigwam.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3rziihbti.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3buykcowe.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3qreerjhq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3rndzntsk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3prxeumjb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ylhwnuco.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3qqoyohvc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxikasru.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3jkpgxkro.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ekazizrd.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3itbfgqoa.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3vdodjipd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3zzdgupju.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ylpxfaup.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xmakpihc.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3aormykoi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3wfmtmwfb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rizxirgx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3lttzhqvy.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3oofujkfk.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3scpmalcv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3yoagnisp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3atovajrv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3favutzhe.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3kjgspqnj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3ndtssjvs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3wrcgmynu.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gzmjadfo.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sobefeex.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3hunhjinu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3amdagwyx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yoxqwqrl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hzllxavf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3nhxkxazp.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jqqkgcku.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3lilzdxse.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xbrtyphp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhxhign.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3gzoaopqi.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3hhryfmxx.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3klizytwf.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qgccfrfr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sxakrkum.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3hadbmchg.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3dbhfpkdt.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pebsocho.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kktzejse.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3gbvqhahl.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3odjlhwgc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fihjojax.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3xcpjyfwl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3zbhptxfz.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3bnmnzwmc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrtblgwq.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zyxwbdts.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3uyyloxty.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmgfvuel.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ondflpol.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3fksbtruh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrlllfq.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3huudrlep.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dqqesxgx.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ubuiimhu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pwwgmjhu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jcpagdrh.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3xiqrgcjg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3asafbddn.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3leuiggpl.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3zymxfsnw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3kvbhebew.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3izihnhlw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3oedeuzcv.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3bkltzhsa.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qyivzxlt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vsxialiu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3dmbvwvia.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3zhwvbrqk.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3oxdmhwqp.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3trkvpcat.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hsykummm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3zyrqbwla.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fgarkyqc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wnvcdppi.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvgonqhz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3cnsirliy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jlvvdhtg.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3xlvxarnv.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3otofctmx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jczcceku.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3smvhbbwg.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3bcsstbjo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wrkkoman.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3trayzpql.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nyimzaci.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3defjfeeo.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3qmtnfkfj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3pacwrfti.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3mserigjf.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3xegnykte.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3szisobla.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3jrelajtg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3gzbtarcv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3ronwevws.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxrpboi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rsgcikmt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zgpkordj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nkzupieq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3wawiujmp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vrkcpvel.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xhcagjok.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dxdblxfc.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bmiwyukq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3mflmcqxt.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qvamylzg.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xzflqkgq.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3shejrixl.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qtackfal.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3oohgjexw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3szuqisnj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3wavdjrdb.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3eluvjhoa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tsgtopja.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3uzjpyxeo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3ojjfgfwf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tkioalzp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mqlvlxwz.html


<!-- 参考信息 -->