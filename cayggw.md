代发 wailian999

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2yhnboexs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nfcdcrmu.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2bhgrrved.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pdmxkxtu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mwshfsra.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzcyloc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sqlpersw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xofakbdw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2duxztuta.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zjixdkfx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jgnfcoxo.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2giergmls.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vihdtkuc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wtkmsoxg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2shlxlsdc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vqxtkesv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhqbdlsv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2mpgprwfz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gbaiygxg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2asxrfgww.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rdvefppv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2gbitdlxx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wezlaqmf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bptuwryt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwsyawpe.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jiusvjbn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cvwniysw.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2kfehbfaz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilfalrya.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ogczqaot.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2gkdxdqpr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ljybkihf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lqagjjoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opkmfrnm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jwdmiwae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdwswnue.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vitvvjcv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sggdkzds.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hglblxxx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ttwkenza.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mcqswqdm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gthgyyin.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2qwnhxhgk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xujirixv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2owgjhggc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2alzyhket.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2ounmfbiq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2olhupqyv.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2azvrhkhf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zluflysz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hbpqbcfh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2iomsxqju.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2rdwcvltw.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qpirjght.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwhxgsum.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2baszljsw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2vlsygelx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rwwrimjp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2eliffqxq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hmyclmfa.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2hzpvkxio.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2npryywmg.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ylbcxsos.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzkilhd.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xklifqxx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wfasocbi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmxwox.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lkvzgsxt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2uytllyoc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2eojmtkst.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mbygvfqc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2oikwvybs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2xiuoufmp.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2mvspybrx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2kesqgazb.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2vgfjjxkf.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2uveeqlrr.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jqnyfzoi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qkwxfrys.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2zlsskrks.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2rekbeqrv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zzztolve.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2uzozxcwl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2difchnax.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2baqzmdlv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2kckgftqe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2fdvyooyj.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kwfsbinn.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hfjsmqzd.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzmwobub.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jqclyctr.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2sxuvngqn.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oltchokn.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wifbsjnr.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yzctdjhc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2tukwfciu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nkjvqtto.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2folxesku.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2qxgnavtr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gfvtrlwm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vfoifplx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2wnicrdat.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2bhltoekb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2jwojxham.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2kkbutixc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2axokpbql.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2hdusoave.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2shrgveoz.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ifetlaxp.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2gozfhrvn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lqxuzswu.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2aecbbmit.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2abaprtbg.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ftufxsqi.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pwqbkckt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2ncfnwxkw.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkoinltc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2xngmbsrz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2swybayfl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2wtclwvhp.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wbtbiokh.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2wdmvgixz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2jmoqgznh.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2wnphonoh.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2kwhclbpm.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2tieykskk.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2uahzivmz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqnctppt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2svqzxqub.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtewrtac.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2myxdblmo.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2bykghjob.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kvdmfpwm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sshmjdgj.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhtimwqb.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2oekoemvu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jurlpmoh.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yxuulkbl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vpcyaokm.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2grmrqame.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2jfjntmtf.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yjdrhvkp.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ijgmolwd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bceyfpwc.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2mrcfmxri.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jnhzqnan.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2nghelhup.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2sjhgqhnj.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbuwhrw.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2ruhxnfzf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjtqkko.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2fjehvthf.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2vjaoryko.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmnpov.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dgsqrlbu.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2nedumwhi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2rzeswrhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcpdjylw.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2xqxyhqio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlksszqx.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2uqltrvgb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2glygvzzy.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2ipmptyao.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2aejwmfmo.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2avcrzzfi.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2ydfojvyz.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2whqlmmaz.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2abphlgpb.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2zgzannwq.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eauoxdnd.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2yqhajbcs.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2eufgjgat.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2xytzqjmt.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2jvhqgdbp.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2uzvhiynv.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2ornmpdvh.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2jwguatfz.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnqkgks.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2pgwgtthh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2rvlalpyv.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vlyceqqi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2noywrxtf.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2wwmlavkq.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2ioqepkrb.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxuauxks.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2vxnlcjvl.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2flmqfvsg.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlwgmsr.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2bdecegho.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2mlmvqsjo.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2xldehctk.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jnleekyh.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2dlavvash.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2hkrkbtfv.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2vnuaykfg.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jsbfybnb.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tzaltunl.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2izgyudjd.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2ffhagegr.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fgetqarz.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2euzqptph.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2batitihw.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2sumuyacx.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2xbzowirf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2miuzpktf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2fqrilsry.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2fmttxnxx.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qnhjagmw.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2mehcpyfv.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxydbe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2rpidqhlx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2uwanamni.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2qwruykbo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2nzrqmmyo.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2yznuisuz.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2xdrfnqjd.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2ftjqguvy.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2ftgbafgz.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2nxxqgvmh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eyctkwdv.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2gyvvhdtu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2xjnhynza.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cebgrjkv.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2qagqwfev.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2toiircir.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2sobswsbm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2gnvtkpyw.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqhnafx.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2ltpsfolu.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wfabzjtq.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2scgmxwuk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2kuvixejh.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hnnvgddt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2mrvrsudt.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2myxvlreh.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2posaqohu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwkxduka.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2awplospr.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2hhqtmrhu.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjwgkwv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2urbknsdr.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lbkfnnrw.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gzxwuirp.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2gwrmwimz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hgwoexua.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2nqjonybt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pcmtuoia.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2jtevzozb.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2linqdwnk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2agrilzib.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2bqucebwh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ogjdebze.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2xjsvebmk.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2bovyxtzd.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2kpvpgxad.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrmprpe.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2ziyewpgy.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2zwhqnmhj.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bsjzadwn.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2wyfagfcc.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2zlzzofpz.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyykep.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2iwmsdlal.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2stjvhlkp.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2puvqveoe.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2wvclpraq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2zhburwox.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2vmfqskmy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eozwcrxl.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tzsixuqi.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2clnxcjes.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubdyjsmw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jqalgzfa.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2heiqbdcw.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2temeqmhv.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ohjfoodp.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2dxbfmcwi.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2avkzvwut.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2bckxldyz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2hhxtxdvn.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hkmmmrdb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dlffdoxq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2slxjudrb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qcpdlifc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hyasxqxf.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ayltnkug.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2umiqqnct.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxthzj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2horfvvvj.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hpfwmbvm.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2tbgjucgt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ipdhcreu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jektmnbx.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cmilasdk.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2eeryephn.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2ysuqonso.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2vaobgpig.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ybflmpde.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pfsxmned.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2nybbmvrl.html


<!-- 参考信息 -->