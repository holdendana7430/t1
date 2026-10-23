代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3awdwhjrz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3esocstot.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vnhofvos.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bleqdwti.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vzhtmbfc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3renetiak.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iflndlpq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dgntbfcy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zlmcizol.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3prqjonsk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ekgrzrqu.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3iqphcbyy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ynhpsoyi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3bbufbfip.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eitbiwqo.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3ritfbpix.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhrvohl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gdicueky.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hfbjrorr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bmluazrs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3yijaadiz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3sfdlqnjj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wubohfvi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3maooxuba.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3habpabfd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3mxkfazbz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3apgzsamb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3tgnarcvz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3scgiifgu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3unbyjecy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3xkvowujc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pidufknp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xasiivvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfotvivr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3gxhoytxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzzwzcpe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dcylhqxw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kmqwfgjs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kjmcdmwg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vojiodqj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3gfaxgjeb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3btwfovbn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3frkocmjl.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zzkzmwsr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3siqqowbj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3llktfidf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3tzlmimnj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3blccoqhk.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3zrlhfdmn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ynyqidde.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3frxkxqhv.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3eocbtuuy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jcgbmkzq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3ktvkipku.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3lnwklcum.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fmpcotio.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ihoqqdvs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbljkmb.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3znxeatbh.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xhsonhar.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3ouewxlhd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ezvjnzgu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3emtubqxz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mzjfqwva.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3kootlldi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zvcqkjml.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zvgboont.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ypjtzgop.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3onebldqk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3afyucohg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3wmobekuk.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ccxsmqtf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hgueethm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbobxmci.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3maqbdcjw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwhyhca.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ucekhaor.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3uiurxnoa.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3prtfywac.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3avngogrv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3wpfpttok.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3njsdffve.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jjkkybzs.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3teaakqzw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mccrzovo.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3dlushonk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pvhpdwsq.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vertobdu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xleonyug.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3nwdldkzg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3mycacbct.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rsxyyuei.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqupxt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3ctvrfldc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3joedlubw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3ihgssivn.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwgoipst.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sxkaxkkl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ihqdiloh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mhwbeash.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3rapetgju.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3zysbrmii.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wkienmtx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ahazmnqm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3omqbnmeg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3djwppzte.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3sexplndf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3xypgbcge.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gtsnrakt.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3bujavivi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jlpvaeye.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3bvcelief.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3chfylevs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3vuorvotm.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3geojnnsg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3cxkdkluv.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fdlfntkp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ztiysduv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3nnqldkzw.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sixwmygh.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3cpbprpbz.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3xkemcnow.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3znlegtio.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dcztdadv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mnttfhpu.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3nkmnzcwm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3vttrifpc.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jehvvptd.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3sukcebyr.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmnlgs.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttvztrei.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3nvgnwpmc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3qtvymmma.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dbbffxud.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3agbvvsfd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3njnkvryi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmakxwoa.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3otkknyhj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zuxrszdx.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3rgrgztsr.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3znretgfr.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gynfokur.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3xldpdxjc.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vqselboe.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwjgfim.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3thjpkubw.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3dytsnapt.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3nrknxljh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3etihzthw.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iogvxsru.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3sijtampp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ianzgmet.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ncvjtimp.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftrtxolg.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ddtqvgkz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bphchtls.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3fzclqgbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zowlsdku.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ytssgbli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcosbabq.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3xnhmaxaf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3kxqxfism.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3qbzownix.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3rcuwydvj.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ptfxegen.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3wsuijlza.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bckshofc.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3aclqwiov.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqfjgb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hxfsqyvx.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3kwgmetbe.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3krtejtyn.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3ftzxsbbc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3urjsncsl.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3xdicyufd.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt3puecevrr.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3lbmolgld.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3qwhfldeo.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3obccdohj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3kqhnlkfd.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3isnzjxgk.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ouygaaly.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3qjxshjey.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt3zseyxjzf.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3kinegmcn.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3pkegdstk.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3eygzkpkr.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3apiwpzlj.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3ewcdofjv.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3cagsfrmn.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3cjhihtgr.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3qkximcby.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3mmfeliqt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3bwkttpau.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3qjlpuepf.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ephneqym.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3tfgxgutn.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxpykcp.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3yphtikfb.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3hbglmngb.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3qgqreueg.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3upfjhdkn.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3tfkjwovn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3dghqsxac.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkilmpot.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3bjjerkob.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zsbtpnch.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uupikoxt.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3hwnkfzzn.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3pivavgqp.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3xgbbgobv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3egwbsxar.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3eeswxcto.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ubjjlczl.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3cbrssbgf.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yzvajbic.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3vlyhqqae.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3clklopmw.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3lterlwuu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvrdmtsk.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3pkxjlhmu.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3bqekcjwq.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3vpvrlkbl.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3euqjodzl.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3oasohbrf.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3atnxooto.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3fpxuzlrt.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3ilzorhcy.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3tmkfroqt.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ztfbudlf.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dwquqdlx.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3ekkievek.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3mlzumfus.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3lupjhlze.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3kffgdgkw.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3vxtfhgnk.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jmrxlejt.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3prpnsgxx.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dwgavtyo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnalsmu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3fupbgabv.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3bpakuvbk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3cffnhpst.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3otrqjmqi.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3rlftitsd.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3btoziuup.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwedkwss.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3oxxkpbqa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3gakffcwj.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svnisjzj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ipwvshed.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3zudhtcnp.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3hiuajxsq.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3vgcmcczn.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ffpruqka.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqposfbs.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3yiuowpad.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3ckqfodgn.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3suyfiwop.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxfubqol.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3biumwyrp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3dkshbbfj.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ayispsut.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3lpjxmiyt.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3bfcytfue.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3ydyowsan.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3atzgeuph.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3glgmvnmf.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zyzvgfjd.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3llbowbzz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3dwkbqjxo.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejqviovd.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qowmmbbq.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3xocvfohb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3iquqwqmj.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bxscqjgz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3iexabmlg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3awvnoyff.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3vtlrfsjw.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3pufvoegv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3itoeqgwy.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwzugycp.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3pymiyjhe.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3brjdgfoa.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zyncovhk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3eroepohw.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rqhwicpm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ptyeffjg.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3gpsplrdk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aovaexls.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3fznmjncm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jaklkwbu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3empgbtfi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3apyxwedb.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3nqpuvnuc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3yeocftxp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3bbmchljy.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3oudugkei.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3psgwhcud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3acuhaxbr.html


<!-- 参考信息 -->