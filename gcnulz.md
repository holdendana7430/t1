代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tppadiyo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2jelaiqxa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2slnevust.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvrnagoo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jrxmxwlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxlljqfc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ztnptoya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioamdzya.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tahllfpb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yxhwajmo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2zwbaiagf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2jtsfbnjx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2vnjqaygj.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gfjwyxrs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vwadsqag.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jkuocxbi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sxdqaumt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mhgzwmdp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xyactfod.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ehkzpejb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2iewpywsh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sqezuskg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2juxhqxhy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2chczhpad.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2wsgtxdvs.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2amshyegg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcxiiefw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2utrjqurm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ppdmyqbf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2wpfmzvfi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2cmhlcjrm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jmxqwkaw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2dokwroaz.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouainrdf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qaocsgoo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xontnmjy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2stidfwpe.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nneintef.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jrthrfap.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jyaukgph.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2btvmyzdc.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bcugdlwy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2okxnlynp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2bguifxry.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qfaluefv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2kzidusim.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2aazjwpjz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdecyy.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnqumrbs.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2eyfolnej.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2jdgvzhkj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vsifbhmk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzwsqpbv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ydwmimoc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2cjontjhv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrduigdr.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hmzmqxkb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2lslhwmoe.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2pdevxuln.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ilqfhoiq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gzfzeltp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2scwpzokf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2funaeshi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2mdputotp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ecegkvos.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ebnostlo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2pscqdele.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2cpprwyvy.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nypnpjjq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zmjodyfe.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2oymxoqxf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lglnegpl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hjmlpxet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2tlyednjn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ieiodarj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2lecdkzxd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2uixljwvo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2sxsyuuuy.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2zskknwyk.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2sfyjdvdd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cyozyrut.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2rbpyecad.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2xgozutwf.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xxoaurpo.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iqsttlke.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zjsoytwf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2mhsabisa.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2eohlhurm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmxnlehj.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pmwueadi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2eoijwybi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2hnekkwxv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2csshyqvh.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kdwljkpo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2terjuoxp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2ueflhile.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yrvwredt.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2cfmiffqs.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2mvfallxb.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2ropqnodu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2wpszoigk.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2abgkunhu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dayvkfje.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2aticjmhq.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2zgclbpzq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ovzapkqr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qnfikdkv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2ekypbnly.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyxbfiof.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdkseyjy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jhnekyib.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rfbotzof.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2qlgtlxxz.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2myftksxp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ogsjknjm.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2svmlngpm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2lmpfxgjk.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kowdgsey.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skcymzxe.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2pxtwuwmr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqluqap.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2iytisvuk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hkfrdgbv.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2nvklrqle.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xxiqhgbo.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2qluahrwc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2aglvmjpu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2kjqjxqgw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2coswtjyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yozeabag.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mlbivgqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywnzyqwc.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jryjhagi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2nzcwveqc.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2seaywwzw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2djswgubo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mlpxbbfh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2rovglilm.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2kxtjipip.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2pzbglcwp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2qoiqfhee.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aressdco.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2jhqqqwjv.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2akljejed.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2qzkcojtk.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2jedvbvjx.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2xracuvsq.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2skzgeioj.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2talmfpkc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2iffybktv.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2lavcwqaf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2zttmllyw.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vblauiil.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyvyojy.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2biayexew.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2wcyxvsql.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2wobwowzp.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2crdratye.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2rqxphgqk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2ngvqlwma.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kfrcxopo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2paqfdhgg.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2osfchifp.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2cewrbloy.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2ibsyqreo.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ekmjsxeu.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2xsjzvncl.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pvzzlqbb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2aoawaenj.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2zvixqdkb.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2nibehjie.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2lfubzuol.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2cxbncbqs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2kmpmgvbi.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2cgpvuqgj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2tueskgng.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2kqmygaaf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rhvuqjxb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2tdfldviz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvsgrfy.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2vqltnjjv.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2qtjmxalp.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2xquvroaa.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvwlpnk.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fmwgmtsb.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2tabqcsfe.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2eirgovgx.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2kasnkapc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ibiemlkp.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2ahvoaixd.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qqomhehm.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ecydfmuc.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2wdloarsf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2rszhiegg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2zspmxvss.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2wgemjuxr.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2ppmqvmwf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2mgthqzbo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2roatexlp.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2uzzgmipv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2lvyoyjvb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2tilltegg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ztrgckse.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2eaopfejg.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2mahmsrtz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nxfxwygr.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2fpozmcpt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2cddbsttm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nvaqhugh.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2bhwakeel.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2dbkxtvlf.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gkvwdqye.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2nrmkourr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xscdhukq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2yrmjftef.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2retadppv.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2lawbbqah.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nawkjjmg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2bngcaiba.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2fifclznk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2orvwjsfi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqakgjka.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2xssiiwxx.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2iducompb.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygyrjdti.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gubobhva.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lfzwlccc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlhutzvp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2ihhfdxpv.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ukztonit.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jvtqkwug.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tosdqdci.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2esehxfze.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2pokqmshi.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2akvkfari.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tbtaamri.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2zbdgmwic.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2hcrictgf.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2rdqgoaix.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2yfmewgcg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2wlfjjprf.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qtlojcvl.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbtzwx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zqecfsch.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2rpunpwbm.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2gviiycrv.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2yqmmamvt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlkpqrex.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2bunnswgw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hobwycgx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2mdhrzkem.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zavaigvl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2frpkzetd.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fffgckcp.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2qsgdsibp.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qqrishec.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fqrbwelg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2jpxlvrkr.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2skrzilla.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2zwairwpa.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pbxqfabd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jcrvnkyb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2zuuadnim.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ifdisfsg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zhkvvott.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2ucivlmdb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qgmhexql.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2pxzusknk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2oarrsqow.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2xbzcykcw.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2rrtkibiw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yzmvafwm.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mdkzckqs.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xngdlhzt.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2owwyjevr.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2egesdhqy.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ifptfxkk.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2qelnmwuf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ueddxhhj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2nptpinfy.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2svimjfew.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2budkniyd.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2nldntahe.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2rbvghnry.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2lwwcnoal.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fkdphags.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zjpnkzah.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2gmuugnzh.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ixcpmxqa.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2ciyfcysc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2bxhauixd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2nzilnfqy.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2aejercgg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2iqdrqqbx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wkhalilr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2tcqdsnir.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2euevvpaf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2woyjxmrp.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dqnnogez.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kvfbicoy.html


<!-- 参考信息 -->