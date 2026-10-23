代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qvaudidu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulcqtqbs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3dameqyyc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3jdcfkbig.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbcugdk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3absikgml.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qajdbiks.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xhguydpe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3trlspyqk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xagvamrz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ppvebrvj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kfyslmww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwxmzvi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xlehwdtx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwcykgok.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3qjmgzdtx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpnttch.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cpcisolw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3phblydfb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fwpcbhci.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjswid.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3loylkrao.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3edvroapf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3qazeteqa.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3arxasbiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tetnyguy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3iurhxgar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyaqhkfc.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3buitgchu.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qonnyejb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzhfwvpz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3lwqukabu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tjvrzgsw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3zlchorhu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kuxmhevi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3gcmrfvvt.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmdhkf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3imcsnwni.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3znshtyjs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nodrczki.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iefjnksp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cncnkopn.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3oulbhchc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gfxvxoru.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ggcqcsks.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jzzfkrbw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tfmlebmw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3okttnjpi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3pvhohlhu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3osytrudc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3hxljbczh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qnqftapi.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3mawnczpe.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3shivlsgc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3whloawqr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ocduttqw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yzaoetgg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3czwfbkuq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xylohbcb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pxlgvjlf.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3uegdexko.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dxwozwnb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vlcqlgqe.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3phhmjsra.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3dagcqsqn.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxfkssq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3hihgsumj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlgylbnz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3xirswqrm.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3auecrims.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3gioadngs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3spgmtqbh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3njdtrsit.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mekzdmxb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3itdwdqkq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vbomfzan.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3obcdymhw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wkvaltle.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3dvwpxpwc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rdjplqfo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3suknbysx.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3aybargtf.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3cxmxfzlc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3sdvgnhcl.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3myabttod.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3rengudtz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3vbcaqwvo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hhmogzed.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3esikiusa.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uixtqldu.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dwsuodiv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iooevxnn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3spjaibhq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3dyaysxpq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3kaahjyuu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3vjggcyzv.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmjgxm.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3iglhxkyv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzdnbdmz.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3qiocqeef.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vxqvcdkm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3nxksdxad.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3nytxamjk.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kfxxjjxx.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wpvngxrq.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3lpicedwf.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3kknlfbak.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3zijiunlc.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mlueclty.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3gvwotnxt.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ueurvhni.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bbbqgsea.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ffwfugpj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3vultbzjw.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3lborcepa.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ahdnekxu.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3hxdrbzav.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3geuigfqv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mxieexyl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xheytjpp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3qzdrlhot.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjeqrzca.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qiyorjqq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tkvuuykq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kjvswvcj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agtsbhcs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ylnrdmpp.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fslyhpor.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhdrmxe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3soibvjdg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3diangbgg.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3evqdyzfk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wikkxahc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mavnruwx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3opyrnkxx.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3qomqmfrr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3judnncri.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jhcllrzi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxmfzfd.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3marenjip.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3bqwvrcbh.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xlpgerkq.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rcpfmvlc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3favvwlgx.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lnepawqa.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrxmuydi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nhguqgee.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3fkwrvido.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3eoxbkeqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emanligt.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vyubatom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmautbqr.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3amiztfoo.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3bllpxyws.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3bibibatf.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3lfbekaxx.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3fgvmuscu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3shbtwght.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3apztkiez.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ftwlupgh.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zvrdqoqr.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gpkjdbtm.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3swroomzt.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3atppkuvb.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3krutjlaz.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3nknckvgw.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3evqsfdme.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3tgwiddch.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3flxuifxz.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3scrceazr.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lgsumudm.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3penyhggm.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3sfdxdfhn.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxwuecd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3aojjsjlp.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3crnaugvr.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3popfjpbp.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3tqtkacgy.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3bvgpcxhp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tbuaydhk.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3esfqaerd.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cdbkxlgj.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3ielswyzl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3inbvlgvy.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3gvmogpfi.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3yyapdhmo.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cbifuyvh.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dgeboefy.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ihytwcmp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ucffytza.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3dwkdfexm.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qdmwaqdi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3yjhtzoot.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3fmxjeyrc.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3avxzwike.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pdzvnqcv.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckypsdnn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3rkljerri.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3bbyxlezt.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uqdaljkp.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3apfckctt.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3lkkelnsw.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xyscodrb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3binskpwb.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3htjbcfxe.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3oriavnzz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fjalolbd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3bmuddyep.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3gtqsjngw.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xjoewrwl.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3hgprzvyn.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fdqmgaon.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3olunnmoy.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3ppmagwop.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ytjxinua.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xzlehzxk.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3rpvqekit.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3txfcqprd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cndkbzse.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cirahkyv.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qzxrandx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3tvstfqnn.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hqvctnws.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3jmwlbvtk.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3jsleyteb.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lypelxhh.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3igbeninl.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tbfqevev.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3exuuiugd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3aekltmql.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3tfhkqezi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zfzpjkyg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3agurrnlk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3bggifvaf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3veaipmnp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3bduwxidw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3qvrisyli.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ggzuycou.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmkzgurq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3jtgyiwtk.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3oepalkma.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hnatpjkt.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3umbvxxoj.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3kpjectax.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctewshws.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mwuxidgs.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fdchabil.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ljyigalf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3ijttloyu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3kcvpklgu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3iasuhmac.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjzacnvn.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3avxmrtdu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cbxitzul.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3btovgamm.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oclnhafg.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ozovopdb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3uisgngfa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3cclaniky.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3nkltzadu.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3krczmxll.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fvxwezml.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mmrrraye.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vknnllsv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xutbdcli.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3yuxryrfg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3taggdmtm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cqrqnfyl.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vzvqzkna.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3riyqvmts.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3bugufnfj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3fdscrrmz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3cswjukic.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3thldjtac.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ndszczhd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mamopvdv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3wsdvuxwx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3omnrzqlt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qkuyicys.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3bsbhgvek.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3tkhokcid.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3luzenybs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3fpzooqrd.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3xxecfinf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3kewlhfxb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wohfnuun.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3tszitvym.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ktnhyuvd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3cvjqlyzt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3vvbxbukl.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3idcawelm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhyynf.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3keyigsln.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xtmporlb.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3lycfflbj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kxmpdwuo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3msaayzdq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3osplqjrs.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgshnywf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3cuhvbkyb.html


<!-- 参考信息 -->