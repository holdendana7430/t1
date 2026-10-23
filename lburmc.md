代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dnvfafpt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hwnwhhfw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jtkazmjb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ptbhhhgt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mhesamks.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyohdpjx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksaexkcs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3ojbqxhsw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bjsdwkyi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfbywkun.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wepyllbh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3orcnjrvd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rsoklsya.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3wqqnomgl.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ckhswdym.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mvshgyie.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgcdjtsk.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3ovwseyga.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3quwpgoxk.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3mpgruzec.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tsaqtrsy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ffnkcjhk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3eysommhw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3czvhukwm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvoqqvgd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3xztudrbt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zwmbyxgf.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vzdcpjsf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3zoaoiprq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dohiivek.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vhrfjxqh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlctrymn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3zcnnpahf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxbccuhl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wxaaafej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebkirotu.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mgzyjrvq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bsdovjva.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3resmsgcx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3zffmdhkz.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nlmkuomg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3tekvstdu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dzlvbeen.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3vwihswtz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yycdrpox.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dkimmnsb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3zathfcsc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvateiz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hzigfsxx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3aiszaeou.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3xztsqgrx.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3blnwgtbt.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgnhlxhc.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3nhqvgjuj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3vvundtfv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hxhgttjm.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3nippjswt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3reeqcbsv.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3uhktywoc.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dzuqxbjr.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tbczkksm.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoylubn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ndmcovoz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohbutukl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3hilghmlj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3udkwatrm.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxxjvvay.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3dcotczxg.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nttphwwx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3iybstplo.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3thvqomiv.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3rleegric.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tiwedvro.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3gnrbikvp.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3covnlwgd.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3kiiowncj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zbflzdue.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3evtsfdth.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3yoswmskc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ryzpzfub.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3shikmjpd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3lcogypmj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3qqsvdldx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3duzwakui.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3fbwzrxtq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3zettorve.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3zwtxpmba.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3pmrxxgts.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kwruvvbh.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zkvqplab.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3zcnmvaxj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jkzwqkgz.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xzygedhz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvmeowb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yftycfec.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwawvle.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dsjaozme.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ceirmrqn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3suolweld.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkfneaho.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3fafouwnl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ipufmuix.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3fcvtfwbf.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dqlutzfh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3jbhwyfpq.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3lujzkeko.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bhlmyycl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3izeeayns.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dforiuyg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qdsvbhxv.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3rzcajvtr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3kozgteav.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ouimixlg.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3unwhvxsm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cluelbww.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3bzzlshpf.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tmuyssvo.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3uchzgilz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3xurwpdxi.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3mfjihaly.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3azoovuob.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bxejueoz.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3gqupemiv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3jueoaowe.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3igesrccn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3dxruzbco.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3rojhuirl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjycvfk.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3dvownboj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkyhgdil.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ubvtkqjo.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3epsobjeo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3jjhenhyi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiwocelz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kbdnjapw.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3robrcefp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpvobihi.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yojrhvzp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3eiicbsxp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uwjeioza.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucnylije.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3czgykgui.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3trgosvry.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3hceyrnus.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3wahrbhbs.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iynbvizu.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3netyvuim.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3llqljkxj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3altloypl.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rxbmpzuj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jylgjxnd.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3wknvnism.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3esfoyqou.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3anjrpkxn.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3edkwviip.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bbdwglwe.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3brevgqjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfengacg.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnxlulgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymtlakhx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3keqywpug.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3oglzjgrs.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3hdgdtymr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwkqgxqy.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3kaiyjnue.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3pvefokww.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3tgsenrux.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3wywuqqin.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3spumcolg.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3paprgoyz.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kuhnebcv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3dmyjwhrf.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3thheujkp.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3ogxodoch.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3agrpjgdi.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3veqxzlof.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3cjjdtamt.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3jqncmgtq.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3kakrdpwh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3qefmrrdl.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ukfftihl.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3hpyquwsp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3vwzrjnjt.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ejuiohff.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvjtrlaw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hzptackk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3krfskkew.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wfbrrhmk.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3gntztpia.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3gjwehgcx.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3brkkfpqq.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3sxgbegpn.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3olyauyxv.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3wfacsloi.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3adzljjxj.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vjurdywb.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3kapsvjeh.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3rdvpdwjf.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3thnccmpc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3mejrgofw.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3pefnnaxb.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3rsghnrcf.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tllkrdkk.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3mjswqtob.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvetbhhz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3kclxjikn.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3tgnqqslf.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ryicthje.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3kcwznazd.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3lqzgjkuu.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3rijgidpy.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3tydhkdcx.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3sgvebsuu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3utahkonm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3vcoydxzw.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3xwnuqurt.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3satwadpk.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ihxxoogn.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3anfuozfn.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwlvrwo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pvjucfgx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fetnpbzj.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iyroyqjj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3fqnhwzhz.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3defeugdk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3vqtntxqk.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ixhidcsf.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3dozsyehc.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3natkfsxw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3jmlhxmab.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3nirwltoe.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdxddui.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3hlxmgkpr.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3vpmkvtyx.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3itxsrvnh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ezlmqvch.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3iokbknef.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3kcvdzzhz.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3cnrmdanq.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3immfwsmq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3lqphdafc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vpbmzxsm.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3xyskycat.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3hvluvvjw.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3vrbwmkbj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3weyrrcvj.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3hyaoytwr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3evdptlfo.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3fozwhlpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xzbgqjzi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3yyjzxgdn.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3iernkyji.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gedfrkun.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3cnxshllf.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ntrdysvo.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3hmhgybej.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3dicrqsju.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ihhdtyct.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vajjfwkf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsmaaxpg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nxqxshrw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3zkhiiqbe.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3rzqudmwy.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ckotiyxa.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3svqvpboa.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3fpezbyem.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xstrglvd.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3xahhsbrj.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3kmffafza.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kqylovci.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yiuaerku.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tyrwhraw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iiqfpugg.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3eguvkerq.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3zwuvqxlf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cdpmpnsu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hugxiyvb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xpvgyiqf.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3zkzvbqkh.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3iyorjkgn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3urfdtufw.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3twqhjfvi.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3gevmjmck.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3ysbnztxc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zzyeghvj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rykqblex.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zuuwpqve.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3gykjravr.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3ukcqxhdp.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nunzpuzj.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3vntcqvqy.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3srcmpikn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3dhpdjzql.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3wqdlrhcf.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3bjxgcenp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hkgfofyq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3lknzytcl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3zbtoahoo.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3zfssdlsw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zicwistk.html


<!-- 参考信息 -->