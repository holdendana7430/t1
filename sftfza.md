代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vciswvli.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3abxlfizn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wvhdlnts.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3noezqcia.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3miduddxj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3frbmormh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3afxunbuk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okupjjny.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cwstwrba.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtazxont.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ljtukpvb.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rwqywxcb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3dfdmuydc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fojerzcr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3demftfff.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nxpmtncb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eblpgjtx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ggvtaobl.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3isujvoub.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ppdcfwco.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jrckbgnz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3wrkbveku.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3higgilhn.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fkvsgyrt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mtbbtlbg.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hasgdobi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qkolawnx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3werkuxwl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vchgaufi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3paqvmwxa.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dihadhhr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ojvbpryt.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbikqmz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3odlwrejt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fmkxakcp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3ipccmjuz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3osenevdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvztpzui.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gnwcnslr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlpezjxb.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vgkqvlxy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxhrfm.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3pgssgojk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3kicuqtbu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3owksmxwc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bkareleg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kxqzefwh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3pqfkvozi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bvvuzyhp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3unnnshqf.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vnffecor.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dtdkownf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ibscqjft.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3citrtkvf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ksccogbb.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3xvdrvqnk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3xotjamoz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hwrxaopx.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3odbetdqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3gjectdur.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3eiruroid.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ygrdkevy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rsqxrmgk.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3afdnwucw.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3xyzukrtb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3bqmlcfrv.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxorsctj.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3sdkcfpcb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qngoiewp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mzljzvin.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jghirrvw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3srsttlwv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3foucwffv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3cazcvacw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hgoekyyx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xrypthtb.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vjzvbsgf.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3djwqaexz.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3zrjowrqg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3qchyyrpp.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3yjbmopko.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3aaxdxvom.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ejyyyywt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3eyjwfnnj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cngzgacj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mzaeaffj.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3oskczxhd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zfjdzbkb.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3blkpofes.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3elwkpobz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3weammdmp.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ssuisoav.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3lwwuatko.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3wrmhkwao.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3avwgvmri.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3byhfzibq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3aalxaxgn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gdgefhhk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ipusrsdi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zddibtgm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gngscllg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aqcpetrl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hnnspqep.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yiqqiajc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iqinopzy.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3sovbfhoz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ibdezjgt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3mksxnonl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3upjjznbc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3vkizexmg.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrdqleck.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3epojhqbt.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hjeyqlae.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3vlhiohqm.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3dgftcexy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3urwkkzyj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3phxtmizc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ubffvurb.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3goiqtmas.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxazjn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3akyqnsde.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eiwnafkk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3ysnmqmex.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wskzfbbz.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3txhxgupn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3hjswhekm.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3artdiayd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3rbiifwtz.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3rwrjhofj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqcvtbnc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3dgbwaron.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3unvxyiuz.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3byunjmgz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfczwkjo.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ddzrfyww.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tzqowcsh.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3yrvnjere.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fktvviaa.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gmhkopfo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3fvxcrjsv.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqjtnscu.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wgituevq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ygfnmcxb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hpijvyrw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3aebdqlst.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rlfkppkk.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3mlfpmxcc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tzibxlof.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3qnvlflbh.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3mihpjznh.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fcsqgzxl.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hyzjgzjf.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3cztvuxqw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3advftoft.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3imaozuxm.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3mwqxzcvi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3qwbgkhhp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3uwjggfkc.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3geivrwtu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3jeziknor.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3avhrwwks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kreqoqeq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnlbzfog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssmthvrq.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vglecpek.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ellnrfdk.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3rnyndmpc.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3etakyzrs.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3rwbsvypi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3frjwgyzy.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3ygdyagdd.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3rueondkk.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3uigfulzh.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ibkyuyih.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3goazsuli.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3lbzttfyi.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3qpzorgtk.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3xrcikyxk.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3kcrozytw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3pdnfvpjb.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3iygqwqlt.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3cbwkjcpb.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3rumbeyvi.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3mhjioumq.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xzyjdipc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cajebchj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3nitxgphb.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3bucwrctq.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3wdmuzarr.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hanwbhvl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3wzjrovkv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3ntokspxz.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ulkhrzvj.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3akclpvrf.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3srmpzkds.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3ddtpayyd.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3fyorraqp.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3onqdijrp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3hzhqjpyk.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lfuostqv.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3erwespyl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbmeaj.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3tmavsjqw.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3ynyizcyt.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3uvnzaxik.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3gnrmdcsq.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3qvfdewmy.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3ddbihqjj.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3jldszkos.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3afzzbsth.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3untwgbfr.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3doycjmcg.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3fqkmrhwy.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3ywxfkgfr.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3uxmdxqvt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3kyxpmnix.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3giiknuth.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3mukwfflo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3azdnjrja.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pieegunr.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3cxxcxpwt.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3xhepmedb.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3emhgdftm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dodbpyvz.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3qdhcmtop.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3hrgivsad.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nfrthmwx.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zahwmrhn.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3aqmzsgfq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3kclfbcck.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3ownjzrep.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3tvjvzaxo.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3wtxfoelj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3pbmeregd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ertpgzfb.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3nfphhwks.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3sprkxpad.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3gydudfds.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3fgjjuyzh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wzfhnnaf.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3xgvtifdw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3qjcymwqd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3cttlbpdi.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xgenhltt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fwldadhf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3yxygsuue.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qvssrmfr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3qdrhonvz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3oumavxub.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrexqba.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3pitjzpbu.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3sslidods.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3xravmcmm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftievuch.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3pdhfxywq.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3jwunpqjp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3gipfjgpm.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3hgihdmsr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3efjvgbtg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3idolowrq.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3buvbbsdj.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3yhzflyvh.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mzxwnikl.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3xmsjnlib.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ddxyfjak.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3ljcerybu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3asjigiju.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sgfpxdhm.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3lsyikwqq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wyfqfbpc.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3feipvknp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3ixqmdptv.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zarkdmuy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3oytkcsni.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3lawgvfpl.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rxnnecte.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jyieiexc.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3ssyamaal.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3tliesreb.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3umgqqwyt.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3afdiayri.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ibakmlhn.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3rscqzonp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ztsubjdk.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3gbkcbpzi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ceebfmyz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xkccksnj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3rlamefyg.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3ircgynsj.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3uzotbwox.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3kfpnqueg.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3khhumzff.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3teolifqo.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3smhlpsux.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3shpgfcpj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxtgen.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wydvlbdz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3nqiaxvhs.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ugcwdovc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3kdkvcpub.html


<!-- 参考信息 -->