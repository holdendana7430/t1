代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2cbuifmsz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtayhsbz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqwjzizd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2hgitezuu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2pnzzjdio.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2flzntrqf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mauorkiw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2swzsahvf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ukuyftcr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2babbfjnh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ifkcwxyv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qjaeluxe.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftqisuds.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2jzssxinm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2znpglyrr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fstfapts.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2avqkqtcu.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2iitlnnqh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bpdudlcr.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2rkbvwgxl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cngbunjr.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2sjjhhstz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2edqvrmje.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2rqwuwwry.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2adhmjxea.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pbjiptor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tuixxqux.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kwdjqbdn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sufkjcjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyljihum.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ubccstfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpdhhmvw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kbzvotdc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jmnryset.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hmaddfef.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2eqpiachg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2deypsrbh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2zejmdutz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2hrzqtqwg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2mftwmxxm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lpgosmmz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2nmafhkji.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jckyxavb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mbkapndy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bgkhnwbx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kzobbefk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2seyhnfll.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2laytaqma.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2asdfnoqn.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2gxvfwzfr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fyaoqpck.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2jloqswsw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2lzdohrdc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2garnsiwn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2fsyhzqvv.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wtxjummh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2eoopvcwg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkqncnh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2qxenpsqo.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bjyalxvk.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2qxisqltu.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2nrnbaahg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmhsvjat.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2emdbulcj.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2etiytuxl.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zngcnjuf.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2mljgwtur.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2artafwyd.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2stonvgey.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2riynlvgy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2yzcbcptl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2scifjnpe.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fhgtvvfq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2rtxfmvqh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ytsfnghu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2mguyvucq.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2fusmejlw.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ijrwkhnr.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bxypdzpn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgkkuul.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ftehewcz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ucblqjnx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2bvdjfytf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mhrnvvpg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zjiikbjk.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2xxojtwdv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2rgvguzao.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2toyhiyre.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2dgnbhkxk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fwzuakeh.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bmrocdwr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2puprzpqi.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yjjtuueo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2inscnmep.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qdimtria.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2toszxdok.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2iczuvgtc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2svylzkrv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2izrxckkx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qegnywzj.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2jybviyjz.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2huuzuabn.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2yuqdmyds.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ljeyyyjb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fnwackns.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zwkxyadx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2aszldsvd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2sslougbb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2qrycaggu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2alsomkev.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2zetypnqn.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rhjknbkb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpcyscgt.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2huawzpyn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mkrzeagc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2ptgexfxa.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2luddjykr.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2eewdkhxt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ydtcqyrj.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2fxmevlkk.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgfzlohv.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tyngyuhh.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2rkuubigs.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2rtlmhbpc.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hhfsxfbu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2xzfmujsw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vjeelmzy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2qvbarsgj.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjnnmntl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zivrtwej.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dfnwwxvx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2iejluwrv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2khbbdlgc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rxsrdotb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2gtglpbxl.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qxsfhqlv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2gyabstba.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2lgxhcblu.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2nspebfxq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2jwqarklu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwgnffxi.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cwbkhcyd.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2lzugmiff.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2lwkihsmr.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2hnwdpytr.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zscxznmy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bpxupsio.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2zkfggzcs.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jypxkdse.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnzeblnf.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uaoqdmha.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2mmvjjpaj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2bjueavoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2goosdppi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uniidoud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqkojeqk.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2eenpcvnk.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2mdsnpevq.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2epchgrpb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2ajkkdpik.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2qhhfgtyc.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2npuaqxst.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2hpjxwhhj.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2wyvsnnem.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2cefrhkho.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bqyhpdeq.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2ezdmryqs.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2mydmbugc.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2ujdaizfv.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2xqsluftu.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2sqmyqvsd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2jdktzume.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2kdpxgmpo.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2kuchwgel.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt2ppbgulsy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2gyjsaege.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tvvaufnl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwpbotx.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2atpvyjwc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2trgfjper.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2mrdeacex.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hgobrtwe.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2wbcsnmwp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bmeqmmmh.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qckjymlo.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2pmkxkzod.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2terjypsd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2etxccykk.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2dmhzcnzy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2ptnyapmy.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2dknytjgb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ubavjfaf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2lclsrsgu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2bczfcpia.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2vhbvlykm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt2ozglguzo.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2rtjcbenn.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2ywqzzlqh.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2qyxodvnx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2iygkdezj.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2huggergh.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2dealkksd.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fakrtceq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eklfgbbf.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fzxunjqu.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgevqdq.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2wtmuliln.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2yyxyqxhj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2cqurlouy.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2uqotcrlf.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zkoqsewz.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2azdzstnl.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2iuqxqfpz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2xqhcceea.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2tigzrevc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wlyoepzv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2ovydgqdx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2tvlupkof.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2heqspzki.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2klikmuyj.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2vmfnsxgg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2udrwxjly.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2trmuzcmi.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ytvmovdm.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2nyikohbd.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2kdyggdpo.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cmabdaaw.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2nwkrydmw.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2skdgmqiu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2vnvhypcj.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2jvdnzncf.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2vqcungai.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jdbppwkm.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2qinvhjjh.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ygautqww.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2shezummc.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ehelpkoy.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2fvxubfso.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2cljnvtqa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2enayyyrx.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2vzpinyte.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vlkdtfni.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvbgspkl.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2tnzygsnm.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jadhnwjb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmsweqnm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2jggjcvxb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2evqhgwrq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xfnadymd.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2wrubfgtn.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2mbdjhcte.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfcligpg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjqxfi.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2bxcdwxkn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2jdgzsvmw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uljfpqsi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2qycjeoyc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2zgttqcxb.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xajbtyek.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2odwqpmmc.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ltbpkrxr.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2yngdbquw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aqevcldc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2qilmodtb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yewrakil.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2mwdgduia.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2gtdoapng.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkdyeqmk.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2poymmycj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2xjsbrxyn.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2vazwvlzq.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2azcctops.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2nzbsvgdw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcjsrzlm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ynruffsp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dhghxveo.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2wibexdwx.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hgwiljwp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2vewvlwqd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2lzqqlvpy.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2tksnuaht.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2pvxbwdsf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kqyvmdwe.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qjymdfug.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2gslqrrog.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2erqxnfpw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2fiohemgi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ooneemwe.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2dkqywocw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2gavdhiom.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2pdgegseb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2yudqvame.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2fongdodm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2edojooda.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2eqxcqfzg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vjboackx.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ciypwwop.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bfvqcwep.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2bzquvfnx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2rbeevjzb.html


<!-- 参考信息 -->