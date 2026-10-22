代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uravugzl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hlkqhbjk.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2cuazumkm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nyvibrkh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kcltjmdx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhuxnlms.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2euezaess.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wovrsqsd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zcmwrjyy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rjtnqnoo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2veghiwkx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ajetzxim.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sarqfgmt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aairbdxi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yfrwlrvo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2agrtvhfw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2twfxlgff.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qmukxtce.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zzuevhxo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2duxzudkx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2aqzgptcl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zpzknnjq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzafxkj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2cyixzbyt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2inikhlfi.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2wuiybvvd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kerzdvux.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2gamgpzpo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sztjxzbf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2begyahet.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cqytoacp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2ymcypsda.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2kolqlpmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwpdrdap.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qepphiqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdeuyfxn.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qginsyun.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2jcevajib.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2peazrwuj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2xcmngsbh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ezkmajhr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gjpufaqz.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2rdjahbfu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ppoevuhm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2aoheibcm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2zwrltqvd.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2uwnpqpmy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bokzttkn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hndhmjlw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2sqfyiwzi.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2gphyibsk.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2lckdvpfa.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwqutcyq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2iebkhkqy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcaalwxd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2jziejrmf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2vkdwkryi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ggyvltpr.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2iquheeze.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zpegwzdx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ttcawfbz.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cslybelk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2rppcvjyy.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2tdqtbvcw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2uowqixec.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2udikpfuq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yjllaboj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2dcxalsgs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2ktmeguuy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2fceccllk.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qwzuzlee.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2cdiykota.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tqmyqisl.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2abzbptmy.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xmdghpau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2iriyzagr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2doyhtvnh.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvmkmka.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vndrnqwx.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqapwlmw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwcvjmyy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hpbjcdab.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ybeqwhbf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ipbmjtaa.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2tqfrkpzb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2ilmfieby.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2wyvxcilf.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vgirwdne.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hmxzfrln.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlbrbcdg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2xswasgei.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2vpdhogyb.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2efkvfcpf.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wngpofvn.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wngxybhm.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xxfhxxta.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2djhcghfc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2fqzbrbps.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2aexfqhmo.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xsrivzbn.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2fedpljcx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2wwkdfctb.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2rbjdhwsv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2qpcbhiuf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2pwyysjeu.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2bzxejnsl.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2fnujckjp.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2jptpphuc.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2paxpaozy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2jlfdgdsx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kjoqlagb.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bqmdnbcn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jltfdsnl.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ypvtrunk.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ujnopidm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ccuxhftd.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iagkoaaz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2pvmdzzlx.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2slfdoyfa.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hoxbittj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qehvzhxq.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2gxlcmnsn.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2ertzzfjd.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2zriycqgs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ftkayqxn.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljiqwnsc.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2qcjjulet.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2iegezzqt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2zwletyov.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2yuksvisp.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2ahnfinfp.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kwrgzhdc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2weztcitd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2htpzlukg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ouoejfoh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2yysmfwzp.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbgqpduk.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hifhsebk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbzczpp.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnfmgwcv.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wennkzaz.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2qnbnyzit.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wytsoiwu.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2mpodazwy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltocxuvt.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2zcbuqkhq.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyrrmpsh.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2mfnaasgw.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mythgdxo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sjitupzd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2brxhmnre.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2mhkmdxsv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2xgwmredx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxzzrafy.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2besjoeeq.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2jecvcplw.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkzvqpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocdnetmi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ywbolgxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iirwzdjt.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2mwltmvkz.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2uafyuivw.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2oqzvfxgp.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2nrmsgbzr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yzbtdggu.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt2sdzajfcn.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2rbekglul.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2rdxhlmag.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2baxbhwwj.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tsbmbufy.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2hmsxyqbv.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2wjlfyzpx.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2lwpulnye.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wjgouvjk.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2bnqztopw.html

[y for x in nested for y in x]
来源：http://www.52xcode.cn/Article/details/gt2gaxvswln.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt2fblifiwr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2erordzjz.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2wkxmdkwv.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2vtjujzbj.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dwkgeofm.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hohnoixm.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2zykunont.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2yaoisbvl.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2asqywrff.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2hpywybtu.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2anheyjdb.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2kywacfak.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2ihyyiflb.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2lxojdjic.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2pxlgpccz.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2kkzspvkr.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2ndaxesrj.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2igryrvxc.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2tcxoarbd.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bdjbupvk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2zexfpjin.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2qtbkhpne.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2jnixhssh.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2hkuvtpye.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2zvfpjsuo.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2eoemwlta.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2gvetguti.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2vbkjawxi.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2lfalbgoj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2npefcule.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2mijpasgk.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2izezdykv.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2fypzdqpb.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2beasvwkg.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2rtgqxqzb.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2tcazvvxz.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2sjfcvquv.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2ojondzxz.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2vopraoct.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2wrwjgqvp.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2fgdqleng.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2hrqzcknt.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2srslovcc.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cszeubzn.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2pwutwaap.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2mrtfegqt.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt2wpeirybf.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2ckukdjkf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2jetdyros.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2aegtmyfa.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2pihlncut.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2svptbkec.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2mkfhqcku.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lsdkshlr.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2mjjervfv.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2qtobhixp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2clbtfgyu.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2ainrosvz.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2mbdcobsk.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2ljvmibxe.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ijirlcxd.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2gcyyxtro.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ovkqibya.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwujsqyp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2qszvwwwj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wetlnqpa.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2mxulpnms.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbcivus.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2voikpass.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2skyubblq.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnxsqstx.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eygmkojn.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2nbeotrok.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2njujeqnj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2harozuoh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2yhncouxk.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2qrlwtpsl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2rvvxiuni.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2cbfcdijd.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2usxjbaqn.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xvnytzna.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2cuuklrol.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2nzjuzwfq.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjcmcryd.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2yfzmpsci.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2grdvpalm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iusllxlg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2bmgfiavs.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2sbzdbrxp.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2hndfkgou.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2snydymur.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2sremllkg.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2aqnwppdy.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qmgejber.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2sikdgbww.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dygmxzfx.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ljhshlog.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2ryonfdqh.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2jwigxmss.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2hbmscdjv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2engvbusd.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2etgqyfmh.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2wlyeoxhd.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2upgvspbh.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2vzrgzdzj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ougvqtqo.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2zvutmjop.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2gbynfsny.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2osdtoxxa.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hvmzpkvx.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bykbfmjm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jpfkmdur.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2umructsa.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhzskbfs.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2insgghio.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwyrnulj.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2jwdbzoxy.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2nfuakxhl.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nbbvlmuu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2homllscu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2ecqrjqoz.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2duxtqfyk.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ozorbryw.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2lwdoootw.html


<!-- 参考信息 -->