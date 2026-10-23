代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hdxuqfmb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmdudjuv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnzxtsvl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ftsjxgoe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oapziyff.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sueaapif.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mnburyvq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3utyfbojo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgispu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jtsaxabv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3mqvdljdq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gckphtpf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3oyqyrvxa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vxluabbp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3vjyiblgc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mglibhax.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wvlpdxwf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nmylrnsk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xcuopqxr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yhtysxwz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycwkotdb.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yjrpohlv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tdlqvibj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3lyampbld.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3forenhcp.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3fbxxadfh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3meeyrabi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nujyegcz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3buiiszfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkzgcvnf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3roozwlmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvcpqmsz.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dzxbsung.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vyhhcelw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3wzzrtihc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3itjvbxgv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ngrrdfbw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3azpxvozq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wqvagdwf.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3salkgxrp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3koyzmzel.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3nfdebgcf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3etogsbll.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gobaagrz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uiezugmc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3usaidbrk.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3rshokkbs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzvqjkb.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3fernqppl.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgpwdf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3itcrwbuo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wgyznogv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lkpzjbun.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kldohubh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bbvmaomf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3imhkrzfa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3vjjigbeb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ckdfdcab.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3nspfelpo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xqcfvhbm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3yidzpnqu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3coxngqrl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3swwpdfkt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zayupbhb.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vnbfruzm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdjanrli.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pufasncf.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3leszryxe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ntporyub.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnptztzl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3betvjqyh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hcmxrmjr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fujtlted.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrmvbob.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3hecwjlsc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ttakaaig.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3husigvvm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xevgdrwu.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xwnunctu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lbmbaoej.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3tfzhciws.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ymnbjasb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ijedsxge.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3sispkguo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3tidkzxha.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3etkcyrju.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3knjyujkx.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wxcobypx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3bizurdpw.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mxtsttwn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3wdttivab.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3jwzwactn.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sslrukme.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uwgggwdy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sqnhhrts.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xduoekux.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bkficceo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xaxmcvsh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3yuaenpgr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mipwyyen.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3ugsfesoc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tczcapvj.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bglswggu.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pxruizxt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3prlnzydu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3idgbikrs.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vmjgpiwm.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3obxauacw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3vxbpxkny.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3rukbugke.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xwbdrqkn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pbtjfdkd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nxxxwojj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3koohnges.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3dshnebuv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwywbxo.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dmavhsek.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3owvrhpnu.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rziuhbtr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3luuxvlqj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpoogjfx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkfxsgzd.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zwdtpito.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwaejrkl.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3mucocjca.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnjirnm.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3hjdpxqoj.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3ezybxzff.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3vjznllec.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hcvpddrs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zsuewizm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3beirptmw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdpsyzq.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nmtabifz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ztcvdlne.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3euwvgxrq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xyowmyti.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3toaddoir.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3soydrqmu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yvvrrjpl.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3ivnxrcuv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3maaynfoy.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhxxqgv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3bwvfrvbe.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zbbnusgr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fmduhzqk.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsikbkil.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3gshciqmg.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3lketyvab.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3ziafavvj.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dqdbuyvh.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3wdhmdzlt.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3tcopbhtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjodyvac.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlohthtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obttusbd.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3pbyocmxc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ngxymmno.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3viozganj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zidsbwrq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3djssbsko.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3eeedbibq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3pamcajon.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aholkzqf.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3utfmcrxs.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3barjacll.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3bipuexbj.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ihyltehq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qjraxkek.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xtinpdev.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3vlbozyxd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3qokwzihq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3orgzszck.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxhabzc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3cijzjbvp.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qtdakhdg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hdzzgqpw.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3vrtobygd.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ccnuckse.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfmgxkl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3xzgucwxk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3fsmwxcpk.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3pbytgabs.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bkgnbcem.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3laouptqg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3cimqemol.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3fwiqqbcb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3yooclqkw.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gscackwz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3vjryvoli.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3fkqpufsi.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ebfaewjy.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3arxfxfgr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yoruvmgw.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3bxywulfn.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3qyfjxcyu.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3rdetuqqs.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3twbsuiny.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3afnmzrsu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3qlzimewd.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3usbcqvyb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3qlbxeark.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3pegxluly.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zpurdxil.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3tdttfxrj.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmmockj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rhjznwik.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbyxvrl.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fvwlnowy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ftdualhg.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3lsszgyrt.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3acstfvom.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3safgfpfy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zyjzxxuh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3vizvgyje.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tprepmaq.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3slcsegaf.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jgagadui.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3farmmrih.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3xkjlzuay.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3jdijrczp.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kyjsodef.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3iovfuybf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3okkomjvz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3rhdeqzeg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3xfyohwdy.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3umrtoswa.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3zrocvnod.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3yjsihpod.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3twuabjmb.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3llybpdve.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3tbfqjoqd.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3kajcofks.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3owszocnl.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3kmbasymz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vtfendkc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3okfcjpaz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3ipoqjafx.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3xgzhoruw.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oefqhqvb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zfhumnkz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3qsmxjdox.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3sjzawajn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqordtu.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3efwacqvh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpbthzym.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ukobxppp.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3bspeifgo.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3vwfcslym.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3gpimbidv.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3apknxbgv.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svgjgtpu.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3snretoar.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nkunilko.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3nynoukyc.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3wlfupmoz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3fyceveob.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cdeftpji.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgnoyytk.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3angmqslz.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3neserakr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lngrwbda.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eaeyznel.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3knpjnlvm.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3mtritajp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rkkepiyr.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3eispvauh.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nmhgnvso.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ycrmtizn.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uukhdrvt.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ugejkept.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3skgozurn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3rfyzwric.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vrtfpjrt.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3amdqojlr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ietxclrw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xwdackoj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhclvjwh.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3jevkktks.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3xerxvwbb.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3yexhlbsg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3pkbdensc.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3eoarmrpj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zdfauggc.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3afehqqhy.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eskaqesn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3eawhdork.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3rreodhyf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3fdqazynl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3ytijmgjq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mdwqdfzh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3ppynjymn.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3kaltpfyu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3eirxcqbs.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3bqxsjahj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3abgyykrt.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3movmbygj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3amrqpfqj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3qttvxjzc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3zhakoehu.html


<!-- 参考信息 -->