代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2elfrolmd.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcvsmyyc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pohfhpdj.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ptumctje.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjgtvlxm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sjpurrpp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2eljsuvmg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2tudqysqn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ohcnvqyr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2nonfzjda.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2nsaexvsw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zereaiyx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gymxqcmv.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2sykaqsar.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2xhgsqezw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qkkkqank.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2htqnzxdg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2tkjjntvx.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2khwotttl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jztkwivc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zpjqvhig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rooxezkz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qcybicvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqwauwwj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2paglhwbk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2egweedus.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rgoetnma.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2reyaddim.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wubuhwdv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zeavoese.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ipigxexg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2yfseqrut.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2oacbeatb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2ydgnglxs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bhpzjycy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zmcxmtnu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2qenqxrxn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qpeptifi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zzpjyrdo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwrranx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vslvhdhl.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2zdobobue.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lodulxxa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qvydezga.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2jsasyoud.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2dglfwwbc.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tnnjpxod.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvgbsnll.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ebnmkjrv.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yshrrnms.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lrmaooyn.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2wrltjryu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2beqecwqy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iacjzyex.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2szvzzxkl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iulonfbw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2umeveqlx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2bewmumcx.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jxjmvaxv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2vnpxwxwp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qwnlyoxd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2uxtujtle.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2cslfegfp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2phontbjz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xpeuvchg.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2gfjymhow.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2cpxnitjx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wnbzrbho.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgenlduu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2nvkrlift.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kgdgncef.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yvwnlbdh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2cadqvvtk.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2gqfuuhbc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2irjrwjla.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2cqrzjzht.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jkvtvqjs.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2kqdeeqdv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cbptoyjk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2reocnztm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kcnxwigi.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cyloimwh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hqleamlh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2usrjgzul.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jguwkgrl.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2jxvsdtdp.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wafwgyoc.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2viinigaj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2gqcxxoyy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2mmrjnixv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2zkxdqjnc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2zqlfqxni.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2guapkcmx.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2qqkkamwd.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2dfnyrhbe.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2teyowfvl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vmvdcsgh.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2omwdgwsi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2wyduxjsh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2mhihdosy.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hysueaop.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2whzruukj.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2sjkpwpxd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ghyjyqho.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xmrqqgqb.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2kimbgywa.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2pdpwlipt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dofedlws.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2xxyqjsow.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2oysukgyd.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2txpfucni.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2byjmpwbj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sllmykog.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wlnyrjvk.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2gbycniti.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mipbaqao.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2anwgcsvq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2icghvgfh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kiyqtwxw.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2jybwbbge.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2pgejanrs.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tkdrxcxc.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vmbmvogi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2xdudjrrt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2fknaujbf.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vijwhjbm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2waizilur.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2akynhxbj.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2wfqinvxd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lgjxezqp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jkhdjovq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2njekvduk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcseponu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bbuzsrrh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rghtwbeh.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2togfjmjm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ktlyybep.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2sfryhajz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ztnhapne.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2gfzjlmbt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zksnublw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2jntyjade.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2htikyqkn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2ljgkengx.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2nolvbnis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2weihcbuk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ohqltdwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yneddewj.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uuqfxkfq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2gawgcmpx.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2pibydmcv.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2vsjcpwvq.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qgrtwgkd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2srqzikvd.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2biwxhzve.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2ettewxgp.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2pudgcowt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jlpxdvjd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2rwqjdvtf.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2bauzxxkm.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pxnyyagk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2sjkiodoc.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kayazbqz.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2jbgorbix.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jdohkors.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2kapftvpd.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ybqhibja.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2dujikeqv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qfaegfkt.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekbxldft.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2mgfgmubo.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2lgxusvir.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2rxjjrmfq.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2rpryyyar.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2iqoxxhfk.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2herkwjgz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2qbaxuggy.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zkbulhsh.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2kysegsyd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2gwzrtlcy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2qnyeigir.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbxmkms.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2ygqczcig.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjaxakz.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2stijjfyu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2yrpdrfqy.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2yxzfhrbi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2rklqsdys.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2mvetxnxh.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2qgziobak.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qnpdiboh.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2aicrtazc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsocewqp.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2rgfxwyue.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2nwjzuisb.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsthzfy.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2yscqctpd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjwbmtb.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2xfsvwgiu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lxgrojrh.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2uftjsxau.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2penlmnrq.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2kacwneol.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2xsktlcxr.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2ilsejxaj.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2vfarnhyz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2zknrfvsg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2grlxbjjt.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2ujgxishr.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2qdpgnqtk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ggwwdytt.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2fqdgezgw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2iutpocqg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2kzkgyhhi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pgrswpos.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2dqetdast.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2qigmmzml.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2qeacmiuo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iwufzsdt.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2jmtjbmud.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nhzcitsl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2xqvqmame.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hlcdvvqw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2gbvvzftc.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hhtmsgle.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ixeqtakd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2hhaibnyb.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pxicmvhx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2lcptgfjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2agkemnrj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gkuacpsr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2qzirieth.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2zpsqxkay.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2rvriagnd.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rbsflfrn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2pjhpttpt.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2wgatxqcx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2klfnxamg.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2hizhjoqh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2efeueram.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ohaejzvw.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2wbxuoamc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2fkmlutju.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2zolmkcut.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2quzazlje.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2agfmnbxi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2zvmihwlb.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2nvcswpoq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2tcisglrm.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ghwitbdh.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtztfbkv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ginfvlws.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ahwuioiz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2uobobjsx.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2mqwukmrx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jodgalsc.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dyxqmhbu.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tsypkyoe.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2wvtnlptg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjlloar.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2kdthmbrd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2rpulocgg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2jxyctmdy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2helgdahs.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2srromefp.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yekmuqfw.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2gyfvnscc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oneejqix.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2cyjznvyu.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dxbiahsb.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2njsqboil.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hcgckzck.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ydzvmweg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2bpvejpux.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bjmgtxjq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ikckshyz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rsdkkftn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xrcjtihv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2virgfski.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbsbwaig.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2urpyfobs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2eswklfkr.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcesukja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ilkciqks.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2csabizme.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2yryowchh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2gyxchvou.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2gegwqfuq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pumomilu.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qdomhrah.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2lhcqksgd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nuhrxdxl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2hcgsxzou.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2fzbeycca.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2totwpxuc.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xlhzgvtq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jpjjlfoc.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2gdppmglw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xbilhpnj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xmgisvwd.html


<!-- 参考信息 -->