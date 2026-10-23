代发 wailian999

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3diuhlgbh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3sflmpirx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uafhcqma.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3adprnotn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yntawcaj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3nshbchyv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ntcasgyn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gihpkzpe.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fevepvyg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vxnrveio.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzlnypia.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vcnycrbf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3czwqmxtg.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3crhgixlc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ctqbgeqd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3pkgxeidu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ufbaeags.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kxqxahbi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ogxalhmg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ygewwmqz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ghjdjxvb.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3fyanlzrc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wiwyplbi.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ggmqllik.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3apfprsyx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yinliexa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3xqdocsbn.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3syonzjtx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3yjlafmgm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qfbvvwsy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3qkllcapb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3vgpdhxob.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3epewdawd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wnyrgwft.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3frecajnu.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrzqtbpi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dnedwsmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptpielrx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pwgqsbzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sddfaylk.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3arpryqlg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3douqkmdg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ylwzvkad.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nppijohk.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3hithpyjt.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3epnmhmcb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tdzmrdok.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3xpvcwbms.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mdqudghb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3xviellks.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3sztyvwdd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxkvbstz.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ttifrgdj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3odozrain.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vkhxifgc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gdlspqly.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nujrdydf.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3pqahpusb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cagsblsf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tlyvnbau.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3jwczkzso.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3tyoocktb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3cdrilzqf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eubhpvcf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3dplymisj.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3efpcajpc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ztgsncmq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3mqnqlzar.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ottydtsj.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3omyjjucf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wuikyqfh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ftvtnvbw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3ypaoaukm.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ejcnoncv.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ssbnkakz.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ccvloidi.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3pkrmfrcj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3fojeovsq.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3auijflfs.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3brnoloeb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3kequbmyk.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yisaiblg.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ggipbxdv.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vkddbpre.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3imjqcere.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3llrzivll.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fmyxrwmi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3csuvpuik.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3nclrngxr.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3ivisaujq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3nsmmboru.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xzgewbki.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3uhmmcmyc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3lmkhcjhl.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3awwlyllr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rlvfloew.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3hnzrsaun.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3heeoqump.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3kadxmtag.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qmuyjdfa.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqzrrtvw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xvyfwehu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3knjysbre.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmibantl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rkdtcbal.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3kysbjpwv.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3sfezfydp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3zzkuskdt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3onajfjmy.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nvylyxpf.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ybubppci.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3wjbcakld.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3vwxspaly.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3mwnbhbrg.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qbziahqi.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3uedyvkjy.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3wbofgkwr.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3arorqfcw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ncllvwch.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3icyimlxn.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jsyrclah.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3epuqlosz.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nrylgkgj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3rylivfnh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gnttbyoy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3cgpxhrvf.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3baqubzhx.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3wdpjravp.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3pqjmausk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3eiwhanvz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3uvuymdlh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ytcewizv.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3qnlksuka.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghgzamir.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oyofpcbn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ktuqceas.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzbifowj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khfiajul.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oohztlqn.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wziknpyj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3upkqgbqr.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ddmfbwog.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vzzdclys.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3hvoovxqs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3akztntji.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fqipiiqm.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nvxfvjxf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3blusvljr.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3uotukuab.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rjrvavpl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdmswnug.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gykeawqg.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3knijmghs.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qouzlvjl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hjbothui.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3yjjuzuim.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3orbrdegj.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3muuxlpqs.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uoydlzmc.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3hduhmudo.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmsordn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tziyzyvw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cwpaphwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsthrtaf.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3gxvftdvb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3vupnjjxt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3kkbwnhlw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3szkwsmyo.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3eqmkuosl.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3vwnzuusi.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3btmcarti.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3zszvxdwy.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3oevdlcir.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lekscoqo.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3oqsfwebq.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3gbjitxch.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3nkhurszr.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3fxbmvuqj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3wdxoyqke.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3ggayiqot.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3xbxyevzo.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfawibm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3jjiqycjc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3uhnumyqb.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ispwbvaa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrbczkf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cyjhqweg.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3maalwxdc.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3aobaqchw.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hqlweuvc.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3izkozxby.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3elslrero.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3zrcnlgmv.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3eveygmio.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3vclgaopt.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pqvmizck.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3mjvmihor.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkysydw.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3jgucylob.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rkjgchcf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3llsgnshr.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3ijgaeefn.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xweyiufc.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3nmacfxwj.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zjtlvywv.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3yomlwrjq.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3oeowcgky.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3gonktzkw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrszsnfz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3tqienvlh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3viomnkmy.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vsksxeik.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ldcqoicc.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3rsoktczu.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3xcfqqzlu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3pogovrvx.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3kuehtzsv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3qflbrmei.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3cmmcclgf.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3fbfeyjah.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3bjgnrfdm.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3eyphruso.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3szfrryur.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kubsoxnm.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zyllgpxe.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rcjaguzn.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zjphhsrv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3xsdyjlvo.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3cgovdvex.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3scggbcjz.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3pgwelvrf.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3dgjcdlle.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ejwsfivf.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3etylwodf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3chjhkfdo.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3imqihfhb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3ruebzfnz.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3mhqlvykd.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3jgccndqh.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3mrlygcod.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3zgivuzof.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3dshkaupz.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vgpjmpdf.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3feerhacn.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3cabmakfv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3sjctuhci.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3oxzwopqb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mrncykvv.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mxuuriln.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3tbhrjowb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqkrripf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3baqbjgev.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3jljvzbtq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vanrholv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3hfbvxhvd.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3pjvhiiii.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3ywrthego.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ypihzxxc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ukzgsptm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgnkhuqc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kgpsfxow.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3weunesvw.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3fpwopxop.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuhiomrr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3wgriwnhz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3lbrxmfff.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qtdeogbh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3dhgafoub.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3wwucwpvt.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3wwukefdq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3yqkarxjq.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3avegmfid.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oclewbhm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wgdnrrot.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3swiyztbb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sipshoak.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3miaclfxz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3kunwaspd.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nosqxrmg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3keyljlvo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3hijjjcio.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vgsjodbx.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3grgcbjhz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzsvsnet.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3uteclsgv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnjfymsd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3lwbgmpqh.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3bcnlgwma.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3naopkdyl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3roeqaidg.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3dazyopea.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3tazhmxem.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3frtpdewz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dyxzbmzz.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3vsatqhzz.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qoaobgii.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3wylsqoid.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3nxsmxqhh.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xppgnxja.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tpsdyoex.html


<!-- 参考信息 -->