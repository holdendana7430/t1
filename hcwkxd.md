代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3gujfzryk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fuxrxpur.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wdrrawwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqfziuyj.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3rytipyhl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3frwlggsg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rusrszou.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3flvxeyxu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ikinxtxk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jffsgomk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3zssqwhov.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hjhbkglj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xlmcsrjj.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bhhcdcpo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3uhobibso.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3jjqnfisr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nctxywvw.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3biusmztf.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jzooklny.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3icimumiv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bjnozcha.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bxtcrlmo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fruqfrce.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ttclnwpk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hbvyrfjd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3bzpejjve.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3omeyhhfx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3gthdrclr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3umkmvtml.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zzkxhpor.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3snddonfm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pjayhxvj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ubvojqtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crsdijkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mhzphtdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfdvscka.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvprgxgo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3xipydujg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxwdchhd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lsadxlme.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nrxlhklx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3lvkfdvta.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3qjjagmdh.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3bwzovzqe.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dqvygkwf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3defxtovd.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3xfjtafdy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mkdjcxzn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ssqqgpal.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdynspgk.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3axyordff.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gftrquan.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3evisttmw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qlhutnxu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjpmjmej.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uwmqnaoj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3eoccuyaj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3noozcheo.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3riisayni.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwrmsias.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zkhsqfwh.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkobsytc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zdlxzckp.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3cwprgpdv.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3niulqnuk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kdezjxmt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vkvgitxh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uuxzepgc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qyrhjwru.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bdqghgrz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mffjcttj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3jcdytkqc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3eafmsnpa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3kbswqnsh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3wnkohrod.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pbdbjklc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gcltlqng.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfgsiobz.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3aaixwmjr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3csbicgno.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3ojhgxugz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3pjnkveoh.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3geclydoc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gosayvdp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nhbsozqd.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qghqtjhx.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ghrkdqas.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3tylsvqbw.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3svesxrrl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbyrqkf.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vikeewqm.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3wuxmtimu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dfjlrivc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yacwcaeu.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3gnmemfzd.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ftjiwean.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bgnjtexl.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3wcqqhpqh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3mdanfejk.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3srkzlbuj.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3deakvcyu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3clrivxln.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3zbsxsgmp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3eswikhmu.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rqpjvjsv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zcrehdit.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3atiwyqve.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3twbtyipl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3itwvuqnr.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3ewbttuqb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ygdnbyuc.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3qvjsjysi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zqphwvjj.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3huwossfw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3ngzdsyoc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3xjupiyru.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3puncgmpc.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3jnwahcsu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3zjxrhyqx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3gpxxqida.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ghaahrwt.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3mufjmcqx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mkbbcqxr.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3bdgkoubf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dykgrzee.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3sastjhgm.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rnbsawno.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3dwmitkfq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3rmhqylqy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqggoohd.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3nvlbihtc.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3sdadnexz.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3ytadsilx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3slscbysa.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3affkmano.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3qtmahsiz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyhyrkpb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3argtrelm.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rlfqmxpp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3zjunckuc.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3pjotdicz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tdnfkfne.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vjspcznw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3iqhnsjiw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3viciklom.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3whyqjquz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3scutnoip.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3ywkqqgij.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkxvmzw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3qqvizpyt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3kehbicke.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3drsjpnzk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uchxceyr.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hlpxwrfi.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gybgemft.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3ynkcfnhw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcaijyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fopgovcw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3esaykkke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpssofis.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3qiynokxm.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3emmrgtis.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3onuybnvz.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3fondvrcq.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3qmrhthqr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3kobvchey.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3fgtvjlut.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3vshpebsi.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3socaliab.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3difvoqgq.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3sfvbnjqq.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3ejsivahd.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3zplnpwgh.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3gvtyzpft.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3knibqnbf.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3hhxpuxiq.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3tcdafako.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3lkctqyjg.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3ybradlbh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3gnvanolv.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3bsofoznx.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3mfeatcol.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3bhvcaygf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwkcffk.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejikdmem.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3hypfutzf.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3asvgrzov.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3mtlwqeza.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3zfvfbztg.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3zbvkmrhd.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3equhdbrl.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cyjbbrcz.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3ysjykjcs.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3jazogluj.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fkrgitct.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3adwibbxb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3byddrygm.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwmerfub.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3fsqukwxm.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvaezxb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3ocpcicpu.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3iyarocni.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3aokpemez.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt3pkjahhfl.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wxanpuwx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3nvsuwnqh.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3mzrgjead.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3belgkdvm.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3ifqqndko.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3hkhbnmyj.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3bkavwdgp.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvkxgcj.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3quijoavu.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3jotdddyx.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3lxukfwah.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3rolywvhu.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3hsdpqclh.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3vxnfcbqs.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3szzwokrz.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3srrroxzo.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gzjxbfdv.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3gygroror.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hiyyaxhl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3lavsmfbi.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3zlbbnbvq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3zzigvdnx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3fhnjndml.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ufabmhun.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xrxklana.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3fpbeuytv.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3flgzjgxf.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3mmbemobv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3mibvcsnp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hhihnnhq.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3knnsmgan.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3wqhwtpgm.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3yzewphhd.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pueojels.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zdulgivz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kjfwdmfg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3vzjkrunx.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3exwmhnen.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3esdaqxgn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3ddaejrcs.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lueqzvst.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3ttxbarcc.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3xfphrbnf.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3seijeaxx.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3ykhjkwfm.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kxrzvpvn.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3dlhshmsl.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3jypuwvio.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3blkkgrmi.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3mhyghuix.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ftonwvoe.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3olrisygb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3bsliwhsu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3hodphnag.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdqclm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aahfuivr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vxrtebru.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3qqrvqzxg.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngdrpzzu.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kyfigrix.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3nksolhaq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3gubdhjzn.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3rjesvbvk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vikfzawn.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3puskdluy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3agsxcfxf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3yrjhjfae.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etfmfqat.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3enbpprim.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xnwxrftn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3xgeqhsni.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3cdlemmav.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3uxakkvna.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xeeseagf.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3ghssqioa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wimveejl.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3jgezrxqs.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ralhjilj.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3rapmkkyk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3liezwnvm.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3fwehznpq.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3zdmedbgs.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3gicqwfjo.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zujuipzl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3elaenvxg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xtljtuut.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bivdsjzm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3lrncqztj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3geltdzcl.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3eobkvcxo.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ryzmmkdy.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3hnazwdov.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ljpckrxu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3knfxquif.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3qyikrxgk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3hzvggdtq.html


<!-- 参考信息 -->