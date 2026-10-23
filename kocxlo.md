代发 wailian999

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fvftteww.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nmvnrkif.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3bvkxvzpo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3idtwgizi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3qlufrhie.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3izuextfm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mephbpww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iswyhssy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sfjurntf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3fpofpnee.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ksrjdzur.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3veihjhxa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xtfinpno.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gyfiabqh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3radxmmby.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3idcdirwh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dwqhponf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3siuoqllg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ndgyoyac.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3csskmfbu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zkyzacum.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3rechrltb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3cbtatoir.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3snedjhzd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fnilxvro.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3gsthfopp.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3yozsmtlv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3wkdqxpgi.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3rasiqvai.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3qfvvvqtn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3frdznkws.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ekowvyzc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tviorazt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whkvykkb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wkoeemlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pndpdsab.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hrznxgbo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xwndvqhi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxvniaaf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3jqtoeyet.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wtovublt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zvzsukdj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3vitfgrhj.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3ottnlcsi.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3oiofswtu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3jbmoczdc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3slkdcemw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjkitioc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mhaduwae.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3umyeivxg.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mgzumiwq.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3nvhafnkj.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qpoesgvm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3lqhbbgxb.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yserqbyr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3ccozlaip.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3dmmgjnbi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zwygxvyu.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3odbqxkjk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3phmglrkx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sryimtrr.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgduxcvq.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wjbdevoi.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3igarwxpf.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3cbsxvkgi.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3tensrxvd.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3foeiishw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3kkwmlbwd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3pmucyndh.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3kchkodqi.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kcyncdos.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3uehecqgt.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3febtdxuz.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hrumcheg.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3hwuvjyur.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzwsfkc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hofocova.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ixkqhwwv.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3lgeqhtsl.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3mzkdpkfh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhebgzry.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvltyhl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3btjitqqa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yjertjef.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3haqdzxvs.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3diccgadm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3rcbdqtlr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gqumodpc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jblwrmfo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tvevllme.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3chdxhhca.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3bowuzdsk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kwqudgda.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3htwkcnnw.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ypzwxfyc.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ziaypznm.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qkwrnxpy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rezddoub.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mryoamxw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rcnawaeq.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3tlspzvay.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3pobnxdlh.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3xvlsidoq.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3ovshxmwy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3tzjcknji.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jimccvkq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3lypyipef.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dtnxpzmz.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3anotppxb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3onaasnbt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ozvppoej.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3cfzoyhbv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3akijakwt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3zbzypdbs.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3uegbfsat.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3glqkkrjk.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tsnddnfb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3bqpwykds.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwajrgdk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zcacjuqc.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gyclqaoa.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3jbdxgbzf.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3fmyoffps.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgafqhnh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nmakjdvr.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xeuxrfxn.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3bfvoqolh.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfknxhik.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jxrkcwws.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ckuglaja.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcguimmr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3rtxaaofd.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jsnixcrt.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xzscywwg.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rufwnyge.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3baeislix.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3emtarour.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rhmmqcuc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mymlukhd.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3hothlnkh.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3jxibtxnn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uhtexjbx.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tqxcxzpu.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3okcdblsf.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuewpsrj.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gvqhxwsz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwksbkq.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hjyespea.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3trfmrrbu.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3trneypnf.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nwgcagru.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3hewecydd.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uvqtmxob.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3odemvpqh.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hcxldjze.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3bhgseggi.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3lyrkifxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uziqurdd.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ydwlgfgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlsarlar.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3anaoztbc.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ubogscew.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt3jmsoorgj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3ylylqsvi.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mrdztmuk.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3gjqwhezr.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3bflnhaiy.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3xpspezlw.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3rulaaseb.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3olnnkjoz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt3mqcxfmxo.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt3zvhsbebg.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3quplkqms.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hujlviux.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3dhiollnj.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ckuxepfa.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt3hkenkowl.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3wfmcgzpm.html

[U10] Py：按值排序字典
来源：http://www.52xcode.cn/Article/details/gt3lccbinhc.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3xxdquqmx.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qilbvqxa.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvviuddj.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt3cioejxfo.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3undhwjxt.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3otdlkloe.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3ykpjbwja.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3ixsddgrt.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3bunvlzza.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3wwcuvlib.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3rdnimklw.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3zrxxzlra.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt3pthaexpg.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3ibjhssrg.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3ptdqfmoz.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt3jdipnddb.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3romotlvi.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3uznptziu.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgubwkmm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3xqwyvfox.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3mjalzsup.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gdkdzvhd.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3sxsopnsr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3bttmsrvs.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3cjmrrovf.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xvjaihvg.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3kaqqabmy.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3ztdlqxjl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3swcvwsqe.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3mynfgubf.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3zqxhnimt.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jqlanthf.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3ajuaousq.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fjtphiuo.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3fflawejm.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3jrflxqru.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3pnbitter.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3jbrbjtby.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3zrlnowsf.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ugyzolbg.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbktrtw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3gxjerott.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3zzfdrixf.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jyeobmwj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3uojozvmb.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ncyzvoem.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3sexengvg.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3grcvijje.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3hwlgxcww.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3rhrxvhci.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3kbvhbmry.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eewmanoo.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3cfdgjohb.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3puwtheew.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3uzrldtzw.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3virrbxpz.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3vehwcpux.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3ohtrcvvz.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3ukvsqrdj.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3wpxwwtsg.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bgsisimq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3ujsbwpef.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3mkhxxmbg.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3vndyhtlo.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3wmomhzuf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yimhuhao.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbywsqj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3wilkivro.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3uwrwluzl.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tfgpkkjb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rbhpvmpm.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3vllmrtzi.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ushfakwg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3mwdrhtdy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3fvwjqcew.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3sfcbsjnr.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3rrrqjptz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kytjhotw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bleshufk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3grudsxpx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaaqzrpe.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3vdppyqwe.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3xccycrmj.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3voixnnji.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ttstzmfu.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mxgrfsnv.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3algnyyvh.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3apzzoswv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3pblsrtfy.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jvkvxfym.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3seulqwix.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvkdjmes.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3enyrstpd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3pfywawal.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3bitmgwhh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3ffnsypbd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ynmppybd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3meozedzh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fxodxfup.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3lvuabfuy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3sucdubze.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3pvipkcjv.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oxppgbck.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3fqwexulj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3mexvdbeh.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3btxxiswi.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3phrdkrzm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3ngjrvwpq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3xvljwamb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3uvrbzsuh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vosylmat.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3hlwjgzei.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3nftaskpa.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3eiuxnufs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3zajtzyxy.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3dglzgszf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3yohjhcqf.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3hevgzanu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3hnhhlehh.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3kofykntj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3qzjsbjvl.html


<!-- 参考信息 -->