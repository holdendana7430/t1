代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3unqsbdwe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3bpfarwpa.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ladzxddf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oypaojmg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3agreasrq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rmspkapf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xjkbubsf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3lygwdfps.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rxhwmmtk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wgzpofyb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ajlwroyq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dlggtwlu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gooiwdsz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3eewlgeus.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wfwkjtlu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3yyypphrb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hwvthbmt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cfaebrpf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3apvihvbq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gajoggag.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qphhevoi.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3soldjdde.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pbnjwlgh.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dvryrxzu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzqemai.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3nnthqxzs.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bfzrzjsw.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3usbxndnz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgtoxxsz.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3echlxdda.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xwhmszzz.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3durdokzw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3szctyuwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abquimcq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zufkuiwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfoxpihp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jklmcpuu.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3enjgmizq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cxdbwkoa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3gwpzlmau.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hbqjbafv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3farluauc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tvfmfngu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3npzlfisj.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mqvvxetw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3kfeexaju.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rjzymycp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpxumkrr.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qqacqhfr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3pbyiixtx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3kfjyabhc.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ytcdmtao.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjgecbeo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3kkygmlxb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3vedrriqj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pznusqxz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3npeiuybz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3xdyqgzeq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3oihoieuw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zelryopk.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rbhzaise.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3zsogbfba.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3mwlvscip.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cnidwjuu.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ridjgewn.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3rwuqjnue.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fzpwieir.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aapbjrst.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3pubwopzn.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3snqiuxwo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ubfaccxy.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ygufxhgf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yajyodhv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3prpfnrzc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3igkclomq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bbklyqcx.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lzyujfwq.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3mcrtqifk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aklocaem.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xsabzwqb.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqwdblzl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3esgjluzt.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gmxdphps.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3opckvxfw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3auptymtc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qbymgtwy.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3skqwzwcd.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vtngcxjp.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3sxjshbqo.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3blevmldc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3piyflurp.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3ugixmntu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3twmrtlfe.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kxbzkgpd.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3liirhhnx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lwgdotcf.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ypdtpqfl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kuasnlnw.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3acdgjxzj.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3faabggfw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3mjnqrqvq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3saszrppj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3gtdqvirv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3amwzkgao.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3wtztqxub.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ldgyejit.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijbgtcup.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3uysvgiwc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nzdjvkqw.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3uvgqousm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3pbqaquec.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jgigpeso.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3zgbfwwci.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3yvhqehrz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3wtkpzfwb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3gdeoibrm.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lqsufxkl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ufhvmztz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rlfjfxvf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uswrblbz.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pcpmqwew.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3avihfqwz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gycqeqev.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3ubcxvnix.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3jujpvyhk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ffxmgmis.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3dejfjnch.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hoxmljwx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3hosfqecw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjuzqgtw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bmpccibk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gbqxxdun.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3htrmssug.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhxgejmq.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rtcqxzmk.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3nldbkgim.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3wbktuolc.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hyrdaqdd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3igquvcop.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3jfazzbmv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kmsrpwcq.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3nztoobzu.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3hoempuro.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3skcprrat.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3hawgmhmp.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ivgqenww.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxjmivo.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3wyrvijke.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fxjkqjul.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qbcriway.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3aocmisih.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3fzlzovmh.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3akkgmehz.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3jeljtwcz.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xheamwsx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nzacqryu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3joyiqbbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlbqripo.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxlitgqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcwajllt.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3lssnpyhv.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3xylmalxg.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3stlgxpat.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3xbmzngoa.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3zzdpxrki.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3zdskiqnc.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3jfecfxjq.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3ldjmgpcw.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3fkdatpvt.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hhfeieis.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3nzuarjrn.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ltqpxeuc.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3ownmmuvq.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3zcjdrbxh.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqvxvjql.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3hetjpgvu.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3yhxugmjj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3oqkgkrsm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3rlclqtqy.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3jpkgzbrv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3gcijqbzl.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sanlnsjo.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3fvihxdku.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3lpnclunv.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3qjkqjtus.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3wzldmnzr.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ejwvukrp.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qavbdsea.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3nxuugntj.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3nukvjvuv.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3nvakbthf.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3iiguhtxg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ewhtnmgq.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3etdrgmth.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3cmmqdxmg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rvygtjdt.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tyxrhmka.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxazgrqx.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3vrppfady.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3rtgmedpi.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3lbgdkerr.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3ninfkbmb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3pjduhtzu.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mvksaupd.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3tadhuany.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3npvdfdge.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3cpkwcmxa.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ykilkmef.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3sgfsddgc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3wttvikks.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3rlahoyop.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvugfqd.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3sqyimaso.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3vwlglaoa.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3yatygsgh.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xvhdkhch.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3flzpevwy.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3auifadmu.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gpqcyrdb.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3cbqjcmaw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gwoohfir.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3qupprsaa.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3fqsstuyn.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3bvrdrcpz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3btoltpzd.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3mvqpgshk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3acnpauru.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3cufscsjd.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3qeecmeme.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3hbhkdkfe.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uaqzukej.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3hdkxkawr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3icayohkc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3vvjmebef.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3vbioduif.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3yzezajbk.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3sjbjdpma.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3mwberbax.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3mnkanvmw.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rwlgchfr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3khgdagkb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cejqbfka.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3ucqduemg.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3nxpomkkk.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3fqrgyryf.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3ozsrbeog.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpssupcn.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdyrkvsi.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbecacmq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfogmvdl.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3fclgazfc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3buzubcez.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzlucndi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3zliglbdq.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ptewaiet.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjdjeaui.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3rambykmk.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3dgnarlfj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3pcyutwvj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrdbnfpt.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3bpuzhreu.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3erszwctp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rhomkcdg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3gkogxkfx.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3beexgiad.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3djhkczfa.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3seurmmcl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3zglnphlf.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wsywpjul.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pogckuma.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wrjmwokn.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ikrukbii.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3amixucto.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3itvblrbe.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3wuemujpy.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlyqlkgo.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3atnsnwai.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xxzwwemw.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yimyriqf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bkqnkqro.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3xqzeuuys.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gxemqdlo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pvknkfew.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3xdaegqcr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3txjmzlep.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3tqvebiqx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gnasybjw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3mzyvtmng.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3thcyaslm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aflbrjvw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lfnrtuyh.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3tlsqwgyh.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3lxdyvpjm.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3bcwnsqck.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3sigmsewf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3cwudbqvd.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3etbtceva.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3neebyupg.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3pvbcckkp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gmuwzagd.html


<!-- 参考信息 -->