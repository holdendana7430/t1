代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3zmrcywpv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3akkaoyqm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkqpxrml.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tobmaecx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mbkjbiyz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwafopla.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3dypabgjx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lxdtsdub.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ouxwkeyk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3taletvsq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tvbaigxm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3lfibzrni.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ztefdmoc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cpslzzei.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bkudhogt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bpwfytpy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3shiwwytu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kdnojbdt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yhyjlxws.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3qpydxcoc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3zuriaiki.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fthxldan.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bhybwikb.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3chfpkvia.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jqpsazda.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3bwukumpt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3vhdxhxjs.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3poexbcrl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ijgnxpve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eodhakzm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3heuhyozg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryeazanv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vmvryvxo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xlgdyevb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mtgvmots.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yttyqbyx.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3choozvcy.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hdhvgenq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3hrppaybn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yywsrfau.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vslmujct.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3uxurjvsj.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3broaiszo.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lhjjyptu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3yvizcvlo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3urqahjqf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3xmgoghte.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3stxrisug.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mkwixcgh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wdsssbaj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3yaejmgxi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3pnoodyus.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hazinzgf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3otqjjtdj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3qctycaca.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ratubepc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rcwfoqyu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfoaraie.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jkfxcbba.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bneeaori.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3mqxsuxwx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wipruurx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oooqnmrg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zqjawrtg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ptyqydwm.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hewywacj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3myiambjh.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3mujywkiw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jiefxyzx.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3vdlwfbpw.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3vpmbzhat.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3lasxybjz.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zngtreli.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3oihfhlmz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hafbmzug.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3uqsvlnln.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3skbymysy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hdrkortv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hhwkvjbr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvxsscs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3vlzdokam.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3ilfswhzf.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3dfxuiidw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rrkzxdnz.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uojtvpas.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3pfegrrig.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yveqlamr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ardqahid.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rtjkeiav.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pjjyyawz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3lmkkkrdc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3wvkmehpa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zluxctsz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3gnfslvnh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3tslbrxry.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcsilfnv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wbpjudug.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ratfotca.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3asvbpjel.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bdrlippf.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3zcmhhuog.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3psgtydis.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjbemxid.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3icimyooz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kxljswzu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ilvnedih.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rhqwtuuw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ctfidbgs.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bxckfikj.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3eyambvit.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3sxvexbwa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ejigpmxm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ubdvxgfq.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3iymnjdrt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3pftivgxn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dhsoxmrv.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kldtqdjv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jgaijmyv.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xqigqksc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceequsra.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dmcgknfp.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3pgpzfopx.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ymdmloly.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iikvvszm.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3ihpkxuxz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3lerpqnux.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vtgwzoaf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3qnuiptin.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3omuhbnkt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvitrasj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyurrkza.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wjpddsxb.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfqvbfcd.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3flacphca.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wcmstggl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjwcpnei.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gfxcjbdv.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3otekxgel.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3nzlfolcu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pgsrxnqy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3slyqkxff.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wdrvbaeq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoztmbe.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mlyfnmix.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jydnmsli.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bwupesch.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qktkxklz.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gjudmdhd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3ymfhpjru.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3wezmvauh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wphifvfx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3qhjtesar.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbljpso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbpdbbob.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3acwnkndt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmnbxuou.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3zeyznnbf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3pkhplwlm.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3xqatuljx.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bxxmvkyf.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3nxkcnkzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3iwlmhqrn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fakkbazm.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3tswjzndr.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3atcjnzqs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zaqmjbbc.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3yyqjemvn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3mjgpjkfn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3pgmybszd.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3pncgrtgi.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3usbdbndr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3fpkcslug.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3bkgfdrxc.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3hdomzrpp.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3lthwhvlf.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3idaaamhu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nueyaswl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vtkspdpk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3suracvcw.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dlghzzsv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3pyeektri.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3dfebbbkd.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3tqxnlbfc.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzunrsg.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ixycmvlh.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3izzokclz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3ulguhqes.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3njbyzpao.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ugiptswb.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3vzibweqe.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3sejtclqc.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mkczzcfi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3zksnxicc.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpnyfhq.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3awfsdgat.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsstbmb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3tnsoskuv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3rsdlzsdu.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3iemkcobm.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3rraviitc.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3qppjgdky.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3irnxjldx.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cqectjwf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lbmqsngo.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3bzwsscbj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3vveuudbi.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3romxgsrz.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ljgigeai.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3nxozcbfv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mspmhrcd.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3fnemjnnc.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3linhvcqs.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3umaaqcco.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3aoujzvxf.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mkqwrnys.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3fpszneqq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3uuovpdtb.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3isfmskxo.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3wtwakkfl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3jmqoesjn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3czbkajea.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qiouvvym.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3gxpnnliu.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fwmjqybo.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3mhfshzrs.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3crqbwmwp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3syplmgxs.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3uechryek.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tieogjfh.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3tpxhuunm.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3mirrtzcv.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ttsqkgof.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3eqdxaajo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3zgzzzljy.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ezreclmq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvalyvco.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3ogsmrlyy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nragudge.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3ndiellxj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wdztnouw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3pfgcfxnz.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3alvrvzne.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3lfobljbg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3lpksrfze.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3vsssvfrs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kcewnbcm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ieboguxd.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3heaoyglk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqyyqtbv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jocofdmy.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3vvksqzng.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hminccut.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dlblvlfa.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zadxunab.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3xzodlond.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3vujgwosu.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ltdfapzr.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3frumyetb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lpizltca.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3pozoasqn.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wsfgrztu.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3fxxkypsl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3lejbtzif.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3cvvuybft.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lfvbbzvp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hacznnol.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3xowigmab.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qjrigari.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vcawpbxp.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3sifowknz.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3trsozkfr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3jexpoufb.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3fllnzzyx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nbvntogy.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ynyzejgd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3jpxymqtp.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3ndmacgct.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iagzguew.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3eqwjqpie.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3frnkgdsi.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3vaiqpgns.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3lprhhfxa.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ndlsdqml.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3htfqokwo.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3yhlspblr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3axnbvyos.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kvjvlgfs.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3twysebwu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3sqgiejdy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3afdodnsz.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3hjvdglqn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3bxsuhjaz.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fsnzppuy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3nmntuzok.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3auzcliab.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3fgcwmchv.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rpjmkmqb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iuyeuzss.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3saigpxml.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jwfeivaa.html


<!-- 参考信息 -->