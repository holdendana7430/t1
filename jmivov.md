代发 wailian999

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nrtxntnk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mbjkdskj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zjqumvaz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ocgsslmv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uoqfaufm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pggwzgia.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3sdcxmgnx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qhdovwqa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3knkommck.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3esimvjcj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xoebxezh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qnvxfzgq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3alxfqusd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3krdlkwjb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ftsxbsoa.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xiiadwoj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cuntkvur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3puyzjkzx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xpqufsfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbfrxypx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fpgbtwsf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zhgwdysj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3gkxwutuz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3yzpjxeak.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3anunanok.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nxbuyfbi.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sqeiocci.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mebdxwfb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cpijdulk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dhuczsar.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hfpadhcf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3srxgjjie.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hdjddavt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfeaowci.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3guxnrmwr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uhuibtyy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3anlpbhky.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3wtmloroi.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qahnltqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pjgacskp.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ityhlemu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qmsvymal.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3asrcsuwk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqudrbbg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3seuziuim.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3icfxwhfp.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jkznufkr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dzwtbbqb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3irxzlqfy.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ujejsfgq.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlecsclh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dluvnvfp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3mnsbkzjc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xrlrbsrr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fijcxurm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ytdexiyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vmmdttux.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3imxjwerj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3awhthwqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3csdxqxcp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3nzamimrt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxbxygqp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3clrqzmjz.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rsgqcyvx.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3btiwgydf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wehwmwlt.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bcdnypjq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zurrnfwz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3snxuzjbf.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3lnwzboyh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3aajtloqx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jidlqiyr.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kkazrjqg.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3yaqqxztq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3abtwfptt.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ckowoibv.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bngqdlst.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ccnyryec.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3uhfthobi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rwxhlfqf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qsofweof.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ylryacqu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3qyxhwqfx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3risryqzr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3gcfvbgqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3fpnqglqh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3pvtafdex.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dyykdzie.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3siwkegks.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kjwvbtti.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jpjbtfdj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cujlvauy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ikrrpuff.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gmcltgep.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3hjqmsaed.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3orwoqcni.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jqdkboxz.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qtccjcmv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mkbvdlur.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3hwggffnq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3erxzlffl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3fwftjamf.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3arojgxst.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wopwrjwq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bivdzukl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bhjlsako.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3nrticknk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbgqrird.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3farhtyap.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bicarbxh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3wgbljiim.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgsliftq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3sjtwwmyq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbvxfrhl.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jtrxobbp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3xcjdngri.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jafuxceh.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3onuchlgl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lorcotoq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3ylichcnt.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3algofxwn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3plhfcwno.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3imkucuuf.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3gvdjrwps.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3horipisp.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ojhpoevc.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eldgrtnx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gliyarld.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxlvecmz.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3bxzrdffe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3qidhaoen.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3ogxxwxaz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jjprtwie.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3pdricqgt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vknkgelt.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3shqvyhxd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ioumwvzv.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3pweiqznv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lxhokpbk.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3mdxbnohe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3gaknixgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iitzkxif.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hagxrgkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfkjutos.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3kplldqut.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3rxrtiino.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ecalutto.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wrketiwv.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3oxbmgith.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3gjszhaaj.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sbarkeoh.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3hmalvwow.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3tcodtgvg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zbltndjc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3fxfyqsas.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3bvhsnojt.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3gnarxhoc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3rtpjbtvq.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3gyetenhc.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3pswboxad.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3iijhfavz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3idhgcpkx.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ilopbcrs.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3azekhchv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gcoozikc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lasfvsdn.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3eccygwgq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3eesrdaxa.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfnedcgt.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fzjfwwmt.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3zmgcazaw.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3crndvwmt.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3systdlxl.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3gwbihuvh.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3szezzool.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3xolwbqfj.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3wuqgwuum.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3hstrbwnq.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3rqctlnnf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3absqfbtq.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3jujwkzfz.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3gysmjqxn.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mktisdbi.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3lrqulqhp.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3akrzfbjd.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3gehwhsfs.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wufcjvow.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3lldtzrlc.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3zannfuhr.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rbdbatqe.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3sarvdvco.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kbhsporr.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bumgoabr.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3uosjgkgc.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3tssxmsyq.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3gmpyiegj.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3solxdsxv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3nvvxhgsh.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hlqeqket.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xzlnblee.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3wkznjena.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jontcopu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lymwwbjt.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyrabzr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3myvvixgc.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3yyshtksn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3weripxsm.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3wampzylw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3xkkdpwbn.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3cllyhifb.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3yyvdftot.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfognob.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3fsnmilmy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3gpsbjjzz.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjlunm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3lfwfspdh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3lqqcdvwr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3klrpveot.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3vazzguur.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3iyeumaun.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rcypwjqn.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3ltcyawbu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3ympsafel.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cefvyutc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3zfwpfrrg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jaelqted.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3yjwctlsn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3xdamhnxt.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3aaaiisjf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ycppwwmp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3dofiudwf.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3snzgnraz.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpxywquf.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zispxnjr.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yozvflbo.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ukhljhnt.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3chzkaerf.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3pewkofov.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3shkzpxce.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ciristjc.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hadhkjjr.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3jhvvdbvy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3lpgargig.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3pikwfvog.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hmdzejyj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3whzgavnq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aunrnpke.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ijpoxddo.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3yfvvulip.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ybddharw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xzvzzzmm.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bbhdnwuj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3fxpvzbzi.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kiqvvdkx.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rmosgjje.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwgqxzhg.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3zgrnefkq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwcopcoc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3eimoufds.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3vahlkyod.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3mwpkmhfn.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3etkfuyxo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3eltpxcvu.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmvgfsa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3yvzyigdc.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xzvsjmzy.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3aqecdcmg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3qymqwgnx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3waroiagw.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3bwbycjpv.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oyycaent.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3zbhmwiij.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrqoeg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3twziewvs.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vydkwecm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xevmmzlh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hsueorxq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3pwhcjijl.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xwigtfsz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ygshvyef.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fehceiqy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hznkkatk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3fkkrevth.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3lllekfcx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ggxfnhiw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vbikesao.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3igczjoyd.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ghvqsuqp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ocmwhrub.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3iovxjjli.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3quyvavdg.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3wgslmbfm.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cjuupvre.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3bagwpntc.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bsxlvssu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3xrdqmlqg.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3yoewafnf.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3oacwmcux.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ghfspsjf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fsrnpmkc.html


<!-- 参考信息 -->