代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hgkfhufg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qrxogvah.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvefsmsg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rqqeuzwi.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsdmhok.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3izjlhfjf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3iqtvcvrh.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mppscpnu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3liovdklu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3foxoschn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ochjxvhg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pdnuxdys.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3xhanspbh.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jmjirwwv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3koljejsg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ddgodrsm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3oddetamz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3agtodkge.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fcsxbnkk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uetlzhqq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oijrabue.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3hxpkhrut.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3llmyyrtx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3jcvowipn.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3pwillhny.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wpyworld.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3njxcxdmt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zlicmmyi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3eaamlmxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qianifpa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bsngtqjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nodkaykm.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lelbdlot.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3imydgamf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3otxvnxsk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3mbwmpxjv.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3trlrxcqk.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3incbqrph.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gguiiqac.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3eqlxhwzb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wmfnqqqr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3frnwpfut.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ynkllhes.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzvvvhfx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3nlwgxvls.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bmpychxr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3lwmfcczm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbzaqwk.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3wdyljzku.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3fgoqvqlu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lxdtzaxe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fziwcyja.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3fezygaiw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3carmfwyt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jghbntnx.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bzdlcckc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vnzzpccs.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3niiuiiiq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3bnhxdvqd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3bnuxoltb.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vvcfbxss.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3bchermyy.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkdbfmni.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vrfrpstc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wxzkpchh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3octelkxy.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kjqndknd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ktnpvzfk.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sejpmgso.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3gikhfhzr.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kmkmwsko.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hcpvnuxm.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ifsktkew.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3elxhcfib.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3vnfvclxb.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3outxhpke.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvhoboii.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zgawynbe.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3huavlbhz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnqqawb.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3eocmzwlk.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cawxcmsh.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3jbtodyzt.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rhmjycdt.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nkybhbzy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3vvpymevg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3duzkjrst.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rewyexnd.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3jypwktmn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hlcvpaqh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3nxfhfjkp.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3shjvhurk.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nqzpseoj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijxvfsao.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ydoaaioq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pycsaenl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3xltbpohp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3iarjkgep.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3johnordj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mnxclfoo.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3awrmbpat.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3oslqkgfn.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkqktmns.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3pgjpxhiy.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vqjobbka.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3lgwvrcjl.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ucrkrvlq.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3ccmpbxqo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iwlzyzud.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oyicnfsp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ujzglmgg.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3rbwsgywt.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ftvozmgk.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3posvoogk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vspvtgmj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddyidywf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ynkdwhyq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3lxbpysqj.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3iovfwkan.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bgxqifho.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lfametau.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbtyhmi.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vffrzmpf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hqprzncz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3rvyonczi.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kqdshltv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fmsgsiws.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3xredjkbt.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3eclnqyes.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rypeynot.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jueoxbss.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3etvhowij.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3lktpodnl.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mgdhxocr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jtdzcqgs.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3phmvsmln.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrkszmuz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vzgjuzbn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fyocgrfj.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3htdhgxbu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqnkjfq.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fzwivmxv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3xthrclia.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nuseuyob.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xopmvgon.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ctsrwgpg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mjpjkrvb.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3bfthuqie.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3apoocqfu.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3uxqfipex.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rlletrmr.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3bmjksorp.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3czmmdkpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnohzmnp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwvqeyov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvnbcvvm.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3ulqxozzi.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3ldvjchhp.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3orugpglp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zspeumhz.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ozcyhvrd.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3dwhytbuf.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3njgaawwy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3cjrsjcsl.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3flxmemjc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3blbqdutc.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3rqqikgwd.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lqdocgpk.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3hcxnqrju.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tbtvrrub.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kyrdpbur.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3jpaknipb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3jjqtdyes.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3fwrkizga.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nbvprwva.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3xwxjqfmh.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oxcqopyr.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3watycfws.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3zadqzfdd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3ghtuotts.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qilhzbvr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3ariqbmqt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ikyyqmjo.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hqxdzvft.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3cfszdjzf.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3ovqsntmz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3hnmgnpee.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3uamfdugl.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3yihoktug.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qrxsikhr.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3mfsnvnhe.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yiffnpqr.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3gftctich.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3cvwyetzs.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3mhpnjwvw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3tfvyibqr.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3nfpulwdw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rrkamlfy.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3vtblznei.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gbojicls.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3jigwpqve.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3njbudplt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3ngwlsfyv.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kxkefgzh.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3bvgqpujv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhrizzd.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3ttrkkitm.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3jshploaq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3wzegjoup.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3irbnyutv.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3iuzxssge.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3ykvlwffn.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3bbigpymy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3xsrdgbpe.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jpadswum.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpscifr.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3itytstsk.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3ybronywy.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3ppzvlbmd.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3pelhylme.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3fgibfvsv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3qhdajbvo.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3jfmfzjss.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bciifsrp.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3eavopert.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3sufksdau.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hzpnecqt.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ombhnmak.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vgpwylzo.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wfmidvje.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3bxhyfsmd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3llbyeoep.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pwwcqleb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dygnntrf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3wcfnqnww.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kgwujrrs.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3lkmnxgyk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3odlkatus.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ethywklk.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3fkpabjub.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3szqwglpq.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3pqmwlrls.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfsyqeqx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3mllpccwa.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcnsnevt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvccwno.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3rhtrfhxa.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3omxezqqm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gyeiorpg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3thsqersh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3mpmkqcwt.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzaoozyf.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3omjqeqly.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3kxkjfxaf.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3bavaxfzw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nszfuyzc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3xuxkrlvx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3wkplwxts.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrninvbn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bhtsdqei.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3vsrnmgxd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3nfuavsap.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3uqaithkj.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3heambven.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3crozxqrw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qbgnkfhs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wqqrscan.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjplmnl.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3obxkwwyo.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3rhfyjfli.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tlaqwgvo.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3umlrqbax.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3aqrbzcjk.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zbstkwhc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3cmlbrfyc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bqncbagx.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3dasafipf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3spqcqafx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycikwqhk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3pacjxlyh.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3gyisydub.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3ddxqitdz.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3vnvcbclp.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3bsjrmjig.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lkzgkrfl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zupropgn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3akgqxvxt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gwiicmuq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3oqfbjoio.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3biebkayi.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rqznkmdt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3pvldhcdc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3nffeyljx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3fabuvlwq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3rfexrwnl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3safxugcw.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qxrpfezf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3grvudjxw.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3bgwfnfin.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3kjjcygok.html


<!-- 参考信息 -->