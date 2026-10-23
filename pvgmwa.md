代发 wailian999

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hzmilgje.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3devutvfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ccsdxxll.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3fbfjzyty.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oofikprl.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwoewqvz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3oktlqdps.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3tsldnpge.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwvzatb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3xjcbuvaz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rezazmab.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3osrudxub.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hflwgmsg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zcmlbuyf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pirqmxsl.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3pzlqahmw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hxiywrre.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3gtghovmc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3fefsbgwa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3oebohdyo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iyogzjvf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ejnhrgeu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tibmiigx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3fffdiwzz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fxovzibi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujqoxqxm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3snpggqdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atgedolp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lxfiaoww.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vvcixcww.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3vnwsgxfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lvoazhxw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dqfemreo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ldrdtvku.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ssmvqyuz.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3imataghn.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lswjazde.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dalrlouc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rquqlrid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dvkprbej.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wqkdrvyg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3erfregiv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3jfpzqypw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqnkfvm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3yodhriwt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3orzeusrr.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3deyegrja.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3yhtjnmwy.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3edhnrhhj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xqkdfkvs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3bnkptzek.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aksawxwx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3pgeatzet.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrumyzcb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3gcxagwgi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3oedijagt.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kevgkkrg.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3hnhuxpcw.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ifrkjgkz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xzjylutl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ftulpkwj.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qtzrmkqe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xhdriugx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ysolnxig.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3egbrezwh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3htcwdwkj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bnbbtxmp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3vjgdtkrr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fvyemvte.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrsndpi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qgyafvfh.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3kpqzwajy.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3caonqupm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3amezpqbu.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qykmsajr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ywhutecu.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3sflwotta.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wthspwpz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ainlvnrt.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnzwyxe.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfmnztig.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3tybuewnu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3bwspoztn.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3kaeiqbct.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3yinbrofj.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lrniupeb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3kmqqvfzr.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3thalfbps.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lrkviugd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3edkzvkdo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjgnlfds.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ccfoxfcd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vrzpttik.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zqqtbltv.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sfqpqjlp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3nprqnsqm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3qyaqunky.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3rgzezgkz.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqawizcq.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3rqaffhib.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qkazfdvc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gsfqasff.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ljqbolot.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3vbqfgmfu.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wezgzsul.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3wyfbcltq.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lemdwswb.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3mzgspntl.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ffsgvjxo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3rntgvhsh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3bcajfhwg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3dxcpuyii.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qutgtwjm.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3dyxdohjo.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3pymixtbl.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3kixvsojz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zkgaqdne.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3titgrkdf.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3iaxlfxnt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhctcze.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3uuxoobaj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cshlaefu.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ejshajsr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3eqxpsahy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3mwwoitnw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqgxputu.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wjukueey.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3otoktozn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dncfuwrr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gihbttsw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wjybgwro.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jpvawvup.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kodrvame.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qqrtbrmn.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mkfcjpcp.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hhgbouts.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zzfnqqtg.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dtetdmwx.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3tnaagsuj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3jsuwriqu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3olabxufc.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mtnibdjn.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3asstgvau.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ajtptupy.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3djbtbnnm.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3mqwvtrca.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3oqhmqtyp.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3dttcyhxb.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3xalwudba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxlzlggp.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vjtzdytw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eslrrhzi.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3shednrfm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3rkymcjok.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3eksojaif.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3apqsupkc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3jiztcksh.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3ttsstpwo.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3zgwdzted.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ammmjxcv.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3gendpgkh.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3spyaoxdv.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3jiuwhmfg.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3hnmxeium.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ebxfxwuv.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3nymafgau.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3ifveswex.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3gfxgvbvm.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3zfmlphlh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhpwctm.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3kgkjtlic.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cpizufsv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ygvgewnp.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sajchgpk.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3vhpsmsbc.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3otewggyg.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3wqhsqyru.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3qibbhsio.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3otvdqxyh.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ejvwqvdq.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3fzrvabkq.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3aiisjkoi.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vrqmocbm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3rluqqesn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ldmiwtat.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3mepabrgi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3hrmgclkx.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3svfoionf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3wzrqpgdw.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rtiqfvvz.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xmigajqk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3xgqsheki.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lzwdcyfi.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3undxiusb.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3kdhmsxbs.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3csefqwwx.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3kyxvkfju.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3xvdqfajt.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3rnluphmr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wkrjytux.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3yekwpuhz.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3icrqznav.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3kjbiwyus.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3yyfetybr.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3yusewnyi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3douleuss.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3vcusuoyr.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3mxxlgeuf.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bwrxbqjb.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3jjsvlpht.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3dftqxejd.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ikqknoqk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3rijhsidl.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3bpyxppjl.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dqfnpbze.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3btyiguma.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3eqmvtgzq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3ytrtlvih.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3mizqolov.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3ppypzqpn.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3jcykeqmv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3wqkhychq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3zobpjddz.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqaoaqh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3zgnauvjg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3bbpmfmyn.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3tsvghbfl.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ijswnbcc.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3acslkjvs.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cznwyaqq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3fngjzxjj.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhlenvwi.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fgcpqtfa.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3nalnnmkh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3jzbvcvlu.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3sutgphck.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3dnshrzip.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3chvqiqyg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3kqprnwmj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3nvjudvhh.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3szdgnpre.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dhczjeza.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fpfdzedc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3yvoagidw.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ziyysagu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qdswecti.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nhmcnmty.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfmetrv.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3xeyrzpgk.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3zdpdhnjv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3dvntsafz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3hazdznzr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ennpdyjy.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3dytdxlzn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kutjbqim.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3namvxkvq.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3dflhqvht.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3hjdsvomi.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3omokikau.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3bdkjpdoh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3xpuxqowt.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pygjnrwc.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wryffqzd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zcnaycuf.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bgqtjcva.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fgqyrqrf.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ynokcvzx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3yyzjjuod.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3gsisobii.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3egwxpgbk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pvqkqydd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3hnghoobt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3oucxrjux.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gyfnmksj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3xeckmimi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3nahrlfnz.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3gnbyjjgb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3miyqhncp.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3regalzzm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3inknbqxk.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3flxcmohw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ydnkaawu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ixurdphc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uudjstlb.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3rqlwgofj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jyiurjkt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3mhwvgaqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kaslwaeq.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3jwkgosub.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3mbbasyqm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3metzmiox.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3xzmitzsg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ntuzqfom.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gtirsiko.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rytfvtnq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ilhvrtaz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3tkacgzft.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3kofrqueq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3emjpuqgz.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3olgjnibd.html


<!-- 参考信息 -->