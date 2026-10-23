代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaocqyct.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gzlorirx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vavqlobv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3qocjsqmx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3snzgromh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gghnkwyq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jxtetdbj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3jnwggegb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vgcdpfvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvnvltfa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rpkghbty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfnuxxko.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gfhnuxea.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tniqdrhu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3hpakpcms.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lgixdsxt.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3figgwuoh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qnlirnni.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3xjbqijfy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxuyuxrw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3zkuibajh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3kawmbtyo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3lywlejiy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbxkijrk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jsuifavh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eyjbcmjy.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ajgmnsve.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3tbeospqy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwelegkl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pkxpjfpy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zjxuqxtl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3zyvevnrl.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3tzuyjkjj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3lmljcums.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3kxjbmbcl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nsbwiehh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mzcmsfik.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dyoeaqip.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jgrvbkmm.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hwmjoxzm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3iirqtrta.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fuhfhlfv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lcotggzk.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kiwyqrjs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rxfgjieg.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3wbxjeldl.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3stwoqflv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3yjavesfq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3trotgvba.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3asckuqri.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3aukwxash.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uoykbvih.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xrlptitx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wimjwszi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ufcuvwmh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3pulsjpeg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3iayvouzf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3swmsntch.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3rbigwkjr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iwcnfleu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3payqxbfj.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3xahwwjwt.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3nccpikxb.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ucsmbydt.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kbgawoqe.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ozmxmxln.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3thhbddml.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3uzhznykp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zgnnajvo.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3fczxpgxk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3edvzfhgv.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3djgxlkko.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3coilhlmf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3inuqwtgq.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3puzcukmn.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkkjbsfv.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rmioriah.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fryowzaz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3eeisxlar.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3aicjphfz.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3exhtavqi.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rmnkiffx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tisrxpfp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nbmcfntb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xgmtprrz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ybikhjvg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3igtbpkeq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3yqecokdv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qrtskfqf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zvcmoyvj.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3spnvgnxt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bezddmvj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aypfotui.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gnuidjqv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qppysmkf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ckuhbrki.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3maooljjf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3lzbmxnuo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qksfitqv.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzjhbzll.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nwusxvoc.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bireqmcb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3xaobkowz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3bifmgpxr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3nlkzrovj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3znepwwqk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kmiuqfhm.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3btrwqwfr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3dbrlciow.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdhjju.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqhudbio.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3enwuqbuk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3bpksrewq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tcnxbhsh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kbflysie.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mskprvmv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3mwfiymis.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wwtyaypz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3esvsyozw.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uonmqmfx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3komniple.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3axachbkv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xmjhuumn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ojxrlpzu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3smceslrs.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3evyakfkj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vctvnetm.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ssfadwhs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qqaaarvg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mfixilka.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mcflmazf.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3lfjahgzp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3inglrxqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtqlnsjb.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zsybbhmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znyxfger.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3onwgfewj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3hoglzfiv.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3iyqeqdmv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdfxnpce.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3gnqojfdj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3znpsdfyi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3klruoukn.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vuftrhml.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3gwyvqipp.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kzpkynyg.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yswmdsrq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3qxsrvogt.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3jjoejqix.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3imglzhhi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qzmhkmbt.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3zubdgxar.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3gxodpyko.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgdmkql.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kckygloj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kdtamtfj.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3humycdvh.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3uckzywbi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3mnqbwjdy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3pxiijwuy.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvwfcxef.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3odqqlana.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3bvgtyiih.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3jegytzku.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3bdrggwrj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3sbsupbve.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3xhcwfwwr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3myvrrldz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3bwfqjmkg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3gugzwowm.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3nffzkesd.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ugbjzvim.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3vofxjrgy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuxdtavm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3oihabrgg.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3giyrjuwh.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3nuanemhu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3vcmigeqk.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3eunydfye.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3lvkzaabm.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xkrdmnap.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3mmlxrmvj.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3uezsqdsz.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ibcrecdd.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hilnkyjh.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3qknurosn.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lujejatv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3itckywxn.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3mfuepgfe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3aodaxcct.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yqzadtvq.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ftujwaht.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gngqsthf.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3jlxleexo.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3eocgjstn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3npdclcch.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3dzremthe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3psngzxtb.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fgxmvvds.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3yikyjjts.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3dabwiywq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3fneqyscn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3xdgxjwnd.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fufsdczd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3poapkshf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwjsrpq.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3pdbgfhoq.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3zroraesc.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mnseqzpj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3kanshzre.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3gqbikawl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3oiaxrdyk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3umrqiylu.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kgnsctao.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3frhzcdsv.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3guwauxur.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3njoxista.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3xthkdkav.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jpxvrddg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqvapkep.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3doyrkwwv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3vsrwklco.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hkrrargf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3hitejsne.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hflsspus.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmeyqmqq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ljhikfxn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3dgqfrjao.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jreivhqz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3cetntrda.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3skksidcx.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rvlkditw.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3czahmjrh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3wfmvebza.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tiqnoowm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efwchglp.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3jrlofblq.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxccjgy.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vcwjdjkk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3brtsqavi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3wrykoaxl.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3saswozbn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dhrudomp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3dvzrgyti.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3vdumlnuc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3amftqgwo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3qfganhhn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3imejgelz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3spzirolj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3poimyizg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3jqtlbyvt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mapoycir.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gnzvxkfg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uvfcuklg.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jacxiczp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvgaqo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3zplxscnp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ncqdlmpz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3yzcpjodx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3stpeysfn.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3xtczxftu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3lzoizhtw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jvtghduo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3yngdfzmv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kumniwtz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgdwjwkl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3enktcudg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3kvwwdwux.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3qhukprlm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3cjbecpno.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3uwkcqkeb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qfewxtdz.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3udhqpfzd.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3yntvqykc.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3vlzgjgnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3yerjsbnd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikagndar.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yzlwwarg.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3rjvrzkwv.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3cpsbwack.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ktelmjjt.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ssqtdita.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fehepusr.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqtfqz.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fieckclk.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3dasveylw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3kpxbpgbn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3tasehwpf.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3iditcfiu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qitfifvx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3migwyqyn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3nogmgqec.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3mimqyack.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jasxprtd.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3ezkqyyvu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3qkwvtewm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3yahqjxul.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qxwquzrf.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3yykllcym.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3awdffjth.html


<!-- 参考信息 -->