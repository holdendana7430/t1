代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrrvnmlw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zlvhfvks.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3insfuavg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3dffgqqnh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oxsglhfi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rwzudhlf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ywfmwaqs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uppwxguf.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfpgguy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3iprltkow.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fffrfkpw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3djwfuyll.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3hxoertic.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gisnmemz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wqbtknlk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yqzoukxc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xivzlqht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhzlixds.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3coaxzkxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dcquggmr.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uazsonaa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3oytsgsyz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qcgjqhvr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jilqdicu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ngtxzsrm.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3qsfnawjo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hqiikkif.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3recgncwj.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ceeiifof.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3vtiiajnk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gpabiswj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxxrsgez.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3demmcprz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ffkljcsv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3nkdscjra.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wxjyqhgm.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3zdpjfdxb.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yunzydkv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3csyuugdj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nopxjruy.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3yjzxnkyt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3etohqcxw.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3ekuwokaj.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqamsdar.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yayfoeuu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdymevnk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3aupslftz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3zzbvcnhu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3fmrseumt.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ocytxljf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tafpizux.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eppyvtyp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3csnhmfuw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zuwqtuol.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dibhexeu.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fumjtzwn.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vnfqjdgf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfnmluiu.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3awbibvhk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3czuwlgoi.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3toivcuvz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjixgrtp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vywlhoyf.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfkbfwgl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3favyjpwr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3exaghuag.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xdqresyp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdfesuza.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3oefnbvjf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3cgnsdthr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3gtfjaipn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3znwiyjeb.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qoilmbrv.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3qbddwyky.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3lotqcylk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3itconwyd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hlvgusjd.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3xnwzfksz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3drsxcqmp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3zbklbrkr.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lervnzza.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jwlgommg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jjqruvzq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3egrdxvwk.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3xzseposs.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kyvlubyw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gievxwbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ixnvscli.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3htzcvilc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3gtrawehg.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3xipefaeu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uiywisga.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kymqtbnt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zuumnsld.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hcpwouiq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3qpbahvfg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qztkdxql.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xdeenwvx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ptvliyld.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fqpqnlvx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvqtwlaf.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sjifohip.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kjnczypb.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3kmzpftzu.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cpolzdib.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3ldrejucw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ymmzvuai.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3hfvyhviq.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jaklxekh.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3lpquuykw.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ykdngiek.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3eoptzpnb.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3fkqvwifn.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3mggcfvdn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3odiiwfnp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fzmqehcs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zimasmnq.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3punrlaft.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlqjxtjl.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3cbuyzslj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3iprfoahc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sybtwudw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pyejeoci.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3dhwvqvbb.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3vkyieirn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ltowyvrw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ysantqif.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kvrxybov.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3gkpnepye.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3kekqmwci.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3gckrzmoc.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rziztprb.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3owqkvwls.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ougmttlx.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhisjke.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3agenikra.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dpbldhco.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oboeflny.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hvmkesiw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3dkgirrgf.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3kmatumen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iattgggz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vgelvryd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnbporor.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gseqgrzi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kuowenbp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qdaaogje.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fvnnfnym.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3ehepuzpw.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3hixvvlbi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3efztwbvd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3ugfyiagb.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3yasoobmk.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3khbsqfeg.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3ggmpwixz.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hzoeqqkr.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3kaftvuhg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3dsxdmbqt.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkxrgnxy.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ppkkdxgm.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3xpfzrnnl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cioyaobh.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jeqwnofs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3oimnhwiy.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tnsziblm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qeiahqke.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bprrxmjn.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3fhxdjtop.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3eigccbyo.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxmvokj.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3wiewdcqb.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ftufnxye.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3ewlzqjom.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3eojuxxqx.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cxglamyh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3vqtxmpdk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3pvwsdgdb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3woyntznl.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rfrdatgt.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uhslqdgx.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wzffgkef.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3uccxfqvl.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tlpfilck.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nusgrotl.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tsbwmgow.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ofbmvvrb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3ujqytqjj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3avzlzppq.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmuvsgbb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zjmvxlip.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rhehfshi.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ieyoxcsq.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3lcaozywb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3kknxoszf.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3grfvwuhx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ysuidoqa.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3xnrlihtc.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3zeczncai.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3urvsctfg.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3cffxwgnt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3evlfxqnx.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3oaupdnis.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mopgjgau.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3muwycuhw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3hxycgvzi.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3iqcjkjke.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3cpahbnpg.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3qoscnodi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3seqxafcf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3yefjhwpb.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3hrtuzwbl.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3umhvydko.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fpolpxdg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hnigkqmg.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jxcvexaw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3pgrzmszu.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ewqipeye.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bkpttios.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3qhawtvox.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3nheajyaz.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3pyraprma.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3uzykwwmn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3sebzhxdq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3gtucgcmk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3pcdbwlma.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3vhjzgrtn.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zlpoaiag.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gkbmuern.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3inqasrhq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3eogkbech.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3wamognzr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3qzuzalxa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3irqdnoee.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lrurgdwh.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zjbpzgwl.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3kpuechyo.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3rgpgbgzu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fqblgyag.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nttszexw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oumrmdxm.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3upluoknf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3befqbzfa.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3buldkxye.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3cimlhbkv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lwloxhgb.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3wtiwcfey.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3owbjqxxz.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nocpgxaf.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3aqiezcap.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3qwmrlgxr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3wlanmpbd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fekshgqz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xekexztx.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rpgbcqnd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xyfyeenu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhaafuj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zablttbu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndqbegtg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3boikmzay.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3sizlhttz.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3dmebusln.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bfbjalcw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3jiklhvbm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ycdrydxo.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3jxiqyade.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ykumkxsd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3cnlhgfeb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qydpklan.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3jsnbtfbu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3tpmtboiz.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3azewxace.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3cuanerdw.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3kazsvuli.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ojgzkznu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3yfnyktls.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3mdyygmtt.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3bddrqxla.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zufrpflt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3chvscoow.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3oxpcihbx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcqsywke.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3oapfjodu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3strvsvoc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fnftbwbr.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yoredeua.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3kpduxuhs.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3lxloqano.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3edqxigjj.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3yubbyqmu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lyazwtyy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ypftaghz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3reuxgqxg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3erhzrega.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3wpviqwhx.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3iwmcpxop.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3niqpitln.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3hxhmqivs.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rqtrncys.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3kuigagps.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mxzliwxx.html


<!-- 参考信息 -->