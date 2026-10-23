代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cgpqrkff.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pgsgudlc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlefzict.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjlvgm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3slljigat.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hsyvqelx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3zciawzld.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3epcbrhdm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lxjblxbr.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mtfrwupj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qyqwgkwn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3bjohesqi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ukxjdogh.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3sujlevbv.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pvuxudhp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3izryeyoy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nexgvziz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3djaczdua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3mrdypekg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pcgwohpr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nfvwbnia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcwwnhhr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3axjahzaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehvopzlz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hxspzfcz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vnvhvmvi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ujjwhusk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3iydydwcn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3shmdsjhz.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3xeqbcymx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3xekgsphm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3lkwsbwks.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3alltkemi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3eplycpjo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ujndgzcg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwieadxu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ylblvsuf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wskionqj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zjxmmleq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3uxuuxofr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3hhjcynet.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ndggzdef.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3colgbfou.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3tdevalqx.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3xclrptqe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cjymdzuo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ooyedtwr.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plehjbuv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3clwdlavd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3qsxlqdps.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtizcfkp.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oreyqqas.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3kedtyqpl.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dieyqugh.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ldbgwhjw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vawebaik.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hotqrqqr.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ymvlvwot.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ljhduggj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lvoltsqx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3iraerygb.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3srjxkkoc.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3qlgwqxbm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3usudyunl.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hugajqqt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbuvmgyr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3sntepzkx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ixmnhxfx.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgpljfbg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xktratpa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3yrrtuvui.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3irrydyls.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3fnovxwks.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3aisccpvl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3eimwqzfq.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3clnsqvwh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3prnznozn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3pdrlkcxn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ibyefpbu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3khrpbstz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hjqumson.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nguikhzm.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3eayfgyrg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3yhfwkypk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fpbivujv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fpenhbny.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zhoqugaw.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfdseatd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fdjqbbax.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3cotdjxzr.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3jkojxkmq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xmcyeoaa.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3cmsymiqj.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvfvpato.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ayqckike.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3scajlxet.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xkiiurdl.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3apzpqejm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3lcxdbvom.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3tqmqrjiq.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3xbcwgpwo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3euonflwv.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3zgpsirxy.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3duwxtfbh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qycvhmdj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqxtcy.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3edsdnksa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3lwxbkbcj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ecdcryzj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3qrdmkbpn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3xhfezzak.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkulayw.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3flhnkqdm.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvnjasin.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3pqazikiw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3gltkzmwo.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3itysyixz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3jubxujyt.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3tcfqfvbt.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dymlhaxc.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3krunlwaw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ofpxolkz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3brbqvewa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ogqrrxfd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3voixlhkk.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hudinqlu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3cceauoxg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xgwetjtl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzfynifl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vtujbbwg.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ubouovhk.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3oafygacm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3yezvqgma.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nwmacjdp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3rejjizgb.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3vqhkwcmd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3slqaurgp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lvamspvj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbaidelm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3efbsrgxy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kwwpzhbw.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3rnssjjna.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uiyqynol.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3ccqmuoho.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3uelkwpkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgbdvjyk.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vcjwdmzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3offykpqm.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3xvlagtjp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3nnkbbcvk.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3smwgoeut.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgrvuhvv.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wdkhczht.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3rkfqmgvz.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3xoowdpnv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3nnlkjjxf.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3pxonciip.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xevwwtxs.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3zhacgejl.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mfmkmbvd.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3tbtltbmc.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3zzxkkbmg.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3jrktexxr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hjllsejc.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3lrslrzvb.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3wjsazoxq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3cahtsalv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3lwrcjgcl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lakqtbpw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycytusua.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3xcwoichx.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3acvbanwi.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3thnpqvhf.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ekqdezvq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3lkrgnoru.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvewsxo.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3hwdshptn.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3bivjdcuu.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3gsoxfsap.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3hhsqsgvb.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3dkfmesce.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3wizkqkvh.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3lcugmnnu.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kskocihr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3wmvwlcbe.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3pwbgymri.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3hwxkxprh.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3edwlwaij.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zoizcskx.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3ztspmvyh.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qjvwztzd.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwteqk.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3rzagzzkf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3ktgmqtxw.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ytrzprhd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mspmksqo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3zyqhhnlf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hyoutjxt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3vovvnjfk.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3kdzpnhse.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3otxsmcal.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3zxtzazej.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3wtnxqxsn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3tumesbjg.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3cpcehevg.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3gndklulz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fkyatxan.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3jfpxnkld.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3nkvwgxii.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3mfydphvo.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kfkcuhec.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3oqoddbew.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3kftfucmo.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wnxsiwly.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3sjsiktyl.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ajsszmuu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mvbkdted.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3botlgxma.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3unjhkdej.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3posfexrt.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3anuqdfyj.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3zrvtbcwe.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kijvrtdc.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3psyfidzh.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3shkvvqqt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kotkkrey.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3xfjbbort.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3thzseeuf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3uvwshulw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3umklcqno.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3znubrudw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwixfyo.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3tsbnqwdf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3odqtlvth.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3txfvtrbx.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3klxoytbt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3vvhmvanp.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3raoprhpf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hyxctgnq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jdarjmga.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xkbqubxz.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3vcssanxz.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3nvxvjlxd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chhfrlkf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3auuwyfaf.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3rstuipdf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3svmxjzlq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3qiyfhzqz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ganitqop.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qelrptdq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bmntfwof.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lscbbxvi.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3fqsyikwa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cwvxkctg.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rwbxcraa.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fopoqozb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mbngxnsk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xpfpxqbu.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzcokzbe.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ykfwflzi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3samfatgy.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3opfjvseg.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3gmdqbccc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3syokrrtt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3wougyozr.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3asescakl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uhcrtqxp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pxrigakz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3hkmaautr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3raoxnwqe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3wfirjoea.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wfdbvyof.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3ejpfytop.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vkioditm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3xxsuyjzv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3nudsvxlh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3nsfwsegz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gagiwrbo.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ktoqbule.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3goqobrbk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xtytctmg.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3aehhtoyt.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3qmuojtaf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3jibegyjs.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3izeqvujg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3icnibzpd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3yjzrmtri.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3fcpbhdrd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rsohrxgj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3dsfzxodo.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vcxxrwmh.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3tpeolwzn.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3ijcapbms.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3lkcbunpr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ychhdext.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ebeudxzd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mogayhdn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gookawep.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3jilzdono.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3icqbvrmb.html


<!-- 参考信息 -->