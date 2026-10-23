代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3kstaspvs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3vymclkzf.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkirpdnt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3awptbwlf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hroaioqw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3txtqzomk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3tcnutqmc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mmdejwmk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gnkghkhk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3jngcgqbu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3fzrvgikc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vijcxzqq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fhkgqpxq.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3yjxlvehn.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xgqgmqzj.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fmfsxklp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3qxitbbzo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ilckiecx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3auoaeupm.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ykysajxo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jquflveu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3lxpdjsyw.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gpczwdjl.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3bfmdmfkb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjbvjxo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vvcvyhfo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3xuqxopiy.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jstnvbfc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3yxohssmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uemhoaac.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ljqukjmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbgxphji.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jgiluvqo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lqkdtarr.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xflwdydc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ffvunrdo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vqslgnsh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ibkuxgqb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vrnntiau.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3yhohgpir.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3smngdasq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3deihqxas.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3eahjsyhu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uyddmoxw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oalnbnrl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3dyzklihl.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ivyrigif.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rhpcovnn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3jgninksv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3quxwrjsr.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3toypsazs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3kyvamvaq.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3zdvemsdz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bsprevzm.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dtoleeth.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjjccfh.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rggquljm.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3aejlqlsg.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3uzypehpw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3grgpwoqt.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3hqsyrrsh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3sfqrqaub.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kthqlexo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bgxgutmy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3hhbqmows.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mtcbrkxr.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kgrtawap.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3aiwofhik.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3enclgsse.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3obpezqmi.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3osvvgiyk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3slitmste.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tykvfdjq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3aapdmqld.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qyvtfmsv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3itymdfpn.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vhszdsip.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wsvzunet.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3inccdkqc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpstxgz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3djyguhas.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3yldsxrdb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3eljmblxx.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3jshmfwvy.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3jxmalvur.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jrqstmmg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lpkcxoxd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3duplzxft.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3juadtxqs.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3euhwhziv.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3irjygcfi.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ztaoqjio.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wkhqmmsf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zyocxoif.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3vxhujsub.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3squroymc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ifgoceyc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3azfnzqof.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3dqklnvmi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3acfibskc.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rkvtudym.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zewojtqh.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzdoagzf.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ycssjbkd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pkumznkv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3jxkttwiz.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3kasuvyzz.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3ylfksfzn.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ibuxonxe.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3dbzfmcbz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3ypkdcjzg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3sxluzhkw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgowxnru.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3oflfdgzk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3kegysddd.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3twdhwluw.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kcokciwt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mubnrygr.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zqnahtar.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3liueizid.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3edkwfvgr.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3fcyyyyjr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3sjqnbrjf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3opiugrxn.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ulgzghjh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3sukdwhph.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pknqrqgv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vhlmuupb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3lgmkszjn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dpjqgdew.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcollolh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3darwdify.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3whinbkgb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zgntyxqo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tkmarpfq.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3xsfjpmlt.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zglearjr.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3moznitkh.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3rvrulppb.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3nuoakztt.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhzjxylt.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3unhxermp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3ycqyadrs.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wdqlicha.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyhkisx.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dxhvsphu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3iiqmwpri.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3zujiezvo.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3egkozevt.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hknsreoh.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3khlkccbn.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3gxwtjnvs.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3miigbqhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pckuxszh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3zfioxhyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmcrsuqc.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3mafmmlqh.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3gbyxqxmb.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3jvadjhtb.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3bvjzrzge.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3xbwchlox.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3mxazqwqc.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3sgeodckd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3xtkupvip.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3zqtzhabc.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qdvfpwek.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3svirihwi.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3ydvujnto.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3pjrttqlu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3bdpzinuo.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3rtanivfn.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3mdaggtyw.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3qlgjnrtv.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3jowsgcdw.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3zoxkfrxd.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3cuosykxt.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oumhssxu.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfewdkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohifbgvf.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3oyearhmb.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cstvfsgl.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3pekiegul.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3myvnjdvy.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xclmddrl.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3puumgxaq.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3wyneiiks.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uegnmshh.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3vwmudxkd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3nrrbeght.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3qhkkuedc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3utpmxnhi.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vbexvvrl.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tcgtfudp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3apzlbrvf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3envicxob.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3psnawuza.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3dgulscbe.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3qjbeqyyd.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3wbxkyxqa.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3wtqinkcf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3cioptxgk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3mgjcfpqx.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3xzgqihhn.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhsxnlc.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3qdonpain.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3cnmvjahx.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3lcpvjazt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3lqnpyxtk.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3qvroctdl.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3chczduff.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3mijfgizj.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3zncarssc.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3akupkggs.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3emzoyvls.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3fbjyhuml.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3wfoukgdw.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3hsvfvnpw.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3dbletsoe.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3veexdzov.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3wjsrcezp.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3eaiofvsc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3wuhntfxn.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3ivtavbru.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvmspjo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3vbmaxkbu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3bkvuyekh.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3mvepmunj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tbocuvsa.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sxfpsolr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3fygkluty.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3opzmfljz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3ogjsntjg.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3aevkqebd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3jspvhtoi.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ovzlfsof.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3sbujfevb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3obtepmki.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3zjxvlqst.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3tlgcptwj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3fmhrptha.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mjpoarvp.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3usukjnlh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3uchzssbr.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgvllzve.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3mlgbvlpc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgrygnjl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3vjsjtirg.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gleinnfi.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3sjejuaij.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3bcmxmlvq.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lgupndys.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3gghxwobi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3wgbtbbah.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3lgeuoowx.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3jjcxtjtn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3ewlbpign.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3iasgclqn.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xctygnpu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3devsmlod.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbvzqo.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3biwbpmte.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3agwcxrnr.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3barajlnc.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3qkfuoggd.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3odanldvq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ycjsqobj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3jzfrndgd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcxxaik.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hoydqiwr.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ufxqhuqu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3vatxmlnh.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ibybtyud.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3chfawqrm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3enxdlphl.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3uhvztcsb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3cqunbdsw.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3wggzbrhz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qioomnpj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3popdbcko.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rsnlovqs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3dqhyhhwf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3jzulkklu.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fiteuqrq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3odnxiinm.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qokdboyc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qvlacvya.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3trybtdbz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qlzdidej.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3whroripc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zdycflzs.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3rjsltsyp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3wcyxrybf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3vxkjpkew.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3jfmioejw.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3areqpfuk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wkamukjq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qolvihtq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3csgptodc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3uyujyszz.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3papffvhn.html


<!-- 参考信息 -->